A super simplified way to track which parts you can manipulate based on ownership status in Roblox.

## How it Works

The script automatically categorizes all `Baseparts` in the workspace into three global tables:

**`_G.F`** = `ReceiveAge == 0` / **Can manipulate** ( you own these parts )

**`_G.U`** = `ReceiveAge ~= 0` / **Either no owner or owner lost** ( unowned parts )

**`_G.A`** = **Anchored Baseparts** ( cannot be moved )

## Usage Example

### Debug
```lua
-- // >> Color parts based on ownership status
game:GetService("RunService").RenderStepped:Connect(function()
    for P in pairs(_G.F) do P.Color = Color3.fromRGB(255, 0, 0) end  -- // >> Red = Owned
    for P in pairs(_G.U) do P.Color = Color3.fromRGB(0, 0, 0) end    -- // >> Black = Unowned
end)
```

### Black Hole
```lua
-- // >> Example: Move all owned parts to your position
local Players = game:GetService("Players")
local Root = Players.LocalPlayer.Character.HumanoidRootPart

for P in pairs(_G.F) do
    P.CFrame = Root.CFrame * CFrame.new(math.random(-10, 10), 0, math.random(-10, 10))
end
```

## Other Debugs

Enable these settings to visualize ownership and simulation radius:

```lua
-- // >> Show which unanchored Baseparts you own
settings()["Physics"].AreOwnersShown = true

-- // >> Show your SimulationRadius
settings()["Physics"].AreRegionsShown = true
```

## Technical Notes

Uses `ReceiveAge` property to determine Owner ( Not 100% reliable )

Filters body parts and destroys trash

Natural Disaster uses Weld system where Baseparts are constantly unanchored. New constructions spawn with unanchored AssemblyRootPart that only gets anchored later, wait(0.8) fixes this issue.
