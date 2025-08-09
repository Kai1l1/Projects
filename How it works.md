## How it Works

The script automatically categorizes all `Baseparts` in the workspace into three global tables:

**`_G.F`** = `ReceiveAge == 0` / **Can manipulate** ( you own these parts )

**`_G.U`** = `ReceiveAge ~= 0` / **Either no owner or owner lost** ( unowned parts )

**`_G.A`** = **Anchored Baseparts** ( cannot be moved )

## Usage Example

### Debug
```lua
loadstring(game:HttpGet("https://gist.githubusercontent.com/Kai1l1/ca7c173328a48aa982920f320e77c02d/raw/4f3efa4f12de7cfa4a8eabde5e4e11ac8028533b/Table"))()

-- // >> Color parts based on Owner or Unowned
game:GetService("RunService").RenderStepped:Connect(function()
    for P in pairs(_G.F) do P.Color = Color3.fromRGB(255, 0, 0) end  -- // >> Red = Owned
    for P in pairs(_G.U) do P.Color = Color3.fromRGB(0, 0, 0) end    -- // >> Black = Unowned
end)
```

### Black Hole
```lua
loadstring(game:HttpGet("https://gist.githubusercontent.com/Kai1l1/ca7c173328a48aa982920f320e77c02d/raw/4f3efa4f12de7cfa4a8eabde5e4e11ac8028533b/Table"))()

-- // >> Move all parts to your root
game:GetService("RunService").Heartbeat:Connect(function()
    local Root = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
    for P in pairs(_G.F) do
        P.AssemblyLinearVelocity = (Root.Position - P.Position) * 50
        P.AssemblyAngularVelocity = Vector3.new(math.random(-50, 50), math.random(-50, 50), math.random(-50, 50))
        P.CanCollide = false
        P.Massless = true
    end
end)
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
