# CLASSES

## Object
**Tags:** NotCreatable, NotReplicated

### Properties
```
ClassName: string [ReadOnly]
className: string [ReadOnly] [Deprecated]
```

### Functions
```
GetPropertyChangedSignal(property: string) → RBXScriptSignal
IsA(className: string) → bool
isA(className: string) → bool [Deprecated]
```

### Events
```
Changed(property: string)
```

---

## Capture
**Extends:** Object
**Tags:** NotCreatable, NotReplicated

### Properties
```
CaptureTime: DateTime [ReadOnly]
CaptureType: CaptureType = __api_dump_failed_to_create_class__ [ReadOnly]
LocalId: string = __api_dump_failed_to_create_class__ [ReadOnly]
SourcePlaceId: int64 = __api_dump_failed_to_create_class__ [ReadOnly]
SourceUniverseId: int64 = __api_dump_failed_to_create_class__ [ReadOnly]
```

---

## ScreenshotCapture
**Extends:** Capture
**Tags:** NotCreatable, NotReplicated

---

## VideoCapture
**Extends:** Capture
**Tags:** NotCreatable, NotReplicated

### Properties
```
FilePath: string = __api_dump_failed_to_create_class__ [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
TimeLength: double = __api_dump_failed_to_create_class__ [ReadOnly]
```

---

## ConfigSnapshot
**Extends:** Object
**Tags:** NotCreatable, NotReplicated

### Properties
```
Error: ConfigSnapshotErrorState [ReadOnly]
Outdated: bool [ReadOnly]
```

### Functions
```
GetValue(key: string, defaultValue: Variant) → Variant
GetValueChangedSignal(key: string) → RBXScriptSignal
Refresh() → null
```

### Events
```
UpdateAvailable()
```

---

## EditableImage
**Extends:** Object
**Tags:** NotCreatable

### Properties
```
ImageData: BinaryString = __api_dump_failed_to_create_class__ [Read:RobloxSecurity] [Write:RobloxSecurity]
IsReplicatedCopy: bool = __api_dump_failed_to_create_class__ [Read:RobloxSecurity] [Write:RobloxSecurity]
Size: Vector2 = __api_dump_failed_to_create_class__ [ReadOnly]
```

### Functions
```
Destroy() → null
DrawCircle(center: Vector2, radius: int, color: Color3, transparency: float, combineType: ImageCombineType) → null
DrawImage(position: Vector2, image: EditableImage, combineType: ImageCombineType) → null
DrawImageProjected(mesh: EditableMesh, projection: Dictionary, brushConfig: Dictionary) → null
DrawImageTransformed(position: Vector2, scale: Vector2, rotation: float, image: EditableImage, options: Dictionary?) → null
DrawLine(p1: Vector2, p2: Vector2, color: Color3, transparency: float, combineType: ImageCombineType) → null
DrawRectangle(position: Vector2, size: Vector2, color: Color3, transparency: float, combineType: ImageCombineType) → null
DrawTriangle(p1: Vector2, p2: Vector2, p3: Vector2, color: Color3, transparency: float) → null [RobloxScriptSecurity]
ReadPixelsBuffer(position: Vector2, size: Vector2) → buffer
WritePixelsBuffer(position: Vector2, size: Vector2, buffer: buffer) → null
```

---

## EditableMesh
**Extends:** Object
**Tags:** NotCreatable

### Properties
```
FixedSize: bool = __api_dump_failed_to_create_class__ [Write:RobloxSecurity] [ReadOnly]
IsReplicatedCopy: bool = __api_dump_failed_to_create_class__ [Read:RobloxSecurity] [Write:RobloxSecurity]
MeshData: SharedString [Read:RobloxSecurity] [Write:RobloxSecurity]
SkinningEnabled: bool = __api_dump_failed_to_create_class__ [Deprecated]
```

### Functions
```
AddBone(boneProperties: Dictionary) → int64
AddColor(color: Color3, alpha: float) → int64
AddNormal(normal: Vector3?) → int64
AddTriangle(vertexId0: int64, vertexId1: int64, vertexId2: int64) → int64
AddUV(uv: Vector2) → int64
AddVertex(p: Vector3) → int64
Destroy() → null
FindClosestPointOnSurface(point: Vector3) → Tuple
FindClosestVertex(toThisPoint: Vector3) → int64
FindVerticesWithinSphere(center: Vector3, radius: float) → Array
GetAdjacentFaces(faceId: int64) → Array
GetAdjacentVertices(vertexId: int64) → Array
GetBoneByName(boneName: string) → int64
GetBoneCFrame(boneId: int64) → CFrame
GetBoneIsVirtual(boneId: int64) → bool
GetBoneName(boneId: int64) → string
GetBoneParent(boneId: int64) → int64
GetBones() → Array
GetCenter() → Vector3
GetColor(colorId: int64) → Color3?
GetColorAlpha(colorId: int64) → float?
GetColors() → Array
GetFaceColors(faceId: int64) → Array
GetFaceNormals(faceId: int64) → Array
GetFaceUVs(faceId: int64) → Array
GetFaceVertices(faceId: int64) → Array
GetFaces() → Array
GetFacesWithAttribute(id: int64) → Array [Deprecated]
GetFacesWithColor(colorId: int64) → Array
GetFacesWithNormal(normalId: int64) → Array
GetFacesWithUV(uvId: int64) → Array
GetFacsCorrectivePose(actions: Array) → Tuple
GetFacsCorrectivePoses() → Array
GetFacsPose(action: FacsActionUnit) → Tuple
GetFacsPoses() → Array
GetNormal(normalId: int64) → Vector3?
GetNormals() → Array
GetPosition(vertexId: int64) → Vector3
GetSize() → Vector3
GetUV(uvId: int64) → Vector2?
GetUVs() → Array
GetVertexBoneWeights(vertexId: int64) → Array
GetVertexBones(vertexId: int64) → Array
GetVertexColors(vertexId: int64) → Array
GetVertexFaceColor(vertexId: int64, faceId: int64) → int64
GetVertexFaceNormal(vertexId: int64, faceId: int64) → int64
GetVertexFaceUV(vertexId: int64, faceId: int64) → int64
GetVertexFaces(vertexId: int64) → Array
GetVertexNormals(vertexId: int64) → Array
GetVertexUVs(vertexId: int64) → Array
GetVertices() → Array
GetVerticesWithAttribute(id: int64) → Array [Deprecated]
GetVerticesWithColor(colorId: int64) → Array
GetVerticesWithNormal(normalId: int64) → Array
GetVerticesWithUV(uvId: int64) → Array
IdDebugString(id: int64) → string
MergeVertices(mergeTolerance: float) → Map
RaycastLocal(origin: Vector3, direction: Vector3) → Tuple
RemoveBone(boneId: int64) → null
RemoveFace(faceId: int64) → null
RemoveUnused() → Array
ResetNormal(normalId: int64) → null
SetBoneCFrame(boneId: int64, cframe: CFrame) → null
SetBoneIsVirtual(boneId: int64, virtual: bool) → null
SetBoneName(boneId: int64, name: string) → null
SetBoneParent(boneId: int64, parentBoneId: int64) → null
SetColor(colorId: int64, color: Color3) → null
SetColorAlpha(colorId: int64, alpha: float) → null
SetFaceColors(faceId: int64, ids: Array) → null
SetFaceNormals(faceId: int64, ids: Array) → null
SetFaceUVs(faceId: int64, ids: Array) → null
SetFaceVertices(faceId: int64, ids: Array) → null
SetFacsBonePose(action: FacsActionUnit, boneId: int64, cframe: CFrame) → null
SetFacsCorrectivePose(actions: Array, boneIds: Array, cframes: Array) → null
SetFacsPose(action: FacsActionUnit, boneIds: Array, cframes: Array) → null
SetNormal(normalId: int64, normal: Vector3) → null
SetPosition(vertexId: int64, p: Vector3) → null
SetUV(uvId: int64, uv: Vector2) → null
SetVertexBoneWeights(vertexId: int64, boneWeights: Array) → null
SetVertexBones(vertexId: int64, boneIDs: Array) → null
SetVertexFaceColor(vertexId: int64, faceId: int64, colorId: int64) → null
SetVertexFaceNormal(vertexId: int64, faceId: int64, normalId: int64) → null
SetVertexFaceUV(vertexId: int64, faceId: int64, uvId: int64) → null
Triangulate() → null
```

---

## Instance
**Extends:** Object
**Tags:** NotCreatable, NotBrowsable

### Properties
```
Archivable: bool
Attributes: string [Read:RobloxSecurity] [Write:RobloxSecurity] [ReadOnly]
AttributesReplicate: string [Read:RobloxSecurity] [Write:RobloxSecurity]
AttributesSerialize: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
Capabilities: SecurityCapabilities
DataCost: int [Read:LocalUserSecurity] [Write:LocalUserSecurity] [ReadOnly] [Deprecated]
DefinesCapabilities: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
HistoryId: UniqueId [Read:RobloxSecurity] [Write:RobloxSecurity]
Name: string
Parent: Instance
PropertyStatusStudio: PropertyStatus [Read:RobloxSecurity] [Write:RobloxSecurity] [ReadOnly]
RobloxLocked: bool [Read:PluginSecurity] [Write:PluginSecurity]
Sandboxed: bool
SourceAssetId: int64 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Tags: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
UniqueId: UniqueId [Read:RobloxScriptSecurity] [Write:RobloxSecurity]
archivable: bool [Deprecated]
numExpectedDirectChildren: int
```

### Functions
```
AddTag(tag: string) → null
ClearAllChildren() → null
Clone() → Instance
Destroy() → null
FindFirstAncestor(name: string) → Instance
FindFirstAncestorOfClass(className: string) → Instance
FindFirstAncestorWhichIsA(className: string) → Instance
FindFirstChild(name: string, recursive: bool) → Instance
FindFirstChildOfClass(className: string) → Instance
FindFirstChildWhichIsA(className: string, recursive: bool) → Instance
FindFirstDescendant(name: string) → Instance
GetActor() → Actor
GetAttribute(attribute: string) → Variant
GetAttributeChangedSignal(attribute: string) → RBXScriptSignal
GetAttributes() → Dictionary
GetChildren() → Instances
GetDebugId(scopeLength: int) → string [PluginSecurity]
GetDescendants() → Array
GetFullName() → string
GetStyled(name: string) → Variant
GetStyledPropertyChangedSignal(property: string) → RBXScriptSignal
GetTags() → Array
HasTag(tag: string) → bool
IsAncestorOf(descendant: Instance) → bool
IsDescendantOf(ancestor: Instance) → bool
IsPropertyModified(property: string) → bool
Remove() → null [Deprecated]
RemoveTag(tag: string) → null
ResetPropertyToDefault(property: string) → null
SetAttribute(attribute: string, value: Variant) → null
WaitForChild(childName: string, timeOut: double) → Instance
children() → Instances [Deprecated]
clone() → Instance [Deprecated]
destroy() → null [Deprecated]
findFirstChild(name: string, recursive: bool) → Instance [Deprecated]
getChildren() → Instances [Deprecated]
isDescendantOf(ancestor: Instance) → bool [Deprecated]
remove() → null [Deprecated]
```

### Events
```
AncestryChanged(child: Instance, parent: Instance)
AttributeChanged(attribute: string)
ChildAdded(child: Instance)
ChildRemoved(child: Instance)
DescendantAdded(descendant: Instance)
DescendantRemoving(descendant: Instance)
Destroying()
StyledPropertiesChanged()
childAdded(child: Instance)
```

---

## AccessoryDescription
**Extends:** Instance

### Properties
```
AccessoryType: AccessoryType = Unknown
AssetId: int64 = 0
Instance: Instance
IsLayered: bool = false
Order: int = 0
Position: Vector3 = 0, 0, 0
Puffiness: float = 1
Rotation: Vector3 = 0, 0, 0
Scale: Vector3 = 1, 1, 1
```

### Functions
```
GetAppliedInstance() → Instance
```

---

## AccountService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
DeviceAccessTokenAvailable() → bool [RobloxScriptSecurity]
DeviceIntegrityAvailable() → bool [RobloxScriptSecurity]
GetDeviceIntegrityToken(data: string) → string [RobloxScriptSecurity]
MagicLogin(data: string) → null [RobloxScriptSecurity]
GetCredentialsHeaders() → string [RobloxScriptSecurity]
GetDeviceAccessToken() → string [RobloxScriptSecurity]
GetDeviceIntegrityTokenYield(data: string) → string [RobloxScriptSecurity]
```

### Events
```
MagicLoginEvent(data: string) [RobloxScriptSecurity]
```

---

## Accoutrement
**Extends:** Instance

### Properties
```
AttachmentForward: Vector3 = -0, -0, -1
AttachmentPoint: CFrame
AttachmentPos: Vector3 = 0, 0, 0
AttachmentRight: Vector3 = 1, 0, 0
AttachmentUp: Vector3 = 0, 1, 0
BackendAccoutrementState: int = 0
```

### Events
```
ServerEquipAccoutrement(character: Instance) [RobloxSecurity]
ServerUnequipAccoutrement(oldCharacter: Instance) [RobloxSecurity]
```

---

## Accessory
**Extends:** Accoutrement

### Properties
```
AccessoryType: AccessoryType = Unknown
```

---

## Hat
**Extends:** Accoutrement
**Tags:** Deprecated

---

## AchievementService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
IsAvailable() → bool [RobloxScriptSecurity]
GrantAchievement(achievementName: string) → bool [RobloxScriptSecurity]
HasAchieved(achievementName: string) → bool [RobloxScriptSecurity]
```

---

## ActivityHistoryEventService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Events
```
WriteActivityHistoryEventFromStudio(eventType: int, resourceId: int64, metadata: string) [RobloxScriptSecurity]
```

---

## AdPortal
**Extends:** Instance

### Properties
```
PortalInvalidReason: string [ReadOnly]
PortalVersion: int64 = 1 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Status: AdUnitStatus = Inactive [ReadOnly]
```

### Functions
```
TeleportConfirmed(placeId: int64, player: Player) → null [RobloxScriptSecurity]
TeleportRejected(shouldCooldown: bool, rejectedByDistance: bool) → null [RobloxScriptSecurity]
```

---

## AdService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
CreateAdRewardFromDevProductId(devProductId: int64) → AdReward
GetAdTeleportInfo() → Tuple [RobloxScriptSecurity]
GetReportAdInfo() → Array [RobloxScriptSecurity]
HandleWhyThisAdClicked(advertiserName: string, payerName: string) → null [RobloxScriptSecurity]
HideEudsaDisclosure() → null [RobloxScriptSecurity]
OnDemandVideoCompleteFromUI(result: ShowAdResult, encryptedAdTrackingData: string, encryptionMetadata: string, rewardDetails: string) → null [RobloxScriptSecurity]
ReturnToPublisherExperience(adTeleportMethod: AdTeleportMethod) → null [RobloxScriptSecurity]
SetAdGuiInteractivityHandlerInitialized() → null [RobloxScriptSecurity]
ShowVideoAd() → null [Deprecated]
UnregisterAdOpportunity(instance: Instance) → null
GetAdAvailabilityNowAsync(adFormat: AdFormat) → Variant
RegisterAdOpportunityAsync(instance: Instance, placementId: int64?) → null
ShowRewardedVideoAdAsync(player: Player, reward: AdReward, placementId: int64?) → ShowAdResult
```

### Events
```
AdTeleportEnded() [RobloxScriptSecurity]
AdTeleportInitiated() [RobloxScriptSecurity]
PortalPrompt(destinationId: int64, portal: Instance, requiresNoButton: bool) [RobloxScriptSecurity]
ReportImpressionSignal(ad_instance_name: string, encrypted_ad_tracking_data: string, encryption_metadata: string) [RobloxSecurity]
ReportTeleportSignal(ad_instance_name: string, encrypted_ad_tracking_data: string, encryption_metadata: string, teleport_type: string, teleport_source_universe_id: int64, teleport_source_place_id: int64, teleport_dest_place_id: int64) [RobloxSecurity]
RewardedVideoAdEnded() [RobloxScriptSecurity]
RewardedVideoAdStarted() [RobloxScriptSecurity]
ServeAdResponseSignal(uuid: string, response: string, isError: bool) [RobloxSecurity]
ServeAdSignal(uuid: string, request: string) [RobloxSecurity]
ShowDynamicEudsaDisclosure(advertiserName: string, payerName: string) [RobloxScriptSecurity]
ShowReportAdPopup(adInfo: Dictionary) [RobloxScriptSecurity]
VideoAdClosed(adShown: bool)
adGuiRegisterUI(adGui: Instance) [RobloxScriptSecurity]
rewardedVideoAdPlayServerToClient(rewardDetails: string) [RobloxSecurity]
rewardedVideoAdPlayServerToClientWithPlacement(rewardDetails: string, placementId: int64) [RobloxSecurity]
rewardedVideoAdResultClientToServer(result: ShowAdResult, encryptedAdTrackingData: string, encryptionMetadata: string) [RobloxSecurity]
```

---

## AdvancedDragger
**Extends:** Instance

---

## AnalyticsService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
ApiKey: string [Read:LocalUserSecurity] [Write:LocalUserSecurity] [Deprecated]
```

### Functions
```
FireCustomEvent(player: Instance, eventCategory: string, customData: Variant) → null [Deprecated]
FireEvent(category: string, value: Variant) → null [Deprecated]
FireInGameEconomyEvent(player: Instance, itemName: string, economyAction: AnalyticsEconomyAction, itemCategory: string, amount: int, currency: string, location: Variant, customData: Variant) → null [Deprecated]
FireLogEvent(player: Instance, logLevel: AnalyticsLogLevel, message: string, debugInfo: Variant, customData: Variant) → null [Deprecated]
FirePlayerProgressionEvent(player: Instance, category: string, progressionStatus: AnalyticsProgressionStatus, location: Variant, statistics: Variant, customData: Variant) → null [Deprecated]
LogCustomEvent(player: Player, eventName: string, value: double, customFields: Dictionary) → null
LogEconomyEvent(player: Player, flowType: AnalyticsEconomyFlowType, currencyType: string, amount: float, endingBalance: float, transactionType: string, itemSku: string, customFields: Dictionary) → null
LogFunnelStepEvent(player: Player, funnelName: string, funnelSessionId: string, step: int, stepName: string, customFields: Dictionary) → null
LogOnboardingFunnelStepEvent(player: Player, step: int, stepName: string, customFields: Dictionary) → null
LogProgressionCompleteEvent(player: Player, progressionPathName: string, level: int, levelName: string, customFields: Dictionary) → null
LogProgressionEvent(player: Player, progressionPathName: string, status: AnalyticsProgressionType, level: int, levelName: string, customFields: Dictionary) → null
LogProgressionFailEvent(player: Player, progressionPathName: string, level: int, levelName: string, customFields: Dictionary) → null
LogProgressionStartEvent(player: Player, progressionPathName: string, level: int, levelName: string, customFields: Dictionary) → null
```

---

## Animation
**Extends:** Instance

### Properties
```
AnimationId: ContentId
```

---

## AnimationClip
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
Guid: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GuidBinaryString: BinaryString [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Loop: bool
Priority: AnimationPriority
```

---

## CurveAnimation
**Extends:** AnimationClip

---

## KeyframeSequence
**Extends:** AnimationClip

### Properties
```
AuthoredHipHeight: float = 2 [Read:PluginSecurity] [Write:PluginSecurity]
```

### Functions
```
AddKeyframe(keyframe: Instance) → null
GetKeyframes() → Instances
RemoveKeyframe(keyframe: Instance) → null
```

---

## AnimationClipProvider
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetAnimationClip(assetId: ContentId) → AnimationClip [PluginSecurity] [Deprecated]
GetAnimationClipById(assetId: int64, useCache: bool) → AnimationClip [PluginSecurity] [Deprecated]
GetMemStats() → Dictionary [RobloxScriptSecurity]
RegisterActiveAnimationClip(animationClip: AnimationClip) → ContentId
RegisterAnimationClip(animationClip: AnimationClip) → ContentId
GetAnimationClipAsync(assetId: ContentId) → AnimationClip
GetAnimations(userId: int64) → Instance
GetClipEvaluatorAsync(assetId: ContentId) → ClipEvaluator
```

---

## AnimationController
**Extends:** Instance

### Functions
```
GetPlayingAnimationTracks() → Array [Deprecated]
LoadAnimation(animation: Animation) → AnimationTrack [Deprecated]
```

### Events
```
AnimationPlayed(animationTrack: AnimationTrack)
```

---

## AnimationFromVideoCreatorService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
CreateJob(filePath: string) → string [RobloxScriptSecurity]
DownloadJobResult(jobId: string, outputFilePath: string) → string [RobloxScriptSecurity]
FullProcess(videoFilePath: string, progressCallback: Function) → string [RobloxScriptSecurity]
GetJobStatus(jobId: string) → string [RobloxScriptSecurity]
```

---

## AnimationFromVideoCreatorStudioService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
IsAgeRestricted() → bool [RobloxScriptSecurity]
CreateAnimationByUploadingVideo(progressCallback: Function) → string [RobloxScriptSecurity]
ImportVideoWithPrompt() → string [RobloxScriptSecurity]
```

---

## AnimationRigData
**Extends:** Instance

### Properties
```
label: BinaryString = 
name: BinaryString = 
parent: BinaryString = 
postTransform: BinaryString = 
preTransform: BinaryString = 
transform: BinaryString = 
```

### Functions
```
LoadFromHumanoid(humanoid: Instance) → bool [RobloxScriptSecurity]
LoadFromModel(model: Instance) → bool [RobloxScriptSecurity]
```

---

## AnimationStreamTrack
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
Animation: TrackerStreamAnimation [ReadOnly]
FACSDataLod: FACSDataLod [ReadOnly]
IsPlaying: bool [ReadOnly]
Priority: AnimationPriority
WeightCurrent: float [ReadOnly]
WeightTarget: float [ReadOnly]
```

### Functions
```
AdjustWeight(weight: float, fadeTime: float) → null [RobloxScriptSecurity]
GetActive() → bool [RobloxScriptSecurity]
GetTrackerData() → Tuple [RobloxScriptSecurity]
Play(fadeTime: float, weight: float) → null [RobloxScriptSecurity]
Stop(fadeTime: float) → null [RobloxScriptSecurity]
TogglePause(paused: bool) → null [RobloxScriptSecurity]
```

### Events
```
Stopped() [RobloxScriptSecurity]
```

---

## AnimationTrack
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
Animation: Animation [ReadOnly]
IsPlaying: bool [ReadOnly]
Length: float [ReadOnly]
Looped: bool
Priority: AnimationPriority
Speed: float [ReadOnly]
TimePosition: float
WeightCurrent: float [ReadOnly]
WeightTarget: float [ReadOnly]
```

### Functions
```
AdjustSpeed(speed: float) → null
AdjustWeight(weight: float, fadeTime: float) → null
GetMarkerReachedSignal(name: string) → RBXScriptSignal
GetTargetInstance(name: string) → Instance
GetTargetNames() → Array
GetTimeOfKeyframe(keyframeName: string) → double
Play(fadeTime: float, weight: float, speed: float) → null
SetTargetInstance(name: string, target: Instance) → null
Stop(fadeTime: float) → null
```

### Events
```
DidLoop()
Ended()
KeyframeReached(keyframeName: string)
Stopped()
```

---

## Animator
**Extends:** Instance

### Properties
```
EvaluationThrottled: bool = false [ReadOnly]
FacsReplicationData: FacsReplicationData [Read:RobloxSecurity] [Write:RobloxSecurity]
PreferLodEnabled: bool = true
RootMotion: CFrame [ReadOnly]
RootMotionWeight: float = 0 [ReadOnly]
```

### Functions
```
ApplyJointVelocities(motors: Variant) → null
GetPlayingAnimationTracks() → Array
GetPlayingAnimationTracksCoreScript() → Array [RobloxScriptSecurity]
LoadAnimation(animation: Animation) → AnimationTrack
LoadAnimationCoreScript(animation: Animation) → AnimationTrack [RobloxScriptSecurity]
LoadStreamAnimation(animation: TrackerStreamAnimation) → AnimationStreamTrack [RobloxScriptSecurity]
LoadStreamAnimationForSelfieView_deprecated(animation: TrackerStreamAnimation, player: Player) → AnimationStreamTrack [RobloxScriptSecurity]
LoadStreamAnimationV2(animation: TrackerStreamAnimation, player: Player, shouldLookupPlayer: bool, shouldReplicate: bool) → AnimationStreamTrack [RobloxScriptSecurity]
RegisterEvaluationParallelCallback(callback: Function) → null
StepAnimations(deltaTime: float) → null [PluginSecurity]
SynchronizeWith(otherAnimator: Animator) → null [RobloxScriptSecurity]
```

### Events
```
AnimationPlayed(animationTrack: AnimationTrack)
AnimationPlayedCoreScript(animationTrack: AnimationTrack) [RobloxScriptSecurity]
AnimationStreamTrackPlayed(animationTrack: AnimationStreamTrack) [RobloxScriptSecurity]
OnCombinedUpdate(animation: ContentId, playState: bool, fadeTime: float, weight: float, speed: float, timePosition: float, priority: AnimationPriority, looping: bool, valuesUpdated: int) [RobloxSecurity]
OnCombinedUpdate2(animation: ContentId, playState: bool, fadeTime: float, weight: float, speed: float, timePosition: float, priority: AnimationPriority, valuesUpdated: int) [RobloxSecurity]
OnStreamingUpdated(fadeTime: float, weight: float, priority: AnimationPriority, valuesUpdated: int) [RobloxSecurity]
OnStreamingUpdated2(fadeTime: float, weight: float, priority: AnimationPriority, maskEnabled: bool, valuesUpdated: int) [RobloxSecurity]
StreamSyncRequest(player: Player) [RobloxSecurity]
```

---

## Annotation
**Extends:** Instance

### Properties
```
AuthorColor3: Color3 = 0, 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AuthorId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ChannelId: string [Read:RobloxSecurity] [Write:RobloxSecurity]
Contents: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CreationTimeUnix: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LastModifiedTimeUnix: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LoadingReplies: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
MessageId: string [Read:RobloxSecurity] [Write:RobloxSecurity]
ReplyCount: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Resolved: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
TaggedUsers: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
GetRequests() → Dictionary [RobloxScriptSecurity]
GetStringUniqueId() → string [RobloxScriptSecurity]
IsThreadParent() → bool [RobloxScriptSecurity]
```

### Events
```
RequestCompleted(requestId: string, requestType: AnnotationRequestType, result: AnnotationRequestStatus) [RobloxScriptSecurity]
RequestInitiated(requestId: string, requestType: AnnotationRequestType) [RobloxScriptSecurity]
```

---

## WorkspaceAnnotation
**Extends:** Annotation

### Properties
```
Adornee: PVInstance [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AdorneeOffset: Vector3 = 0, 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
GetAbsolutePosition() → Vector3 [RobloxScriptSecurity]
SetAdorneeOffsetFromAbsolutePosition(position: Vector3) → null [RobloxScriptSecurity]
```

---

## AnnotationsService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
AnnotationsLoadingStatus: AnnotationRequestStatus = Loading [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AnnotationsVisible: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Hovered: Annotation [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Mode: AnnotationEditingMode = None [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ResolvedLoadingStatus: AnnotationRequestStatus = Loading [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Selected: Annotation [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
CreateAnnotation(annotation: Annotation) → null [RobloxScriptSecurity]
DeleteAnnotation(annotation: Annotation) → null [RobloxScriptSecurity]
EditAnnotation(uniqueId: string, contents: string, taggedUsers: string) → null [RobloxScriptSecurity]
GetAnnotationThreads() → Instances [RobloxScriptSecurity]
LoadAnnotationReplies(annotation: Annotation, reverseOrder: bool, loadAll: bool) → null [RobloxScriptSecurity]
LoadAnnotations(resolved: bool) → null [RobloxScriptSecurity]
LoadResolvedAnnotations(count: int) → null [RobloxScriptSecurity] [Deprecated]
ResolveAnnotation(annotation: Annotation, resolved: bool) → null [RobloxScriptSecurity]
```

### Events
```
AnnotationAdded(requestId: string, annotation: Annotation, channelId: string) [RobloxScriptSecurity]
AnnotationDeleted(requestId: string, annotation: Annotation) [RobloxScriptSecurity]
AnnotationEdited(requestId: string, uniqueId: string, contents: string, taggedUsers: string) [RobloxScriptSecurity]
AnnotationResolved(requestId: string, annotation: Annotation, resolved: bool) [RobloxScriptSecurity]
ServerLoadAnnotationReplies(annotation: Annotation, reverseOrder: bool, loadAll: bool) [RobloxSecurity]
ServerLoadAnnotations(resolved: bool) [RobloxSecurity]
ServerLoadResolvedAnnotations(count: int) [RobloxSecurity]
```

---

## AppLifecycleObserverService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetCurrentState() → AppLifecycleManagerState [RobloxScriptSecurity]
IsDidDetachSupported() → bool [RobloxScriptSecurity]
TriggerOnLandingPageMount() → null [RobloxScriptSecurity]
TriggerOnLuaAppInteractive() → null [RobloxScriptSecurity]
```

### Events
```
OnBecomeActive() [RobloxScriptSecurity]
OnDetach() [RobloxScriptSecurity]
OnHide() [RobloxScriptSecurity]
OnResignActive() [RobloxScriptSecurity]
OnStart() [RobloxScriptSecurity]
OnUnhide() [RobloxScriptSecurity]
```

---

## AppUpdateService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
CanPerformBinaryUpdate() → bool [RobloxScriptSecurity]
CheckForUpdate(handler: Function) → null [RobloxScriptSecurity]
PerformManagedUpdate() → bool [RobloxScriptSecurity]
```

---

## AssetCounterService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## AssetDeliveryProxy
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
Interface: string
Port: int = 0
StartServer: bool = false
```

---

## AssetImportService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetAllPresets() → Dictionary [RobloxScriptSecurity]
GetPreset(name: string) → Dictionary [RobloxScriptSecurity]
RemovePreset(name: string) → null [RobloxScriptSecurity]
SavePreset(name: string, preset: Dictionary) → bool [RobloxScriptSecurity]
StartSessionWithPath(filePath: string) → AssetImportSession [RobloxScriptSecurity]
PickImageFileWithPrompt() → string [RobloxScriptSecurity]
PickMeshFileWithPrompt() → string [RobloxScriptSecurity]
PickMultipleFilesWithPrompt() → Array [RobloxScriptSecurity]
StartSessionWithPathAsync(filePath: string) → AssetImportSession [RobloxScriptSecurity]
```

---

## AssetManagerService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetMeshIdFromAliasName(aliasName: string) → int64 [RobloxScriptSecurity]
GetMeshIdFromAssetId(assetId: int64) → int64 [RobloxScriptSecurity]
GetTextureIdFromAliasName(aliasName: string) → int64 [RobloxScriptSecurity]
GetTextureIdFromAssetId(assetId: int64) → int64 [RobloxScriptSecurity]
InsertAudio(assetId: int64, assetName: string) → null [RobloxScriptSecurity]
InsertImage(assetId: int64) → null [RobloxScriptSecurity]
InsertImages(assetIds: Array) → null [RobloxScriptSecurity]
InsertMesh(aliasName: string, insertWithLocation: bool, sourceAssetId: int64) → null [RobloxScriptSecurity]
InsertMeshesWithLocation(aliasNames: Array, meshIds: Array) → null [RobloxScriptSecurity]
InsertModel(modelId: int64) → null [RobloxScriptSecurity]
InsertPackage(packageId: int64) → null [RobloxScriptSecurity]
InsertVideo(assetId: int64, assetName: string) → null [RobloxScriptSecurity]
OpenPlace(placeId: int64) → null [RobloxScriptSecurity]
ShowPackageDetails(packageId: int64) → null [RobloxScriptSecurity]
UpdateAllPackages(packageId: int64) → null [RobloxScriptSecurity]
ViewPackageOnWebsite(packageId: int64) → null [RobloxScriptSecurity]
AddNewPlace() → int64 [RobloxScriptSecurity]
CreateAlias(assetType: int, assetId: int64, aliasName: string) → null [RobloxScriptSecurity]
DeleteAlias(aliasName: string) → null [RobloxScriptSecurity]
RemovePlace(placeId: int64) → null [RobloxScriptSecurity]
RenameAlias(assetType: int, assetId: int64, oldAliasName: string, newAliasName: string) → null [RobloxScriptSecurity]
RenameModel(modelId: int64, newName: string) → null [RobloxScriptSecurity]
RenamePlace(placeId: int64, newName: string) → null [RobloxScriptSecurity]
```

### Events
```
AssetImportedSignal(assetType: AssetType, assetId: string, assetName: int64) [RobloxScriptSecurity]
ImportSessionFinished() [RobloxScriptSecurity]
ImportSessionStarted() [RobloxScriptSecurity]
```

---

## AssetPatchSettings
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
ContentId: string
OutputPath: string
PatchId: string
```

---

## AssetService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
CreateEditableImage(editableImageOptions: Dictionary?) → EditableImage
CreateEditableMesh(editableMeshOptions: Dictionary?) → EditableMesh
DeserializeInstance(serializedInstance: string) → Instance [RobloxScriptSecurity]
GetBundleDetailsSync(bundleId: int64) → Dictionary [RobloxScriptSecurity]
RegisterUGCValidationFunction(function: Function) → null [RobloxScriptSecurity]
CanEditAssetAsync(content: Content) → bool [RobloxScriptSecurity]
CreateAssetAsync(object: Object, assetType: AssetType, requestParameters: Dictionary) → Tuple
CreateAssetVersionAsync(object: Object, assetType: AssetType, assetId: int64, requestParameters: Dictionary) → Tuple
CreateEditableImageAsync(content: Content, editableImageOptions: Dictionary?) → EditableImage
CreateEditableMeshAsync(content: Content, editableMeshOptions: Dictionary?) → EditableMesh
CreateEditableMeshStripSkinningAsync(meshId: ContentId) → EditableMesh [RobloxScriptSecurity]
CreateMeshPartAsync(meshContent: Content, options: Dictionary) → MeshPart
CreatePlaceAsync(placeName: string, templatePlaceID: int64, description: string) → int64
CreatePlaceInPlayerInventoryAsync(player: Instance, placeName: string, templatePlaceID: int64, description: string) → int64
CreateSurfaceAppearanceAsync(content: Dictionary) → SurfaceAppearance
GetAssetIdsForPackage(packageAssetId: int64) → Array
GetAudioMetadataAsync(idList: Array) → Array
GetBundleDetailsAsync(bundleId: int64) → Dictionary
GetCreatorAssetID(creationID: int64) → int64 [Deprecated]
GetGamePlacesAsync() → Instance
PromptCreateAssetAsync(player: Player, instance: Instance, assetType: AssetType) → Tuple
PromptImportAnimationClipFromVideoAsync(player: Player, progressCallback: Function) → Tuple
SavePlaceAsync() → null
SearchAudio(searchParameters: AudioSearchParams) → AudioPages
```

### Events
```
AudioMetadataFailedResponse(requestid: int64) [RobloxScriptSecurity]
AudioMetadataRequest(requestid: int64, request: Array) [RobloxScriptSecurity]
AudioMetadataResponse(requestid: int64, response: Array) [RobloxScriptSecurity]
OpenCreateResultModal(resultType: PromptCreateAssetResult) [RobloxScriptSecurity]
OpenPublishResultModal(resultType: PromptPublishAssetResult) [RobloxScriptSecurity]
```

---

## Atmosphere
**Extends:** Instance

### Properties
```
Color: Color3 = 0.7843, 0.6667, 0.4235
Decay: Color3 = 0.3608, 0.2353, 0.0549
Density: float = 0.395000011
Glare: float = 0
Haze: float = 0
Offset: float = 0
```

---

## Attachment
**Extends:** Instance

### Properties
```
Axis: Vector3 = 1, 0, 0
CFrame: CFrame
Orientation: Vector3 = -0, 0, 0
Position: Vector3 = 0, 0, 0
Rotation: Vector3 = -0, 0, -0 [Deprecated]
SecondaryAxis: Vector3 = 0, 1, 0
Visible: bool = false
WorldAxis: Vector3 = 1, 0, 0
WorldCFrame: CFrame
WorldOrientation: Vector3 = -0, 0, 0
WorldPosition: Vector3 = 0, 0, 0
WorldRotation: Vector3 = -0, 0, -0 [ReadOnly] [Deprecated]
WorldSecondaryAxis: Vector3 = 0, 1, 0
```

### Functions
```
GetAxis() → Vector3 [Deprecated]
GetConstraints() → Instances
GetSecondaryAxis() → Vector3 [Deprecated]
SetAxis(axis: Vector3) → null [Deprecated]
SetSecondaryAxis(axis: Vector3) → null [Deprecated]
```

---

## Bone
**Extends:** Attachment

### Properties
```
Transform: CFrame
TransformedCFrame: CFrame [ReadOnly]
TransformedWorldCFrame: CFrame [ReadOnly]
```

---

## AudioAnalyzer
**Extends:** Instance

### Properties
```
PeakLevel: float = 0 [ReadOnly]
RmsLevel: float = 0 [ReadOnly]
SpectrumEnabled: bool = true
WindowSize: AudioWindowSize = Medium
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
GetSpectrum() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioChannelMixer
**Extends:** Instance

### Properties
```
Layout: AudioChannelLayout = Stereo
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioChannelSplitter
**Extends:** Instance

### Properties
```
Layout: AudioChannelLayout = Stereo
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioChorus
**Extends:** Instance

### Properties
```
Bypass: bool = false
Depth: float = 0.449999988
Mix: float = 0.850000024
Rate: float = 5
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioCompressor
**Extends:** Instance

### Properties
```
Attack: float = 0.100000001
Bypass: bool = false
Editor: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
MakeupGain: float = 0
Ratio: float = 40
Release: float = 0.100000001
Threshold: float = -40
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioDeviceInput
**Extends:** Instance

### Properties
```
AccessList: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
AccessType: AccessModifierType = Deny
Active: bool = true [Write:RobloxScriptSecurity]
IsReady: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Muted: bool = false
MutedByLocalUser: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Player: Player
Volume: float = 1
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
GetUserIdAccessList() → Array
SetUserIdAccessList(userIds: Array) → null
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioDeviceOutput
**Extends:** Instance

### Properties
```
Player: Player
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioDistortion
**Extends:** Instance

### Properties
```
Bypass: bool = false
Level: float = 0.5
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioEcho
**Extends:** Instance

### Properties
```
Bypass: bool = false
DelayTime: float = 1
DryLevel: float = 0
Feedback: float = 0.5
RampTime: float = 0
WetLevel: float = 0
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
Reset() → null [RobloxScriptSecurity]
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioEmitter
**Extends:** Instance

### Properties
```
AngleAttenuation: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
AudioInteractionGroup: string
DistanceAttenuation: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
PositionOverride: Instance [Read:RobloxSecurity] [Write:RobloxSecurity]
SimulationFidelity: AudioSimulationFidelity = Automatic
```

### Functions
```
GetAngleAttenuation() → Dictionary
GetAudibilityFor(listener: AudioListener) → float
GetConnectedWires(pin: string) → Instances
GetDistanceAttenuation() → Dictionary
GetInputPins() → Array
GetInteractingListeners() → Instances
GetOutputPins() → Array
SetAngleAttenuation(curve: Dictionary) → null
SetDistanceAttenuation(curve: Dictionary) → null
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioEqualizer
**Extends:** Instance

### Properties
```
Bypass: bool = false
Editor: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
HighGain: float = 0
LowGain: float = 0
MidGain: float = 0
MidRange: NumberRange = 400 4000 
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioFader
**Extends:** Instance

### Properties
```
Bypass: bool = false
Volume: float = 1
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioFilter
**Extends:** Instance

### Properties
```
Bypass: bool = false
Editor: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
FilterType: AudioFilterType = Peak
Frequency: float = 2000
Gain: float = 0
Q: float = 0.707000017
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetGainAt(frequency: float) → float
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioFlanger
**Extends:** Instance

### Properties
```
Bypass: bool = false
Depth: float = 0.449999988
Mix: float = 0.850000024
Rate: float = 5
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioFocusService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
AcquireFocus(contextId: int) → bool [RobloxScriptSecurity]
GetFocusedContextId() → int [RobloxScriptSecurity]
GetRegisteredContexts() → Array [RobloxScriptSecurity]
RegisterContextIdFromLua(contextId: int) → null [RobloxScriptSecurity]
RequestFocus(contextId: int, priority: int) → bool [RobloxScriptSecurity]
```

### Events
```
OnContextRegistered(contextId: int) [RobloxScriptSecurity]
OnContextUnregistered(contextId: int) [RobloxScriptSecurity]
OnDeafenVoiceAudio(contextId: int) [RobloxScriptSecurity]
OnUndeafenVoiceAudio(contextId: int) [RobloxScriptSecurity]
```

---

## AudioGate
**Extends:** Instance

### Properties
```
Attack: float = 0.00999999978
Bypass: bool = false
Release: float = 0.100000001
Threshold: NumberRange = -36 -24 
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
Reset() → null [RobloxScriptSecurity]
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioLimiter
**Extends:** Instance

### Properties
```
Bypass: bool = false
Editor: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
MaxLevel: float = 0
Release: float = 0.00999999978
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioListener
**Extends:** Instance

### Properties
```
AngleAttenuation: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
AudioInteractionGroup: string
DistanceAttenuation: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
PositionOverride: Instance [Read:RobloxSecurity] [Write:RobloxSecurity]
SimulationFidelity: AudioSimulationFidelity = Automatic
```

### Functions
```
GetAngleAttenuation() → Dictionary
GetAudibilityFor(emitter: AudioEmitter) → float
GetConnectedWires(pin: string) → Instances
GetDistanceAttenuation() → Dictionary
GetInputPins() → Array
GetInteractingEmitters() → Instances
GetOutputPins() → Array
Reset() → null [RobloxScriptSecurity]
SetAngleAttenuation(curve: Dictionary) → null
SetDistanceAttenuation(curve: Dictionary) → null
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioPitchShifter
**Extends:** Instance

### Properties
```
Bypass: bool = false
Pitch: float = 1.25
WindowSize: AudioWindowSize = Medium
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioPlayer
**Extends:** Instance

### Properties
```
Asset: ContentId
AssetId: string [Deprecated]
AutoLoad: bool = true
IsMutedForCapture: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
IsPlaying: bool = false [Write:RobloxSecurity]
IsReady: bool = false [ReadOnly]
LoopRegion: NumberRange = 0 60000 
Looping: bool = false
PlaybackRegion: NumberRange = 0 60000 
PlaybackSpeed: double = 1
TimeLength: double = 0 [ReadOnly]
TimePosition: double = 0
Volume: float = 1
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
Play() → null
Stop() → null
GetWaveformAsync(timeRange: NumberRange, samples: int) → Array
```

### Events
```
Ended()
Looped()
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioRecorder
**Extends:** Instance
**Tags:** NotBrowsable

### Properties
```
IsRecording: bool = false [Write:RobloxSecurity]
TimeLength: double = 0 [ReadOnly]
```

### Functions
```
Clear() → null
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
GetTemporaryContent() → Content
Stop() → null
CanRecordAsync() → bool
GetUnrecordableInstancesAsync() → Instances
RecordAsync() → null
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioReverb
**Extends:** Instance

### Properties
```
Bypass: bool = false
DecayRatio: float = 0.5
DecayTime: float = 1.5
Density: float = 1
Diffusion: float = 1
DryLevel: float = 0
EarlyDelayTime: float = 0.0199999996
HighCutFrequency: float = 20000
LateDelayTime: float = 0.0399999991
LowShelfFrequency: float = 250
LowShelfGain: float = 0
ReferenceFrequency: float = 5000
WetLevel: float = -6
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
Reset() → null [RobloxScriptSecurity]
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioSearchParams
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
Album: string
Artist: string
AudioSubType: AudioSubType = Music
AudioSubtype: AudioSubType = Music [Deprecated]
MaxDuration: int = 2147483647
MinDuration: int = 0
SearchKeyword: string
Tag: string
Title: string
```

---

## AudioSpeechToText
**Extends:** Instance
**Tags:** NotBrowsable

### Properties
```
Enabled: bool = false
Text: string
VoiceDetected: bool = false [ReadOnly]
```

### Functions
```
GetConnectedWires(pin: string) → Instances
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AudioTextToSpeech
**Extends:** Instance

### Properties
```
IsLoaded: bool = false [ReadOnly]
IsPlaying: bool = false [Write:RobloxSecurity]
Looping: bool = false
Pitch: float = 0
PlaybackSpeed: float = 1
Speed: float = 1
Text: string
TimeLength: double = 0 [ReadOnly]
TimePosition: double = 0
VoiceId: string
Volume: float = 1
```

### Functions
```
GetConnectedWires(pin: string) → Instances
Pause() → null
Play() → null
Unload() → null
GetWaveformAsync(timeRange: NumberRange, samples: int) → Array
LoadAsync() → AssetFetchStatus
```

### Events
```
Ended()
Looped()
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## AuroraScriptObject
**Extends:** Instance
**Tags:** NotCreatable, Deprecated

### Properties
```
BehaviorWeak: AuroraScript [Read:RobloxSecurity] [Write:RobloxSecurity]
BoundInstanceWeak: Instance [Read:RobloxSecurity] [Write:RobloxSecurity]
FrameId: int
LODLevel: int
MaxFrequency: int
PriorFrameInvoked: int
```

---

## AuroraScriptService
**Extends:** Instance
**Tags:** NotCreatable, Service, Deprecated

### Functions
```
GetLocalFrameId() → int
SendMessage(instance: Instance, behaviorName: string, functionName: string, args: Tuple) → null
```

---

## AuroraService
**Extends:** Instance
**Tags:** NotCreatable, Service, Deprecated

### Properties
```
BufferFullInputCount: int [Read:RobloxSecurity] [Write:RobloxSecurity]
HashRoundingPoint: double
IgnoreRotation: bool
InputDropRate: float [Read:RobloxSecurity] [Write:RobloxSecurity]
LockStepIdOffset: bool
OutOfOrderInputCount: int [Read:RobloxSecurity] [Write:RobloxSecurity]
RCCHeartbeatFPS: double [Read:RobloxSecurity] [Write:RobloxSecurity]
RollbackOffset: int
TooOldInputCount: int [Read:RobloxSecurity] [Write:RobloxSecurity]
```

### Functions
```
GetPredictedInstances() → Array
GetRemoteWorldStepId() → int
GetServerView(target: Instance) → Instance
GetWorldStepId() → int
IsPredicted(target: Instance) → bool
PlayInputRecording() → null
SetIncomingReplicationLag(seconds: float) → null
SetPropertyIsInput(target: Instance, propertyName: string, isInput: bool) → null
ShowDebugVisualizer(state: bool) → null
StartInputRecording() → null
StartPrediction(target: Instance) → null
StepPhysics(worldSteps: int, parts: Instances) → null
StopInputRecording() → null
StopPrediction(target: Instance) → null
UpdateProperties(target: Instance) → null
```

### Events
```
FixedRateTick(deltaTime: double, worldStepId: int)
Misprediction(worldStepId: int, mispredictedInstances: Array)
Rollback(worldStepId: int)
Step()
```

---

## AvatarAccessoryRules
**Extends:** Instance

### Properties
```
AccessoryMode: AvatarSettingsAccessoryMode = PlayerChoice [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomAccessoryMode: AvatarSettingsCustomAccessoryMode = PlayerChoice [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomBackAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomBackAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomFaceAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomFaceAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomFrontAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomFrontAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomHairAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomHairAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomHeadAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomHeadAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomNeckAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomNeckAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomShoulderAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomShoulderAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomWaistAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomWaistAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
EnableSound: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
EnableVFX: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LimitBounds: Vector3 = 0, 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LimitMethod: AvatarSettingsAccessoryLimitMethod = Remove [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
willRemoveAccessory(humanoid: Humanoid, accessory: Accoutrement) → bool [RobloxScriptSecurity]
```

---

## AvatarAnimationRules
**Extends:** Instance

### Properties
```
AnimationClipsMode: AvatarSettingsAnimationClipsMode = PlayerChoice [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AnimationPacksMode: AvatarSettingsAnimationPacksMode = PlayerChoice [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomClimbAnimationEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomClimbAnimationId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomFallAnimationEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomFallAnimationId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomIdleAlt1AnimationEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomIdleAlt1AnimationId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomIdleAlt2AnimationEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomIdleAlt2AnimationId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomIdleAnimationEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomIdleAnimationId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomJumpAnimationEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomJumpAnimationId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomRunAnimationEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomRunAnimationId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomSwimAnimationEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomSwimAnimationId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomSwimIdleAnimationEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomSwimIdleAnimationId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomWalkAnimationEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomWalkAnimationId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

---

## AvatarBodyRules
**Extends:** Instance

### Properties
```
AppearanceMode: AvatarSettingsAppearanceMode = PlayerChoice [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
BuildMode: AvatarSettingsBuildMode = PlayerChoice [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomBodyBundleId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomBodyType: AvatarSettingsCustomBodyType = AvatarReference [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomBodyTypeScale: NumberRange = 0 1  [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomEyebrowEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomEyebrowId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomEyelashEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomEyelashId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomFaceEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomFaceId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomHeadEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomHeadId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomHeadScale: NumberRange = 0.95 1  [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomHeight: NumberRange = 5.5 5.5  [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomHeightScale: NumberRange = 0.9 1.05  [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomLeftArmEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomLeftArmId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomLeftLegEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomLeftLegId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomMoodEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomMoodId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomProportionsScale: NumberRange = 0 1  [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomRightArmEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomRightArmId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomRightLegEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomRightLegId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomTorsoEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomTorsoId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomWidthScale: NumberRange = 0.7 1  [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
KeepPlayerHead: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ScaleMode: AvatarSettingsScaleMode = PlayerChoice [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

---

## AvatarChatService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
ClientFeatures: int = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
ClientFeaturesInitialized: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
ServerFeatures: int = 0 [Read:RobloxScriptSecurity] [Write:RobloxSecurity]
```

### Functions
```
DebugCounterGet(label: string, playerId: int64) → int64 [RobloxScriptSecurity]
EnableVoice() → bool [RobloxScriptSecurity]
IsEnabled(mask: int, feature: AvatarChatServiceFeature) → bool [RobloxScriptSecurity]
IsPlaceEnabled() → bool [RobloxScriptSecurity]
IsUniverseEnabled() → bool [RobloxScriptSecurity]
PollClientFeatures() → int [RobloxScriptSecurity]
PollServerFeatures() → int [RobloxScriptSecurity]
deviceMeetsRequirementsForFeature(feature: DeviceFeatureType) → bool [RobloxScriptSecurity]
GetClientFeaturesAsync() → int [RobloxScriptSecurity]
GetServerFeaturesAsync() → int [RobloxScriptSecurity]
```

### Events
```
OnClientFeatures(features: int) [RobloxSecurity]
RefreshClientFeatures() [RobloxSecurity]
```

---

## AvatarClothingRules
**Extends:** Instance

### Properties
```
ClothingMode: AvatarSettingsClothingMode = PlayerChoice [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomClassicPantsAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomClassicPantsAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomClassicShirtsAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomClassicShirtsAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomClassicTShirtsAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomClassicTShirtsAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomClothingMode: AvatarSettingsCustomClothingMode = PlayerChoice [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomDressSkirtAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomDressSkirtAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomJacketAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomJacketAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomLeftShoesAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomLeftShoesAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomPantsAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomPantsAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomRightShoesAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomRightShoesAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomShirtAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomShirtAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomShortsAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomShortsAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomSweaterAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomSweaterAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomTShirtAccessoryEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CustomTShirtAccessoryId: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LimitBounds: Vector3 = 0, 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

---

## AvatarCollisionRules
**Extends:** Instance

### Properties
```
CollisionMode: AvatarSettingsCollisionMode = Default [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
HitAndTouchDetectionMode: AvatarSettingsHitAndTouchDetectionMode = UseParts [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LegacyCollisionMode: AvatarSettingsLegacyCollisionMode = InnerBoxColliders [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
SingleColliderSize: Vector3 = 2, 4, 1 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

---

## AvatarCreationService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
DeserializeAvatarModel(serializedModel: string) → Instance [RobloxScriptSecurity]
GetValidationRules() → Dictionary
AutoSetupAvatarAsync(player: Player, model: Model, progressCallback: Function?) → string
GenerateAvatar2DPreviewAsync(avatarGeneration2dPreviewParams: Dictionary) → string
GenerateAvatarAsync(avatarGenerationParams: Dictionary) → string
GetBatchTokenDetailsAsync(tokenIds: Array) → Array
LoadAvatar2DPreviewAsync(previewId: string) → EditableImage
LoadGeneratedAvatarAsync(generationId: string) → HumanoidDescription
PrepareAvatarForPreviewAsync(humanoidModel: Model) → null
PromptCreateAvatarAsync(tokenId: string, player: Player, humanoidDescription: HumanoidDescription) → Tuple
PromptSelectAvatarGenerationImageAsync(player: Player) → string
RequestAvatarGenerationSessionAsync(player: Player, callback: Function) → Tuple
ValidateUGCAccessoryAsync(player: Player, accessory: Instance, accessoryType: AccessoryType) → Tuple
ValidateUGCBodyPartAsync(player: Player, instance: Instance, bodyPart: BodyPart) → Tuple
ValidateUGCFullBodyAsync(player: Player, humanoidDescription: HumanoidDescription) → Tuple
```

### Events
```
AvatarModerationCompleted(outfitId: int64, moderationStatus: ModerationStatus)
ReplicateAvatarGenerationImageId(fileId: string, error: string) [RobloxSecurity]
ReplicateAvatarModel(id: string, success: bool, serializedModel: string, bufferTable: Dictionary) [RobloxSecurity]
ReplicateAvatarPreviewUrl(id: string, downloadUrl: string) [RobloxSecurity]
RequestAvatarGenerationImage() [RobloxSecurity]
RequestAvatarModel(id: string) [RobloxSecurity]
RequestAvatarPreviewUrl(id: string) [RobloxSecurity]
UgcValidationFailure(guid: string, errorMessage: string) [RobloxScriptSecurity]
UgcValidationSuccess(guid: string, serializedModel: string, price: int64) [RobloxScriptSecurity]
```

---

## AvatarEditorService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetAccessoryType(avatarAssetType: AvatarAssetType) → AccessoryType
NoPromptCreateOutfit(humanoidDescription: HumanoidDescription, rigType: HumanoidRigType, name: string, gearAssetId: int64) → bool [RobloxScriptSecurity]
NoPromptDeleteOutfit(outfitId: int64) → bool [RobloxScriptSecurity]
NoPromptRenameOutfit(outfitId: int64, name: string) → bool [RobloxScriptSecurity]
NoPromptSaveAvatar(humanoidDescription: HumanoidDescription, rigType: HumanoidRigType, saveDict: Dictionary, gearAssetId: int64) → bool [RobloxScriptSecurity]
NoPromptSaveAvatarThumbnailCustomization(thumbnailType: AvatarThumbnailCustomizationType, emoteAssetId: int64, cameraDistanceScale: float, yRotDeg: float, fieldOfViewDeg: float) → bool [RobloxScriptSecurity]
NoPromptSetFavorite(itemId: int64, itemType: AvatarItemType, shouldFavorite: bool) → bool [RobloxScriptSecurity]
NoPromptUpdateOutfit(outfitId: int64, humanoidDescription: HumanoidDescription, rigType: HumanoidRigType, gearAssetId: int64) → bool [RobloxScriptSecurity]
PerformCreateOutfitWithDescription(humanoidDescription: HumanoidDescription, name: string) → null [RobloxScriptSecurity]
PerformDeleteOutfit() → null [RobloxScriptSecurity]
PerformRenameOutfit(name: string) → null [RobloxScriptSecurity]
PerformSaveAvatarWithDescription(humanoidDescription: HumanoidDescription, addedAssets: Array, removedAssets: Array) → null [RobloxScriptSecurity]
PerformSetFavorite() → null [RobloxScriptSecurity]
PerformUpdateOutfit(humanoidDescription: HumanoidDescription) → null [RobloxScriptSecurity]
PromptAllowInventoryReadAccess() → null
PromptCreateOutfit(outfit: HumanoidDescription, rigType: HumanoidRigType) → null
PromptDeleteOutfit(outfitId: int64) → null
PromptRenameOutfit(outfitId: int64) → null
PromptSaveAvatar(humanoidDescription: HumanoidDescription, rigType: HumanoidRigType) → null
PromptSetFavorite(itemId: int64, itemType: AvatarItemType, shouldFavorite: bool) → null
PromptUpdateOutfit(outfitId: int64, updatedOutfit: HumanoidDescription, rigType: HumanoidRigType) → null
SetAllowInventoryReadAccess(inventoryReadAccessGranted: bool) → null [RobloxScriptSecurity]
SignalCreateOutfitFailed() → null [RobloxScriptSecurity]
SignalCreateOutfitPermissionDenied() → null [RobloxScriptSecurity]
SignalDeleteOutfitFailed() → null [RobloxScriptSecurity]
SignalDeleteOutfitPermissionDenied() → null [RobloxScriptSecurity]
SignalRenameOutfitFailed() → null [RobloxScriptSecurity]
SignalRenameOutfitPermissionDenied() → null [RobloxScriptSecurity]
SignalSaveAvatarFailed() → null [RobloxScriptSecurity]
SignalSaveAvatarPermissionDenied() → null [RobloxScriptSecurity]
SignalSetFavoriteFailed() → null [RobloxScriptSecurity]
SignalSetFavoritePermissionDenied() → null [RobloxScriptSecurity]
SignalUpdateOutfitFailed() → null [RobloxScriptSecurity]
SignalUpdateOutfitPermissionDenied() → null [RobloxScriptSecurity]
refreshAvatarThumbnails(thumbnailTypes: Array) → null [RobloxScriptSecurity]
CheckApplyDefaultClothing(humanoidDescription: HumanoidDescription) → HumanoidDescription
ConformToAvatarRules(humanoidDescription: HumanoidDescription) → HumanoidDescription
GetAvatarRules() → Dictionary
GetBatchItemDetails(itemIds: Array, itemType: AvatarItemType) → Array
GetFavorite(itemId: int64, itemType: AvatarItemType) → bool
GetInventory(assetTypes: Array) → InventoryPages
GetItemDetails(itemId: int64, itemType: AvatarItemType) → Dictionary
GetOutfitDetails(outfitId: int64) → Dictionary
GetOutfits(outfitSource: OutfitSource, outfitType: OutfitType) → OutfitPages
GetRecommendedAssets(assetType: AvatarAssetType, contextAssetId: int64) → Array
GetRecommendedBundles(bundleId: int64) → Array
SearchCatalog(searchParameters: CatalogSearchParams) → CatalogPages
```

### Events
```
OpenAllowInventoryReadAccess() [RobloxScriptSecurity]
OpenPromptCreateOufit(humanoidDescription: HumanoidDescription, rigType: HumanoidRigType) [RobloxScriptSecurity]
OpenPromptDeleteOutfit(outfitId: int64) [RobloxScriptSecurity]
OpenPromptRenameOutfit(outfitId: int64) [RobloxScriptSecurity]
OpenPromptSaveAvatar(humanoidDescription: HumanoidDescription, rigType: HumanoidRigType) [RobloxScriptSecurity]
OpenPromptSetFavorite(itemId: int64, itemType: AvatarItemType, shouldFavorite: bool) [RobloxScriptSecurity]
OpenPromptUpdateOutfit(outfitId: int64, humanoidDescription: HumanoidDescription, rigType: HumanoidRigType) [RobloxScriptSecurity]
PromptAllowInventoryReadAccessCompleted(result: AvatarPromptResult)
PromptCreateOutfitCompleted(result: AvatarPromptResult, failureType: Variant)
PromptDeleteOutfitCompleted(result: AvatarPromptResult)
PromptRenameOutfitCompleted(result: AvatarPromptResult)
PromptSaveAvatarCompleted(result: AvatarPromptResult, humanoidDescription: HumanoidDescription)
PromptSaveAvatarThumbnailCustomizationCompleted(result: AvatarPromptResult, failureType: Variant) [RobloxScriptSecurity]
PromptSetFavoriteCompleted(result: AvatarPromptResult)
PromptUpdateOutfitCompleted(result: AvatarPromptResult)
```

---

## AvatarImportService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
ImportFBXAnimationFromFilePathUserMayChooseModel(fbxFilePath: string, selectedRig: Instance, userChooseModelThenImportCB: Function) → Instance [RobloxScriptSecurity]
ImportFBXAnimationUserMayChooseModel(selectedRig: Instance, userChooseModelThenImportCB: Function) → Instance [RobloxScriptSecurity]
ImportFbxRigWithoutSceneLoad(isR15: bool) → Instance [RobloxScriptSecurity]
ImportLoadedFBXAnimation(useFBXModel: bool) → Instance [RobloxScriptSecurity]
LoadRigAndDetectType(promptR15Callback: Function) → Instance [RobloxScriptSecurity]
```

---

## AvatarPreloader
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
PreloadModelAssets(models: Instances) → Array [RobloxScriptSecurity]
```

---

## AvatarRules
**Extends:** Instance

### Properties
```
AvatarType: GameAvatarType = R15 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

---

## AvatarSettings
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
Loaded: bool = false [Read:RobloxScriptSecurity] [Write:NotAccessibleSecurity]
```

### Functions
```
Discard() → null [RobloxScriptSecurity]
Publish() → null [RobloxScriptSecurity]
```

### Events
```
DiscardRequested() [RobloxSecurity]
RefreshPluginState() [RobloxScriptSecurity]
```

---

## Backpack
**Extends:** Instance

---

## BadgeService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
AwardBadge(userId: int64, badgeId: int64) → bool
CheckUserBadgesAsync(userId: int64, badgeIds: Array) → Array
GetBadgeInfoAsync(badgeId: int64) → Dictionary
IsDisabled(badgeId: int64) → bool [Deprecated]
IsLegal(badgeId: int64) → bool [Deprecated]
UserHasBadge(userId: int64, badgeId: int64) → bool [Deprecated]
UserHasBadgeAsync(userId: int64, badgeId: int64) → bool
```

### Events
```
BadgeAwarded(message: string, userId: int64, badgeId: int64) [RobloxScriptSecurity]
OnBadgeAwarded(userId: int64, creatorId: int64, badgeId: int64) [RobloxScriptSecurity]
```

---

## BaseImportData
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
Id: string [ReadOnly]
ImportName: string
ShouldImport: bool
```

### Functions
```
CreatePresetFromData() → Dictionary [RobloxScriptSecurity]
GetPreview() → Instance [RobloxScriptSecurity]
GetStatuses() → Dictionary [RobloxScriptSecurity]
```

### Events
```
StatusRemoved(status: Dictionary)
StatusReported(status: Dictionary)
```

---

## AnimationImportData
**Extends:** BaseImportData
**Tags:** NotCreatable, NotReplicated

---

## FacsImportData
**Extends:** BaseImportData
**Tags:** NotCreatable, NotReplicated

---

## GroupImportData
**Extends:** BaseImportData
**Tags:** NotCreatable, NotReplicated

### Properties
```
Anchored: bool
ImportAsModelAsset: bool
InsertInWorkspace: bool
```

---

## JointImportData
**Extends:** BaseImportData
**Tags:** NotCreatable, NotReplicated

---

## MaterialImportData
**Extends:** BaseImportData
**Tags:** NotCreatable, NotReplicated

### Properties
```
DiffuseFilePath: string
IsPbr: bool [ReadOnly]
MetalnessFilePath: string
NormalFilePath: string
RoughnessFilePath: string
```

---

## MeshImportData
**Extends:** BaseImportData
**Tags:** NotCreatable, NotReplicated

### Properties
```
Anchored: bool
CageManifold: bool [ReadOnly]
CageMeshIntersectedPreview: bool
CageMeshNotIntersected: bool [ReadOnly]
CageNoOverlappingVertices: bool [ReadOnly]
CageNonManifoldPreview: bool
CageOverlappingVerticesPreview: bool
CageUVMatched: bool [ReadOnly]
CageUVMisMatchedPreview: bool
Dimensions: Vector3 [ReadOnly]
DoubleSided: bool
IgnoreVertexColors: bool
IrrelevantCageModifiedPreview: bool
MeshHoleDetectedPreview: bool
MeshNoHoleDetected: bool [ReadOnly]
NoIrrelevantCageModified: bool [ReadOnly]
NoOuterCageFarExtendedFromMesh: bool [ReadOnly]
OuterCageFarExtendedFromMeshPreview: bool
PolygonCount: float [ReadOnly]
UseImportedPivot: bool
```

---

## RootImportData
**Extends:** BaseImportData
**Tags:** NotCreatable, NotReplicated

### Properties
```
AddModelToInventory: bool
Anchored: bool
AnimationIdForRestPose: float
ExistingPackageId: string
FileDimensions: Vector3 [ReadOnly]
ImportAsModelAsset: bool
ImportAsPackage: bool
InsertInWorkspace: bool
InsertWithScenePosition: bool
InvertNegativeFaces: bool
KeepZeroInfluenceBones: bool
MergeMeshes: bool
PolygonCount: float [ReadOnly]
PreferredUploadId: int64
RestPose: RestPose
RigScale: RigScale
RigType: RigType
RigVisualization: bool
ScaleUnit: MeshScaleUnit
UseSceneOriginAsPivot: bool
UsesCages: bool
ValidateUgcBody: bool
WorldForward: NormalId
WorldUp: NormalId
```

---

## BasePlayerGui
**Extends:** Instance
**Tags:** NotCreatable

### Functions
```
GetGuiObjectsAtPosition(x: int, y: int) → Instances
GetGuiObjectsInCircle(position: Vector2, radius: float) → Instances [RobloxScriptSecurity]
```

---

## CoreGui
**Extends:** BasePlayerGui
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
SelectionImageObject: GuiObject [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Version: int [ReadOnly]
```

### Functions
```
SetUserGuiRendering(enabled: bool, guiAdornee: Instance, faceId: NormalId, horizontalCurvature: float) → null [RobloxScriptSecurity]
TakeScreenshot() → null [RobloxScriptSecurity]
ToggleRecording() → null [RobloxScriptSecurity]
```

### Events
```
UserGuiRenderingChanged(enabled: bool, guiAdornee: Instance, faceId: NormalId, horizontalCurvature: float) [RobloxScriptSecurity]
```

---

## PlayerGui
**Extends:** BasePlayerGui
**Tags:** NotCreatable, PlayerReplicated

### Properties
```
CurrentScreenOrientation: ScreenOrientation = LandscapeLeft [ReadOnly]
ScreenOrientation: ScreenOrientation = LandscapeSensor
SelectionImageObject: GuiObject
```

### Functions
```
GetTopbarTransparency() → float [Deprecated]
SetTopbarTransparency(transparency: float) → null [Deprecated]
```

### Events
```
TopbarTransparencyChangedSignal(transparency: float)
```

---

## StarterGui
**Extends:** BasePlayerGui
**Tags:** NotCreatable, Service

### Properties
```
ProcessUserInput: bool [Read:PluginSecurity] [Write:PluginSecurity]
ResetPlayerGuiOnSpawn: bool [Deprecated]
RtlTextSupport: RtlTextSupport
ScreenOrientation: ScreenOrientation
ShowDevelopmentGui: bool
StudioDefaultStyleSheet: StyleSheet [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
StudioInsertWidgetLayerCollectorAutoLinkStyleSheet: StyleSheet [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
VirtualCursorMode: VirtualCursorMode
```

### Functions
```
GetCoreGuiEnabled(coreGuiType: CoreGuiType) → bool
RegisterGetCore(parameterName: string, getFunction: Function) → null [RobloxScriptSecurity]
RegisterSetCore(parameterName: string, setFunction: Function) → null [RobloxScriptSecurity]
SetCore(parameterName: string, value: Variant) → null
SetCoreGuiEnabled(coreGuiType: CoreGuiType, enabled: bool) → null
GetCore(parameterName: string) → Variant
```

### Events
```
CoreGuiChangedSignal(coreGuiType: CoreGuiType, enabled: bool) [RobloxScriptSecurity]
```

---

## BaseRemoteEvent
**Extends:** Instance
**Tags:** NotCreatable

---

## RemoteEvent
**Extends:** BaseRemoteEvent

### Functions
```
FireAllClients(arguments: Tuple) → null
FireClient(player: Player, arguments: Tuple) → null
FireServer(arguments: Tuple) → null
```

### Events
```
OnClientEvent(arguments: Tuple)
OnRemoteServerEvent(arguments: Tuple) [RobloxSecurity]
OnServerEvent(player: Player, arguments: Tuple)
```

---

## UnreliableRemoteEvent
**Extends:** BaseRemoteEvent

### Functions
```
FireAllClients(arguments: Tuple) → null
FireClient(player: Player, arguments: Tuple) → null
FireServer(arguments: Tuple) → null
```

### Events
```
OnClientEvent(arguments: Tuple)
OnRemoteServerEvent(arguments: Tuple) [RobloxSecurity]
OnServerEvent(player: Player, arguments: Tuple)
```

---

## BaseWrap
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
CageMeshContent: Content [Write:PluginSecurity]
CageMeshId: ContentId [Write:PluginSecurity]
CageOrigin: CFrame [Write:PluginSecurity]
CageOriginWorld: CFrame [ReadOnly]
HSRAssetId: ContentId [Read:RobloxSecurity] [Write:RobloxSecurity]
HSRData: SharedString [Read:RobloxSecurity] [Write:RobloxSecurity]
HSRMeshIdData: SharedString [Read:RobloxSecurity] [Write:RobloxSecurity]
ImportInProcess: bool [Write:RobloxScriptSecurity]
ImportOrigin: CFrame [Write:PluginSecurity]
ImportOriginWorld: CFrame [ReadOnly]
TemporaryCageMeshId: ContentId [Read:RobloxSecurity] [Write:RobloxSecurity]
```

### Functions
```
GetCageOffset() → Vector3 [RobloxScriptSecurity]
GetFaces(cageType: CageType) → Array [RobloxScriptSecurity]
GetUVs(cageType: CageType) → Array [RobloxScriptSecurity]
GetVertices(cageType: CageType) → Array [RobloxScriptSecurity]
IsHSRReady() → bool [RobloxScriptSecurity]
ModifyVertices(cageType: CageType, vertices: Array) → null [RobloxScriptSecurity]
```

### Events
```
VerticesModified(vertices: Array) [RobloxScriptSecurity]
```

---

## WrapDeformer
**Extends:** BaseWrap

### Functions
```
SetCageMeshContent(content: Content, cageOrigin: CoordinateFrame?) → null
CreateEditableMeshAsync() → EditableMesh
GetDeformedCFrameAsync(originalCFrame: CFrame) → CFrame
```

---

## WrapLayer
**Extends:** BaseWrap

### Properties
```
AutoSkin: WrapLayerAutoSkin = Disabled
BindOffset: CFrame [Write:PluginSecurity]
Color: Color3 = 1, 1, 1
DebugMode: WrapLayerDebugMode = None
Enabled: bool = true
MaxSize: Vector3 = 0, 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Offset: Vector3 = 0, 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Order: int = 1
Puffiness: float = 1
ReferenceMeshContent: Content [Write:PluginSecurity]
ReferenceMeshId: ContentId [Write:PluginSecurity]
ReferenceOrigin: CFrame [Write:PluginSecurity]
ReferenceOriginWorld: CFrame [ReadOnly]
ShrinkFactor: float = 0 [Write:PluginSecurity]
TemporaryReferenceId: ContentId [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## WrapTarget
**Extends:** BaseWrap

### Properties
```
Color: Color3 = 1, 1, 1
DebugMode: WrapTargetDebugMode = None
Stiffness: float = 0 [Write:PluginSecurity]
```

---

## Beam
**Extends:** Instance

### Properties
```
Attachment0: Attachment
Attachment1: Attachment
Brightness: float = 1
Color: ColorSequence = 0 1 1 1 0 1 1 1 1 0 
CurveSize0: float = 0
CurveSize1: float = 0
Enabled: bool = true
FaceCamera: bool = false
LightEmission: float = 0
LightInfluence: float = 0
LocalTransparencyModifier: float = 0
Segments: int = 10
Texture: ContentId
TextureLength: float = 1
TextureMode: TextureMode = Stretch
TextureSpeed: float = 1
Transparency: NumberSequence = 0 0.5 0 1 0.5 0 
Width0: float = 1
Width1: float = 1
ZOffset: float = 0
```

### Functions
```
SetTextureOffset(offset: float) → null
```

---

## BindableEvent
**Extends:** Instance

### Functions
```
Fire(arguments: Tuple) → null
```

### Events
```
Event(arguments: Tuple)
```

---

## BindableFunction
**Extends:** Instance

### Functions
```
Invoke(arguments: Tuple) → Tuple
```

---

## BodyMover
**Extends:** Instance
**Tags:** NotCreatable, Deprecated

---

## BodyAngularVelocity
**Extends:** BodyMover
**Tags:** Deprecated

### Properties
```
AngularVelocity: Vector3 = 0, 2, 0
MaxTorque: Vector3 = 4000, 4000, 4000
P: float = 1250
angularvelocity: Vector3 = 0, 2, 0 [Deprecated]
maxTorque: Vector3 = 4000, 4000, 4000 [Deprecated]
```

---

## BodyForce
**Extends:** BodyMover
**Tags:** Deprecated

### Properties
```
Force: Vector3 = 0, 1, 0
force: Vector3 = 0, 1, 0 [Deprecated]
```

---

## BodyGyro
**Extends:** BodyMover
**Tags:** Deprecated

### Properties
```
CFrame: CFrame
D: float = 500
MaxTorque: Vector3 = 400000, 0, 400000
P: float = 3000
cframe: CFrame [Deprecated]
maxTorque: Vector3 = 400000, 0, 400000 [Deprecated]
```

---

## BodyPosition
**Extends:** BodyMover
**Tags:** Deprecated

### Properties
```
D: float = 1250
MaxForce: Vector3 = 4000, 4000, 4000
P: float = 10000
Position: Vector3 = 0, 50, 0
maxForce: Vector3 = 4000, 4000, 4000 [Deprecated]
position: Vector3 = 0, 50, 0 [Deprecated]
```

### Functions
```
GetLastForce() → Vector3
lastForce() → Vector3 [Deprecated]
```

### Events
```
ReachedTarget()
```

---

## BodyThrust
**Extends:** BodyMover
**Tags:** Deprecated

### Properties
```
Force: Vector3 = 0, 1, 0
Location: Vector3 = 0, 0, 0
force: Vector3 = 0, 1, 0 [Deprecated]
location: Vector3 = 0, 0, 0 [Deprecated]
```

---

## BodyVelocity
**Extends:** BodyMover
**Tags:** Deprecated

### Properties
```
MaxForce: Vector3 = 4000, 4000, 4000
P: float = 1250
Velocity: Vector3 = 0, 2, 0
maxForce: Vector3 = 4000, 4000, 4000 [Deprecated]
velocity: Vector3 = 0, 2, 0 [Deprecated]
```

### Functions
```
GetLastForce() → Vector3
lastForce() → Vector3
```

---

## RocketPropulsion
**Extends:** BodyMover
**Tags:** Deprecated

### Properties
```
Active: bool = false
CartoonFactor: float = 0.699999988
MaxSpeed: float = 30
MaxThrust: float = 4000
MaxTorque: Vector3 = 400000, 400000, 0
Target: BasePart
TargetOffset: Vector3 = 0, 0, 0
TargetRadius: float = 4
ThrustD: float = 0.00100000005
ThrustP: float = 5
TurnD: float = 500
TurnP: float = 3000
```

### Functions
```
Abort() → null
Fire() → null
fire() → null [Deprecated]
```

### Events
```
ReachedTarget()
```

---

## BodyPartDescription
**Extends:** Instance

### Properties
```
AssetId: int64 = 0
BodyPart: BodyPart = Head
Color: Color3 = 0, 0, 0
Instance: Instance
```

---

## Breakpoint
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
Condition: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ContinueExecution: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Enabled: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Id: int = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Line: int = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
LogMessage: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
MetaBreakpointId: int = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
RemoveOnHit: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Script: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Valid: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Verified: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

---

## BrowserService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
CloseBrowserWindow() → null [RobloxScriptSecurity]
CopyAuthCookieFromBrowserToEngine() → null [RobloxScriptSecurity]
EmitHybridEvent(moduleName: string, eventName: string, params: string) → null [RobloxScriptSecurity]
ExecuteJavaScript(javascript: string) → null [RobloxScriptSecurity]
OpenBrowserWindow(url: string) → null [RobloxScriptSecurity]
OpenNativeOverlay(title: string, url: string) → null [RobloxScriptSecurity]
OpenWeChatAuthWindow() → null [RobloxScriptSecurity]
ReturnToJavaScript(callbackId: string, success: bool, params: string) → null [RobloxScriptSecurity]
SendCommand(command: string) → null [RobloxScriptSecurity]
```

### Events
```
AuthCookieCopiedToEngine() [RobloxScriptSecurity]
BrowserWindowClosed() [RobloxScriptSecurity]
BrowserWindowWillNavigate(url: string) [RobloxScriptSecurity]
JavaScriptCallback(content: string) [RobloxScriptSecurity]
```

---

## BugReporterService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
IsAvailable() → bool [RobloxScriptSecurity]
```

### Events
```
BugReportRequested(trigger: string) [RobloxScriptSecurity]
```

---

## BulkImportService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
LaunchBulkImport(assetTypeToImport: int) → null [RobloxScriptSecurity]
ShowBulkImportView() → null [RobloxScriptSecurity]
```

### Events
```
AssetImported(assetType: AssetType, name: string, id: int64) [RobloxScriptSecurity]
BulkImportFinished(state: int) [RobloxScriptSecurity]
BulkImportStarted() [RobloxScriptSecurity]
```

---

## CacheableContentProvider
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## HSRDataContentProvider
**Extends:** CacheableContentProvider
**Tags:** NotCreatable, Service, NotReplicated

---

## MeshContentProvider
**Extends:** CacheableContentProvider
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetContentMemoryData() → Dictionary [RobloxScriptSecurity]
```

---

## SlimContentProvider
**Extends:** CacheableContentProvider
**Tags:** NotCreatable, Service

### Functions
```
GetContentMemoryData() → Dictionary [RobloxSecurity]
```

---

## SolidModelContentProvider
**Extends:** CacheableContentProvider
**Tags:** NotCreatable, Service, NotReplicated

---

## CalloutService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
AttachCallout(definitionId: string, locationId: string, target: Instance) → null [RobloxScriptSecurity]
DefineCallout(definitionId: string, title: string, description: string, learnMoreURL: string) → null [RobloxScriptSecurity]
DetachCalloutsByDefinitionId(definitionId: string) → null [RobloxScriptSecurity]
```

---

## CaptureService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
CanCaptureVideo() → bool [RobloxScriptSecurity]
CaptureScreenshot(onCaptureReady: Function) → null
DeleteCapture(capturePath: string) → null [RobloxScriptSecurity]
DeleteVideoCapture(videoCapture: VideoCapture) → null [RobloxScriptSecurity]
GetDeviceInfo() → Dictionary
IsCapturingVideo() → bool [RobloxScriptSecurity]
OnCaptureBegan() → null [RobloxScriptSecurity]
OnCaptureEnded() → null [RobloxScriptSecurity]
OnCapturePermissionsPromptFinished(promptId: int64, wasAccepted: bool) → null [RobloxScriptSecurity]
OnCaptureShared(capturePath: string) → null [RobloxScriptSecurity]
OnSavePromptFinished(promptId: int64, results: Dictionary) → null [RobloxScriptSecurity]
OnSharePromptFinished(promptId: int64, accepted: bool) → null [RobloxScriptSecurity]
OnVideoCaptureShared(videoCapture: VideoCapture) → null [RobloxScriptSecurity]
PreVideoCaptureShared(videoCapture: VideoCapture) → string [RobloxScriptSecurity]
PromptCaptureGalleryPermission(captureGalleryPermission: CaptureGalleryPermission, onAcceptedCallback: Function, onDeniedCallback: Function) → null
PromptSaveCapturesToGallery(captures: Array, resultCallback: Function) → null
PromptShareCapture(captureContent: Content, launchData: string, onAcceptedCallback: Function, onDeniedCallback: Function) → null
RetrieveCaptures() → Array [RobloxScriptSecurity]
SaveCaptureToExternalStorage(capturePath: string) → null [RobloxScriptSecurity]
SaveScreenshotCapture(additionalInfo: string) → null [RobloxScriptSecurity]
SaveVideoCaptureToExternalStorage(videoCapture: VideoCapture) → null [RobloxScriptSecurity]
StopVideoCapture() → null
StopVideoCaptureInternal() → null [RobloxScriptSecurity]
TakeCapture(onCaptureReady: Function, captureParams: Dictionary) → null
CreatePostAsync(pathArr: Array, caption: string) → Dictionary [RobloxScriptSecurity]
DeleteCapturesAsync(pathArr: Array) → int64 [RobloxScriptSecurity]
DeleteVideoCaptureAsync(videoCapture: VideoCapture) → bool [RobloxScriptSecurity]
GetCaptureFilePathAsync(captureContent: Content) → string [RobloxScriptSecurity]
GetCaptureSizeAsync(captureContent: Content) → Vector2 [RobloxScriptSecurity]
GetCaptureStorageSizeAsync(pathArr: Array) → int64 [RobloxScriptSecurity]
GetCaptureUploadDataAsync(capturePath: string) → Dictionary [RobloxScriptSecurity]
ReadCapturesFromGalleryAsync(captureTypeFilters: Array) → Tuple
SaveCapturesToExternalStorageAsync(pathArr: Array) → int64 [RobloxScriptSecurity]
StartVideoCaptureAsync(onCaptureReady: Function, captureParams: Dictionary) → VideoCaptureStartedResult
StartVideoCaptureInternalAsync() → VideoCaptureStartedResult [RobloxScriptSecurity]
UploadCaptureAsync(capture: Capture) → Tuple
```

### Events
```
CaptureBegan(captureType: CaptureType)
CaptureEnded(captureType: CaptureType)
CaptureSaved(captureInfo: Dictionary)
CaptureSavedInternal(captureInfo: Dictionary, triggerSource: string) [RobloxScriptSecurity]
OnCaptureAndMetadataSignatureResult(content: string, captureSignature: string, captureSignatureVersion: int, metadataSignature: string, metadataSignatureVersion: int) [RobloxSecurity]
OnCaptureSignatureResult(content: string, signature: string, signatureVersion: int) [RobloxSecurity]
OpenCapturePermissionsPrompt(promptId: int64, captureGalleryPermission: CaptureGalleryPermission) [RobloxScriptSecurity]
OpenSaveCapturesPrompt(promptId: int64, captures: Array) [RobloxScriptSecurity]
OpenShareCapturePrompt(promptId: int64, captureContent: Variant, launchData: string) [RobloxScriptSecurity]
RequestCaptureAndMetadataSignature(content: string, audioAssetIds: string) [RobloxSecurity]
RequestCaptureSignature(content: string) [RobloxSecurity]
RequestCaptureSignatureV2(content: string) [RobloxSecurity]
UserCaptureSaved(captureContentId: ContentId)
UserVideoCaptureFailed(result: VideoCaptureResult) [RobloxScriptSecurity]
UserVideoCaptureStartFailed(result: VideoCaptureStartedResult) [RobloxScriptSecurity]
VideoCaptureInProgress(isInProgress: bool, captureTrigger: string) [RobloxScriptSecurity]
```

---

## ChangeHistoryService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
FinishRecording(identifier: string, operation: FinishRecordingOperation, finalOptions: Dictionary?) → null [PluginSecurity]
GetCanRedo() → Tuple [PluginSecurity]
GetCanUndo() → Tuple [PluginSecurity]
IsRecordingInProgress(identifier: string?) → bool [PluginSecurity]
Redo() → null [PluginSecurity]
ResetWaypoints() → null [PluginSecurity]
SetEnabled(state: bool) → null [PluginSecurity]
SetWaypoint(name: string) → null [PluginSecurity]
TryBeginRecording(name: string, displayName: string?) → string? [PluginSecurity]
Undo() → null [PluginSecurity]
```

### Events
```
OnRecordingFinished(name: string, displayName: string?, identifier: string?, operation: FinishRecordingOperation, finalOptions: Dictionary?) [PluginSecurity]
OnRecordingStarted(name: string, displayName: string?) [PluginSecurity]
OnRedo(waypoint: string) [PluginSecurity]
OnUndo(waypoint: string) [PluginSecurity]
```

---

## CharacterAppearance
**Extends:** Instance
**Tags:** NotCreatable

---

## BodyColors
**Extends:** CharacterAppearance

### Properties
```
HeadColor: BrickColor
HeadColor3: Color3 = 0.992157, 0.917647, 0.552941
LeftArmColor: BrickColor
LeftArmColor3: Color3 = 0.992157, 0.917647, 0.552941
LeftLegColor: BrickColor
LeftLegColor3: Color3 = 0.0509804, 0.411765, 0.67451
RightArmColor: BrickColor
RightArmColor3: Color3 = 0.992157, 0.917647, 0.552941
RightLegColor: BrickColor
RightLegColor3: Color3 = 0.0509804, 0.411765, 0.67451
TorsoColor: BrickColor
TorsoColor3: Color3 = 0.156863, 0.498039, 0.278431
```

---

## CharacterMesh
**Extends:** CharacterAppearance

### Properties
```
BaseTextureId: int64 = 0
BodyPart: BodyPart = Head
MeshId: int64 = 0
OverlayTextureId: int64 = 0
```

---

## Clothing
**Extends:** CharacterAppearance
**Tags:** NotCreatable

### Properties
```
Color3: Color3
Outfit1: ContentId
Outfit2: ContentId
```

---

## Pants
**Extends:** Clothing

### Properties
```
PantsTemplate: ContentId
```

---

## Shirt
**Extends:** Clothing

### Properties
```
ShirtTemplate: ContentId
```

---

## ShirtGraphic
**Extends:** CharacterAppearance

### Properties
```
Color3: Color3 = 1, 1, 1
Graphic: ContentId
```

---

## Skin
**Extends:** CharacterAppearance
**Tags:** Deprecated

### Properties
```
SkinColor: BrickColor
```

---

## Chat
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
BubbleChatEnabled: bool = false
IsAutoMigrated: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LoadDefaultChat: bool = true [Write:NotAccessibleSecurity]
```

### Functions
```
Chat(partOrCharacter: Instance, message: string, color: ChatColor) → null
ChatLocal(partOrCharacter: Instance, message: string, color: ChatColor) → null [RobloxScriptSecurity]
GetShouldUseLuaChat() → bool [RobloxScriptSecurity]
InvokeChatCallback(callbackType: ChatCallbackType, callbackArguments: Tuple) → Tuple
RegisterChatCallback(callbackType: ChatCallbackType, callbackFunction: Function) → null
SetBubbleChatSettings(settings: Variant) → null
CanUserChatAsync(userId: int64) → bool
CanUsersChatAsync(userIdFrom: int64, userIdTo: int64) → bool
FilterStringAsync(stringToFilter: string, playerFrom: Player, playerTo: Player) → string
FilterStringForBroadcast(stringToFilter: string, playerFrom: Player) → string
FilterStringForPlayerAsync(stringToFilter: string, playerToFilterFor: Player) → string [Deprecated]
```

### Events
```
BubbleChatSettingsChanged(settings: Variant) [RobloxScriptSecurity]
Chatted(part: Instance, message: string, color: ChatColor)
ClientToServerFilterMessageSignalV2(sender: Instance, receiver: Instance, unfilteredMessage: string) [RobloxSecurity]
ClientToServerReportUnfilteredSignal(unfilteredText: string, match: string, instancePath: string, instanceType: string) [RobloxSecurity]
ServerToClientUnderOver13FilteredResponseSignal(sender: Instance, unfilteredMessage: string, isError: bool, errorStr: string, under13: string, over13: string) [RobloxSecurity]
TimeoutChatAttempt(isPermanentTimeout: bool, endTime: int64) [RobloxScriptSecurity]
```

---

## ChatbotUIService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
DisplayContent(contentType: string, data: Dictionary) → null [RobloxScriptSecurity]
GetSettings() → Dictionary [RobloxScriptSecurity]
```

### Events
```
ActionActivatedSignal(action: string) [RobloxScriptSecurity]
FindVariationsSignal(action: string) [RobloxScriptSecurity]
SetMaterialSettingsSignal(guid: string, studsPerTile: double, isOrganic: bool) [RobloxScriptSecurity]
SettingChangedSignal(setting: string, value: Variant) [RobloxScriptSecurity]
ShiftToAssetIdSignal(action: string, change: int64) [RobloxScriptSecurity]
ShiftVariationSignal(action: string, change: int) [RobloxScriptSecurity]
```

---

## ClickDetector
**Extends:** Instance

### Properties
```
CursorIcon: ContentId
MaxActivationDistance: float = 32
```

### Events
```
MouseActionReplicated(player: Player, actionType: int) [RobloxSecurity]
MouseClick(playerWhoClicked: Player)
MouseHoverEnter(playerWhoHovered: Player)
MouseHoverLeave(playerWhoHovered: Player)
RightMouseClick(playerWhoClicked: Player)
mouseClick(playerWhoClicked: Player)
```

---

## DragDetector
**Extends:** ClickDetector

### Properties
```
ActivatedCursorIcon: ContentId
ApplyAtCenterOfMass: bool = false
Axis: Vector3 = 0, 1, 0
DragFrame: CFrame
DragStyle: DragDetectorDragStyle = TranslatePlane
Enabled: bool = true
GamepadModeSwitchKeyCode: KeyCode = ButtonR1
KeyboardModeSwitchKeyCode: KeyCode = LeftControl
MaxDragAngle: float = 0
MaxDragTranslation: Vector3 = 0, 0, 0
MaxForce: float = 10000000
MaxTorque: float = 10000
MinDragAngle: float = 0
MinDragTranslation: Vector3 = 0, 0, 0
Orientation: Vector3 = -0, 180, 90
PermissionPolicy: DragDetectorPermissionPolicy = Everybody
PhysicalDragClickedPart: Instance
PhysicalDragHitPoint: Vector3 = 0, 0, 0
PhysicalDragIsInVR: bool = false
PhysicalDragTargetFrame: CFrame
ReferenceInstance: Instance
ResponseStyle: DragDetectorResponseStyle = Physical
Responsiveness: float = 10
RunLocally: bool = false
SecondaryAxis: Vector3 = 1, 0, 0
TrackballRadialPullFactor: float = 1
TrackballRollFactor: float = 1
VRSwitchKeyCode: KeyCode = ButtonL2
WorldAxis: Vector3 = 0, 1, 0
WorldSecondaryAxis: Vector3 = 1, 0, 0
```

### Functions
```
AddConstraintFunction(priority: int, function: Function) → RBXScriptConnection
GetReferenceFrame() → CFrame
RestartDrag() → null
SetDragStyleFunction(function: Function) → null
SetPermissionPolicyFunction(function: Function) → null
```

### Events
```
DragContinue(playerWhoDragged: Player, cursorRay: Ray, viewFrame: CFrame, vrInputFrame: OptionalCoordinateFrame, isModeSwitchKeyDown: bool)
DragContinueReplicate(playerWhoDragged: Player, cursorRay: Ray, viewFrame: CFrame, vrInputFrame: OptionalCoordinateFrame, isModeSwitchKeyDown: bool)
DragEnd(playerWhoDragged: Player)
DragEndReplicate(playerWhoDragged: Player)
DragStart(playerWhoDragged: Player, cursorRay: Ray, viewFrame: CFrame, hitFrame: CFrame, clickedPart: BasePart, vrInputFrame: OptionalCoordinateFrame, isModeSwitchKeyDown: bool)
DragStartReplicate(playerWhoDragged: Player, cursorRay: Ray, viewFrame: CFrame, hitFrame: CFrame, clickedPart: BasePart, vrInputFrame: OptionalCoordinateFrame, isModeSwitchKeyDown: bool)
RestartPhysicalDragReplicate(hitPoint: Vector3)
```

---

## CloudCRUDService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## Clouds
**Extends:** Instance

### Properties
```
Color: Color3 = 1, 1, 1
Cover: float = 0.5
Density: float = 0.699999988
Enabled: bool = true
```

---

## ClusterPacketCache
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## Collaborator
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
CFrame: CFrame
CollaboratorColor: int = 0 [Deprecated]
CollaboratorColor3: Color3 = 0, 0, 0
CurDocGUID: string
CurScriptLineNumber: int = 0
IsIdle: bool = false
Status: CollaboratorStatus = None
UserId: int64 = 0
Username: string
```

---

## CollaboratorsService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
GetCollaboratorsList() → Instances [RobloxScriptSecurity]
GetSelectionHighlightsEnabled() → bool [RobloxScriptSecurity]
RequestFlyToCollaborator(collaboratorId: int64) → null [RobloxScriptSecurity]
ToggleSelectionHighlights(showHighlights: bool) → null [RobloxScriptSecurity]
ToggleTeamCreate(on: bool) → null [RobloxScriptSecurity]
```

### Events
```
CollaboratorIdleUpdate(collaboratorId: int64, isIdle: bool) [RobloxScriptSecurity]
CollaboratorInstanceCreatedSignal(collaboratorId: int64) [RobloxScriptSecurity]
CollaboratorInstanceDestroyedSignal(collaboratorId: int64) [RobloxScriptSecurity]
CollaboratorStatusUpdateRequestedSignal(collaboratorId: int64, newStatus: CollaboratorStatus) [RobloxScriptSecurity]
CollaboratorStatusUpdatedSignal(collaboratorId: int64, newStatus: CollaboratorStatus) [RobloxScriptSecurity]
ToggleSelectionHighlightsSignal(areHighlightsShown: bool) [RobloxScriptSecurity]
```

---

## CollectionService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
AddTag(instance: Instance, tag: string) → null
GetAllTags() → Array
GetCollection(class: string) → Instances [Deprecated]
GetInstanceAddedSignal(tag: string) → RBXScriptSignal
GetInstanceRemovedSignal(tag: string) → RBXScriptSignal
GetTagged(tag: string) → Instances
GetTags(instance: Instance) → Array
HasTag(instance: Instance, tag: string) → bool
RemoveTag(instance: Instance, tag: string) → null
```

### Events
```
ItemAdded(instance: Instance)
ItemRemoved(instance: Instance)
TagAdded(tag: string)
TagRemoved(tag: string)
```

---

## CommerceService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
PromptCommerceProductPurchase(user: Player, commerceProductId: string) → null
PromptRealWorldCommerceBrowser(player: Player, url: string) → null
SignalPromptCommerceProductPurchaseFinished(productId: string, didTryPurchase: bool, checkoutSessionId: string) → null [RobloxScriptSecurity]
GetCommerceProductInfoAsync(commerceProductId: string) → Dictionary
PrepareCommerceProductPurchase(commerceProductId: string) → Dictionary [RobloxScriptSecurity]
UserEligibleForRealWorldCommerceAsync() → bool
```

### Events
```
BenefitStatusReceived(isGranted: bool) [RobloxScriptSecurity]
FetchReceipt() [RobloxSecurity]
InExperienceBrowserRequested(url: string) [RobloxSecurity]
PromptCommerceProductPurchaseFinished(user: Player, productId: string)
PromptCommerceProductPurchaseRequested(commerceProductId: string) [RobloxScriptSecurity]
PurchaseBrowserClosed() [RobloxScriptSecurity]
```

---

## ConfigService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
ClearTestingValue(key: string) → null
SetTestingValue(key: string, value: Variant) → null
GetConfigAsync() → ConfigSnapshot
GetConfigForPlayerAsync(player: Player) → ConfigSnapshot
```

---

## Configuration
**Extends:** Instance

---

## ConfigureServerService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## ConnectivityService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
NetworkStatus: NetworkStatus = Unknown [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Functions
```
IsNetworkStateAvailable() → bool [RobloxScriptSecurity]
```

---

## Constraint
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
Active: bool [ReadOnly]
Attachment0: Attachment
Attachment1: Attachment
Color: BrickColor
Enabled: bool
Visible: bool
```

### Functions
```
GetDebugAppliedForce(bodyId: int) → Vector3 [Deprecated]
GetDebugAppliedTorque(bodyId: int) → Vector3 [Deprecated]
```

---

## AlignOrientation
**Extends:** Constraint

### Properties
```
AlignType: AlignType = AllAxes
CFrame: CFrame
LookAtPosition: Vector3 = 0, 0, 0
MaxAngularVelocity: float = INF
MaxTorque: float = 10000
Mode: OrientationAlignmentMode = TwoAttachment
PrimaryAxis: Vector3 = 1, 0, 0
PrimaryAxisOnly: bool = false
ReactionTorqueEnabled: bool = false
Responsiveness: float = 10
RigidityEnabled: bool = false
SecondaryAxis: Vector3 = 0, 1, 0
```

---

## AlignPosition
**Extends:** Constraint

### Properties
```
ApplyAtCenterOfMass: bool = false
ForceLimitMode: ForceLimitMode = Magnitude
ForceRelativeTo: ActuatorRelativeTo = World
MaxAxesForce: Vector3 = 10000, 10000, 10000
MaxForce: float = 10000
MaxVelocity: float = INF
Mode: PositionAlignmentMode = TwoAttachment
Position: Vector3 = 0, 0, 0
ReactionForceEnabled: bool = false
Responsiveness: float = 10
RigidityEnabled: bool = false
```

---

## AngularVelocity
**Extends:** Constraint

### Properties
```
AngularVelocity: Vector3 = 0, 0, 0
MaxTorque: float = 0
ReactionTorqueEnabled: bool = false
RelativeTo: ActuatorRelativeTo = World
```

---

## AnimationConstraint
**Extends:** Constraint

### Properties
```
C0: CFrame [ReadOnly] [Deprecated]
C1: CFrame [ReadOnly] [Deprecated]
IsKinematic: bool = false
MaxForce: float = 10000
MaxTorque: float = 10000
Part0: BasePart [ReadOnly] [Deprecated]
Part1: BasePart [ReadOnly] [Deprecated]
Transform: CFrame
```

---

## BallSocketConstraint
**Extends:** Constraint

### Properties
```
LimitsEnabled: bool = false
MaxFrictionTorque: float = 0
MaxFrictionTorqueXml: float = 0
Radius: float = 0.150000006
Restitution: float = 0
TwistLimitsEnabled: bool = false
TwistLowerAngle: float = -45
TwistUpperAngle: float = 45
UpperAngle: float = 45
```

---

## HingeConstraint
**Extends:** Constraint

### Properties
```
ActuatorType: ActuatorType = None
AngularResponsiveness: float = 45
AngularSpeed: float = 0
AngularVelocity: float = 0
CurrentAngle: float = 0 [ReadOnly]
LimitsEnabled: bool = false
LowerAngle: float = -45
MotorMaxAcceleration: float = 500000
MotorMaxTorque: float = 0
Radius: float = 0.150000006
Restitution: float = 0
ServoMaxTorque: float = 0
SoftlockServoUponReachingTarget: bool = false [Deprecated]
TargetAngle: float = 0
UpperAngle: float = 45
```

---

## LineForce
**Extends:** Constraint

### Properties
```
ApplyAtCenterOfMass: bool = false
InverseSquareLaw: bool = false
Magnitude: float = 1000
MaxForce: float = INF
ReactionForceEnabled: bool = false
```

---

## LinearVelocity
**Extends:** Constraint

### Properties
```
ForceLimitMode: ForceLimitMode = Magnitude
ForceLimitsEnabled: bool = true
LineDirection: Vector3 = 1, 0, 0
LineVelocity: float = -0
MaxAxesForce: Vector3 = 1000, 1000, 1000
MaxForce: float = 1000
MaxPlanarAxesForce: Vector2 = 1000, 1000
PlaneVelocity: Vector2 = 0, 0
PrimaryTangentAxis: Vector3 = 1, 0, 0
ReactionForceEnabled: bool = true
RelativeTo: ActuatorRelativeTo = World
SecondaryTangentAxis: Vector3 = 0, 1, 0
VectorVelocity: Vector3 = 0, 0, 0
VelocityConstraintMode: VelocityConstraintMode = Vector
```

---

## PlaneConstraint
**Extends:** Constraint

---

## Plane
**Extends:** PlaneConstraint
**Tags:** Deprecated

---

## RigidConstraint
**Extends:** Constraint

---

## RodConstraint
**Extends:** Constraint

### Properties
```
CurrentDistance: float = 0 [ReadOnly]
Length: float = 5
LimitAngle0: float = 90
LimitAngle1: float = 90
LimitsEnabled: bool = false
Thickness: float = 0.100000001
```

---

## RopeConstraint
**Extends:** Constraint

### Properties
```
CurrentDistance: float = 0 [ReadOnly]
Length: float = 5
Restitution: float = 0
Thickness: float = 0.100000001
WinchEnabled: bool = false
WinchForce: float = 10000
WinchResponsiveness: float = 45
WinchSpeed: float = 2
WinchTarget: float = 5
```

---

## SlidingBallConstraint
**Extends:** Constraint
**Tags:** NotCreatable

### Properties
```
ActuatorType: ActuatorType
CurrentPosition: float [ReadOnly]
LimitsEnabled: bool
LinearResponsiveness: float
LowerLimit: float
MotorMaxAcceleration: float
MotorMaxForce: float
Restitution: float
ServoMaxForce: float
Size: float
SoftlockServoUponReachingTarget: bool [Deprecated]
Speed: float
TargetPosition: float
UpperLimit: float
Velocity: float
```

---

## CylindricalConstraint
**Extends:** SlidingBallConstraint

### Properties
```
AngularActuatorType: ActuatorType = None
AngularLimitsEnabled: bool = false
AngularResponsiveness: float = 45
AngularRestitution: float = 0
AngularSpeed: float = 0
AngularVelocity: float = 0
CurrentAngle: float = 0 [ReadOnly]
InclinationAngle: float = 0
LowerAngle: float = -45
MotorMaxAngularAcceleration: float = 500000
MotorMaxTorque: float = 0
RotationAxisVisible: bool = false
ServoMaxTorque: float = 0
SoftlockAngularServoUponReachingTarget: bool = false [Deprecated]
TargetAngle: float = 0
UpperAngle: float = 45
WorldRotationAxis: Vector3 = 1, 0, 0 [ReadOnly]
```

---

## PrismaticConstraint
**Extends:** SlidingBallConstraint

---

## SpringConstraint
**Extends:** Constraint

### Properties
```
Coils: float = 3
CurrentLength: float = 0 [ReadOnly]
Damping: float = 0
FreeLength: float = 1
LimitsEnabled: bool = false
MaxForce: float = INF
MaxLength: float = 5
MinLength: float = 0
Radius: float = 0.400000006
Stiffness: float = 0
Thickness: float = 0.100000001
```

---

## Torque
**Extends:** Constraint

### Properties
```
RelativeTo: ActuatorRelativeTo = Attachment0
Torque: Vector3 = 0, 0, 0
```

---

## TorsionSpringConstraint
**Extends:** Constraint

### Properties
```
Coils: float = 8
CurrentAngle: float = 0 [ReadOnly]
Damping: float = 0.00999999978
LimitEnabled: bool = false [Deprecated]
LimitsEnabled: bool = false
MaxAngle: float = 45
MaxTorque: float = INF
Radius: float = 0.400000006
Restitution: float = 0
Stiffness: float = 100
```

---

## UniversalConstraint
**Extends:** Constraint

### Properties
```
LimitsEnabled: bool = false
MaxAngle: float = 45
Radius: float = 0.200000003
Restitution: float = 0
```

---

## VectorForce
**Extends:** Constraint

### Properties
```
ApplyAtCenterOfMass: bool = false
Force: Vector3 = 1000, 0, 0
RelativeTo: ActuatorRelativeTo = Attachment0
```

---

## ContentProvider
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
BaseUrl: string [ReadOnly]
RequestQueueSize: int [ReadOnly]
```

### Functions
```
GetAssetFetchStatus(contentId: ContentId) → AssetFetchStatus
GetAssetFetchStatusChangedSignal(contentId: ContentId) → RBXScriptSignal
GetDependencyContentIds(root: Instance) → Array [RobloxScriptSecurity]
GetFailedRequests() → Array [RobloxScriptSecurity]
ListEncryptedAssets() → Array
Preload(contentId: ContentId) → null [Deprecated]
RegisterDefaultEncryptionKey(encryptionKey: string) → null
RegisterDefaultSessionKey(sessionKey: string) → null
RegisterEncryptedAsset(assetId: ContentId, encryptionKey: string) → null
RegisterSessionEncryptedAsset(contentId: ContentId, sessionKey: string) → null
SetBaseUrl(url: string) → null [LocalUserSecurity]
UnregisterDefaultEncryptionKey() → null
UnregisterEncryptedAsset(assetId: ContentId) → null
PreloadAsync(contentIdList: Array, callbackFunction: Function) → null
```

### Events
```
AssetFetchFailed(assetId: ContentId)
```

---

## ContextActionService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
BindAction(actionName: string, functionToBind: Function, createTouchButton: bool, inputTypes: Tuple) → null
BindActionAtPriority(actionName: string, functionToBind: Function, createTouchButton: bool, priorityLevel: int, inputTypes: Tuple) → null
BindActionToInputTypes(actionName: string, functionToBind: Function, createTouchButton: bool, inputTypes: Tuple) → null [Deprecated]
BindActivate(userInputTypeForActivation: UserInputType, keyCodesForActivation: Tuple) → null
BindCoreAction(actionName: string, functionToBind: Function, createTouchButton: bool, inputTypes: Tuple) → null [RobloxScriptSecurity]
BindCoreActionAtPriority(actionName: string, functionToBind: Function, createTouchButton: bool, priorityLevel: int, inputTypes: Tuple) → null [RobloxScriptSecurity]
BindCoreActivate(userInputTypeForActivation: UserInputType, keyCodesForActivation: Tuple) → null [RobloxScriptSecurity]
CallFunction(actionName: string, state: UserInputState, inputObject: Instance) → Tuple [RobloxScriptSecurity]
FireActionButtonFoundSignal(actionName: string, actionButton: Instance) → null [RobloxScriptSecurity]
GetAllBoundActionInfo() → Dictionary
GetAllBoundCoreActionInfo() → Dictionary [RobloxScriptSecurity]
GetBoundActionInfo(actionName: string) → Dictionary
GetBoundCoreActionInfo(actionName: string) → Dictionary [RobloxScriptSecurity]
GetCurrentLocalToolIcon() → string
SetDescription(actionName: string, description: string) → null
SetImage(actionName: string, image: string) → null
SetPosition(actionName: string, position: UDim2) → null
SetTitle(actionName: string, title: string) → null
UnbindAction(actionName: string) → null
UnbindActivate(userInputTypeForActivation: UserInputType, keyCodeForActivation: KeyCode) → null
UnbindAllActions() → null
UnbindCoreAction(actionName: string) → null [RobloxScriptSecurity]
UnbindCoreActivate(userInputTypeForActivation: UserInputType, keyCodeForActivation: KeyCode) → null [RobloxScriptSecurity]
GetButton(actionName: string) → Instance
```

### Events
```
BoundActionAdded(actionAdded: string, createTouchButton: bool, functionInfoTable: Dictionary, isCore: bool) [RobloxScriptSecurity]
BoundActionChanged(actionChanged: string, changeName: string, changeTable: Dictionary) [RobloxScriptSecurity]
BoundActionRemoved(actionRemoved: string, functionInfoTable: Dictionary, isCore: bool) [RobloxScriptSecurity]
GetActionButtonEvent(actionName: string) [RobloxScriptSecurity]
LocalToolEquipped(toolEquipped: Instance)
LocalToolUnequipped(toolUnequipped: Instance)
```

---

## Controller
**Extends:** Instance
**Tags:** NotCreatable

### Functions
```
BindButton(button: Button, caption: string) → null
GetButton(button: Button) → bool
UnbindButton(button: Button) → null
bindButton(button: Button, caption: string) → null [Deprecated]
getButton(button: Button) → bool [Deprecated]
```

### Events
```
ButtonChanged(button: Button)
```

---

## HumanoidController
**Extends:** Controller

---

## SkateboardController
**Extends:** Controller

### Properties
```
Steer: float = 0 [ReadOnly]
Throttle: float = 0 [ReadOnly]
```

### Events
```
AxisChanged(axis: string)
```

---

## VehicleController
**Extends:** Controller

---

## ControllerBase
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
Active: bool [ReadOnly]
BalanceRigidityEnabled: bool
MoveSpeedFactor: float
```

---

## AirController
**Extends:** ControllerBase

### Properties
```
BalanceMaxTorque: float = 10000
BalanceSpeed: float = 100
LinearImpulse: Vector3 = 0, 0, 0
MaintainAngularMomentum: bool = true
MaintainLinearMomentum: bool = true
MoveMaxForce: float = 1000
TurnMaxTorque: float = 10000
TurnSpeedFactor: float = 1
```

---

## ClimbController
**Extends:** ControllerBase

### Properties
```
AccelerationTime: float = 0
BalanceMaxTorque: float = 10000
BalanceSpeed: float = 100
MoveMaxForce: float = 10000
```

---

## GroundController
**Extends:** ControllerBase

### Properties
```
AccelerationLean: float = 1
AccelerationTime: float = 0
BalanceMaxTorque: float = 10000
BalanceSpeed: float = 100
DecelerationTime: float = 0
Friction: float = 2
FrictionWeight: float = 1
GroundOffset: float = 1
StandForce: float = 10000
StandSpeed: float = 100
TurnSpeedFactor: float = 1
```

---

## SwimController
**Extends:** ControllerBase

### Properties
```
AccelerationTime: float = 0
PitchMaxTorque: float = 10000
PitchSpeedFactor: float = 1
RollMaxTorque: float = 10000
RollSpeedFactor: float = 1
```

---

## ControllerManager
**Extends:** Instance

### Properties
```
ActiveController: ControllerBase
BaseMoveSpeed: float = 16
BaseTurnSpeed: float = 8
ClimbSensor: ControllerSensor
FacingDirection: Vector3 = 0, 0, 1
GroundSensor: ControllerSensor
MovingDirection: Vector3 = 0, 0, 0
RootPart: BasePart
UpDirection: Vector3 = 0, 1, 0
```

---

## ControllerService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## ConversationalAIAcceptanceService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
AlternativeAssetSelected(requestId: string, previousAssetId: int64, assetId: int64) → null [RobloxScriptSecurity]
AssetInserted(requestId: string, assetId: int64) → null [RobloxScriptSecurity]
CodeRunnerActivated(requestId: string, code: string, serverAutorun: bool, autorunEnabled: bool, autoExpandDropdowns: bool) → null [RobloxScriptSecurity]
CodeRunnerCompleted(requestId: string, success: bool, errorMessage: string) → null [RobloxScriptSecurity]
CodeRunnerUndone(requestId: string) → null [RobloxScriptSecurity]
DataModelHierarchyLatency(requestId: string, latency: double) → null [RobloxScriptSecurity]
ErrorTelemetry(requestId: string, errorId: string, errorType: string, errorMessage: string) → null [RobloxScriptSecurity]
InstanceInserted(requestId: string) → null [RobloxScriptSecurity]
RecordingActionEnded(requestId: string, waypointName: string) → null [RobloxScriptSecurity]
ReportJSONEncodeFailure(instanceName: string, className: string) → null [RobloxScriptSecurity]
SendCommandErrorTelemetry(requestId: string, commandName: string, errorMessage: string) → null [RobloxScriptSecurity]
SendMeshGenActivatedTelemetry() → null [RobloxScriptSecurity]
SendMeshGenCompletedTelemetry(requestId: string, generationId: string, success: bool, errorMessage: string, prompt: string) → null [RobloxScriptSecurity]
SendMeshGenMeshInsertedTelemetry(requestId: string, generationId: string, success: bool, errorMessage: string) → null [RobloxScriptSecurity]
SendMeshGenPublishedAssetsTelemetry(requestId: string, generationId: string, success: bool, errorMessage: string, meshId: int64?, imageId: int64?) → null [RobloxScriptSecurity]
```

---

## CookiesService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## CorePackages
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## CoreScriptDebuggingManagerHelper
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## CoreScriptSyncService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetScriptFilePath(script: Instance) → Variant [RobloxScriptSecurity]
```

---

## CreationDBService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## CreatorStoreService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
GetAssetInfoAsync(assetId: int64) → Dictionary [RobloxScriptSecurity]
GetCreatorStoreProductInfoAsync(productTargetId: int64, assetType: string) → Dictionary [RobloxScriptSecurity]
PerformCreatorStorePurchase(productTargetId: int64, assetType: string) → Dictionary [RobloxScriptSecurity]
```

---

## CrossDMScriptChangeListener
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
IsWatchingScriptLine(scriptRef: string, lineNumber: int) → bool [RobloxScriptSecurity]
StartWatchingScriptLine(scriptRef: string, debuggerConnectionId: int, lineNumber: int) → null [RobloxScriptSecurity]
```

### Events
```
GuidLineContentsChanged(guid: string, lineNumber: int, contents: string) [RobloxScriptSecurity]
GuidNameChanged(guid: string, fullName: string) [RobloxScriptSecurity]
```

---

## CustomEvent
**Extends:** Instance
**Tags:** Deprecated

### Properties
```
PersistedCurrentValue: float = 0
```

### Functions
```
GetAttachedReceivers() → Instances
SetValue(newValue: float) → null
```

### Events
```
ReceiverConnected(receiver: Instance)
ReceiverDisconnected(receiver: Instance)
```

---

## CustomEventReceiver
**Extends:** Instance
**Tags:** Deprecated

### Properties
```
Source: Instance
```

### Functions
```
GetCurrentValue() → float
```

### Events
```
EventConnected(event: Instance)
EventDisconnected(event: Instance)
SourceValueChanged(newValue: float)
```

---

## CustomLog
**Extends:** Instance
**Tags:** NotReplicated

### Functions
```
Close() → null
GetLogPath() → string
Open() → null
WriteAppend(append: string) → null
```

---

## DataModelMesh
**Extends:** Instance
**Tags:** NotCreatable, NotBrowsable

### Properties
```
Offset: Vector3
Scale: Vector3
VertexColor: Vector3
```

---

## BevelMesh
**Extends:** DataModelMesh
**Tags:** NotCreatable, NotBrowsable, Deprecated

### Properties
```
Bevel: float
Bevel Roundness: float
Bulge: float
```

---

## BlockMesh
**Extends:** BevelMesh

---

## CylinderMesh
**Extends:** BevelMesh
**Tags:** Deprecated

---

## FileMesh
**Extends:** DataModelMesh

### Properties
```
MeshId: ContentId
TextureId: ContentId
```

---

## SpecialMesh
**Extends:** FileMesh

### Properties
```
MeshType: MeshType = Head
```

---

## DataModelPatchService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetLuaVersion(patchName: string) → string [RobloxScriptSecurity]
GetPatch(patchName: string) → Instance [RobloxScriptSecurity]
RegisterPatch(patchName: string, behaviorName: string, localConfigPath: string, userId: int64) → null [RobloxScriptSecurity]
UpdatePatch(userId: int64, patchName: string, callbackFunction: Function) → null [RobloxScriptSecurity]
```

---

## DataModelSession
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
CurrentDataModelType: StudioDataModelType [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
SessionId: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Events
```
CurrentDataModelTypeAboutToChange(dataModelType: StudioDataModelType) [RobloxScriptSecurity]
CurrentDataModelTypeChanged() [RobloxScriptSecurity]
```

---

## DataStoreGetOptions
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
UseCache: bool = true
```

---

## DataStoreIncrementOptions
**Extends:** Instance
**Tags:** NotReplicated

### Functions
```
GetMetadata() → Dictionary
SetMetadata(attributes: Dictionary) → null
```

---

## DataStoreInfo
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
CreatedTime: int64 [ReadOnly]
DataStoreName: string [ReadOnly]
UpdatedTime: int64 [ReadOnly]
```

---

## DataStoreKey
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
KeyName: string [ReadOnly]
```

---

## DataStoreKeyInfo
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
CreatedTime: int64 [ReadOnly]
UpdatedTime: int64 [ReadOnly]
Version: string [ReadOnly]
```

### Functions
```
GetMetadata() → Dictionary
GetUserIds() → Array
```

---

## DataStoreObjectVersionInfo
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
CreatedTime: int64 [ReadOnly]
IsDeleted: bool [ReadOnly]
Version: string [ReadOnly]
```

---

## DataStoreOptions
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
AllScopes: bool = false
```

### Functions
```
SetExperimentalFeatures(experimentalFeatures: Dictionary) → null
```

---

## DataStoreService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
AutomaticRetry: bool = true [Read:LocalUserSecurity] [Write:LocalUserSecurity]
LegacyNamingScheme: bool = false [Read:LocalUserSecurity] [Write:LocalUserSecurity] [Deprecated]
```

### Functions
```
GetDataStore(name: string, scope: string, options: Instance) → DataStore
GetGlobalDataStore() → DataStore
GetOrderedDataStore(name: string, scope: string) → OrderedDataStore
GetRequestBudgetForRequestType(requestType: DataStoreRequestType) → int
ListDataStoresAsync(prefix: string, pageSize: int, cursor: string) → DataStoreListingPages
```

---

## DataStoreSetOptions
**Extends:** Instance
**Tags:** NotReplicated

### Functions
```
GetMetadata() → Dictionary
SetMetadata(attributes: Dictionary) → null
```

---

## Debris
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
MaxItems: int [Deprecated]
```

### Functions
```
AddItem(item: Instance, lifetime: double) → null
SetLegacyMaxItems(enabled: bool) → null [LocalUserSecurity]
addItem(item: Instance, lifetime: double) → null [Deprecated]
```

---

## DebugSettings
**Extends:** Instance
**Tags:** NotCreatable, Settings, NotReplicated, NotBrowsable

### Properties
```
DataModel: int [ReadOnly]
InstanceCount: int [ReadOnly]
IsScriptStackTracingEnabled: bool
JobCount: int [ReadOnly]
PlayerCount: int [ReadOnly]
ReportSoundWarnings: bool
RobloxVersion: string [ReadOnly]
TickCountPreciseOverride: TickCountSampleMethod
```

---

## DebuggablePluginWatcher
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## DebuggerBreakpoint
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
Condition: string
ContinueExecution: bool
IsEnabled: bool
Line: int [ReadOnly]
LogExpression: string
isContextDependentBreakpoint: bool
line: int
```

---

## DebuggerConnection
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
ErrorMessage: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
HasError: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Id: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
IsPaused: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Functions
```
AddBreakpoint(script: string, line: int, breakpoint: Breakpoint) → null [RobloxScriptSecurity]
Close() → null [RobloxScriptSecurity]
EvaluateWatch(expression: string, frame: StackFrame, callback: Function) → int [RobloxScriptSecurity]
GetFrameById(id: int) → StackFrame [RobloxScriptSecurity]
GetSource(scriptRef: string, status: Function) → int [RobloxScriptSecurity]
GetThreadById(id: int) → ThreadState [RobloxScriptSecurity]
GetThreads(callback: Function) → int [RobloxScriptSecurity]
GetVariableById(id: int) → DebuggerVariable [RobloxScriptSecurity]
Pause(thread: ThreadState, status: Function) → int [RobloxScriptSecurity]
Populate(instance: Instance, callback: Function) → int [RobloxScriptSecurity]
RemoveBreakpoint(breakpoint: Breakpoint) → null [RobloxScriptSecurity]
Resume(thread: ThreadState, status: Function) → int [RobloxScriptSecurity]
SetExceptionBreakMode(breakMode: DebuggerExceptionBreakMode, callback: Function) → int [RobloxScriptSecurity]
SetVariable(variable: DebuggerVariable, value: string, callback: Function) → int [RobloxScriptSecurity]
Step(thread: ThreadState, callback: Function) → int [RobloxScriptSecurity]
StepIn(thread: ThreadState, callback: Function) → int [RobloxScriptSecurity]
StepOut(thread: ThreadState, callback: Function) → int [RobloxScriptSecurity]
UpdateSelectedFrame(threadId: int, frameNumber: int) → null [RobloxScriptSecurity]
```

### Events
```
BreakpointAdded(breakpoint: Breakpoint) [RobloxScriptSecurity]
BreakpointChanged(breakpoint: Breakpoint) [RobloxScriptSecurity]
BreakpointRemoved(breakpoint: Breakpoint, reason: BreakpointRemoveReason) [RobloxScriptSecurity]
Paused(pausedState: PausedState, reason: DebuggerPauseReason) [RobloxScriptSecurity]
Resumed(pausedState: PausedState) [RobloxScriptSecurity]
```

---

## LocalDebuggerConnection
**Extends:** DebuggerConnection
**Tags:** NotCreatable, NotReplicated

---

## DebuggerConnectionManager
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
Timeout: double [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
ConnectLocal(dataModel: DataModel) → int [RobloxScriptSecurity]
ConnectRemote(host: string, port: int) → int [RobloxScriptSecurity]
FocusConnection(connection: DebuggerConnection) → null [RobloxScriptSecurity]
GetAvailableConnection() → DebuggerConnection [RobloxScriptSecurity]
GetConnectionById(id: int) → DebuggerConnection [RobloxScriptSecurity]
```

### Events
```
ConnectionEnded(connection: DebuggerConnection, reason: DebuggerEndReason) [RobloxScriptSecurity]
ConnectionStarted(connection: DebuggerConnection) [RobloxScriptSecurity]
FocusChanged(connection: DebuggerConnection) [RobloxScriptSecurity]
```

---

## DebuggerLuaResponse
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
IsError: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
IsSuccess: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Message: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
RequestId: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Status: DebuggerStatus [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Functions
```
GetArg() → Variant [RobloxScriptSecurity]
```

---

## DebuggerManager
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
DebuggingEnabled: bool [ReadOnly]
```

### Functions
```
AddDebugger(script: Instance) → Instance
EnableDebugging() → null [LocalUserSecurity]
GetDebuggers() → Instances
Resume() → null
StepIn() → null [Deprecated]
StepOut() → null [Deprecated]
StepOver() → null [Deprecated]
```

### Events
```
DebuggerAdded(debugger: Instance)
DebuggerRemoved(debugger: Instance)
```

---

## DebuggerUIService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
EditBreakpoint(metaBreakpointId: int) → null [RobloxScriptSecurity]
EditWatch(expression: string) → null [RobloxScriptSecurity]
IsConnectionForPlayDataModel(debuggerConnectionId: int) → bool [RobloxScriptSecurity]
OpenExceptionMessagePopup(exceptionMessage: string, pausedLine: int) → null [RobloxScriptSecurity]
OpenScriptAtLine(guid: string, debuggerConnectionId: int, line: int, showErrorOnFail: bool) → null [RobloxScriptSecurity]
Pause() → null [RobloxScriptSecurity]
RemoveScriptLineMarkers(debuggerConnectionId: int, allMarkers: bool) → null [RobloxScriptSecurity]
Resume() → null [RobloxScriptSecurity]
SetCurrentThreadId(debuggerThreadId: int) → null [RobloxScriptSecurity]
SetScriptLineMarker(guid: string, debuggerConnectionId: int, line: int, lineMarkerType: bool) → null [RobloxScriptSecurity]
SetWatchExpressions(expressions: Array) → null [RobloxScriptSecurity]
```

### Events
```
ExpressionAdded(expression: string) [RobloxScriptSecurity]
ExpressionsCleared() [RobloxScriptSecurity]
```

---

## DebuggerVariable
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
Name: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Populated: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Type: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Value: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
VariableId: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
VariablesCount: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Functions
```
GetVariableByIndex(index: int) → DebuggerVariable [RobloxScriptSecurity]
GetVariableByName(name: string) → DebuggerVariable [RobloxScriptSecurity]
```

---

## DebuggerWatch
**Extends:** Instance

### Properties
```
Expression: string
```

---

## DeviceIdService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetDeviceId() → string [RobloxScriptSecurity]
```

---

## Dialog
**Extends:** Instance

### Properties
```
BehaviorType: DialogBehaviorType = SinglePlayer
ConversationDistance: float = 25
GoodbyeChoiceActive: bool = true
GoodbyeDialog: string
InUse: bool = false
InitialPrompt: string
Purpose: DialogPurpose = Help
Tone: DialogTone = Neutral
TriggerDistance: float = 0
TriggerOffset: Vector3 = 0, 0, 0
```

### Functions
```
GetCurrentPlayers() → Instances
SetGuiObject(gui: BillboardGui) → null [RobloxScriptSecurity]
SetPlayerIsUsing(player: Instance, isUsing: bool) → null [RobloxScriptSecurity]
SignalDialogChoiceSelected(player: Instance, dialogChoice: Instance) → null [RobloxScriptSecurity]
```

### Events
```
DialogChoiceSelected(player: Instance, dialogChoice: Instance)
```

---

## DialogChoice
**Extends:** Instance

### Properties
```
GoodbyeChoiceActive: bool = true
GoodbyeDialog: string
ResponseDialog: string
UserDialog: string
```

---

## DraftsService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
DiscardEdits(scripts: Instances) → null [RobloxScriptSecurity]
GetDraftStatus(script: Instance) → DraftStatusCode [RobloxScriptSecurity]
GetEditors(script: Instance) → Instances [RobloxScriptSecurity]
RestoreScripts(scripts: Instances) → null [RobloxScriptSecurity]
ShowDiffsAgainstBase(scripts: Instances) → null [RobloxScriptSecurity]
ShowDiffsAgainstServer(scripts: Instances) → null [RobloxScriptSecurity]
ShowSourceDiffsAgainstCurrent(sources: Array, scripts: Instances) → null [RobloxScriptSecurity]
CommitEdits(scripts: Instances) → null [RobloxScriptSecurity]
GetDrafts() → Instances [RobloxScriptSecurity]
UpdateToLatestVersion(scripts: Instances) → null [RobloxScriptSecurity]
```

### Events
```
CommitStatusChanged(script: Instance, status: DraftStatusCode) [RobloxScriptSecurity]
DraftAdded(script: Instance) [RobloxScriptSecurity]
DraftRemoved(script: Instance) [RobloxScriptSecurity]
DraftStatusChanged(script: Instance) [RobloxScriptSecurity]
EditorsListChanged(script: Instance) [RobloxScriptSecurity]
UpdateStatusChanged(script: Instance, status: DraftStatusCode) [RobloxScriptSecurity]
```

---

## Dragger
**Extends:** Instance

### Functions
```
AxisRotate(axis: Axis) → null
MouseDown(mousePart: Instance, pointOnMousePart: Vector3, parts: Instances) → null
MouseMove(mouseRay: Ray) → null
MouseUp() → null
```

---

## DraggerService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
AlignDraggedObjects: bool
AngleSnapEnabled: bool
AngleSnapIncrement: float
AnimateHover: bool
CollisionsEnabled: bool
DraggerCoordinateSpace: DraggerCoordinateSpace
DraggerMovementMode: DraggerMovementMode
GeometrySnapColor: Color3
HoverAnimateFrequency: float
HoverLineThickness: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
HoverThickness: float
JointsEnabled: bool
LinearSnapEnabled: bool
LinearSnapIncrement: float
PartSnapEnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
PivotSnapToGeometry: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ShowHover: bool
ShowPivotIndicator: bool
```

---

## EditableService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
EditableStatus: EditableStatus = Unknown [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## EulerRotationCurve
**Extends:** Instance

### Properties
```
RotationOrder: RotationOrder = XYZ
```

### Functions
```
GetAnglesAtTime(time: float) → Array
GetRotationAtTime(time: float) → CFrame
X() → FloatCurve
Y() → FloatCurve
Z() → FloatCurve
```

---

## EventIngestService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
SendEventDeferred(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null [RobloxScriptSecurity]
SendEventImmediately(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null [RobloxScriptSecurity]
SetRBXEvent(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null [RobloxScriptSecurity]
SetRBXEventStream(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null [RobloxScriptSecurity]
```

---

## ExampleService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
PrintHello() → null [RobloxScriptSecurity]
```

### Events
```
OnPolo(message: string) [RobloxScriptSecurity]
```

---

## ExampleV2Service
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
PrintHello() → null [RobloxScriptSecurity]
```

### Events
```
OnPolo(message: string) [RobloxScriptSecurity]
```

---

## ExperienceAuthService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
ScopeCheckUIComplete(guid: string, scopes: Array, result: ScopeCheckResult, metadata: Dictionary) → null [RobloxScriptSecurity]
```

### Events
```
OpenAuthPrompt(guid: string, scopes: Array, metadata: Dictionary) [RobloxScriptSecurity]
ScopeCheckResult(guid: string, result: ScopeCheckResult, token: string, scopes: Array, metadata: Dictionary) [RobloxSecurity]
```

---

## ExperienceInviteOptions
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
InviteMessageId: string
InviteUser: int64 = 0
LaunchData: string
PromptMessage: string
```

---

## ExperienceNotificationService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
InvokeOptInPromptClosed() → null [RobloxScriptSecurity]
PromptOptIn() → null
CanPromptOptInAsync() → bool
```

### Events
```
OptInPromptClosed()
PromptOptInRequested() [RobloxScriptSecurity]
```

---

## ExperienceService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
ExecuteCrossExperienceCall(callId: string, params: Dictionary, successCallback: Function, errorCallback: Function) → null [RobloxScriptSecurity]
GetPendingJoinAttempt() → Dictionary [RobloxScriptSecurity]
LaunchExperience(params: Dictionary) → string [RobloxScriptSecurity]
LaunchExperienceFromSource(params: Dictionary, source: string) → string [RobloxScriptSecurity]
LaunchExperienceFromSourceWithCallback(params: Dictionary, source: string, callback: Function) → null [RobloxScriptSecurity]
RegisterForExperienceJoin(callback: Function) → RBXScriptConnection [RobloxScriptSecurity]
RegisterForExperienceLeave(callback: Function) → RBXScriptConnection [RobloxScriptSecurity]
StartCrossExperience(type: string, params: Dictionary) → null [RobloxScriptSecurity]
StopCrossExperience(type: string, params: Dictionary) → null [RobloxScriptSecurity]
```

### Events
```
OnCrossExperienceStarted(type: string, params: Dictionary) [RobloxScriptSecurity]
OnCrossExperienceStopped(type: string, params: Dictionary) [RobloxScriptSecurity]
OnNewJoinAttempt(params: Dictionary) [RobloxScriptSecurity]
```

---

## ExperienceStateCaptureService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
HiddenSelectionEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
IsInBackground: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
IsInCaptureMode: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Functions
```
CanEnterCaptureMode() → bool [RobloxScriptSecurity]
ResetHighlight() → null [RobloxScriptSecurity]
ToggleCaptureMode() → null [RobloxScriptSecurity]
```

### Events
```
ItemSelectedInCaptureMode(instance: Instance) [RobloxScriptSecurity]
```

---

## ExperienceStateRecordingService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## ExplorerFilter
**Extends:** Instance
**Tags:** NotReplicated

### Functions
```
BeginSearch(root: Instance) → null [RobloxScriptSecurity]
GetAutocompleter() → ExplorerFilterAutocompleter [RobloxScriptSecurity]
GetErrors() → Array [RobloxScriptSecurity]
GetLexemes() → Array [RobloxScriptSecurity]
GetSearchResults(maxCandidatesToExplore: int) → Instances [RobloxScriptSecurity]
HasMoreResults() → bool [RobloxScriptSecurity]
InstancePassesFilter(instance: Instance) → bool [RobloxScriptSecurity]
SetFilter(search: string) → null [RobloxScriptSecurity]
```

---

## ExplorerFilterAutocompleter
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
ReplaceRange: Vector2 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
RequiresOutsideContext: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Functions
```
GetSuggestions() → Array [RobloxScriptSecurity]
```

---

## ExplorerServiceVisibilityService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetServiceVisibility(service: Instance) → bool
```

---

## Explosion
**Extends:** Instance

### Properties
```
BlastPressure: float = 500000
BlastRadius: float = 4
DestroyJointRadiusPercent: float = 1
ExplosionType: ExplosionType = Craters
LocalTransparencyModifier: float = 0
Position: Vector3 = 0, 0, 0
TimeScale: float = 1
Visible: bool = true
```

### Events
```
Hit(part: BasePart, distance: float)
```

---

## FaceAnimatorService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
AudioAnimationEnabled: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
FaceTrackingStatusEnum: TrackerFaceTrackingStatus = FaceTrackingUninitialized [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
FlipHeadOrientation: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
VideoAnimationEnabled: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
GetTrackerLodController() → TrackerLodController [RobloxScriptSecurity]
Init(videoEnabled: bool, audioEnabled: bool) → null [RobloxScriptSecurity]
IsStarted() → bool [RobloxScriptSecurity]
Start() → null [RobloxScriptSecurity]
Step() → null [RobloxScriptSecurity]
Stop() → null [RobloxScriptSecurity]
```

### Events
```
TrackerError(error: TrackerError) [RobloxScriptSecurity]
TrackerPrompt(prompt: TrackerPromptEvent) [RobloxScriptSecurity]
```

---

## FaceControls
**Extends:** Instance

### Properties
```
ChinRaiser: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
ChinRaiserUpperLip: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
Corrugator: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
EyesLookDown: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
EyesLookLeft: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
EyesLookRight: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
EyesLookUp: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
FlatPucker: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
Funneler: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
JawDrop: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
JawLeft: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
JawRight: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftBrowLowerer: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftCheekPuff: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftCheekRaiser: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftDimpler: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftEyeClosed: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftEyeUpperLidRaiser: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftInnerBrowRaiser: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftLipCornerDown: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftLipCornerPuller: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftLipStretcher: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftLowerLipDepressor: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftNoseWrinkler: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftOuterBrowRaiser: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LeftUpperLipRaiser: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LipPresser: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LipsTogether: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
LowerLipSuck: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
MouthLeft: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
MouthRight: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
Pucker: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightBrowLowerer: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightCheekPuff: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightCheekRaiser: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightDimpler: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightEyeClosed: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightEyeUpperLidRaiser: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightInnerBrowRaiser: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightLipCornerDown: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightLipCornerPuller: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightLipStretcher: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightLowerLipDepressor: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightNoseWrinkler: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightOuterBrowRaiser: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
RightUpperLipRaiser: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
TongueDown: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
TongueOut: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
TongueUp: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
UpperLipSuck: float = 0 [Read:PluginSecurity] [Write:PluginSecurity]
```

---

## FaceInstance
**Extends:** Instance
**Tags:** NotCreatable, NotBrowsable

### Properties
```
Face: NormalId
```

---

## Decal
**Extends:** FaceInstance

### Properties
```
Color3: Color3 = 1, 1, 1
LocalTransparencyModifier: float = 0
MetalnessMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
MetalnessMapContent: Content [Write:PluginSecurity]
NormalMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
NormalMapContent: Content [Write:PluginSecurity]
RoughnessMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
RoughnessMapContent: Content [Write:PluginSecurity]
Shiny: float = 20 [Deprecated]
Specular: float = 0 [Deprecated]
Texture: ContentId
TextureContent: Content
Transparency: float = 0
UVOffset: Vector2 = 0, 0
UVScale: Vector2 = 1, 1
ZIndex: int = 1
```

---

## Texture
**Extends:** Decal

### Properties
```
OffsetStudsU: float = 0
OffsetStudsV: float = 0
StudsPerTileU: float = 2
StudsPerTileV: float = 2
```

---

## FacialAgeEstimationService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
IsAvailable() → bool [RobloxScriptSecurity]
InquiryAsync(inquiryRequest: Dictionary) → Dictionary [RobloxScriptSecurity]
```

---

## FacialAnimationRecordingService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
BiometricDataConsent: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
IsAgeRestricted() → bool [RobloxScriptSecurity]
CheckOrRequestCameraPermission() → string [RobloxScriptSecurity]
```

---

## FacialAnimationStreamingServiceStats
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
Get(label: string) → int64 [RobloxScriptSecurity]
GetWithPlayerId(label: string, playerId: int64) → int64 [RobloxScriptSecurity]
```

---

## FacialAnimationStreamingServiceV2
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
ServiceState: int = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
GetStats() → FacialAnimationStreamingServiceStats [RobloxScriptSecurity]
IsAudioEnabled(mask: int) → bool [RobloxScriptSecurity]
IsPlaceEnabled(mask: int) → bool [RobloxScriptSecurity]
IsServerEnabled(mask: int) → bool [RobloxScriptSecurity]
IsVideoEnabled(mask: int) → bool [RobloxScriptSecurity]
ResolveStateForUser(userId: int64) → int [RobloxScriptSecurity]
```

---

## FacialAnimationStreamingSubsessionStats
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

---

## Feature
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
FaceId: NormalId
InOut: InOut
LeftRight: LeftRight
TopBottom: TopBottom
```

---

## Hole
**Extends:** Feature
**Tags:** Deprecated

---

## MotorFeature
**Extends:** Feature
**Tags:** Deprecated

---

## FeatureRestrictionManager
**Extends:** Instance
**Tags:** NotCreatable, Service

### Events
```
TimeoutChatAttempt(isPermanentTimeout: bool, endTime: int64) [RobloxScriptSecurity]
UpdateExperienceChatTimeout(startTime: int64, duration: int64) [RobloxSecurity]
```

---

## File
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
Size: int64 [Read:PluginSecurity] [Write:PluginSecurity] [ReadOnly]
```

### Functions
```
GetBinaryContents() → string [PluginSecurity]
GetTemporaryId() → ContentId [PluginSecurity]
```

---

## Fire
**Extends:** Instance

### Properties
```
Color: Color3 = 0.92549, 0.545098, 0.27451
Enabled: bool = true
Heat: float = 9
LocalTransparencyModifier: float = 0
SecondaryColor: Color3 = 0.545098, 0.313726, 0.215686
Size: float = 5
TimeScale: float = 1
heat_xml: float = 9
size: float = 5 [Deprecated]
size_xml: float = 5
```

### Functions
```
FastForward(numFrames: int) → null [RobloxScriptSecurity]
```

---

## FlagStandService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## FloatCurve
**Extends:** Instance

### Properties
```
Length: int = 0 [ReadOnly]
ValuesAndTimes: BinaryString = 
```

### Functions
```
GetKeyAtIndex(index: int) → FloatCurveKey
GetKeyIndicesAtTime(time: float) → Array
GetKeys() → Array
GetValueAtTime(time: float) → float?
InsertKey(key: FloatCurveKey) → Array
RemoveKeyAtIndex(startingIndex: int, count: int) → int
SetKeys(keys: Array) → int
```

---

## FlyweightService
**Extends:** Instance
**Tags:** Service

---

## CSGDictionaryService
**Extends:** FlyweightService
**Tags:** Service

---

## NonReplicatedCSGDictionaryService
**Extends:** FlyweightService
**Tags:** Service

---

## Folder
**Extends:** Instance

### Properties
```
ReplicatedGuiInsertionOrder: int = 2147483647 [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## ForceField
**Extends:** Instance

### Properties
```
Visible: bool = true
```

---

## FriendService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
GetPlatformFriends() → Array [RobloxScriptSecurity]
```

### Events
```
FriendsUpdated(friendData: Array) [RobloxScriptSecurity]
RemoteFriendEventSignal(userId: int64, userId: int64, event: FriendRequestEvent) [RobloxSecurity]
RemoteFriendStatusSignal(userId: int64, userId: int64, status: FriendStatus) [RobloxSecurity]
```

---

## FunctionalTest
**Extends:** Instance
**Tags:** Deprecated

### Properties
```
AllowSleep: bool = true
Description: string = ?
HasMigratedSettingsToTestService: bool = false
Is30FpsThrottleEnabled: bool = true
PhysicsEnvironmentalThrottle: bool = true
Timeout: double = 60
```

### Functions
```
Error(message: string) → null
Failed(message: string) → null
Pass(message: string) → null
Passed(message: string) → null
Warn(message: string) → null
```

---

## GamePassService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
PlayerHasPass(player: Player, gamePassId: int64) → bool [Deprecated]
```

---

## GameSettings
**Extends:** Instance
**Tags:** NotCreatable, Settings, NotReplicated, NotBrowsable

### Properties
```
VideoCaptureEnabled: bool
VideoRecording: bool [Read:RobloxScriptSecurity] [Write:RobloxSecurity]
```

### Events
```
VideoRecordingChangeRequest(recording: bool) [RobloxScriptSecurity]
```

---

## GamepadService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
GamepadCursorEnabled: bool = false [Write:RobloxScriptSecurity]
```

### Functions
```
DisableGamepadCursor() → null
EnableGamepadCursor(guiObject: Instance) → null
GetGamepadCursorPosition() → Vector2 [RobloxScriptSecurity]
SetGamepadCursorPosition(position: Vector2) → null [RobloxScriptSecurity]
```

### Events
```
GamepadThumbstick1Changed(event: Vector2) [RobloxScriptSecurity]
```

---

## GenerationService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
GenerateMeshAsync(inputs: Dictionary, player: Player, options: Dictionary, intermediateResultCallback: Function?) → Tuple
InternalGenerateMeshAsync(inputs: Dictionary, userId: int64, options: Dictionary, intermediateResultCallback: Function?) → Tuple [RobloxScriptSecurity]
LoadGeneratedMeshAsync(generationId: string) → MeshPart
```

### Events
```
ReplicateGeneration(id: string, success: bool, serializedModel: string) [RobloxSecurity]
RequestGenerationReplication(id: string) [RobloxSecurity]
```

---

## GenericChallengeService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
SignalChallengeAbandoned(challengeID: string) → null [RobloxScriptSecurity]
SignalChallengeCompleted(challengeID: string, challengeType: string, challengeMetadata: string) → null [RobloxScriptSecurity]
SignalChallengeInvalidated(challengeID: string) → null [RobloxScriptSecurity]
SignalChallengeLoaded(challengeID: string, success: bool) → null [RobloxScriptSecurity]
SignalChallengeRequired(challengeID: string, challengeType: string, challengeMetadata: string) → null [RobloxScriptSecurity]
```

### Events
```
ChallengeAbandonedEvent(challengeID: string) [RobloxScriptSecurity]
ChallengeCompletedEvent(challengeID: string, challengeType: string, challengeMetadata: string) [RobloxScriptSecurity]
ChallengeInvalidatedEvent(challengeID: string) [RobloxScriptSecurity]
ChallengeLoadedEvent(challengeID: string, success: bool) [RobloxScriptSecurity]
ChallengeRequiredEvent(challengeID: string, challengeType: string, challengeMetadata: string) [RobloxScriptSecurity]
```

---

## Geometry
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## GeometryService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
CalculateConstraintsToPreserve(source: Instance, destination: Array, options: Dictionary) → Array
HashMeshAsync(meshId: ContentId) → string [RobloxScriptSecurity]
IntersectAsync(part: Instance, parts: Array, options: Dictionary) → Array
SubtractAsync(part: Instance, parts: Array, options: Dictionary) → Array
UnionAsync(part: Instance, parts: Array, options: Dictionary) → Array
```

---

## GetTextBoundsParams
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
Font: Font
RichText: bool = false
Size: float = 20
Text: string
Width: float = 0
```

---

## GlobalDataStore
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
OnUpdate(key: string, callback: Function) → RBXScriptConnection [Deprecated]
GetAsync(key: string, options: DataStoreGetOptions) → Tuple
IncrementAsync(key: string, delta: int, userIds: Array, options: DataStoreIncrementOptions) → Variant
RemoveAsync(key: string) → Tuple
SetAsync(key: string, value: Variant, userIds: Array, options: DataStoreSetOptions) → Variant
UpdateAsync(key: string, transformFunction: Function) → Tuple
```

---

## DataStore
**Extends:** GlobalDataStore
**Tags:** NotCreatable, NotReplicated

### Functions
```
GetVersionAsync(key: string, version: string) → Tuple
GetVersionAtTimeAsync(key: string, timestamp: int64) → Tuple
ListKeysAsync(prefix: string, pageSize: int, cursor: string, excludeDeleted: bool) → DataStoreKeyPages
ListVersionsAsync(key: string, sortDirection: SortDirection, minDate: int64, maxDate: int64, pageSize: int) → DataStoreVersionPages
RemoveVersionAsync(key: string, version: string) → null
```

---

## OrderedDataStore
**Extends:** GlobalDataStore
**Tags:** NotCreatable, NotReplicated

### Functions
```
GetSortedAsync(ascending: bool, pagesize: int, minValue: Variant, maxValue: Variant) → DataStorePages
```

---

## GroupService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetAlliesAsync(groupId: int64) → StandardPages
GetEnemiesAsync(groupId: int64) → StandardPages
GetGroupInfoAsync(groupId: int64) → Variant
GetGroupsAsync(userId: int64) → Array
```

---

## GuiBase
**Extends:** Instance
**Tags:** NotCreatable

---

## GuiBase2d
**Extends:** GuiBase
**Tags:** NotCreatable, NotBrowsable

### Properties
```
AbsolutePosition: Vector2 [ReadOnly]
AbsoluteRotation: float [ReadOnly]
AbsoluteSize: Vector2 [ReadOnly]
ActiveQueryNames: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AutoLocalize: bool
ClippedRect: Rect [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
IsNotOccluded: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Localize: bool [Deprecated]
RawRect2D: Rect [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
ReplicatedInsertionOrder: int [Read:RobloxSecurity] [Write:RobloxSecurity]
RootLocalizationTable: LocalizationTable
SelectionBehaviorDown: SelectionBehavior
SelectionBehaviorLeft: SelectionBehavior
SelectionBehaviorRight: SelectionBehavior
SelectionBehaviorUp: SelectionBehavior
SelectionGroup: bool
TotalGroupScale: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Events
```
SelectionChanged(amISelected: bool, previousSelection: GuiObject, newSelection: GuiObject)
```

---

## GuiObject
**Extends:** GuiBase2d
**Tags:** NotCreatable, NotBrowsable

### Properties
```
Active: bool
AnchorPoint: Vector2
AutomaticSize: AutomaticSize
BackgroundColor: BrickColor [Deprecated]
BackgroundColor3: Color3
BackgroundTransparency: float
BorderColor: BrickColor [Deprecated]
BorderColor3: Color3
BorderMode: BorderMode
BorderSizePixel: int
ClipsDescendants: bool
DragBeginConnectionCount: int
DragStoppedConnectionCount: int
Draggable: bool [Deprecated]
GuiState: GuiState [ReadOnly]
Interactable: bool
LayoutOrder: int
MouseEnterConnectionCount: int
MouseLeaveConnectionCount: int
MouseMovedConnectionCount: int
MouseWheelBackwardConnectionCount: int
MouseWheelForwardConnectionCount: int
NextSelectionDown: GuiObject
NextSelectionLeft: GuiObject
NextSelectionRight: GuiObject
NextSelectionUp: GuiObject
Position: UDim2
Rotation: float
Selectable: bool
SelectionImageObject: GuiObject
SelectionOrder: int
SelectionRect2D: Rect [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Size: UDim2
SizeConstraint: SizeConstraint
Transparency: float
Visible: bool
ZIndex: int
```

### Functions
```
TweenPosition(endPosition: UDim2, easingDirection: EasingDirection, easingStyle: EasingStyle, time: float, override: bool, callback: Function) → bool
TweenSize(endSize: UDim2, easingDirection: EasingDirection, easingStyle: EasingStyle, time: float, override: bool, callback: Function) → bool
TweenSizeAndPosition(endSize: UDim2, endPosition: UDim2, easingDirection: EasingDirection, easingStyle: EasingStyle, time: float, override: bool, callback: Function) → bool
```

### Events
```
DragBegin(initialPosition: UDim2)
DragStopped(x: int, y: int)
InputBegan(input: InputObject)
InputChanged(input: InputObject)
InputEnded(input: InputObject)
MouseEnter(x: int, y: int)
MouseLeave(x: int, y: int)
MouseMoved(x: int, y: int)
MouseWheelBackward(x: int, y: int)
MouseWheelForward(x: int, y: int)
SelectionGained()
SelectionLost()
TouchLongPress(touchPositions: Array, state: UserInputState)
TouchPan(touchPositions: Array, totalTranslation: Vector2, velocity: Vector2, state: UserInputState)
TouchPinch(touchPositions: Array, scale: float, velocity: float, state: UserInputState)
TouchRotate(touchPositions: Array, rotation: float, velocity: float, state: UserInputState)
TouchSwipe(swipeDirection: SwipeDirection, numberOfTouches: int)
TouchTap(touchPositions: Array)
```

---

## CanvasGroup
**Extends:** GuiObject

### Properties
```
GroupColor3: Color3 = 1, 1, 1
GroupTransparency: float = 0
ResolutionScale: float = 1 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

---

## Frame
**Extends:** GuiObject

### Properties
```
Style: FrameStyle = Custom
```

---

## GuiButton
**Extends:** GuiObject
**Tags:** NotCreatable, NotBrowsable

### Properties
```
AutoButtonColor: bool
HoverHapticEffect: HapticEffect
Modal: bool
MouseButton1ClickConnectionCount: int
MouseButton1DownConnectionCount: int
MouseButton1UpConnectionCount: int
MouseButton2ClickConnectionCount: int
MouseButton2DownConnectionCount: int
MouseButton2UpConnectionCount: int
PressHapticEffect: HapticEffect
Selected: bool
Style: ButtonStyle
```

### Events
```
Activated(inputObject: InputObject, clickCount: int)
MouseButton1Click()
MouseButton1Down(x: int, y: int)
MouseButton1Up(x: int, y: int)
MouseButton2Click()
MouseButton2Down(x: int, y: int)
MouseButton2Up(x: int, y: int)
```

---

## ImageButton
**Extends:** GuiButton

### Properties
```
ContentImageSize: Vector2 = 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
HoverImage: ContentId
HoverImageContent: Content
Image: ContentId
ImageColor3: Color3 = 1, 1, 1
ImageContent: Content
ImageRectOffset: Vector2 = 0, 0
ImageRectSize: Vector2 = 0, 0
ImageTransparency: float = 0
IsLoaded: bool = false [ReadOnly]
PressedImage: ContentId
PressedImageContent: Content
ResampleMode: ResamplerMode = Default
ScaleType: ScaleType = Stretch
SliceCenter: Rect = 0, 0, 0, 0
SliceScale: float = 1
TileSize: UDim2 = {1, 0}, {1, 0}
```

### Functions
```
SetEnableContentImageSizeChangedEvents(enabled: bool) → null [RobloxScriptSecurity]
```

---

## TextButton
**Extends:** GuiButton

### Properties
```
Confidential: bool = false [Read:RobloxSecurity] [Write:RobloxSecurity]
ContentText: string = Button [ReadOnly]
Font: Font = Legacy
FontFace: Font
FontSize: FontSize = Size8 [Deprecated]
LineHeight: float = 1
LocalizationMatchIdentifier: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LocalizationMatchedSourceText: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LocalizedText: string [ReadOnly]
MaxVisibleGraphemes: int = -1
OpenTypeFeatures: string
OpenTypeFeaturesError: string [ReadOnly]
RichText: bool = false
Text: string = Button
TextBounds: Vector2 = 0, 0 [ReadOnly]
TextColor: BrickColor [Deprecated]
TextColor3: Color3 = 0.105882, 0.164706, 0.207843
TextDirection: TextDirection = Auto
TextFits: bool = false [ReadOnly]
TextScaled: bool = false
TextSize: float = 8
TextStrokeColor3: Color3 = 0, 0, 0
TextStrokeTransparency: float = 1
TextTransparency: float = 0
TextTruncate: TextTruncate = None
TextWrap: bool = false [Deprecated]
TextWrapped: bool = false
TextXAlignment: TextXAlignment = Center
TextYAlignment: TextYAlignment = Center
```

### Functions
```
SetTextFromInput(text: string) → null [RobloxScriptSecurity]
```

---

## GuiLabel
**Extends:** GuiObject
**Tags:** NotCreatable

---

## ImageLabel
**Extends:** GuiLabel

### Properties
```
ContentImageSize: Vector2 = 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Image: ContentId
ImageColor3: Color3 = 1, 1, 1
ImageContent: Content
ImageRectOffset: Vector2 = 0, 0
ImageRectSize: Vector2 = 0, 0
ImageTransparency: float = 0
IsLoaded: bool = false [ReadOnly]
ResampleMode: ResamplerMode = Default
ScaleType: ScaleType = Stretch
SliceCenter: Rect = 0, 0, 0, 0
SliceScale: float = 1
TileSize: UDim2 = {1, 0}, {1, 0}
```

### Functions
```
SetEnableContentImageSizeChangedEvents(enabled: bool) → null [RobloxScriptSecurity]
```

---

## TextLabel
**Extends:** GuiLabel

### Properties
```
Confidential: bool = false [Read:RobloxSecurity] [Write:RobloxSecurity]
ContentText: string = Label [ReadOnly]
Font: Font = Legacy
FontFace: Font
FontSize: FontSize = Size8 [Deprecated]
LineHeight: float = 1
LocalizationMatchIdentifier: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LocalizationMatchedSourceText: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LocalizedText: string [ReadOnly]
MaxVisibleGraphemes: int = -1
OpenTypeFeatures: string
OpenTypeFeaturesError: string [ReadOnly]
RichText: bool = false
Text: string = Label
TextBounds: Vector2 = 0, 0 [ReadOnly]
TextColor: BrickColor [Deprecated]
TextColor3: Color3 = 0.105882, 0.164706, 0.207843
TextDirection: TextDirection = Auto
TextFits: bool = false [ReadOnly]
TextScaled: bool = false
TextSize: float = 8
TextStrokeColor3: Color3 = 0, 0, 0
TextStrokeTransparency: float = 1
TextTransparency: float = 0
TextTruncate: TextTruncate = None
TextWrap: bool = false [Deprecated]
TextWrapped: bool = false
TextXAlignment: TextXAlignment = Center
TextYAlignment: TextYAlignment = Center
```

### Functions
```
SetTextFromInput(text: string) → null [RobloxScriptSecurity]
```

---

## RelativeGui
**Extends:** GuiObject
**Tags:** NotReplicated

---

## ScrollingFrame
**Extends:** GuiObject

### Properties
```
AbsoluteCanvasSize: Vector2 = 0, 0 [ReadOnly]
AbsoluteWindowSize: Vector2 = 0, 0 [ReadOnly]
AutomaticCanvasSize: AutomaticSize = None
BottomImage: ContentId = rbxasset://textures/ui/Scroll/scroll-bottom.png
BottomImageContent: Content
CanvasPosition: Vector2 = 0, 0
CanvasSize: UDim2 = {0, 0}, {2, 0}
DraggingScrollBar: DraggingScrollBar = None [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
ElasticBehavior: ElasticBehavior = WhenScrollable
HorizontalBarRect: Rect = 0, 0, 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
HorizontalScrollBarInset: ScrollBarInset = None
MaxCanvasPosition: Vector2 = 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
MidImage: ContentId = rbxasset://textures/ui/Scroll/scroll-middle.png
MidImageContent: Content
ScrollBarImageColor3: Color3 = 1, 1, 1
ScrollBarImageTransparency: float = 0
ScrollBarThickness: int = 12
ScrollRate: float = 1 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ScrollVelocity: Vector2 = 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ScrollingDirection: ScrollingDirection = XY
ScrollingEnabled: bool = true
SmoothScroll: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
TopImage: ContentId = rbxasset://textures/ui/Scroll/scroll-top.png
TopImageContent: Content
VerticalBarRect: Rect = 0, 0, 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
VerticalScrollBarInset: ScrollBarInset = None
VerticalScrollBarPosition: VerticalScrollBarPosition = Right
```

### Functions
```
ClearInertialScrolling() → null [RobloxScriptSecurity]
GetSampledInertialVelocity() → Vector2 [RobloxScriptSecurity]
ScrollToTop() → null [RobloxScriptSecurity]
```

---

## TextBox
**Extends:** GuiObject

### Properties
```
ClearTextOnFocus: bool = true
Confidential: bool = false [Read:RobloxSecurity] [Write:RobloxSecurity]
ContentText: string = TextBox [ReadOnly]
CursorPosition: int = 1
Font: Font = Legacy
FontFace: Font
FontSize: FontSize = Size8 [Deprecated]
LineHeight: float = 1
LocalizationMatchIdentifier: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LocalizationMatchedSourceText: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LocalizedPlaceholderText: string [Read:RobloxSecurity] [Write:RobloxSecurity] [ReadOnly]
ManualFocusRelease: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
MaxVisibleGraphemes: int = -1
MultiLine: bool = false
OpenTypeFeatures: string
OpenTypeFeaturesError: string [ReadOnly]
OverlayNativeInput: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
PlaceholderColor3: Color3 = 0.7, 0.7, 0.7
PlaceholderText: string
ReturnKeyType: ReturnKeyType = Default [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
RichText: bool = false
SelectionStart: int = -1
ShouldEmitReturnEvents: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ShouldEmitTabEvents: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ShouldEmitUpAndDownArrowEvents: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ShowNativeInput: bool = true
Text: string = TextBox
TextBounds: Vector2 = 0, 0 [ReadOnly]
TextColor: BrickColor [Deprecated]
TextColor3: Color3 = 0.105882, 0.164706, 0.207843
TextDirection: TextDirection = Auto
TextEditable: bool = true
TextFits: bool = false [ReadOnly]
TextInputType: TextInputType = Default [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
TextScaled: bool = false
TextSize: float = 8
TextStrokeColor3: Color3 = 0, 0, 0
TextStrokeTransparency: float = 1
TextTransparency: float = 0
TextTruncate: TextTruncate = None
TextWrap: bool = false [Deprecated]
TextWrapped: bool = false
TextXAlignment: TextXAlignment = Center
TextYAlignment: TextYAlignment = Center
```

### Functions
```
CaptureFocus() → null
IsFocused() → bool
ReleaseFocus(submitted: bool) → null
ResetKeyboardMode() → null [RobloxScriptSecurity]
SetTextFromInput(text: string) → null [RobloxScriptSecurity]
```

### Events
```
FocusLost(enterPressed: bool, inputThatCausedFocusLoss: InputObject)
Focused()
ReturnPressedFromOnScreenKeyboard()
```

---

## VideoDisplay
**Extends:** GuiObject
**Tags:** NotBrowsable

### Properties
```
ResampleMode: ResamplerMode = Default
ScaleType: ScaleType = Stretch
TileSize: UDim2 = {1, 0}, {1, 0}
VideoColor3: Color3 = 1, 1, 1
VideoRectOffset: Vector2 = 0, 0
VideoRectSize: Vector2 = 0, 0
VideoTransparency: float = 0
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

### Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## VideoFrame
**Extends:** GuiObject

### Properties
```
IsLoaded: bool = false [ReadOnly]
Looped: bool = false
Playing: bool = false
PlayingReplicating: bool = false
Resolution: Vector2 = 0, 0 [ReadOnly]
TimeLength: double = 0 [ReadOnly]
TimePosition: double = 0
TimePositionReplicating: double = 0
Video: ContentId
VideoContent: Content
Volume: float = 1
```

### Functions
```
Pause() → null
Play() → null
SetStudioPreview(isPreview: bool) → null [RobloxScriptSecurity]
```

### Events
```
DidLoop(video: string)
Ended(video: string)
Loaded(video: string)
Paused(video: string)
Played(video: string)
PlayingUpdatedFromServer(value: bool) [RobloxSecurity]
TimePositionUpdatedFromServer(value: double) [RobloxSecurity]
```

---

## ViewportFrame
**Extends:** GuiObject

### Properties
```
Ambient: Color3 = 0.784314, 0.784314, 0.784314
CameraCFrame: CFrame
CameraFieldOfView: float = 1.22173059
CurrentCamera: Camera
ImageColor3: Color3 = 1, 1, 1
ImageTransparency: float = 0
IsMirrored: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LightColor: Color3 = 0.54902, 0.54902, 0.54902
LightDirection: Vector3 = -1, -1, -1
```

### Functions
```
CaptureSnapshotAsync() → ContentId [RobloxScriptSecurity]
```

---

## LayerCollector
**Extends:** GuiBase2d
**Tags:** NotCreatable, NotBrowsable

### Properties
```
Enabled: bool
ResetOnSpawn: bool
ZIndexBehavior: ZIndexBehavior
```

### Functions
```
GetGuiObjectsAtPosition(x: int, y: int) → Instances [RobloxScriptSecurity]
GetLayoutNodeTree() → Dictionary [Deprecated]
```

---

## BillboardGui
**Extends:** LayerCollector

### Properties
```
Active: bool = false
Adornee: Instance
AlwaysOnTop: bool = false
Brightness: float = 1
ClipsDescendants: bool = false
CurrentDistance: float = 0 [ReadOnly]
DistanceLowerLimit: float = 0
DistanceStep: float = 0
DistanceUpperLimit: float = -1
ExtentsOffset: Vector3 = 0, 0, 0
ExtentsOffsetWorldSpace: Vector3 = 0, 0, 0
LightInfluence: float = 0
MaxDistance: float = INF
PlayerToHideFrom: Instance
Size: UDim2 = {0, 0}, {0, 0}
SizeOffset: Vector2 = 0, 0
StudsOffset: Vector3 = 0, 0, 0
StudsOffsetWorldSpace: Vector3 = 0, 0, 0
```

### Functions
```
GetScreenSpaceBounds() → Variant [RobloxScriptSecurity]
```

---

## PluginGui
**Extends:** LayerCollector
**Tags:** NotCreatable, NotReplicated

### Properties
```
Title: string
```

### Functions
```
BindToClose(function: Function) → null
GetRelativeMousePosition() → Vector2 [PluginSecurity]
```

### Events
```
InputBegan(input: InputObject, gameProcessedEvent: bool) [RobloxScriptSecurity]
InputChanged(input: InputObject, gameProcessedEvent: bool) [RobloxScriptSecurity]
InputEnded(input: InputObject, gameProcessedEvent: bool) [RobloxScriptSecurity]
MouseEnter() [RobloxScriptSecurity]
MouseLeave() [RobloxScriptSecurity]
PluginDragDropped(dragData: Dictionary) [PluginSecurity]
PluginDragEntered(dragData: Dictionary) [PluginSecurity]
PluginDragLeft(dragData: Dictionary) [PluginSecurity]
PluginDragMoved(dragData: Dictionary) [PluginSecurity]
WindowFocusReleased() [PluginSecurity]
WindowFocused() [PluginSecurity]
```

---

## DockWidgetPluginGui
**Extends:** PluginGui
**Tags:** NotCreatable, NotReplicated

### Properties
```
HostWidgetWasRestored: bool = false [ReadOnly]
```

### Functions
```
RequestRaise() → null [RobloxScriptSecurity]
```

---

## QWidgetPluginGui
**Extends:** PluginGui
**Tags:** NotCreatable, NotReplicated

---

## ScreenGui
**Extends:** LayerCollector

### Properties
```
ClipToDeviceSafeArea: bool = true
DisplayOrder: int = 0
IgnoreGuiInset: bool = false
OnTopOfCoreBlur: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
SafeAreaCompatibility: SafeAreaCompatibility = FullscreenExtension
ScreenInsets: ScreenInsets = CoreUISafeInsets
```

---

## GuiMain
**Extends:** ScreenGui
**Tags:** Deprecated

---

## SurfaceGuiBase
**Extends:** LayerCollector
**Tags:** NotCreatable

### Properties
```
Active: bool
Adornee: Instance
Face: NormalId
```

---

## AdGui
**Extends:** SurfaceGuiBase

### Properties
```
AdShape: AdShape = HorizontalRectangle
EnableVideoAds: bool = true
FallbackImage: ContentId
Status: AdUnitStatus = Inactive [ReadOnly]
```

### Functions
```
GetSingleReportAdInfo() → Map [RobloxScriptSecurity]
HandleLuaUIEvent(eventType: AdUIEventType) → null [RobloxScriptSecurity]
forwardStateToLuaUI() → null [RobloxScriptSecurity]
```

### Events
```
AdEvent(adEventType: AdEventType) [RobloxSecurity]
ReportIsSubscribedToVideoCompletion() [RobloxSecurity]
adGuiStateChanged(adUIState: Variant) [RobloxScriptSecurity]
```

---

## SurfaceGui
**Extends:** SurfaceGuiBase

### Properties
```
AlwaysOnTop: bool = false
Brightness: float = 1
CanvasSize: Vector2 = 800, 600
ClipsDescendants: bool = false
HorizontalCurvature: float = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LightInfluence: float = 0
MaxDistance: float = 0
PixelsPerStud: float = 50
Shape: SurfaceGuiShape = Flat [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
SizingMode: SurfaceGuiSizingMode = FixedSize
ToolPunchThroughDistance: float = 0
ZOffset: float = 0
```

---

## GuiBase3d
**Extends:** GuiBase
**Tags:** NotCreatable

### Properties
```
Color: BrickColor [Deprecated]
Color3: Color3
Transparency: float
Visible: bool
```

---

## FloorWire
**Extends:** GuiBase3d
**Tags:** Deprecated

### Properties
```
CycleOffset: float = 0
From: BasePart
StudsBetweenTextures: float = 4
Texture: ContentId
TextureSize: Vector2 = 1, 1
To: BasePart
Velocity: float = 2
WireRadius: float = 0.0625
```

---

## InstanceAdornment
**Extends:** GuiBase3d
**Tags:** NotCreatable

### Properties
```
Adornee: Instance
```

---

## SelectionBox
**Extends:** InstanceAdornment

### Properties
```
LineThickness: float = 0.150000006
StudioSelectionBox: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
SurfaceColor: BrickColor [Deprecated]
SurfaceColor3: Color3 = 0.0509804, 0.411765, 0.67451
SurfaceTransparency: float = 1
```

---

## PVAdornment
**Extends:** GuiBase3d
**Tags:** NotCreatable

### Properties
```
Adornee: PVInstance
```

---

## HandleAdornment
**Extends:** PVAdornment
**Tags:** NotCreatable

### Properties
```
AdornCullingMode: AdornCullingMode
AlwaysOnTop: bool
CFrame: CFrame
SizeRelativeOffset: Vector3
ZIndex: int
```

### Events
```
MouseButton1Down()
MouseButton1Up()
MouseEnter()
MouseLeave()
```

---

## BoxHandleAdornment
**Extends:** HandleAdornment

### Properties
```
Size: Vector3 = 1, 1, 1
```

---

## ConeHandleAdornment
**Extends:** HandleAdornment

### Properties
```
Height: float = 2
Radius: float = 0.5
```

---

## CylinderHandleAdornment
**Extends:** HandleAdornment

### Properties
```
Angle: float = 360
Height: float = 1
InnerRadius: float = 0
Radius: float = 1
```

---

## ImageHandleAdornment
**Extends:** HandleAdornment

### Properties
```
Image: ContentId = rbxasset://textures/SurfacesDefault.png
Size: Vector2 = 1, 1
```

---

## LineHandleAdornment
**Extends:** HandleAdornment

### Properties
```
Length: float = 5
Thickness: float = 1
```

---

## SphereHandleAdornment
**Extends:** HandleAdornment

### Properties
```
Radius: float = 1
```

---

## WireframeHandleAdornment
**Extends:** HandleAdornment

### Properties
```
Scale: Vector3 = 1, 1, 1
Thickness: float = 1
```

### Functions
```
AddLine(from: Vector3, to: Vector3) → null
AddLines(points: Array) → null
AddPath(points: Array, loop: bool) → null
AddText(point: Vector3, text: string, size: int) → null
Clear() → null
```

---

## ParabolaAdornment
**Extends:** PVAdornment

### Properties
```
A: float = 1 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
B: float = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
C: float = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Range: float = 1 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Thickness: float = 1 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
FindPartOnParabola(ignoreDescendentsTable: Instances) → Tuple [RobloxScriptSecurity]
```

---

## SelectionSphere
**Extends:** PVAdornment

### Properties
```
SurfaceColor: BrickColor [Deprecated]
SurfaceColor3: Color3 = 0.0509804, 0.411765, 0.67451
SurfaceTransparency: float = 1
```

---

## PartAdornment
**Extends:** GuiBase3d
**Tags:** NotCreatable

### Properties
```
Adornee: BasePart
```

---

## HandlesBase
**Extends:** PartAdornment
**Tags:** NotCreatable

---

## ArcHandles
**Extends:** HandlesBase

### Properties
```
Axes: Axes = X, Y, Z
MouseButton1DownConnectionCount: int = 0
MouseButton1UpConnectionCount: int = 0
MouseDragConnectionCount: int = 0
MouseEnterConnectionCount: int = 0
MouseLeaveConnectionCount: int = 0
```

### Events
```
MouseButton1Down(axis: Axis)
MouseButton1Up(axis: Axis)
MouseDrag(axis: Axis, relativeAngle: float, deltaRadius: float)
MouseEnter(axis: Axis)
MouseLeave(axis: Axis)
```

---

## Handles
**Extends:** HandlesBase

### Properties
```
Faces: Faces = Right, Top, Back, Left, Bottom, Front
MouseButton1DownConnectionCount: int = 0
MouseButton1UpConnectionCount: int = 0
MouseDragConnectionCount: int = 0
MouseEnterConnectionCount: int = 0
MouseLeaveConnectionCount: int = 0
Style: HandlesStyle = Resize
```

### Events
```
MouseButton1Down(face: NormalId)
MouseButton1Up(face: NormalId)
MouseDrag(face: NormalId, distance: float)
MouseEnter(face: NormalId)
MouseLeave(face: NormalId)
```

---

## SurfaceSelection
**Extends:** PartAdornment

### Properties
```
TargetSurface: NormalId = Right
```

---

## SelectionLasso
**Extends:** GuiBase3d
**Tags:** NotCreatable

### Properties
```
Humanoid: Humanoid
```

---

## SelectionPartLasso
**Extends:** SelectionLasso
**Tags:** Deprecated

### Properties
```
Part: BasePart
```

---

## SelectionPointLasso
**Extends:** SelectionLasso
**Tags:** Deprecated

### Properties
```
Point: Vector3 = 0, 0, 0
```

---

## Path2D
**Extends:** GuiBase

### Properties
```
Closed: bool = false
Color3: Color3 = 0, 0, 0
PropertiesSerialize: BinaryString [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
SelectedControlPoint: int = 1 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
SelectedControlPointData: Path2DControlPoint [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Thickness: float = 1
Transparency: float = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Visible: bool = true
ZIndex: int = 1
```

### Functions
```
GetBoundingRect() → Rect
GetControlPoint(index: int) → Path2DControlPoint
GetControlPoints() → Array
GetLength() → float
GetMaxControlPoints() → int
GetPositionOnCurve(t: float) → UDim2
GetPositionOnCurveArcLength(t: float) → UDim2
GetSegmentCount() → int [RobloxScriptSecurity]
GetTangentOnCurve(t: float) → Vector2
GetTangentOnCurveArcLength(t: float) → Vector2
InsertControlPoint(index: int, point: Path2DControlPoint) → null
RemoveControlPoint(index: int) → null
SetControlPoints(controlPoints: Array) → null
UpdateControlPoint(index: int, point: Path2DControlPoint) → null
```

### Events
```
ControlPointChanged()
```

---

## GuiService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
AutoSelectGuiEnabled: bool
CoreEffectFolder: Folder [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CoreGuiFolder: Folder [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CoreGuiNavigationEnabled: bool
GuiNavigationEnabled: bool
IsModalDialog: bool [ReadOnly] [Deprecated]
IsWindows: bool [ReadOnly] [Deprecated]
MenuIsOpen: bool [ReadOnly]
PreferredTextSize: PreferredTextSize [ReadOnly]
PreferredTransparency: float [ReadOnly]
ReducedMotionEnabled: bool [ReadOnly]
SelectedCoreObject: GuiObject [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
SelectedObject: GuiObject
TopbarInset: Rect [ReadOnly]
TouchControlsEnabled: bool
ViewportDisplaySize: DisplaySize [ReadOnly]
ViewportSizeInMM: Vector2 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Functions
```
AddCenterDialog(dialog: Instance, centerDialogType: CenterDialogType, showFunction: Function, hideFunction: Function) → null [RobloxScriptSecurity]
AddKey(key: string) → null [RobloxScriptSecurity]
AddSelectionParent(selectionName: string, selectionParent: Instance) → null [Deprecated]
AddSelectionTuple(selectionName: string, selections: Tuple) → null [Deprecated]
AddSpecialKey(key: SpecialKey) → null [RobloxScriptSecurity]
BroadcastNotification(data: string, notificationType: int) → null [RobloxScriptSecurity]
ClearError() → null [RobloxScriptSecurity]
CloseInspectMenu() → null
CloseStatsBasedOnInputString(input: string) → bool [RobloxScriptSecurity]
DismissNotification(notificationId: string) → bool
ForceTenFootInterface(isForced: bool) → null [RobloxScriptSecurity]
GetBrickCount() → int [RobloxScriptSecurity]
GetClosestDialogToPosition(position: Vector3) → Instance [RobloxScriptSecurity]
GetClosestVisibleDialogToPosition(position: Vector3) → Dialog [RobloxScriptSecurity]
GetEmotesMenuOpen() → bool
GetErrorCode() → ConnectionError [RobloxScriptSecurity]
GetErrorDetails() → Dictionary [RobloxScriptSecurity]
GetErrorMessage() → string [RobloxScriptSecurity] [Deprecated]
GetErrorType() → ConnectionError [RobloxScriptSecurity]
GetGameplayPausedNotificationEnabled() → bool
GetGuiInset() → Tuple
GetGuiIsVisible(guiType: GuiType) → bool [RobloxScriptSecurity]
GetHardwareSafeViewport() → Vector2 [RobloxScriptSecurity]
GetInspectMenuEnabled() → bool
GetNotificationTypeList() → Dictionary [RobloxScriptSecurity]
GetRawScreenScale() → float [RobloxScriptSecurity]
GetResolutionScale() → int [RobloxScriptSecurity]
GetSafeZoneOffsets() → Dictionary [RobloxScriptSecurity]
GetUiMessage() → string [RobloxScriptSecurity]
InspectPlayerFromHumanoidDescription(humanoidDescription: Instance, name: string) → null
InspectPlayerFromUserId(userId: int64) → null
InspectPlayerFromUserIdWithCtx(userId: int64, ctx: string) → null [RobloxScriptSecurity]
IsMemoryTrackerEnabled() → bool [RobloxScriptSecurity]
IsTenFootInterface() → bool
OnNotificationDisplayed(notificationId: string) → null [RobloxScriptSecurity]
OnNotificationInteraction(notificationId: string, buttonIndex: int) → null [RobloxScriptSecurity]
OpenBrowserWindow(url: string) → null [RobloxScriptSecurity] [Deprecated]
OpenNativeOverlay(title: string, url: string) → null [RobloxScriptSecurity] [Deprecated]
RemoveCenterDialog(dialog: Instance) → null [RobloxScriptSecurity]
RemoveKey(key: string) → null [RobloxScriptSecurity]
RemoveSelectionGroup(selectionName: string) → null [Deprecated]
RemoveSpecialKey(key: SpecialKey) → null [RobloxScriptSecurity]
Select(selectionParent: Instance) → null
SendNotification(notificationInfo: Dictionary) → string
SendUIOcclusionMetricsForQueryRegion(position: UDim2, size: UDim2, regionName: string) → null [RobloxScriptSecurity]
SetEmotesMenuOpen(isOpen: bool) → null
SetGameplayPausedNotificationEnabled(enabled: bool) → null
SetGlobalGuiInset(x1: int, y1: int, x2: int, y2: int) → null [RobloxScriptSecurity]
SetHardwareSafeAreaInsets(left: float, top: float, right: float, bottom: float) → null [RobloxScriptSecurity]
SetInspectMenuEnabled(enabled: bool) → null
SetMenuIsOpen(open: bool, menuName: string) → null [RobloxScriptSecurity]
SetPurchasePromptIsShown(isShown: bool) → null [RobloxScriptSecurity]
SetSafeZoneOffsets(top: float, bottom: float, left: float, right: float) → null [RobloxScriptSecurity]
SetTopbarInset(topbarInset: Rect) → null [RobloxScriptSecurity]
SetUiMessage(msgType: UiMessageType, uiMessage: string) → null [LocalUserSecurity]
ShowStatsBasedOnInputString(input: string) → bool [RobloxScriptSecurity]
ToggleFullscreen() → null [RobloxScriptSecurity]
ToggleGuiIsVisibleForCaptures(guiType: GuiType) → null [RobloxScriptSecurity]
ToggleGuiIsVisibleIfAllowed(guiType: GuiType) → null [RobloxScriptSecurity]
GetScreenResolution() → Vector2 [RobloxScriptSecurity]
```

### Events
```
BrowserWindowClosed() [RobloxScriptSecurity]
CloseInspectMenuRequest() [RobloxScriptSecurity]
CoreGuiRenderOverflowed() [RobloxScriptSecurity]
EmotesMenuOpenChanged(isOpen: bool) [RobloxScriptSecurity]
ErrorMessageChanged(newErrorMessage: string) [RobloxScriptSecurity]
GuiVisibilityChangedSignal(guiType: GuiType, visible: bool) [RobloxScriptSecurity]
InspectMenuEnabledChangedSignal(enabled: bool) [RobloxScriptSecurity]
InspectPlayerFromHumanoidDescriptionRequest(humanoidDescription: Instance, name: string) [RobloxScriptSecurity]
InspectPlayerFromUserIdWithCtxRequest(userId: int64, ctx: string) [RobloxScriptSecurity]
KeyPressed(key: string, modifiers: string) [RobloxScriptSecurity]
MenuClosed()
MenuOpened()
NativeClose() [RobloxScriptSecurity]
NetworkPausedEnabledChanged(enabled: bool) [RobloxScriptSecurity]
Open9SliceEditor(selectedImageObject: Instance) [RobloxScriptSecurity]
OpenStyleEditor(styleBase: Instance) [RobloxScriptSecurity]
PurchasePromptShown() [RobloxScriptSecurity]
SafeZoneOffsetsChanged() [RobloxScriptSecurity]
ShowLeaveConfirmation() [RobloxScriptSecurity]
SpecialKeyPressed(key: SpecialKey, modifiers: string) [RobloxScriptSecurity]
UiMessageChanged(msgType: UiMessageType, newUiMessage: string) [RobloxScriptSecurity]
```

---

## GuidRegistryService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## HandRigDescription
**Extends:** Instance
**Tags:** NotBrowsable

### Properties
```
Index1: Instance
Index1TposeAdjustment: CFrame
Index2: Instance
Index2TposeAdjustment: CFrame
Index3: Instance
Index3TposeAdjustment: CFrame
IndexRange: Vector3 = 0, 0, 0
IndexSize: float = 0
Middle1: Instance
Middle1TposeAdjustment: CFrame
Middle2: Instance
Middle2TposeAdjustment: CFrame
Middle3: Instance
Middle3TposeAdjustment: CFrame
MiddleRange: Vector3 = 0, 0, 0
MiddleSize: float = 0
Pinky1: Instance
Pinky1TposeAdjustment: CFrame
Pinky2: Instance
Pinky2TposeAdjustment: CFrame
Pinky3: Instance
Pinky3TposeAdjustment: CFrame
PinkyRange: Vector3 = 0, 0, 0
PinkySize: float = 0
Ring1: Instance
Ring1TposeAdjustment: CFrame
Ring2: Instance
Ring2TposeAdjustment: CFrame
Ring3: Instance
Ring3TposeAdjustment: CFrame
RingRange: Vector3 = 0, 0, 0
RingSize: float = 0
Side: HandRigDescriptionSide = None
Thumb1: Instance
Thumb1TposeAdjustment: CFrame
Thumb2: Instance
Thumb2TposeAdjustment: CFrame
Thumb3: Instance
Thumb3TposeAdjustment: CFrame
ThumbRange: Vector3 = 0, 0, 0
ThumbSize: float = 0
```

### Functions
```
GetFingerControl(fingerIndex: int) → Vector3
GetFingerTip(fingerIndex: int) → Vector3
SetFingerControl(fingerIndex: int, control: Vector3) → null
SetFingerTip(fingerIndex: int, point: Vector3) → null
```

---

## HapticEffect
**Extends:** Instance

### Properties
```
Looped: bool = false
Position: Vector3 = 0, 0, 0
Radius: float = 3
Type: HapticEffectType = UIClick
Waveform: FloatCurve [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
Play() → null
SetWaveformKeys(keys: Array) → null
Stop() → null
```

---

## HapticService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetMotor(inputType: UserInputType, vibrationMotor: VibrationMotor) → Tuple
IsMotorSupported(inputType: UserInputType, vibrationMotor: VibrationMotor) → bool
IsVibrationSupported(inputType: UserInputType) → bool
SetMotor(inputType: UserInputType, vibrationMotor: VibrationMotor, vibrationValues: Tuple) → null
```

---

## HarmonyService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## HeapProfilerService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
ClientRequestDataAsync(player: Player) → string [PluginSecurity]
ServerRequestDataAsync() → string [PluginSecurity]
```

### Events
```
OnNewData(player: Player, jsonString: buffer, id: int, compressedLength: int, uncompressedLength: int) [PluginSecurity]
RequestData(id: int) [RobloxSecurity]
```

---

## HeatmapService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## HeightmapImporterService
**Extends:** Instance
**Tags:** Service, NotReplicated

### Functions
```
CancelImportHeightmap() → null [RobloxScriptSecurity]
IsValidColormap(colormapAssetId: ContentId) → Tuple [RobloxScriptSecurity]
IsValidHeightmap(heightmapAssetId: ContentId) → Tuple [RobloxScriptSecurity]
SetImportHeightmapPaused(paused: bool) → null [RobloxScriptSecurity]
GetHeightmapPreviewAsync(heightmapAssetId: ContentId) → Tuple [RobloxScriptSecurity]
ImportHeightmap(region: Region3, heightmapAssetId: ContentId, colormapAssetId: ContentId, defaultMaterial: Material) → null [RobloxScriptSecurity]
```

### Events
```
ColormapHasUnknownPixels() [RobloxScriptSecurity]
ProgressUpdate(progressRatio: float, operation: string) [RobloxScriptSecurity]
```

---

## HiddenSurfaceRemovalAsset
**Extends:** Instance

### Properties
```
HSRData: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
HSRMeshIdData: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## Highlight
**Extends:** Instance

### Properties
```
Adornee: Instance
DepthMode: HighlightDepthMode = AlwaysOnTop
Enabled: bool = true
FillColor: Color3 = 1, 0, 0
FillTransparency: float = 0.5
LineThickness: int = 1 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
OutlineColor: Color3 = 1, 1, 1
OutlineTransparency: float = 0
ReservedId: ReservedHighlightId = Standard [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

---

## Hopper
**Extends:** Instance
**Tags:** NotCreatable, Service, Deprecated

---

## HttpRbxApiService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
GetDocumentationUrl(partialUrl: string) → string [RobloxScriptSecurity]
GetAsync(apiUrlPath: string, priority: ThrottlingPriority, httpRequestType: HttpRequestType) → string [RobloxScriptSecurity]
GetAsyncFullUrl(apiUrl: string, priority: ThrottlingPriority, httpRequestType: HttpRequestType) → string [RobloxScriptSecurity]
PostAsync(apiUrlPath: string, data: string, priority: ThrottlingPriority, content_type: HttpContentType, httpRequestType: HttpRequestType) → string [RobloxScriptSecurity]
PostAsyncFullUrl(apiUrl: string, data: string, priority: ThrottlingPriority, content_type: HttpContentType, httpRequestType: HttpRequestType) → string [RobloxScriptSecurity]
RequestAsync(requestOptions: Dictionary, priority: ThrottlingPriority, content_type: HttpContentType, httpRequestType: HttpRequestType) → string [RobloxScriptSecurity]
RequestLimitedAsync(requestOptions: Dictionary, priority: ThrottlingPriority, content_type: HttpContentType, httpRequestType: HttpRequestType) → string
```

---

## HttpRequest
**Extends:** Instance
**Tags:** NotCreatable

### Functions
```
Cancel() → null [RobloxScriptSecurity]
Start(callback: Function) → null [RobloxScriptSecurity]
```

---

## HttpService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
HttpEnabled: bool = false [Write:LocalUserSecurity]
```

### Functions
```
GenerateGUID(wrapInCurlyBraces: bool) → string
GetHttpEnabled() → bool [RobloxScriptSecurity]
GetSecret(key: string) → Secret
GetUserAgent() → string [RobloxScriptSecurity]
JSONDecode(input: string) → Variant
JSONEncode(input: Variant) → string
RequestInternal(options: Dictionary) → Instance [RobloxScriptSecurity]
SetHttpEnabled(enabled: bool) → null [RobloxScriptSecurity]
UrlEncode(input: string) → string
GetAsync(url: Variant, nocache: bool, headers: Variant) → string
PostAsync(url: Variant, data: string, content_type: HttpContentType, compress: bool, headers: Variant) → string
RequestAsync(requestOptions: Dictionary) → Dictionary
```

---

## Humanoid
**Extends:** Instance

### Properties
```
AutoJumpEnabled: bool = true
AutoRotate: bool = true
AutomaticScalingEnabled: bool = true
BreakJointsOnDeath: bool = true
CameraMaxDistance: float = 400
CameraMinDistance: float = 0
CameraMode: CameraMode = Classic
CameraOffset: Vector3 = 0, 0, 0
CollisionType: HumanoidCollisionType = OuterBox [Write:PluginSecurity] [Deprecated]
DisplayDistanceType: HumanoidDisplayDistanceType = Viewer
DisplayName: string
EvaluateStateMachine: bool = true
FloorMaterial: Material = Air [ReadOnly]
Health: float = 100
HealthDisplayDistance: float = 100
HealthDisplayType: HumanoidHealthDisplayType = DisplayWhenDamaged
Health_XML: float = 100
HipHeight: float = 0
InternalBodyScale: Vector3 = 1, 1, 1
InternalDisplayName: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
InternalHeadScale: float = 1
InternalOriginalHipHeight: float = 0
Jump: bool = false
JumpHeight: float = 7.19999981
JumpPower: float = 50
JumpReplicate: bool = false
LeftLeg: BasePart [Deprecated]
MaxHealth: float = 100
MaxSlopeAngle: float = 89
MoveDirection: Vector3 = 0, 0, 0 [ReadOnly]
MoveDirectionInternal: Vector3 = 0, 0, 0
NameDisplayDistance: float = 100
NameOcclusion: NameOcclusion = OccludeAll
NetworkHumanoidState: HumanoidStateType = FallingDown
OverrideDefaultCollisions: bool = false [Read:RobloxSecurity] [Write:RobloxSecurity]
PlatformStand: bool = false
RequiresNeck: bool = true
RigType: HumanoidRigType = R6
RightLeg: BasePart [Deprecated]
RootPart: BasePart [ReadOnly]
RotationType: RotationType = MovementRelative [Read:RobloxSecurity] [Write:RobloxSecurity]
SeatPart: BasePart [ReadOnly]
Sit: bool = false
Strafe: bool = false
TargetPoint: Vector3 = 0, 0, 0
Torso: BasePart [Deprecated]
UseJumpPower: bool = true
WalkAngleError: float = 0
WalkDirection: Vector3 = 0, 0, 0
WalkSpeed: float = 16
WalkToPart: BasePart
WalkToPoint: Vector3 = 0, 0, 0
maxHealth: float = 100 [Deprecated]
```

### Functions
```
AddAccessory(accessory: Instance) → null
AddCustomStatus(status: string) → bool [Deprecated]
AddStatus(status: Status) → bool [Deprecated]
BuildRigFromAttachments() → null
CacheDefaults() → null [RobloxScriptSecurity]
ChangeState(state: HumanoidStateType) → null
ComputeOriginalSizeForPart(part: Instance) → Vector3? [RobloxScriptSecurity]
ComputeR15BodyBoundingBox() → void [RobloxScriptSecurity]
EquipTool(tool: Instance) → null
GetAccessories() → Array
GetAccessoryHandleScale(instance: Instance, partType: BodyPartR15) → Vector3 [RobloxScriptSecurity]
GetAppliedDescription() → HumanoidDescription
GetBodyPartR15(part: Instance) → BodyPartR15
GetLimb(part: Instance) → Limb
GetMoveVelocity() → Vector3
GetPlayingAnimationTracks() → Array [Deprecated]
GetState() → HumanoidStateType
GetStateEnabled(state: HumanoidStateType) → bool
GetStatuses() → Array [Deprecated]
HasCustomStatus(status: string) → bool [Deprecated]
HasStatus(status: Status) → bool [Deprecated]
LoadAnimation(animation: Animation) → AnimationTrack [Deprecated]
Move(moveDirection: Vector3, relativeToCamera: bool) → null
MoveTo(location: Vector3, part: Instance) → null
RemoveAccessories() → null
RemoveCustomStatus(status: string) → bool [Deprecated]
RemoveStatus(status: Status) → bool [Deprecated]
ReplaceBodyPartR15(bodyPart: BodyPartR15, part: BasePart) → bool
SetClickToWalkEnabled(enabled: bool) → null [RobloxScriptSecurity]
SetStateEnabled(state: HumanoidStateType, enabled: bool) → null
TakeDamage(amount: float) → null
UnequipTools() → null
loadAnimation(animation: Animation) → AnimationTrack [Deprecated]
takeDamage(amount: float) → null [Deprecated]
ApplyAvatarRules(avatarRules: AvatarRules) → null [RobloxScriptSecurity]
ApplyDescription(humanoidDescription: HumanoidDescription, assetTypeVerification: AssetTypeVerification) → null
ApplyDescriptionClientServer(humanoidDescription: HumanoidDescription) → null [RobloxScriptSecurity]
ApplyDescriptionReset(humanoidDescription: HumanoidDescription, assetTypeVerification: AssetTypeVerification) → null
PlayEmote(emoteName: string) → bool
PlayEmoteAndGetAnimTrackById(emoteId: int64) → Tuple [RobloxScriptSecurity]
```

### Events
```
AnimationPlayed(animationTrack: AnimationTrack)
ApplyDescriptionFinished(description: HumanoidDescription)
Climbing(speed: float)
ClusterCompositionFinished() [RobloxScriptSecurity]
CustomStatusAdded(status: string)
CustomStatusRemoved(status: string)
Died()
EmoteTriggered(success: bool, animationTrack: AnimationTrack) [RobloxScriptSecurity]
FallingDown(active: bool)
FreeFalling(active: bool)
GettingUp(active: bool)
HealthChanged(health: float)
Jumping(active: bool)
MoveToFinished(reached: bool)
PlatformStanding(active: bool)
Ragdoll(active: bool)
Running(speed: float)
Seated(active: bool, currentSeatPart: BasePart)
ServerApplyDescription(status: bool) [RobloxSecurity]
ServerBreakJoints() [RobloxSecurity]
ServerEquipTool(tool: Tool) [RobloxSecurity]
StateChanged(old: HumanoidStateType, new: HumanoidStateType)
StateEnabledChanged(state: HumanoidStateType, isEnabled: bool)
StatusAdded(status: Status)
StatusRemoved(status: Status)
Strafing(active: bool)
Swimming(speed: float)
Touched(touchingPart: BasePart, humanoidPart: BasePart)
```

---

## HumanoidDescription
**Extends:** Instance

### Properties
```
AccessoryBlob: string = []
BackAccessory: string
BodyTypeScale: float = 0.300000012
ClimbAnimation: int64 = 0
DepthScale: float = 1
EmotesDataInternal: string
EquippedEmotesDataInternal: string
Face: int64 = 0
FaceAccessory: string
FallAnimation: int64 = 0
FrontAccessory: string
GraphicTShirt: int64 = 0
HairAccessory: string
HatAccessory: string
Head: int64 = 0
HeadColor: Color3 = 0, 0, 0
HeadScale: float = 1
HeightScale: float = 1
IdleAnimation: int64 = 0
JumpAnimation: int64 = 0
LeftArm: int64 = 0
LeftArmColor: Color3 = 0, 0, 0
LeftLeg: int64 = 0
LeftLegColor: Color3 = 0, 0, 0
MoodAnimation: int64 = 0
NeckAccessory: string
NumberEmotesLoaded: int = -1 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Pants: int64 = 0
ProportionScale: float = 1
ResetIncludesBodyParts: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
RightArm: int64 = 0
RightArmColor: Color3 = 0, 0, 0
RightLeg: int64 = 0
RightLegColor: Color3 = 0, 0, 0
RunAnimation: int64 = 0
Shirt: int64 = 0
ShouldersAccessory: string
SwimAnimation: int64 = 0
Torso: int64 = 0
TorsoColor: Color3 = 0, 0, 0
WaistAccessory: string
WalkAnimation: int64 = 0
WidthScale: float = 1
```

### Functions
```
AddEmote(name: string, assetId: int64) → null
GetAccessories(includeRigidAccessories: bool) → Array
GetEmotes() → Dictionary
GetEquippedEmotes() → Array
RemoveEmote(name: string) → null
SetAccessories(accessories: Array, includeRigidAccessories: bool) → null
SetEmotes(emotes: Dictionary) → null
SetEquippedEmotes(equippedEmotes: Array) → null
```

### Events
```
EmotesChanged(newEmotes: Dictionary)
EquippedEmotesChanged(newEquippedEmotes: Array)
```

---

## HumanoidRigDescription
**Extends:** Instance
**Tags:** NotBrowsable

### Properties
```
Chest: Instance
ChestRangeMax: Vector3 = 0, 0, 0
ChestRangeMin: Vector3 = 0, 0, 0
ChestSize: float = 0
ChestTposeAdjustment: CFrame
HeadBase: Instance
HeadBaseRangeMax: Vector3 = 0, 0, 0
HeadBaseRangeMin: Vector3 = 0, 0, 0
HeadBaseSize: float = 0
HeadBaseTposeAdjustment: CFrame
LeftAnkle: Instance
LeftAnkleRangeMax: Vector3 = 0, 0, 0
LeftAnkleRangeMin: Vector3 = 0, 0, 0
LeftAnkleSize: float = 0
LeftAnkleTposeAdjustment: CFrame
LeftClavicle: Instance
LeftClavicleRangeMax: Vector3 = 0, 0, 0
LeftClavicleRangeMin: Vector3 = 0, 0, 0
LeftClavicleSize: float = 0
LeftClavicleTposeAdjustment: CFrame
LeftElbow: Instance
LeftElbowRangeMax: Vector3 = 0, 0, 0
LeftElbowRangeMin: Vector3 = 0, 0, 0
LeftElbowSize: float = 0
LeftElbowTposeAdjustment: CFrame
LeftHip: Instance
LeftHipRangeMax: Vector3 = 0, 0, 0
LeftHipRangeMin: Vector3 = 0, 0, 0
LeftHipSize: float = 0
LeftHipTposeAdjustment: CFrame
LeftKnee: Instance
LeftKneeRangeMax: Vector3 = 0, 0, 0
LeftKneeRangeMin: Vector3 = 0, 0, 0
LeftKneeSize: float = 0
LeftKneeTposeAdjustment: CFrame
LeftShoulder: Instance
LeftShoulderRangeMax: Vector3 = 0, 0, 0
LeftShoulderRangeMin: Vector3 = 0, 0, 0
LeftShoulderSize: float = 0
LeftShoulderTposeAdjustment: CFrame
LeftToes: Instance
LeftToesRangeMax: Vector3 = 0, 0, 0
LeftToesRangeMin: Vector3 = 0, 0, 0
LeftToesSize: float = 0
LeftToesTposeAdjustment: CFrame
LeftWrist: Instance
LeftWristRangeMax: Vector3 = 0, 0, 0
LeftWristRangeMin: Vector3 = 0, 0, 0
LeftWristSize: float = 0
LeftWristTposeAdjustment: CFrame
Neck: Instance
NeckRangeMax: Vector3 = 0, 0, 0
NeckRangeMin: Vector3 = 0, 0, 0
NeckSize: float = 0
NeckTposeAdjustment: CFrame
Pelvis: Instance
PelvisRangeMax: Vector3 = 0, 0, 0
PelvisRangeMin: Vector3 = 0, 0, 0
PelvisSize: float = 0
PelvisTposeAdjustment: CFrame
RightAnkle: Instance
RightAnkleRangeMax: Vector3 = 0, 0, 0
RightAnkleRangeMin: Vector3 = 0, 0, 0
RightAnkleSize: float = 0
RightAnkleTposeAdjustment: CFrame
RightClavicle: Instance
RightClavicleRangeMax: Vector3 = 0, 0, 0
RightClavicleRangeMin: Vector3 = 0, 0, 0
RightClavicleSize: float = 0
RightClavicleTposeAdjustment: CFrame
RightElbow: Instance
RightElbowRangeMax: Vector3 = 0, 0, 0
RightElbowRangeMin: Vector3 = 0, 0, 0
RightElbowSize: float = 0
RightElbowTposeAdjustment: CFrame
RightHip: Instance
RightHipRangeMax: Vector3 = 0, 0, 0
RightHipRangeMin: Vector3 = 0, 0, 0
RightHipSize: float = 0
RightHipTposeAdjustment: CFrame
RightKnee: Instance
RightKneeRangeMax: Vector3 = 0, 0, 0
RightKneeRangeMin: Vector3 = 0, 0, 0
RightKneeSize: float = 0
RightKneeTposeAdjustment: CFrame
RightShoulder: Instance
RightShoulderRangeMax: Vector3 = 0, 0, 0
RightShoulderRangeMin: Vector3 = 0, 0, 0
RightShoulderSize: float = 0
RightShoulderTposeAdjustment: CFrame
RightToes: Instance
RightToesRangeMax: Vector3 = 0, 0, 0
RightToesRangeMin: Vector3 = 0, 0, 0
RightToesSize: float = 0
RightToesTposeAdjustment: CFrame
RightWrist: Instance
RightWristRangeMax: Vector3 = 0, 0, 0
RightWristRangeMin: Vector3 = 0, 0, 0
RightWristSize: float = 0
RightWristTposeAdjustment: CFrame
Root: Instance
RootRangeMax: Vector3 = 0, 0, 0
RootRangeMin: Vector3 = 0, 0, 0
RootSize: float = 0
RootTposeAdjustment: CFrame
Waist: Instance
WaistRangeMax: Vector3 = 0, 0, 0
WaistRangeMin: Vector3 = 0, 0, 0
WaistSize: float = 0
WaistTposeAdjustment: CFrame
```

### Functions
```
Automap(character: Instance) → null
GetJointFromName(name: string) → Instance
GetJointNames() → Array
GetR15JointNames() → Array
GetR6JointNames() → Array
```

---

## IKControl
**Extends:** Instance

### Properties
```
ChainRoot: Instance
Enabled: bool = true
EndEffector: Instance
EndEffectorOffset: CFrame
Offset: CFrame
Pole: Instance
Priority: int = 0
SmoothTime: float = 0.0500000007
Target: Instance
Type: IKControlType = Transform
Weight: float = 1
```

### Functions
```
GetChainCount() → int
GetChainLength() → float
GetNodeLocalCFrame(index: int) → CFrame
GetNodeWorldCFrame(index: int) → CFrame
GetRawFinalTarget() → CFrame
GetSmoothedFinalTarget() → CFrame
Solve() → null [RobloxScriptSecurity]
```

---

## ILegacyStudioBridge
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## LegacyStudioBridge
**Extends:** ILegacyStudioBridge
**Tags:** NotCreatable, Service, NotReplicated

---

## IXPService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
ClearUserLayers() → null [LocalUserSecurity]
GetBrowserTrackerLayerLoadingStatus() → IXPLoadingStatus [LocalUserSecurity]
GetBrowserTrackerLayerVariables(layerName: string) → Dictionary [LocalUserSecurity]
GetBrowserTrackerStatusForLayer(layerName: string) → IXPLoadingStatus? [LocalUserSecurity]
GetRegisteredUserLayersToStatus() → Dictionary [LocalUserSecurity]
GetUserLayerLoadingStatus() → IXPLoadingStatus [LocalUserSecurity]
GetUserLayerVariables(layerName: string) → Dictionary [LocalUserSecurity]
GetUserStatusForLayer(layerName: string) → IXPLoadingStatus? [LocalUserSecurity]
InitializeUserLayers(userId: int64) → null [LocalUserSecurity]
LogBrowserTrackerLayerExposure(layerName: string) → null [LocalUserSecurity]
LogFlagLinkedUserLayerExposure(layerName: string) → null [LocalUserSecurity]
LogUserLayerExposure(layerName: string) → null [LocalUserSecurity]
RegisterUserLayers(userLayers: Variant) → null [LocalUserSecurity]
```

### Events
```
OnBrowserTrackerLayerLoadingStatusChanged(status: IXPLoadingStatus) [LocalUserSecurity]
OnUserLayerLoadingStatusChanged(status: IXPLoadingStatus) [LocalUserSecurity]
```

---

## ImportSession
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
Cancel() → null [RobloxScriptSecurity]
GetFilename() → string [RobloxScriptSecurity]
GetStatuses() → Dictionary [RobloxScriptSecurity]
Upload() → null [RobloxScriptSecurity]
```

### Events
```
UploadComplete(results: Dictionary)
UploadProgress(progressRatio: float)
```

---

## AssetImportSession
**Extends:** ImportSession
**Tags:** NotCreatable, NotReplicated

### Functions
```
ApplyPreset(preset: Dictionary) → null [RobloxScriptSecurity]
CreatePresetFromData(importData: Instance) → Dictionary [RobloxScriptSecurity]
GetImportTree() → Instance [RobloxScriptSecurity]
GetRigVisualization(importDataInstance: Instance) → Instance [RobloxScriptSecurity]
GetUploadStatus() → Dictionary [RobloxScriptSecurity]
HasAnimation() → bool [RobloxScriptSecurity]
IsAvatar() → bool [RobloxScriptSecurity]
IsGltf() → bool [RobloxScriptSecurity]
IsR15() → bool [RobloxScriptSecurity]
Reset() → null [RobloxScriptSecurity]
usesCustomRestPoseLua() → bool [RobloxScriptSecurity]
```

---

## IncrementalPatchBuilder
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
AddPathsToBundle: bool = false
BuildDebouncePeriod: double = 0.10000000000000000555
HighCompression: bool = false
SerializePatch: bool = true
ZstdCompression: bool = false
```

---

## InputAction
**Extends:** Instance

### Properties
```
BoolState: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Direction1DState: float = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Direction2DState: Vector2 = 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Direction3DState: Vector3 = 0, 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Enabled: bool = true
Type: InputActionType = Bool
```

### Functions
```
Fire(state: Variant) → null
GetState() → Variant
```

### Events
```
Pressed()
Released()
StateChanged(value: Variant)
```

---

## InputBinding
**Extends:** Instance

### Properties
```
Backward: KeyCode = Unknown
Down: KeyCode = Unknown
Forward: KeyCode = Unknown
KeyCode: KeyCode = Unknown
Left: KeyCode = Unknown
PressedThreshold: float = 0.5
ReleasedThreshold: float = 0.200000003
Right: KeyCode = Unknown
Scale: float = 1
UIButton: GuiButton
Up: KeyCode = Unknown
Vector2Scale: Vector2 = 1, 1
```

---

## InputContext
**Extends:** Instance

### Properties
```
Enabled: bool = true
Priority: int = 1000
Sink: bool = false
```

---

## InputObject
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
Delta: Vector3 = 0, 0, 0
KeyCode: KeyCode = Unknown
Position: Vector3 = 0, 0, 0
UserInputState: UserInputState = None
UserInputType: UserInputType = None
```

### Functions
```
IsModifierKeyDown(modifierKey: ModifierKey) → bool
```

---

## InsertService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
AllowClientInsertModels: bool = false
AllowInsertFreeModels: bool = false [Deprecated]
```

### Functions
```
ApproveAssetId(assetId: int64) → null [Deprecated]
ApproveAssetVersionId(assetVersionId: int64) → null [Deprecated]
GetLocalFileContents(contentId: string) → string [RobloxScriptSecurity]
Insert(instance: Instance) → null [Deprecated]
LoadLocalAsset(assetPath: string) → Instance [RobloxScriptSecurity]
LoadPackageAsset(url: ContentId) → Instances [RobloxScriptSecurity]
CreateMeshPartAsync(meshId: ContentId, collisionFidelity: CollisionFidelity, renderFidelity: RenderFidelity) → MeshPart
GetBaseCategories() → Array [Deprecated]
GetBaseSets() → Array [Deprecated]
GetCollection(categoryId: int64) → Array [Deprecated]
GetFreeDecals(searchText: string, pageNum: int) → Array
GetFreeModels(searchText: string, pageNum: int) → Array
GetLatestAssetVersionAsync(assetId: int64) → int64
GetUserCategories(userId: int64) → Array [Deprecated]
GetUserSets(userId: int64) → Array [Deprecated]
LoadAsset(assetId: int64) → Instance
LoadAssetVersion(assetVersionId: int64) → Instance
LoadAssetWithFormat(assetId: int64, format: string) → Instances [RobloxScriptSecurity]
LoadPackageAssetAsync(url: ContentId) → Instances [RobloxScriptSecurity]
loadAsset(assetId: int64) → Instance [Deprecated]
```

### Events
```
InternalDelete(instance: Instance)
```

---

## InternalSyncItem
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
AutoSync: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Enabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Path: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Target: Instance [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

---

## InternalSyncService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## JointInstance
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
Active: bool [ReadOnly]
C0: CFrame
C1: CFrame
Enabled: bool
Part0: BasePart
Part1: BasePart
part1: BasePart [Deprecated]
```

---

## DynamicRotate
**Extends:** JointInstance
**Tags:** NotCreatable

### Properties
```
BaseAngle: float
```

---

## RotateP
**Extends:** DynamicRotate
**Tags:** Deprecated

---

## RotateV
**Extends:** DynamicRotate
**Tags:** Deprecated

---

## Glue
**Extends:** JointInstance
**Tags:** Deprecated

### Properties
```
F0: Vector3 = 0, 0, 0
F1: Vector3 = 0, 0, 0
F2: Vector3 = 0, 0, 0
F3: Vector3 = 0, 0, 0
```

---

## ManualSurfaceJointInstance
**Extends:** JointInstance
**Tags:** NotCreatable, Deprecated

---

## ManualGlue
**Extends:** ManualSurfaceJointInstance
**Tags:** Deprecated

---

## ManualWeld
**Extends:** ManualSurfaceJointInstance
**Tags:** Deprecated

---

## Motor
**Extends:** JointInstance

### Properties
```
CurrentAngle: float = 0
DesiredAngle: float = 0
MaxVelocity: float = 0
ReplicateCurrentAngle: float = 0 [Read:RobloxSecurity] [Write:RobloxSecurity]
```

### Functions
```
SetDesiredAngle(value: float) → null
```

---

## Motor6D
**Extends:** Motor

### Properties
```
ChildName: string [ReadOnly]
ParentName: string [ReadOnly]
ReplicateCurrentAngle6D: Vector3 = 0, 0, 0 [Read:RobloxSecurity] [Write:RobloxSecurity]
ReplicateCurrentOffset6D: Vector3 = 0, 0, 0 [Read:RobloxSecurity] [Write:RobloxSecurity]
Transform: CFrame
```

---

## Rotate
**Extends:** JointInstance
**Tags:** Deprecated

---

## Snap
**Extends:** JointInstance
**Tags:** Deprecated

---

## VelocityMotor
**Extends:** JointInstance

### Properties
```
CurrentAngle: float = 0
DesiredAngle: float = 0
Hole: Hole
MaxVelocity: float = 0
```

---

## Weld
**Extends:** JointInstance

---

## JointsService
**Extends:** Instance
**Tags:** NotCreatable, Service, Deprecated

### Functions
```
ClearJoinAfterMoveJoints() → null
CreateJoinAfterMoveJoints() → null
SetJoinAfterMoveInstance(joinInstance: Instance) → null
SetJoinAfterMoveTarget(joinTarget: Instance) → null
ShowPermissibleJoints() → null
```

---

## KeyboardService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## Keyframe
**Extends:** Instance

### Properties
```
Time: float = 0
```

### Functions
```
AddMarker(marker: Instance) → null
AddPose(pose: Instance) → null
GetMarkers() → Instances
GetPoses() → Instances
RemoveMarker(marker: Instance) → null
RemovePose(pose: Instance) → null
```

---

## KeyframeMarker
**Extends:** Instance

### Properties
```
Value: string
```

---

## KeyframeSequenceProvider
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetKeyframeSequence(assetId: ContentId) → Instance [PluginSecurity] [Deprecated]
GetKeyframeSequenceById(assetId: int64, useCache: bool) → Instance [PluginSecurity] [Deprecated]
GetMemStats() → Dictionary [RobloxScriptSecurity]
RegisterActiveKeyframeSequence(keyframeSequence: Instance) → ContentId
RegisterKeyframeSequence(keyframeSequence: Instance) → ContentId
GetAnimations(userId: int64) → Instance
GetKeyframeSequenceAsync(assetId: ContentId) → Instance
```

---

## LSPFileSyncService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## LanguageService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetCapabilitiesUsedInPackageAsync(instances: Instances) → Dictionary
```

---

## Light
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
Brightness: float
Color: Color3
Enabled: bool
Shadows: bool
```

---

## PointLight
**Extends:** Light

### Properties
```
Range: float
```

---

## SpotLight
**Extends:** Light

### Properties
```
Angle: float
Face: NormalId
Range: float
```

---

## SurfaceLight
**Extends:** Light

### Properties
```
Angle: float
Face: NormalId
Range: float
```

---

## Lighting
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
Ambient: Color3 = 0.5, 0.5, 0.5
Brightness: float = 1
ClockTime: float = 14
ColorShift_Bottom: Color3 = 0, 0, 0
ColorShift_Top: Color3 = 0, 0, 0
EnvironmentDiffuseScale: float = 0
EnvironmentSpecularScale: float = 0
ExposureCompensation: float = 0
ExtendLightRangeTo120: RolloutState = Default
FogColor: Color3 = 0.75, 0.75, 0.75
FogEnd: float = 100000
FogStart: float = 0
GeographicLatitude: float = 41.7332993
GlobalShadows: bool = false
LightingStyle: LightingStyle = Realistic
OutdoorAmbient: Color3 = 0.5, 0.5, 0.5
Outlines: bool = true [Deprecated]
PrioritizeLightingQuality: bool = true
ShadowColor: Color3 = 0.7, 0.7, 0.72 [Deprecated]
ShadowSoftness: float = 0.5
Technology: Technology = Compatibility [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
TimeOfDay: string = 14:00:00
```

### Functions
```
GetMinutesAfterMidnight() → double
GetMoonDirection() → Vector3
GetMoonPhase() → float
GetSunDirection() → Vector3
SetMinutesAfterMidnight(minutes: double) → null
getMinutesAfterMidnight() → double [Deprecated]
setMinutesAfterMidnight(minutes: double) → null [Deprecated]
```

### Events
```
LightingChanged(skyChanged: bool)
```

---

## LinkingService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
DetectUrl(url: string) → null [RobloxScriptSecurity]
GetAndClearLastPendingUrl() → Dictionary [RobloxScriptSecurity]
GetLastLuaUrl() → string? [RobloxScriptSecurity]
IsUrlRegistered(url: string) → bool [RobloxScriptSecurity]
RegisterLuaUrl(url: string) → null [RobloxScriptSecurity]
StartLuaUrlDelivery() → Dictionary? [RobloxScriptSecurity]
StopLuaUrlDelivery() → null [RobloxScriptSecurity]
OpenUrl(url: string) → bool [RobloxScriptSecurity]
SupportsSwitchToSettingsApp() → bool [RobloxScriptSecurity]
SwitchToSettingsApp(route: string?) → null [RobloxScriptSecurity]
```

### Events
```
OnLuaUrl(url: string, matchedUrl: string, attributionUrl: string?) [RobloxScriptSecurity]
```

---

## LiveScriptingService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
ServerLiveEditingMode: ServerLiveEditingMode = Uninitialized
```

### Events
```
BeginEdit(id: int64, guid: string) [RobloxSecurity]
BroadcastMessage(message: string, type: LiveEditingBroadcastMessageType) [RobloxSecurity]
EndEdit(id: int64) [RobloxSecurity]
FailedToOpen(id: int64, legalToOpenLocal: bool) [RobloxSecurity]
KickFromEdit(id: int64, msg: string) [RobloxSecurity]
LiveEditingClientConfiguration(serializedConfig: string) [RobloxSecurity]
OpenedWithSource(id: int64, source: string) [RobloxSecurity]
SendAtomicOperation(requestId: int, guid: string, op: string, hash: string) [RobloxSecurity]
SendAtomicUpdateResponse(guid: int, response: LiveEditingAtomicUpdateResponse) [RobloxSecurity]
SendOperation(id: int64, op: string) [RobloxSecurity]
```

---

## LiveSyncService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
HasSyncedInstances: bool = false [ReadOnly]
```

### Functions
```
GetSyncState(instance: Instance) → Tuple
```

### Events
```
SyncStatusChanged(instance: Instance)
```

---

## LocalStorageService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
Flush() → null [RobloxScriptSecurity]
GetItem(key: string) → string [RobloxScriptSecurity]
SetItem(key: string, value: string) → null [RobloxScriptSecurity]
WhenLoaded(callback: Function) → null [RobloxScriptSecurity]
```

### Events
```
ItemWasSet(key: string, value: string) [RobloxScriptSecurity]
StoreWasCleared() [RobloxScriptSecurity]
```

---

## AppStorageService
**Extends:** LocalStorageService
**Tags:** NotCreatable, Service, NotReplicated

---

## UserStorageService
**Extends:** LocalStorageService
**Tags:** NotCreatable, Service, NotReplicated

---

## LocalizationService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
ForcePlayModeGameLocaleId: string [Read:LocalUserSecurity] [Write:LocalUserSecurity]
ForcePlayModeRobloxLocaleId: string [Read:LocalUserSecurity] [Write:LocalUserSecurity]
GameSourceLanguageId: string
IsTextScraperRunning: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LocaleManifest: string
RobloxForcePlayModeGameLocaleId: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
RobloxForcePlayModeRobloxLocaleId: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
RobloxLocaleId: string [ReadOnly]
ShouldUseCloudTable: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
SystemLocaleId: string [ReadOnly]
```

### Functions
```
GetCorescriptLocalizations() → Instances
GetTableEntries(instance: Instance) → Array
GetTranslatorForPlayer(player: Instance) → Instance
SetRobloxLocaleId(locale: string) → null [RobloxScriptSecurity]
StartTextScraper() → null [RobloxScriptSecurity]
StopTextScraper() → null [RobloxScriptSecurity]
GetCountryRegionForPlayerAsync(player: Instance) → string
GetTranslatorForLocaleAsync(locale: string) → Instance
GetTranslatorForPlayerAsync(player: Instance) → Instance
PromptDownloadGameTableToCSV(table: Instance) → null [RobloxScriptSecurity]
PromptExportToCSVs() → null [RobloxScriptSecurity]
PromptImportFromCSVs() → null [RobloxScriptSecurity]
PromptUploadCSVToGameTable() → Instance [RobloxScriptSecurity]
```

### Events
```
AutoTranslateWillRun() [RobloxScriptSecurity]
DynamicTranslationServerToClientResponse(entries: Tuple) [RobloxSecurity]
TextScraperClientMessageWithPlayerSignal(version: int, player: Instance, message: Tuple) [RobloxSecurity]
```

---

## LocalizationTable
**Extends:** Instance

### Properties
```
Contents: string = []
DevelopmentLanguage: string = en-us [Deprecated]
IsExemptFromUGCAnalytics: bool = false
Root: Instance [Deprecated]
SourceLocaleId: string = en-us
```

### Functions
```
GetContents() → string [Deprecated]
GetEntries() → Array
GetString(targetLocaleId: string, key: string) → string [Deprecated]
GetTranslator(localeId: string) → Instance
RemoveEntry(key: string, source: string, context: string) → null
RemoveEntryValue(key: string, source: string, context: string, localeId: string) → null
RemoveKey(key: string) → null [Deprecated]
RemoveTargetLocale(localeId: string) → null
SetContents(contents: string) → null [Deprecated]
SetEntries(entries: Variant) → null
SetEntry(key: string, targetLocaleId: string, text: string) → null [Deprecated]
SetEntryContext(key: string, source: string, context: string, newContext: string) → null
SetEntryExample(key: string, source: string, context: string, example: string) → null
SetEntryKey(key: string, source: string, context: string, newKey: string) → null
SetEntrySource(key: string, source: string, context: string, newSource: string) → null
SetEntryValue(key: string, source: string, context: string, localeId: string, text: string) → null
SetIsExemptFromUGCAnalytics(value: bool) → null [RobloxScriptSecurity]
```

---

## CloudLocalizationTable
**Extends:** LocalizationTable
**Tags:** NotCreatable, NotReplicated

---

## LodDataEntity
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
EntityData: SharedString
EntityLodEnabled: bool = true
EntityPosition: CFrame
EntityScale: Vector3 = 0, 0, 0
EntitySource: Instance
```

---

## LodDataService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## LogReporterService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
ReportLog(fingerprint: string, uuid: string, desc: string, attributes: Dictionary, annotations: Dictionary) → bool [RobloxScriptSecurity]
ReportMultipleLogs(fingerprint: string, uuid: string, desc: string, attributes: Dictionary, annotations: Dictionary, numLogs: int) → bool [RobloxScriptSecurity]
```

---

## LogService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
ClearOutput() → null
ExecuteScript(source: string) → null [RobloxScriptSecurity]
GetHttpResultHistory() → Array [RobloxScriptSecurity]
GetLogHistory() → Array
RequestHttpResultApproved() → null [RobloxScriptSecurity]
RequestServerHttpResult() → null [RobloxScriptSecurity]
RequestServerOutput() → null [RobloxScriptSecurity]
```

### Events
```
HttpResultOut(httpResult: Dictionary) [RobloxScriptSecurity]
MessageOut(message: string, messageType: MessageType)
OnHttpResultApproved(isApproved: bool) [RobloxScriptSecurity]
RequestHttpResultApprovedSignal(requestingPlayer: Instance) [RobloxSecurity]
RequestScriptExecutionSignal(requestingPlayer: Instance, source: string) [RobloxSecurity]
RequestServerHttpResultSignal(requestingPlayer: Instance) [RobloxSecurity]
RequestServerOutputSignal(requestingPlayer: Instance) [RobloxSecurity]
RequestSettingsChange(requestingPlayer: Instance, expressivePrinting: bool) [RobloxSecurity]
ServerHttpResultOut(httpResult: Dictionary) [RobloxScriptSecurity]
ServerMessageOut(message: string, messageType: MessageType, timestamp: double) [RobloxScriptSecurity]
ServerVariantMessageOut(data: Dictionary) [RobloxSecurity]
```

---

## LoginService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
Logout() → null [RobloxSecurity]
PromptLogin() → null [RobloxSecurity]
```

### Events
```
LoginFailed(loginError: string) [RobloxSecurity]
LoginSucceeded(username: string) [RobloxSecurity]
```

---

## LuaSettings
**Extends:** Instance
**Tags:** NotCreatable, Settings, NotReplicated

---

## LuaSourceContainer
**Extends:** Instance
**Tags:** NotCreatable, NotBrowsable

### Properties
```
CachedRemoteSource: ProtectedString
CachedRemoteSourceLoadState: int
HasAssociatedDrafts: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
IsDifferentFromFileSystem: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
SandboxedSource: ProtectedString [Read:RobloxSecurity] [Write:RobloxSecurity]
ScriptGuid: string
isPlayerScript: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## AuroraScript
**Extends:** LuaSourceContainer
**Tags:** Deprecated

### Properties
```
AuroraScriptBindingsSerialize: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
EnableCulling: bool [Read:PluginSecurity] [Write:PluginSecurity]
EnableLOD: bool [Read:PluginSecurity] [Write:PluginSecurity]
LODCriticality: int [Read:PluginSecurity] [Write:PluginSecurity]
Priority: int [Read:PluginSecurity] [Write:PluginSecurity]
Source: ProtectedString [Read:PluginSecurity] [Write:PluginSecurity]
```

### Functions
```
AddTo(instance: Instance) → null
IsOnInstance(instance: Instance) → bool
RemoveFrom(instance: Instance) → null
SignalFired(instance: Instance, topic: string) → RBXScriptSignal
```

### Events
```
SynchronizeState(frameId: int, instance: Instance, state: Dictionary, ingressHeaders: string, ingressArgs: Array, egressHeaders: string, egressArgs: Array, lodLevel: int, priorInvocationFrame: int) [RobloxSecurity]
```

---

## BaseScript
**Extends:** LuaSourceContainer
**Tags:** NotCreatable

### Properties
```
Disabled: bool
Enabled: bool
LinkedSource: ContentId [Deprecated]
RunContext: RunContext [Write:PluginSecurity]
```

---

## CoreScript
**Extends:** BaseScript
**Tags:** NotCreatable, NotReplicated

---

## Script
**Extends:** BaseScript

### Properties
```
Source: ProtectedString
```

### Functions
```
GetHash() → string [LocalUserSecurity]
```

---

## LocalScript
**Extends:** Script

---

## ModuleScript
**Extends:** LuaSourceContainer

### Properties
```
Confidential: bool = false [Read:RobloxSecurity] [Write:RobloxSecurity]
LinkedSource: ContentId [Deprecated]
Source: ProtectedString
```

---

## LuaWebService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## LuauScriptAnalyzerService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## MLModelDeliveryService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## MLService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
CreateSessionAsync(assetId: string) → MLSession
```

---

## MarkerCurve
**Extends:** Instance

### Properties
```
Length: int = 0 [ReadOnly]
ValuesAndTimes: BinaryString = 
```

### Functions
```
GetMarkerAtIndex(index: int) → Dictionary
GetMarkers() → Array
InsertMarkerAtTime(time: float, marker: string) → Array
RemoveMarkerAtIndex(startingIndex: int, count: int) → int
```

---

## MarketplaceService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
PlayerCanMakePurchases(player: Instance) → bool [RobloxScriptSecurity]
PrepareCollectiblesPurchase(player: Instance, assetId: int64, collectibleItemId: string, collectibleItemInstanceId: string, collectibleProductId: string, expectedPrice: int) → null [RobloxScriptSecurity]
PromptBulkPurchase(player: Player, lineItems: Array, options: Dictionary) → null
PromptBundlePurchase(player: Instance, bundleId: int64) → null
PromptCancelSubscription(user: Player, subscriptionId: string) → null
PromptCollectiblesPurchase(player: Instance, assetId: int64, collectibleItemId: string, collectibleItemInstanceId: string, collectibleProductId: string, expectedPrice: int) → null [RobloxScriptSecurity]
PromptGamePassPurchase(player: Instance, gamePassId: int64) → null
PromptNativePurchase(player: Instance, productId: string) → null [RobloxScriptSecurity]
PromptNativePurchaseWithLocalPlayer(productId: string) → null [RobloxScriptSecurity]
PromptPremiumPurchase(player: Instance) → null
PromptProductPurchase(player: Instance, productId: int64, equipIfPurchased: bool, currencyType: CurrencyType) → null
PromptPurchase(player: Instance, assetId: int64, equipIfPurchased: bool, currencyType: CurrencyType) → null
PromptRobloxPurchase(assetId: int64, equipIfPurchased: bool) → null [RobloxScriptSecurity]
PromptSubscriptionPurchase(user: Player, subscriptionId: string) → null
PromptThirdPartyPurchase(player: Instance, productId: string) → null [LocalUserSecurity]
ReportAssetSale(assetId: string, robuxAmount: int) → null [RobloxScriptSecurity]
ReportRobuxUpsellStarted() → null [RobloxScriptSecurity]
SignalAssetTypePurchased(player: Instance, assetType: AssetType) → null [RobloxScriptSecurity]
SignalClientPurchaseSuccess(ticket: string, playerId: int64, productId: int64) → null [RobloxScriptSecurity]
SignalMockPurchasePremium() → null [RobloxScriptSecurity]
SignalPromptBulkPurchaseFinished(status: MarketplaceBulkPurchasePromptStatus, results: Dictionary) → null [RobloxScriptSecurity]
SignalPromptBundlePurchaseFinished(player: Instance, bundleId: int64, success: bool) → null [RobloxScriptSecurity]
SignalPromptGamePassPurchaseFinished(player: Instance, gamePassId: int64, success: bool) → null [RobloxScriptSecurity]
SignalPromptPremiumPurchaseFinished(didTryPurchasing: bool) → null [RobloxScriptSecurity]
SignalPromptProductPurchaseFinished(userId: int64, productId: int64, success: bool) → null [RobloxScriptSecurity]
SignalPromptPurchaseFinished(player: Instance, assetId: int64, success: bool) → null [RobloxScriptSecurity]
SignalPromptSubscriptionPurchaseFinished(subscriptionId: string, didTryPurchasing: bool) → null [RobloxScriptSecurity]
SignalServerLuaDialogClosed(value: bool) → null [RobloxScriptSecurity]
SignalUserSubscriptionStatusChanged(subscriptionId: string) → null [RobloxScriptSecurity]
GetDeveloperProductsAsync() → Instance
GetDeveloperProductsForExperienceDetailsPageAsync() → Instance [RobloxScriptSecurity]
GetProductInfo(assetId: int64, infoType: InfoType) → Dictionary
GetRobuxBalance() → int [RobloxScriptSecurity]
GetSubscriptionProductInfoAsync(subscriptionId: string) → Dictionary
GetSubscriptionPurchaseInfoAsync(subscriptionId: string) → Dictionary [RobloxScriptSecurity]
GetUserSubscriptionDetailsAsync(user: Player, subscriptionId: string) → Dictionary
GetUserSubscriptionDetailsInternalAsync(subscriptionId: string) → Dictionary [RobloxScriptSecurity]
GetUserSubscriptionPaymentHistoryAsync(user: Player, subscriptionId: string) → Array
GetUserSubscriptionStatusAsync(user: Player, subscriptionId: string) → Dictionary
GetUsersPriceLevelsAsync(userIds: Array) → Array
PerformBulkPurchase(orderRequest: Dictionary, options: Dictionary) → Dictionary [RobloxScriptSecurity]
PerformCancelSubscription(subscriptionId: string) → null [RobloxScriptSecurity]
PerformPurchase(infoType: InfoType, productId: int64, expectedPrice: int, requestId: string, isRobloxPurchase: bool, collectibleItemId: string, collectibleProductId: string, idempotencyKey: string, purchaseAuthToken: string) → Dictionary [RobloxScriptSecurity]
PerformPurchaseV2(infoType: InfoType, productId: int64, expectedPrice: int, requestId: string, isRobloxPurchase: bool, collectiblesProductDetails: Dictionary) → Dictionary [RobloxScriptSecurity]
PerformSubscriptionPurchase(subscriptionId: string) → string [RobloxScriptSecurity]
PerformSubscriptionPurchaseV2(subscriptionId: string, paymentProvider: string) → null [RobloxScriptSecurity]
PlayerOwnsAsset(player: Instance, assetId: int64) → bool
PlayerOwnsBundle(player: Player, bundleId: int64) → bool
UserOwnsGamePassAsync(userId: int64, gamePassId: int64) → bool
```

### Events
```
AssetTypePurchased(player: Instance, assetType: AssetType) [RobloxScriptSecurity]
ClientLuaDialogRequested(arguments: Tuple) [RobloxScriptSecurity]
ClientPurchaseSuccess(ticket: string, playerId: int64, productId: int64) [RobloxScriptSecurity]
ConfirmPlayerMembership() [RobloxScriptSecurity]
ConfirmUserSubscriptionPurchase(subscriptionId: string) [RobloxSecurity]
LuaDialogCallbackSignal(value: bool, player: Instance) [RobloxScriptSecurity]
MockConfirmUserSubscriptionPurchase(userId: int64, subscriptionId: string) [RobloxSecurity]
MockPurchasePremium() [RobloxScriptSecurity]
NativePurchaseFinished(player: Instance, productId: string, wasPurchased: bool) [RobloxScriptSecurity]
NativePurchaseFinishedWithLocalPlayer(productId: string, wasPurchased: bool) [RobloxScriptSecurity]
PrepareCollectiblesPurchaseRequested(player: Instance, assetId: int64, collectibleItemId: string, collectibleItemInstanceId: string, collectibleProductId: string, expectedPrice: int) [RobloxScriptSecurity]
PromptBulkPurchaseFinished(player: Instance, status: MarketplaceBulkPurchasePromptStatus, results: Dictionary)
PromptBulkPurchaseRequested(player: Instance, displayData: Array, orderRequest: Dictionary, purchaserRobuxBalance: int64, orderTotalRobux: int64, options: Dictionary) [RobloxScriptSecurity]
PromptBundlePurchaseFinished(player: Instance, bundleId: int64, wasPurchased: bool)
PromptBundlePurchaseRequested(player: Instance, bundleId: int64) [RobloxScriptSecurity]
PromptCancelSubscriptionRequested(subscriptionId: string) [RobloxScriptSecurity]
PromptCollectibleBundlePurchaseRequested(player: Instance, bundleId: int64, collectibleItemId: string, collectibleItemInstanceId: string, collectibleProductId: string, expectedPrice: int, idempotencyKey: string, purchaseAuthToken: string) [RobloxScriptSecurity]
PromptCollectiblesPurchaseRequested(player: Instance, assetId: int64, collectibleItemId: string, collectibleItemInstanceId: string, collectibleProductId: string, expectedPrice: int, idempotencyKey: string, purchaseAuthToken: string) [RobloxScriptSecurity]
PromptGamePassPurchaseFinished(player: Instance, gamePassId: int64, wasPurchased: bool)
PromptGamePassPurchaseRequested(player: Instance, gamePassId: int64) [RobloxScriptSecurity]
PromptNativePurchaseRequested(player: Instance, productId: string) [RobloxSecurity]
PromptNativePurchaseRequestedWithLocalPlayer(userId: int64, productId: string) [RobloxSecurity]
PromptPremiumPurchaseFinished()
PromptPremiumPurchaseRequested(player: Instance) [RobloxScriptSecurity]
PromptProductPurchaseFinished(userId: int64, productId: int64, isPurchased: bool)
PromptProductPurchaseRequested(player: Instance, productId: int64, equipIfPurchased: bool, currencyType: CurrencyType) [RobloxScriptSecurity]
PromptPurchaseFinished(player: Instance, assetId: int64, isPurchased: bool)
PromptPurchaseRequested(player: Instance, assetId: int64, equipIfPurchased: bool, currencyType: CurrencyType) [RobloxScriptSecurity]
PromptPurchaseRequestedV2(player: Instance, assetId: int64, equipIfPurchased: bool, currencyType: CurrencyType, idempotencyKey: string, purchaseAuthToken: string) [RobloxScriptSecurity]
PromptRobloxPurchaseRequested(assetId: int64, equipIfPurchased: bool) [RobloxScriptSecurity]
PromptSubscriptionPurchaseFinished(user: Player, subscriptionId: string, didTryPurchasing: bool)
PromptSubscriptionPurchaseRequested(subscriptionId: string) [RobloxScriptSecurity]
PromptThirdPartyPurchaseRequested(player: Instance, productId: string) [RobloxSecurity]
ServerPurchaseVerification(serverResponseTable: Dictionary) [RobloxScriptSecurity]
ThirdPartyPurchaseFinished(player: Instance, productId: string, receipt: string, wasPurchased: bool) [LocalUserSecurity]
UserSubscriptionStatusChanged(subscriptionId: string) [RobloxScriptSecurity]
```

---

## MatchmakingService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetServerAttribute(name: string) → Tuple
InitializeServerAttributesForStudio(serverAttributes: Dictionary) → Tuple
SetServerAttribute(name: string, value: Variant) → Tuple
```

---

## MaterialGenerationService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GenerateMaterialVariantsAsync(prompt: string, samples: int64) → Dictionary [RobloxScriptSecurity]
```

---

## MaterialService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
AsphaltName: string = Asphalt [Read:RobloxSecurity] [Write:RobloxSecurity]
BasaltName: string = Basalt [Read:RobloxSecurity] [Write:RobloxSecurity]
BrickName: string = Brick [Read:RobloxSecurity] [Write:RobloxSecurity]
CardboardName: string = Cardboard [Read:RobloxSecurity] [Write:RobloxSecurity]
CarpetName: string = Carpet [Read:RobloxSecurity] [Write:RobloxSecurity]
CeramicTilesName: string = CeramicTiles [Read:RobloxSecurity] [Write:RobloxSecurity]
ClayRoofTilesName: string = ClayRoofTiles [Read:RobloxSecurity] [Write:RobloxSecurity]
CobblestoneName: string = Cobblestone [Read:RobloxSecurity] [Write:RobloxSecurity]
ConcreteName: string = Concrete [Read:RobloxSecurity] [Write:RobloxSecurity]
CorrodedMetalName: string = CorrodedMetal [Read:RobloxSecurity] [Write:RobloxSecurity]
CrackedLavaName: string = CrackedLava [Read:RobloxSecurity] [Write:RobloxSecurity]
DiamondPlateName: string = DiamondPlate [Read:RobloxSecurity] [Write:RobloxSecurity]
FabricName: string = Fabric [Read:RobloxSecurity] [Write:RobloxSecurity]
FoilName: string = Foil [Read:RobloxSecurity] [Write:RobloxSecurity]
GlacierName: string = Glacier [Read:RobloxSecurity] [Write:RobloxSecurity]
GraniteName: string = Granite [Read:RobloxSecurity] [Write:RobloxSecurity]
GrassName: string = Grass [Read:RobloxSecurity] [Write:RobloxSecurity]
GroundName: string = Ground [Read:RobloxSecurity] [Write:RobloxSecurity]
IceName: string = Ice [Read:RobloxSecurity] [Write:RobloxSecurity]
LeafyGrassName: string = LeafyGrass [Read:RobloxSecurity] [Write:RobloxSecurity]
LeatherName: string = Leather [Read:RobloxSecurity] [Write:RobloxSecurity]
LimestoneName: string = Limestone [Read:RobloxSecurity] [Write:RobloxSecurity]
MarbleName: string = Marble [Read:RobloxSecurity] [Write:RobloxSecurity]
MetalName: string = Metal [Read:RobloxSecurity] [Write:RobloxSecurity]
MudName: string = Mud [Read:RobloxSecurity] [Write:RobloxSecurity]
PavementName: string = Pavement [Read:RobloxSecurity] [Write:RobloxSecurity]
PebbleName: string = Pebble [Read:RobloxSecurity] [Write:RobloxSecurity]
PlasterName: string = Plaster [Read:RobloxSecurity] [Write:RobloxSecurity]
PlasticName: string = Plastic [Read:RobloxSecurity] [Write:RobloxSecurity]
RockName: string = Rock [Read:RobloxSecurity] [Write:RobloxSecurity]
RoofShinglesName: string = RoofShingles [Read:RobloxSecurity] [Write:RobloxSecurity]
RubberName: string = Rubber [Read:RobloxSecurity] [Write:RobloxSecurity]
SaltName: string = Salt [Read:RobloxSecurity] [Write:RobloxSecurity]
SandName: string = Sand [Read:RobloxSecurity] [Write:RobloxSecurity]
SandstoneName: string = Sandstone [Read:RobloxSecurity] [Write:RobloxSecurity]
SlateName: string = Slate [Read:RobloxSecurity] [Write:RobloxSecurity]
SmoothPlasticName: string = SmoothPlastic [Read:RobloxSecurity] [Write:RobloxSecurity]
SnowName: string = Snow [Read:RobloxSecurity] [Write:RobloxSecurity]
Use2022Materials: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Use2022MaterialsXml: bool = false
WoodName: string = Wood [Read:RobloxSecurity] [Write:RobloxSecurity]
WoodPlanksName: string = WoodPlanks [Read:RobloxSecurity] [Write:RobloxSecurity]
```

### Functions
```
GetBaseMaterialOverride(material: Material) → string
GetIsMaterialActionAsToolEnabled() → bool [RobloxScriptSecurity]
GetMaterialOverrideChanged(material: Material) → RBXScriptSignal [RobloxScriptSecurity]
GetMaterialVariant(material: Material, name: string) → MaterialVariant
GetOverrideStatus(material: Material) → PropertyStatus [RobloxScriptSecurity]
SetBaseMaterialOverride(material: Material, name: string) → null
SetCurrentMaterial(baseMaterial: Material, materialVariant: string) → null [RobloxScriptSecurity]
ToggleMaterialFillToolEnabled() → null [RobloxScriptSecurity]
```

### Events
```
MaterialFillToolEnabledChanged(shouldEnable: bool) [RobloxScriptSecurity]
OverrideStatusChanged(material: Material) [RobloxScriptSecurity]
```

---

## MaterialVariant
**Extends:** Instance

### Properties
```
AvgMetalness: int = 0
AvgRoughness: int = 127
BaseMaterial: Material = Plastic [Write:PluginSecurity]
ColorMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
ColorMapContent: Content [Read:PluginSecurity] [Write:PluginSecurity]
CustomPhysicalProperties: PhysicalProperties = default
MaterialPattern: MaterialPattern = Regular
MetalnessMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
MetalnessMapContent: Content [Read:PluginSecurity] [Write:PluginSecurity]
NormalMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
NormalMapContent: Content [Read:PluginSecurity] [Write:PluginSecurity]
RoughnessMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
RoughnessMapContent: Content [Read:PluginSecurity] [Write:PluginSecurity]
StudsPerTile: float = 10
TexturePack: ContentId
```

---

## MemStorageConnection
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
Disconnect() → null [PluginSecurity]
```

---

## MemStorageService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
Bind(key: string, callback: Function) → MemStorageConnection [RobloxScriptSecurity]
BindAndFire(key: string, callback: Function) → MemStorageConnection [RobloxScriptSecurity]
Call(key: string, input: Variant) → Variant [RobloxScriptSecurity]
Fire(key: string, value: string) → null [RobloxScriptSecurity]
GetItem(key: string, defaultValue: string) → string [RobloxScriptSecurity]
HasItem(key: string) → bool [RobloxScriptSecurity]
RemoveItem(key: string) → bool [RobloxScriptSecurity]
SetItem(key: string, value: string) → null [RobloxScriptSecurity]
```

---

## MemoryStoreHashMap
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
GetAsync(key: string) → Variant
ListItemsAsync(count: int) → MemoryStoreHashMapPages
RemoveAsync(key: string) → null
SetAsync(key: string, value: Variant, expiration: int64) → bool
UpdateAsync(key: string, transformFunction: Function, expiration: int64) → Variant
```

---

## MemoryStoreQueue
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
AddAsync(value: Variant, expiration: int64, priority: double) → null
GetSizeAsync(excludeInvisible: bool) → int
ReadAsync(count: int, allOrNothing: bool, waitTimeout: double) → Tuple
RemoveAsync(id: string) → null
```

---

## MemoryStoreService
**Extends:** Instance
**Tags:** Service

### Functions
```
GetHashMap(name: string) → MemoryStoreHashMap
GetQueue(name: string, invisibilityTimeout: int) → MemoryStoreQueue
GetSortedMap(name: string) → MemoryStoreSortedMap
```

---

## MemoryStoreSortedMap
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
GetAsync(key: string) → Tuple
GetRangeAsync(direction: SortDirection, count: int, exclusiveLowerBound: Variant, exclusiveUpperBound: Variant) → Array
GetSizeAsync() → int
RemoveAsync(key: string) → null
SetAsync(key: string, value: Variant, expiration: int64, sortKey: Variant) → bool
UpdateAsync(key: string, transformFunction: Function, expiration: int64) → Tuple
```

---

## Message
**Extends:** Instance
**Tags:** Deprecated

### Properties
```
Text: string
```

---

## Hint
**Extends:** Message
**Tags:** Deprecated

---

## MessageBusConnection
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
Disconnect() → null [RobloxScriptSecurity]
```

---

## MessageBusService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
Call(key: string, input: Variant) → Variant [RobloxScriptSecurity]
GetLast(mid: string) → Variant [RobloxScriptSecurity]
GetMessageId(domainName: string, messageName: string) → string [RobloxScriptSecurity]
GetProtocolMethodRequestMessageId(protocolName: string, methodName: string) → string [RobloxScriptSecurity]
GetProtocolMethodResponseMessageId(protocolName: string, methodName: string) → string [RobloxScriptSecurity]
MakeRequest(protocolName: string, methodName: string, message: Variant, callback: Function, customTelemetryData: Variant) → null [RobloxScriptSecurity]
Publish(mid: string, params: Variant) → null [RobloxScriptSecurity]
PublishProtocolMethodRequest(protocolName: string, methodName: string, message: Variant, customTelemetryData: Variant) → null [RobloxScriptSecurity]
PublishProtocolMethodResponse(protocolName: string, methodName: string, message: Variant, responseCode: int, customTelemetryData: Variant) → null [RobloxScriptSecurity]
SetRequestHandler(protocolName: string, methodName: string, callback: Function) → null [RobloxScriptSecurity]
Subscribe(mid: string, callback: Function, once: bool, sticky: bool) → Instance [RobloxScriptSecurity]
SubscribeToProtocolMethodRequest(protocolName: string, methodName: string, callback: Function, once: bool, sticky: bool) → Instance [RobloxScriptSecurity]
SubscribeToProtocolMethodResponse(protocolName: string, methodName: string, callback: Function, once: bool, sticky: bool) → Instance [RobloxScriptSecurity]
```

---

## MessagingService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
PublishAsync(topic: string, message: Variant) → null
SubscribeAsync(topic: string, callback: Function) → RBXScriptConnection
```

---

## MetaBreakpoint
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
Condition: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ContinueExecution: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Enabled: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Id: int = 4 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
IsLogpoint: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Line: int = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LogMessage: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
RemoveOnHit: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Script: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Valid: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Functions
```
GetContextBreakpoints() → Dictionary [RobloxScriptSecurity]
Remove(status: Function) → int [RobloxScriptSecurity]
SetChildBreakpointEnabledByScriptAndContext(script: string, contextGST: int, enabled: bool) → null [RobloxScriptSecurity]
SetContextEnabled(context: int, enabled: bool) → null [RobloxScriptSecurity]
SetContinueExecution(enabled: bool) → null [RobloxScriptSecurity]
SetEnabled(enabled: bool) → null [RobloxScriptSecurity]
SetLine(line: int, status: Function) → int [RobloxScriptSecurity]
SetRemoveOnHit(enabled: bool) → null [RobloxScriptSecurity]
```

---

## MetaBreakpointContext
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
ContextDataInternal: string = 0 1 2 
```

---

## MetaBreakpointManager
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
AddBreakpoint(script: Instance, line: int, condition: Instance) → Instance [RobloxScriptSecurity]
GetBreakpointById(metaBreakpointId: int) → MetaBreakpoint [RobloxScriptSecurity]
RemoveBreakpointById(metaBreakpointId: int) → null [RobloxScriptSecurity]
```

### Events
```
MetaBreakpointAdded(breakpoint: MetaBreakpoint) [RobloxScriptSecurity]
MetaBreakpointChanged(breakpoint: MetaBreakpoint) [RobloxScriptSecurity]
MetaBreakpointRemoved(breakpoint: MetaBreakpoint) [RobloxScriptSecurity]
MetaBreakpointSetChanged(breakpoint: MetaBreakpoint, detail: Dictionary) [RobloxScriptSecurity]
```

---

## MicroProfilerService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## ModerationService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
InternalCreateReviewableContentAsync(config: Dictionary) → string
InternalRequestReviewableContentReviewAsync(config: Dictionary) → null
```

---

## Mouse
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
Hit: CFrame [ReadOnly]
Icon: ContentId
Origin: CFrame [ReadOnly]
Target: BasePart [ReadOnly]
TargetFilter: Instance
TargetSurface: NormalId [ReadOnly]
UnitRay: Ray [ReadOnly]
ViewSizeX: int [ReadOnly]
ViewSizeY: int [ReadOnly]
X: int [ReadOnly]
Y: int [ReadOnly]
hit: CFrame [ReadOnly] [Deprecated]
target: BasePart [ReadOnly] [Deprecated]
```

### Events
```
Button1Down()
Button1Up()
Button2Down()
Button2Up()
Idle()
KeyDown(key: string)
KeyUp(key: string)
Move()
WheelBackward()
WheelForward()
keyDown(key: string)
```

---

## PlayerMouse
**Extends:** Mouse
**Tags:** NotCreatable

---

## PluginMouse
**Extends:** Mouse
**Tags:** NotCreatable

### Events
```
DragEnter(instances: Instances) [PluginSecurity]
```

---

## MouseService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Events
```
MouseEnterStudioViewport() [RobloxScriptSecurity]
MouseLeaveStudioViewport() [RobloxScriptSecurity]
```

---

## MultipleDocumentInterfaceInstance
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
FocusedDataModelSession: DataModelSession [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Events
```
DataModelSessionEnded(dataModelSession: Instance) [RobloxScriptSecurity]
DataModelSessionStarted(dataModelSession: Instance) [RobloxScriptSecurity]
```

---

## NetworkMarker
**Extends:** Instance
**Tags:** NotCreatable, NotBrowsable

### Events
```
Received()
```

---

## NetworkPeer
**Extends:** Instance
**Tags:** NotCreatable, NotBrowsable

### Functions
```
SetOutgoingKBPSLimit(limit: int) → null [PluginSecurity]
```

---

## NetworkClient
**Extends:** NetworkPeer
**Tags:** NotCreatable, Service, NotReplicated

### Events
```
ConnectionAccepted(peer: string, replicator: Instance)
ConnectionFailed(peer: string, code: int, reason: string)
```

---

## NetworkServer
**Extends:** NetworkPeer
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
EncryptStringForPlayerId(toEncrypt: string, playerId: int64) → string
```

---

## NetworkReplicator
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
GetPlayer() → Instance
```

---

## ClientReplicator
**Extends:** NetworkReplicator
**Tags:** NotCreatable, NotReplicated

### Functions
```
RequestRCCProfilerData(frameRate: int, timeFrame: int) → null [RobloxScriptSecurity]
RequestServerLuauHeapData() → null [RobloxScriptSecurity]
RequestServerScriptProfiling(start: bool, frequency: int?) → null [RobloxScriptSecurity]
RequestServerScriptProfilingData() → null [RobloxScriptSecurity]
RequestServerStats(request: bool) → null [RobloxScriptSecurity]
```

### Events
```
RCCProfilerDataComplete(success: bool, message: string) [RobloxScriptSecurity]
StatsReceived(stats: Dictionary) [RobloxScriptSecurity]
```

---

## ServerReplicator
**Extends:** NetworkReplicator
**Tags:** NotCreatable, NotReplicated

---

## NetworkSettings
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated, NotBrowsable

### Properties
```
EmulatedTotalMemoryInMB: int [Read:PluginSecurity] [Write:PluginSecurity]
FreeMemoryMBytes: float [Read:PluginSecurity] [Write:PluginSecurity] [ReadOnly]
HttpProxyEnabled: bool [Write:RobloxScriptSecurity]
HttpProxyURL: string [Write:RobloxScriptSecurity]
IncomingReplicationLag: double
OpenCertManagerDialog: int [Read:NotAccessibleSecurity] [Write:NotAccessibleSecurity]
PrintJoinSizeBreakdown: bool
PrintPhysicsErrors: bool
PrintStreamInstanceQuota: bool
RandomizeJoinInstanceOrder: bool
RenderStreamedRegions: bool
ShowActiveAnimationAsset: bool
```

---

## NoCollisionConstraint
**Extends:** Instance

### Properties
```
Enabled: bool = true
Part0: BasePart
Part1: BasePart
```

---

## Noise
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
NoiseType: NoiseType = SimplexGabor [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Seed: int = 1234 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
SampleDirectional(position: Vector3, direction: Vector3) → float [RobloxScriptSecurity]
SampleUniform(position: Vector3) → float [RobloxScriptSecurity]
```

---

## NotificationService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
IsConnected: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
IsLuaChatEnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
IsLuaGameDetailsEnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
SelectedTheme: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
ActionEnabled(actionType: AppShellActionType) → null [RobloxScriptSecurity]
ActionTaken(actionType: AppShellActionType) → null [RobloxScriptSecurity]
CancelAllNotification(userId: int64) → null [LocalUserSecurity]
CancelNotification(userId: int64, alertId: int) → null [LocalUserSecurity]
ScheduleNotification(userId: int64, alertId: int, alertMsg: string, minutesToFire: int) → null [LocalUserSecurity]
SwitchedToAppShellFeature(appShellFeature: AppShellFeature) → null [RobloxScriptSecurity]
GetScheduledNotifications(userId: int64) → Array [LocalUserSecurity]
```

### Events
```
Roblox17sConnectionChanged(connectionName: string, connectionState: ConnectionState, namespaceSequenceNumbers: string)
Roblox17sEventReceived(eventData: Map)
RobloxConnectionChanged(connectionName: string, connectionState: ConnectionState, sequenceNumber: string, namespaceSequenceNumbers: string) [RobloxScriptSecurity]
RobloxEventReceived(eventData: Map) [RobloxScriptSecurity]
```

---

## OmniRecommendationsService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
ClearSessionId() → null [RobloxScriptSecurity]
GetSessionId() → string [RobloxScriptSecurity]
MakeRequest(nextPageToken: string) → HttpRequest [RobloxScriptSecurity]
```

---

## OpenCloudApiV1
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
CreateModel(name: string) → OpenCloudModel
CreateUserNotificationAsync(user: string, userNotification: OpenCloudModel) → OpenCloudModel
```

---

## OpenCloudService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetApiV1() → OpenCloudApiV1
RegisterOpenCloud(version: string, methodName: string, method: Function) → null [RobloxScriptSecurity]
RegistrationComplete() → null [RobloxScriptSecurity]
HttpRequestAsync(options: Dictionary) → Dictionary [RobloxScriptSecurity]
InvokeAsync(version: string, methodName: string, arguments: Dictionary, headers: Dictionary) → Dictionary
```

---

## OperationGraph
**Extends:** Instance

---

## PVInstance
**Extends:** Instance
**Tags:** NotCreatable, NotBrowsable

### Properties
```
Origin: CFrame
Pivot Offset: CFrame
```

### Functions
```
GetPivot() → CFrame
PivotTo(targetCFrame: CFrame) → null
```

---

## BasePart
**Extends:** PVInstance
**Tags:** NotCreatable, NotBrowsable

### Properties
```
Anchored: bool
AssemblyAngularVelocity: Vector3
AssemblyCenterOfMass: Vector3 [ReadOnly]
AssemblyLinearVelocity: Vector3
AssemblyMass: float [ReadOnly]
AssemblyRootPart: BasePart [ReadOnly]
AudioCanCollide: bool
BackParamA: float [Deprecated]
BackParamB: float [Deprecated]
BackSurface: SurfaceType
BackSurfaceInput: InputType [Deprecated]
BottomParamA: float [Deprecated]
BottomParamB: float [Deprecated]
BottomSurface: SurfaceType
BottomSurfaceInput: InputType [Deprecated]
BrickColor: BrickColor
CFrame: CFrame
CanCollide: bool
CanQuery: bool
CanTouch: bool
CastShadow: bool
CenterOfMass: Vector3 [ReadOnly]
CollisionGroup: string
CollisionGroupId: int [Deprecated]
CollisionGroupReplicate: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Color: Color3
Color3uint8: Color3uint8
CurrentPhysicalProperties: PhysicalProperties [ReadOnly]
CustomPhysicalProperties: PhysicalProperties
DraggingV1: bool
Elasticity: float [Deprecated]
EnableFluidForces: bool
ExtentsCFrame: CFrame [ReadOnly]
ExtentsSize: Vector3 [ReadOnly]
Friction: float [Deprecated]
FrontParamA: float [Deprecated]
FrontParamB: float [Deprecated]
FrontSurface: SurfaceType
FrontSurfaceInput: InputType [Deprecated]
LeftParamA: float [Deprecated]
LeftParamB: float [Deprecated]
LeftSurface: SurfaceType
LeftSurfaceInput: InputType [Deprecated]
LocalSimulationValidation: int
LocalTransparencyModifier: float
Locked: bool
Mass: float [ReadOnly]
Massless: bool
Material: Material
MaterialVariant: string
MaterialVariantSerialized: string
NetworkIsSleeping: bool
NetworkOwnerV3: SystemAddress
NetworkOwnershipRule: NetworkOwnership
Orientation: Vector3
PhysicsRepRootPart: BasePart [Read:RobloxSecurity] [Write:RobloxSecurity]
PivotOffset: CFrame
Position: Vector3
ReceiveAge: float [ReadOnly]
Reflectance: float
ReplicationPV: ReplicationPV [Read:RobloxSecurity] [Write:RobloxSecurity]
ResizeIncrement: int [ReadOnly]
ResizeableFaces: Faces [ReadOnly]
RightParamA: float [Deprecated]
RightParamB: float [Deprecated]
RightSurface: SurfaceType
RightSurfaceInput: InputType [Deprecated]
RootPriority: int
RotVelocity: Vector3 [Deprecated]
Rotation: Vector3
Size: Vector3
SpecificGravity: float [ReadOnly] [Deprecated]
TopParamA: float [Deprecated]
TopParamB: float [Deprecated]
TopSurface: SurfaceType
TopSurfaceInput: InputType [Deprecated]
Transparency: float
Velocity: Vector3 [Deprecated]
brickColor: BrickColor [Deprecated]
siz: Vector3
size: Vector3
```

### Functions
```
AngularAccelerationToTorque(angAcceleration: Vector3, angVelocity: Vector3) → Vector3
ApplyAngularImpulse(impulse: Vector3) → null
ApplyImpulse(impulse: Vector3) → null
ApplyImpulseAtPosition(impulse: Vector3, position: Vector3) → null
BreakJoints() → null [Deprecated]
CanCollideWith(part: BasePart) → bool
CanSetNetworkOwnership() → Tuple
GetClosestPointOnSurface(position: Vector3) → Vector3
GetConnectedParts(recursive: bool) → Instances
GetJoints() → Instances
GetMass() → float
GetNetworkOwner() → Instance
GetNetworkOwnershipAuto() → bool
GetNoCollisionConstraints() → Instances
GetPhysicsCost() → float [RobloxScriptSecurity]
GetRenderCFrame() → CFrame [Deprecated]
GetRootPart() → Instance [Deprecated]
GetTouchingParts() → Instances
GetVelocityAtPosition(position: Vector3) → Vector3
IsGrounded() → bool
MakeJoints() → null [Deprecated]
Resize(normalId: NormalId, deltaAmount: int) → bool
SetNetworkOwner(playerInstance: Player) → null
SetNetworkOwnershipAuto() → null
SetPredictionMode(mode: PredictionMode) → null [RobloxScriptSecurity] [Deprecated]
TorqueToAngularAcceleration(torque: Vector3, angVelocity: Vector3) → Vector3
breakJoints() → null [Deprecated]
getMass() → float [Deprecated]
makeJoints() → null [Deprecated]
resize(normalId: NormalId, deltaAmount: int) → bool [Deprecated]
IntersectAsync(parts: Instances, collisionfidelity: CollisionFidelity, renderFidelity: RenderFidelity) → Instance
SubtractAsync(parts: Instances, collisionfidelity: CollisionFidelity, renderFidelity: RenderFidelity) → Instance
UnionAsync(parts: Instances, collisionfidelity: CollisionFidelity, renderFidelity: RenderFidelity) → Instance
```

### Events
```
LocalSimulationTouched(part: BasePart)
NetworkOwnerChanged(systemAddress: SystemAddress) [LocalUserSecurity]
OutfitChanged()
StoppedTouching(otherPart: BasePart)
TouchEnded(otherPart: BasePart)
Touched(otherPart: BasePart)
```

---

## CornerWedgePart
**Extends:** BasePart

---

## FormFactorPart
**Extends:** BasePart
**Tags:** NotCreatable

### Properties
```
FormFactor: FormFactor [Deprecated]
formFactor: FormFactor [Deprecated]
formFactorRaw: FormFactor
```

---

## Part
**Extends:** FormFactorPart

### Properties
```
Shape: PartType = Block
shap: PartType = __api_dump_write_only_property__
shape: PartType = Block
```

---

## FlagStand
**Extends:** Part
**Tags:** Deprecated

### Properties
```
TeamColor: BrickColor
```

### Events
```
FlagCaptured(player: Instance)
```

---

## Platform
**Extends:** Part
**Tags:** NotCreatable

### Events
```
RemoteCreateMotor6D(humanoid: Instance)
RemoteDestroyMotor6D()
```

---

## Seat
**Extends:** Part

### Properties
```
Disabled: bool = false
Occupant: Humanoid [ReadOnly]
```

### Functions
```
Sit(humanoid: Instance) → null
```

### Events
```
RemoteCreateSeatWeld(humanoid: Instance)
RemoteDestroySeatWeld()
```

---

## SkateboardPlatform
**Extends:** Part
**Tags:** Deprecated

### Properties
```
Controller: SkateboardController [ReadOnly]
ControllingHumanoid: Humanoid [ReadOnly]
MoveState: MoveState = Stopped
Steer: int = 0
StickyWheels: bool = true
Throttle: int = 0
```

### Functions
```
ApplySpecificImpulse(impulseWorld: Vector3) → null
```

### Events
```
Equipped(humanoid: Instance, skateboardController: Instance)
MoveStateChanged(newState: MoveState, oldState: MoveState)
RemoteCreateMotor6D(humanoid: Instance)
RemoteDestroyMotor6D()
Unequipped(humanoid: Instance)
equipped(humanoid: Instance, skateboardController: Instance)
unequipped(humanoid: Instance)
```

---

## SpawnLocation
**Extends:** Part

### Properties
```
AllowTeamChangeOnTouch: bool = false
Duration: int = 10
Enabled: bool = true
Neutral: bool = true
TeamColor: BrickColor
```

---

## WedgePart
**Extends:** FormFactorPart

---

## Terrain
**Extends:** BasePart
**Tags:** NotCreatable

### Properties
```
AcquisitionMethod: TerrainAcquisitionMethod = None [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ClusterGrid: string = __api_dump_write_only_property__
ClusterGridV2: string = __api_dump_write_only_property__
ClusterGridV3: BinaryString = __api_dump_write_only_property__
Decoration: bool = false
GrassLength: float = 0.699999988
IsSmooth: bool = true [ReadOnly] [Deprecated]
LastUsedModificationMethod: TerrainAcquisitionMethod = None [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
MaterialColors: BinaryString
MaxExtents: Region3int16 [ReadOnly]
PhysicsGrid: BinaryString = 
SmoothGrid: BinaryString = 
SmoothVoxelsUpgraded: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
WaterColor: Color3 = 0.05, 0.33, 0.36
WaterReflectance: float = 1
WaterTransparency: float = 0.300000012
WaterWaveSize: float = 0.150000006
WaterWaveSpeed: float = 10
```

### Functions
```
AutowedgeCell(x: int, y: int, z: int) → bool [Deprecated]
AutowedgeCells(region: Region3int16) → null [Deprecated]
CanSmoothVoxelsBeUpgraded() → bool [RobloxScriptSecurity]
CellCenterToWorld(x: int, y: int, z: int) → Vector3
CellCornerToWorld(x: int, y: int, z: int) → Vector3
Clear() → null
ClearVoxelsAsync_beta(region: Region3, channelIds: Array) → null
ConvertToSmooth() → null [PluginSecurity] [Deprecated]
CopyRegion(region: Region3int16) → TerrainRegion
CountCells() → int
FillBall(center: Vector3, radius: float, material: Material) → null
FillBlock(cframe: CFrame, size: Vector3, material: Material) → null
FillCylinder(cframe: CFrame, height: float, radius: float, material: Material) → null
FillRegion(region: Region3, resolution: float, material: Material) → null
FillWedge(cframe: CFrame, size: Vector3, material: Material) → null
GetCell(x: int, y: int, z: int) → Tuple [Deprecated]
GetMaterialColor(material: Material) → Color3
GetTerrainWireframe(cframe: CFrame, size: Vector3) → Array [RobloxScriptSecurity]
GetWaterCell(x: int, y: int, z: int) → Tuple [Deprecated]
IterateVoxelsAsync_beta(region: Region3, resolution: int, channelIds: Array) → TerrainIterateOperation
ModifyVoxelsAsync_beta(region: Region3, resolution: int, channelIds: Array) → TerrainModifyOperation
PasteRegion(region: TerrainRegion, corner: Vector3int16, pasteEmptyCells: bool) → null
ReadVoxelChannels(region: Region3, resolution: float, channelIds: Array) → Dictionary
ReadVoxels(region: Region3, resolution: float) → Tuple
ReadVoxelsAsync_beta(region: Region3, resolution: int, channelIds: Array) → TerrainReadOperation
ReplaceMaterial(region: Region3, resolution: float, sourceMaterial: Material, targetMaterial: Material) → null
ReplaceMaterialInTransform(cframe: CFrame, size: Vector3, sourceMaterial: Material, targetMaterial: Material) → null [RobloxScriptSecurity]
ReplaceMaterialInTransformSubregion(cframe: CFrame, size: Vector3, sourceMaterial: Material, targetMaterial: Material, targetRegion: Region3int16) → null [RobloxScriptSecurity]
SetCell(x: int, y: int, z: int, material: CellMaterial, block: CellBlock, orientation: CellOrientation) → null [Deprecated]
SetCells(region: Region3int16, material: CellMaterial, block: CellBlock, orientation: CellOrientation) → null [Deprecated]
SetMaterialColor(material: Material, value: Color3) → null
SetMaterialInTransform(cframe: CFrame, size: Vector3, targetMaterial: Material) → null [RobloxScriptSecurity]
SetMaterialInTransformSubregion(cframe: CFrame, size: Vector3, targetMaterial: Material, targetRegion: Region3int16) → null [RobloxScriptSecurity]
SetWaterCell(x: int, y: int, z: int, force: WaterForce, direction: WaterDirection) → null [Deprecated]
SmoothRegion(region: Region3, resolution: float, strength: float) → Tuple [RobloxScriptSecurity]
WorldToCell(position: Vector3) → Vector3
WorldToCellPreferEmpty(position: Vector3) → Vector3
WorldToCellPreferSolid(position: Vector3) → Vector3
WriteVoxelChannels(region: Region3, resolution: float, channels: Dictionary) → null
WriteVoxels(region: Region3, resolution: float, materials: Array, occupancy: Array) → null
WriteVoxelsAsync_beta(region: Region3, resolution: int, channelIds: Array) → TerrainWriteOperation
```

---

## TriangleMeshPart
**Extends:** BasePart
**Tags:** NotCreatable

### Properties
```
AeroMeshData: SharedString [Read:RobloxSecurity] [Write:RobloxSecurity]
CollisionFidelity: CollisionFidelity [Write:PluginSecurity]
ConvexDecompHolder: NetAssetRef [Read:RobloxSecurity] [Write:RobloxSecurity]
FluidFidelity: FluidFidelity [Write:PluginSecurity]
FluidFidelityInternal: FluidFidelity [Read:RobloxSecurity] [Write:RobloxSecurity]
InertiaMigrated: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
MeshSize: Vector3 [ReadOnly]
PhysicalConfigData: SharedString [Read:RobloxSecurity] [Write:RobloxSecurity]
UnscaledCofm: Vector3 [Read:RobloxSecurity] [Write:RobloxSecurity]
UnscaledVolInertiaDiags: Vector3 [Read:RobloxSecurity] [Write:RobloxSecurity]
UnscaledVolInertiaOffDiags: Vector3 [Read:RobloxSecurity] [Write:RobloxSecurity]
UnscaledVolume: float [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## MeshPart
**Extends:** TriangleMeshPart

### Properties
```
AlternateMeshHash: int64 = 0 [Read:RobloxSecurity] [Write:RobloxSecurity] [ReadOnly]
DoubleSided: bool = false [Write:PluginSecurity]
EditableMeshString: SharedString [Read:RobloxSecurity] [Write:RobloxSecurity]
HasJointOffset: bool = false [Write:NotAccessibleSecurity]
HasSkinnedMesh: bool = false [Write:NotAccessibleSecurity]
InitialSize: Vector3 = 0, 0, 0 [Read:RobloxSecurity] [Write:RobloxSecurity]
JointOffset: Vector3 = 0, 0, 0 [Write:NotAccessibleSecurity]
MeshContent: Content [Write:NotAccessibleSecurity]
MeshID: ContentId [Deprecated]
MeshId: ContentId [Write:NotAccessibleSecurity]
PhysicsData: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
RenderFidelity: RenderFidelity = Automatic [Write:PluginSecurity]
RenderFidelityReplicate: RenderFidelity = Automatic [Write:PluginSecurity]
TextureContent: Content
TextureID: ContentId
VertexCount: int = 0 [Read:RobloxSecurity] [Write:RobloxSecurity]
```

### Functions
```
ApplyMesh(meshPart: Instance) → null
```

---

## PartOperation
**Extends:** TriangleMeshPart

### Properties
```
AssetId: ContentId [Read:RobloxSecurity] [Write:RobloxSecurity]
ChildData: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
ChildData2: SharedString [Read:RobloxSecurity] [Write:RobloxSecurity]
ComponentIndex: int = -1 [Read:RobloxSecurity] [Write:RobloxSecurity]
DCDPropertyData: CSGPropertyData [Read:RobloxSecurity] [Write:RobloxSecurity]
FormFactor: FormFactor = Custom [Read:RobloxSecurity] [Write:RobloxSecurity]
InitialSize: Vector3 = 1, 1, 1 [Read:RobloxSecurity] [Write:RobloxSecurity]
ManifoldMesh_DEPRECATED: SharedString [Read:RobloxSecurity] [Write:RobloxSecurity] [Deprecated]
MeshData: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
MeshData2: SharedString [Read:RobloxSecurity] [Write:RobloxSecurity]
OffCentered: bool = false [Read:RobloxSecurity] [Write:RobloxSecurity]
PhysicsData: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
RenderFidelity: RenderFidelity = Automatic [Write:PluginSecurity]
SerializedCSGTree: SharedString
SerializedOperationGraph: SharedString
SmoothingAngle: float = 0 [Write:PluginSecurity]
SolidMeshHolder: NetAssetRef
TriangleCount: int = 0 [ReadOnly]
UsePartColor: bool = false
```

### Functions
```
SubstituteGeometry(source: Instance) → null
```

---

## IntersectOperation
**Extends:** PartOperation

---

## NegateOperation
**Extends:** PartOperation

### Properties
```
PreviousOperation: NegateOperationHiddenHistory = None [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## UnionOperation
**Extends:** PartOperation

---

## TrussPart
**Extends:** BasePart

### Properties
```
Style: Style = AlternatingSupports
style: Style = AlternatingSupports
```

---

## VehicleSeat
**Extends:** BasePart

### Properties
```
AreHingesDetected: int = 0 [ReadOnly]
Disabled: bool = false
HeadsUpDisplay: bool = true
MaxSpeed: float = 25
Occupant: Humanoid [ReadOnly]
Steer: int = 0
SteerFloat: float = 0
Throttle: int = 0
ThrottleFloat: float = 0
Torque: float = 10
TurnSpeed: float = 1
```

### Functions
```
Sit(humanoid: Instance) → null
```

### Events
```
RemoteCreateSeatWeld(humanoid: Instance)
RemoteDestroySeatWeld()
```

---

## Camera
**Extends:** PVInstance
**Tags:** NotReplicated

### Properties
```
CFrame: CFrame
CameraSubject: Instance
CameraType: CameraType = Fixed
CoordinateFrame: CFrame [Deprecated]
DiagonalFieldOfView: float = 88.8765335
FieldOfView: float = 70
FieldOfViewMode: FieldOfViewMode = Vertical
Focus: CFrame
HeadLocked: bool = true
HeadScale: float = 1
MaxAxisFieldOfView: float = 70
NearPlaneZ: float = -0.5 [ReadOnly]
VRTiltAndRollEnabled: bool = false
ViewportSize: Vector2 = 1, 1 [ReadOnly]
focus: CFrame [Deprecated]
```

### Functions
```
GetLargestCutoffDistance(ignoreList: Instances) → float [Deprecated]
GetPanSpeed() → float [Deprecated]
GetPartsObscuringTarget(castPoints: Array, ignoreList: Instances) → Instances
GetRenderCFrame() → CFrame
GetRoll() → float
GetTiltSpeed() → float [Deprecated]
Interpolate(endPos: CFrame, endFocus: CFrame, duration: float) → null [Deprecated]
PanUnits(units: int) → null [Deprecated]
ScreenPointToRay(x: float, y: float, depth: float) → Ray
SetCameraPanMode(mode: CameraPanMode) → null [Deprecated]
SetImageServerView(modelCoord: CFrame) → null [RobloxScriptSecurity]
SetRoll(rollAngle: float) → null
TiltUnits(units: int) → bool [Deprecated]
ViewportPointToRay(x: float, y: float, depth: float) → Ray
WorldToScreenPoint(worldPoint: Vector3) → Tuple
WorldToViewportPoint(worldPoint: Vector3) → Tuple
Zoom(distance: float) → bool [RobloxScriptSecurity]
ZoomToExtents(boundingBoxCFrame: CFrame, boundingBoxSize: Vector3) → null
```

### Events
```
FirstPersonTransition(entering: bool) [LocalUserSecurity]
InterpolationFinished()
```

---

## Model
**Extends:** PVInstance

### Properties
```
LevelOfDetail: ModelLevelOfDetail = Automatic [Read:PluginSecurity] [Write:PluginSecurity]
LodEntity: LodDataEntity
ModelMeshCFrame: CFrame
ModelMeshData: SharedString
ModelMeshSize: Vector3 = 0, 0, 0
ModelStreamingMode: ModelStreamingMode = Default
NeedsPivotMigration: bool = false
PrimaryPart: BasePart
Scale: float = 1
ScaleFactor: float = 1
SlimHash: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
WorldPivot: CFrame
WorldPivotData: OptionalCoordinateFrame
```

### Functions
```
AddPersistentPlayer(playerInstance: Player) → null
BreakJoints() → null [Deprecated]
GetBoundingBox() → void
GetExtentsSize() → Vector3
GetModelCFrame() → CFrame [Deprecated]
GetModelSize() → Vector3 [Deprecated]
GetPersistentPlayers() → Instances
GetPrimaryPartCFrame() → CFrame [Deprecated]
GetScale() → float
MakeJoints() → null [Deprecated]
MoveTo(position: Vector3) → null
RemovePersistentPlayer(playerInstance: Player) → null
ResetOrientationToIdentity() → null [Deprecated]
ScaleTo(newScaleFactor: float) → null
SetIdentityOrientation() → null [Deprecated]
SetPrimaryPartCFrame(cframe: CFrame) → null [Deprecated]
TranslateBy(delta: Vector3) → null
breakJoints() → null [Deprecated]
makeJoints() → null [Deprecated]
move(location: Vector3) → null [Deprecated]
moveTo(location: Vector3) → null [Deprecated]
```

---

## Actor
**Extends:** Model

### Functions
```
BindToMessage(topic: string, function: Function) → RBXScriptConnection
BindToMessageParallel(topic: string, function: Function) → RBXScriptConnection
SendMessage(topic: string, message: Tuple) → null
```

---

## BackpackItem
**Extends:** Model
**Tags:** NotCreatable

### Properties
```
TextureId: ContentId
```

---

## HopperBin
**Extends:** BackpackItem
**Tags:** Deprecated

### Properties
```
Active: bool = false
BinType: BinType = Script
Command: string = __api_dump_write_only_property__
TextureName: string = __api_dump_write_only_property__
```

### Functions
```
Disable() → null [RobloxScriptSecurity]
ToggleSelect() → null [RobloxScriptSecurity]
```

### Events
```
Deselected()
ReplicatedSelected()
Selected(mouse: Instance)
```

---

## Tool
**Extends:** BackpackItem

### Properties
```
CanBeDropped: bool = true
Enabled: bool = true
Grip: CFrame
GripForward: Vector3 = -0, -0, -1
GripPos: Vector3 = 0, 0, 0
GripRight: Vector3 = 1, 0, 0
GripUp: Vector3 = 0, 1, 0
ManualActivationOnly: bool = false
RequiresHandle: bool = true
ToolTip: string
```

### Functions
```
Activate() → null
Deactivate() → null
```

### Events
```
Activated()
Deactivated()
Equipped(mouse: Mouse)
Unequipped()
VRLaserPointerClicked(player: Player) [RobloxSecurity]
```

---

## Flag
**Extends:** Tool
**Tags:** Deprecated

### Properties
```
TeamColor: BrickColor
```

---

## Status
**Extends:** Model
**Tags:** NotCreatable, Deprecated

---

## WorldRoot
**Extends:** Model
**Tags:** NotCreatable

### Properties
```
PhysicsStepTime: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
ArePartsTouchingOthers(partList: Instances, overlapIgnored: float) → bool
Blockcast(cframe: CFrame, size: Vector3, direction: Vector3, params: RaycastParams) → RaycastResult?
BulkMoveTo(partList: Instances, cframeList: Array, eventMode: BulkMoveMode) → null
CacheCurrentTerrain(id: string, center: Vector3, radius: float) → string [RobloxScriptSecurity]
ClearCachedTerrain(id: string) → bool [RobloxScriptSecurity]
FindPartOnRay(ray: Ray, ignoreDescendantsInstance: Instance, terrainCellsAreCubes: bool, ignoreWater: bool) → Tuple [Deprecated]
FindPartOnRayWithIgnoreList(ray: Ray, ignoreDescendantsTable: Instances, terrainCellsAreCubes: bool, ignoreWater: bool) → Tuple [Deprecated]
FindPartOnRayWithWhitelist(ray: Ray, whitelistDescendantsTable: Instances, ignoreWater: bool) → Tuple [Deprecated]
FindPartsInRegion3(region: Region3, ignoreDescendantsInstance: Instance, maxParts: int) → Instances [Deprecated]
FindPartsInRegion3WithIgnoreList(region: Region3, ignoreDescendantsTable: Instances, maxParts: int) → Instances [Deprecated]
FindPartsInRegion3WithWhiteList(region: Region3, whitelistDescendantsTable: Instances, maxParts: int) → Instances [Deprecated]
GetAwakeContactNormals() → Array [RobloxScriptSecurity]
GetAwakeContactParts() → Array [RobloxScriptSecurity]
GetAwakeContactPositions() → Array [RobloxScriptSecurity]
GetAwakeRootParts() → Instances [RobloxScriptSecurity]
GetPartBoundsInBox(cframe: CFrame, size: Vector3, overlapParams: OverlapParams) → Instances
GetPartBoundsInRadius(position: Vector3, radius: float, overlapParams: OverlapParams) → Instances
GetPartsInPart(part: BasePart, overlapParams: OverlapParams) → Instances
IKMoveTo(part: BasePart, target: CFrame, translateStiffness: float, rotateStiffness: float, collisionsMode: IKCollisionsMode) → null [PluginSecurity]
IsRegion3Empty(region: Region3, ignoreDescendentsInstance: Instance) → bool [Deprecated]
IsRegion3EmptyWithIgnoreList(region: Region3, ignoreDescendentsTable: Instances) → bool [Deprecated]
Raycast(origin: Vector3, direction: Vector3, raycastParams: RaycastParams) → RaycastResult?
RaycastCachedTerrain(id: string, origin: Vector3, direction: Vector3, ignoreWater: bool) → RaycastResult? [RobloxScriptSecurity]
SetInsertPoint(point: Vector3) → null [RobloxScriptSecurity]
Shapecast(part: BasePart, direction: Vector3, params: RaycastParams) → RaycastResult?
Spherecast(position: Vector3, radius: float, direction: Vector3, params: RaycastParams) → RaycastResult?
StepPhysics(dt: float, parts: Instances) → null [PluginSecurity]
findPartOnRay(ray: Ray, ignoreDescendantsInstance: Instance, terrainCellsAreCubes: bool, ignoreWater: bool) → Tuple [Deprecated]
findPartsInRegion3(region: Region3, ignoreDescendantsInstance: Instance, maxParts: int) → Instances [Deprecated]
```

---

## Workspace
**Extends:** WorldRoot
**Tags:** NotCreatable, Service

### Properties
```
AirDensity: float
AllowThirdPartySales: bool
AuthorityMode: AuthorityMode [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AvatarUnificationMode: AvatarUnificationMode
ClientAnimatorThrottling: ClientAnimatorThrottlingMode
CollisionGroupData: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
CollisionGroups: string
ConvexDecompCompressed: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
CurrentCamera: Camera
DataModelPlaceVersion: int
DistributedGameTime: double
ExplicitAutoJoints: bool
FallHeightEnabled: bool [Write:PluginSecurity]
FallenPartsDestroyHeight: float [Write:PluginSecurity]
FilteringEnabled: bool [Write:PluginSecurity] [Deprecated]
FluidForces: FluidForces
GlobalWind: Vector3
Gravity: float
IKControlConstraintSupport: IKControlConstraintSupport
InsertPoint: Vector3
InterpolationThrottling: InterpolationThrottlingMode [Write:PluginSecurity] [Deprecated]
LuauTypeCheckMode: LuauTypeCheckMode [Read:PluginSecurity] [Write:PluginSecurity]
MeshPartHeadsAndAccessories: MeshPartHeadsAndAccessories
ModelStreamingBehavior: ModelStreamingBehavior
MoverConstraintRootBehavior: MoverConstraintRootBehaviorMode
PathfindingUseImprovedSearch: PathfindingUseImprovedSearch
PhysicsImprovedSleep: RolloutState
PhysicsSteppingMethod: PhysicsSteppingMethod
PlayerCharacterDestroyBehavior: PlayerCharacterDestroyBehavior
PrimalPhysicsSolver: PrimalPhysicsSolver
RejectCharacterDeletions: RejectCharacterDeletions
RenderingCacheOptimizations: RenderingCacheOptimizationMode
ReplicateInstanceDestroySetting: ReplicateInstanceDestroySetting
Retargeting: AnimatorRetargetingMode
SandboxedInstanceMode: SandboxedInstanceMode
SignalBehavior: SignalBehavior
SignalBehavior2: SignalBehavior
StreamOutBehavior: StreamOutBehavior
StreamingEnabled: bool [Write:PluginSecurity]
StreamingIntegrityMode: StreamingIntegrityMode
StreamingMinRadius: int
StreamingPauseMode: StreamingPauseMode
StreamingTargetRadius: int
Terrain: Terrain [ReadOnly]
TerrainWeldsFixed: bool
TouchEventsUseCollisionGroups: RolloutState
TouchesUseCollisionGroups: bool
UseImprovedModelLod: RolloutState
UseNewLuauTypeSolver: RolloutState
```

### Functions
```
BreakJoints(objects: Instances) → null [PluginSecurity] [Deprecated]
CalculateJumpDistance(gravity: float, jumpPower: float, walkSpeed: float) → float [RobloxScriptSecurity]
CalculateJumpHeight(gravity: float, jumpPower: float) → float [RobloxScriptSecurity]
CalculateJumpPower(gravity: float, jumpHeight: float) → float [RobloxScriptSecurity]
ExperimentalSolverIsEnabled() → bool [LocalUserSecurity]
GetNumAwakeParts() → int
GetPhysicsThrottling() → int
GetRealPhysicsFPS() → double
GetServerTimeNow() → double
JoinToOutsiders(objects: Instances, jointType: JointCreationMode) → null
MakeJoints(objects: Instances) → null [PluginSecurity] [Deprecated]
PGSIsEnabled() → bool
SetAvatarUnificationMode(value: AvatarUnificationMode) → null [RobloxScriptSecurity]
SetMeshPartHeadsAndAccessories(value: MeshPartHeadsAndAccessories) → null [RobloxScriptSecurity]
SetPhysicsThrottleEnabled(value: bool) → null [LocalUserSecurity]
UnjoinFromOutsiders(objects: Instances) → null
ZoomToExtents() → null [PluginSecurity]
```

### Events
```
PersistentLoaded(player: Player)
```

---

## WorldModel
**Extends:** WorldRoot

---

## PackageLink
**Extends:** Instance
**Tags:** NotCreatable, NotBrowsable

### Properties
```
AutoUpdate: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CanAutoUpdate: bool = false [Read:RobloxSecurity] [Write:RobloxSecurity]
Creator: string [ReadOnly]
DefaultName: string [Write:NotAccessibleSecurity]
HasNewVersion: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ModifiedState: int = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
PackageAssetName: string [ReadOnly]
PackageGuid: int64 = 0
PackageId: ContentId [ReadOnly]
PackageIdSerialize: ContentId
PermissionLevel: PackagePermission = None [ReadOnly]
SerializedDefaultAttributes: BinaryString [Write:NotAccessibleSecurity]
Status: string = Up To Date [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
VersionIdSerialize: int64 = 0
VersionNumber: int64 = 0 [Write:NotAccessibleSecurity]
```

---

## PackageService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## PackageUIService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
ConvertToMockPackage(instance: Instance) → null [RobloxScriptSecurity]
ConvertToPackageUpload(uploadUrl: string, cloneInstances: Instances, originalInstances: Instances) → null [RobloxScriptSecurity]
GetPackageInfo(packageAssetId: int64) → Dictionary [RobloxScriptSecurity]
PublishPackage(packageInstance: Instance, addUndoWayPoint: bool) → null [RobloxScriptSecurity]
SetPackageVersion(packageInstance: Instance, versionNumber: int64) → Instance [RobloxScriptSecurity]
```

### Events
```
OnConvertToPackageResult(isSuccessful: bool, errorMessage: string) [RobloxScriptSecurity]
OnOpenConvertToPackagePlugin(instances: Instances, name: string, cloneInstances: Instances) [RobloxScriptSecurity]
```

---

## Pages
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
IsFinished: bool [ReadOnly]
```

### Functions
```
GetCurrentPage() → Array
AdvanceToNextPageAsync() → null
```

---

## AudioPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

---

## BanHistoryPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

---

## CapturesPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

---

## CatalogPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

---

## DataStoreKeyPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

### Properties
```
Cursor: string [ReadOnly]
```

---

## DataStoreListingPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

### Properties
```
Cursor: string [ReadOnly]
```

---

## DataStorePages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

---

## DataStoreVersionPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

---

## FriendPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

---

## InventoryPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

---

## EmotesPages
**Extends:** InventoryPages
**Tags:** NotCreatable, NotReplicated

---

## MemoryStoreHashMapPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

---

## OutfitPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

---

## RecommendationPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

---

## StandardPages
**Extends:** Pages
**Tags:** NotCreatable, NotReplicated

---

## PartOperationAsset
**Extends:** Instance

### Properties
```
ChildData: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
MeshData: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## ParticleEmitter
**Extends:** Instance

### Properties
```
Acceleration: Vector3 = 0, 0, 0
Brightness: float = 1
Color: ColorSequence = 0 1 1 1 0 1 1 1 1 0 
Drag: float = 0
EmissionDirection: NormalId = Top
Enabled: bool = true
FlipbookFramerate: NumberRange = 1 1 
FlipbookIncompatible: string = Particle texture must be 1024 by 1024 to use flipbooks.
FlipbookLayout: ParticleFlipbookLayout = None
FlipbookMode: ParticleFlipbookMode = Loop
FlipbookStartRandom: bool = false
Lifetime: NumberRange = 5 10 
LightEmission: float = 0
LightInfluence: float = 0
LocalTransparencyModifier: float = 0
LockedToPart: bool = false
Orientation: ParticleOrientation = FacingCamera
Rate: float = 20
RotSpeed: NumberRange = 0 0 
Rotation: NumberRange = 0 0 
Shape: ParticleEmitterShape = Box
ShapeInOut: ParticleEmitterShapeInOut = Outward
ShapePartial: float = 1
ShapeStyle: ParticleEmitterShapeStyle = Volume
Size: NumberSequence = 0 1 0 1 1 0 
Speed: NumberRange = 5 5 
SpreadAngle: Vector2 = 0, 0
Squash: NumberSequence = 0 0 0 1 0 0 
Texture: ContentId = rbxasset://textures/particles/sparkles_main.dds
TimeScale: float = 1
Transparency: NumberSequence = 0 0 0 1 0 0 
VelocityInheritance: float = 0
VelocitySpread: float = 0 [Deprecated]
WindAffectsDrag: bool = false
ZOffset: float = 0
```

### Functions
```
Clear() → null
Emit(particleCount: int) → null
FastForward(numFrames: int) → null [RobloxScriptSecurity]
```

### Events
```
OnClearRequested()
OnEmitRequested(particleCount: int)
```

---

## PartyEmulatorService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
CreateNewParty() → string [RobloxScriptSecurity]
DeleteParty(partyId: string) → null [RobloxScriptSecurity]
GetEmulatedPartyConfiguration() → Dictionary [RobloxScriptSecurity]
GetIsEmulationEnabled() → bool [RobloxScriptSecurity]
OnTestPlayerCountChanged(newPlayerCount: int) → null [RobloxScriptSecurity]
SetIsEmulationEnabled(isEnabled: bool) → null [RobloxScriptSecurity]
SetPlayerPartyId(userId: int64, partyId: string) → null [RobloxScriptSecurity]
applyPartyIdToPlayer(player: Player) → null [RobloxScriptSecurity]
GetEmulatedPartyAsync(partyId: string) → Array [RobloxScriptSecurity]
```

### Events
```
ConfigurationChanged(configuration: Dictionary) [RobloxScriptSecurity]
```

---

## PatchBundlerFileWatch
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## PatchMapping
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
FlattenTree: bool = false
PatchId: string
TargetPath: string
```

---

## Path
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
Status: PathStatus [ReadOnly]
```

### Functions
```
GetPointCoordinates() → Array [Deprecated]
GetWaypoints() → Array
CheckOcclusionAsync(start: int) → int
ComputeAsync(start: Vector3, finish: Vector3) → null
```

### Events
```
Blocked(blockedWaypointIdx: int)
Unblocked(unblockedWaypointIdx: int)
```

---

## PathfindingLink
**Extends:** Instance

### Properties
```
Attachment0: Attachment
Attachment1: Attachment
IsBidirectional: bool = true
Label: string
```

---

## PathfindingModifier
**Extends:** Instance

### Properties
```
Label: string
PassThrough: bool = false
```

---

## PathfindingService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
EmptyCutoff: float = 0 [Deprecated]
```

### Functions
```
CreatePath(agentParameters: Dictionary) → Path
ComputeRawPathAsync(start: Vector3, finish: Vector3, maxDistance: float) → Path [Deprecated]
ComputeSmoothPathAsync(start: Vector3, finish: Vector3, maxDistance: float) → Path [Deprecated]
FindPathAsync(start: Vector3, finish: Vector3) → Path
```

---

## PausedState
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
AllThreadsPaused: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Reason: DebuggerPauseReason [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
ThreadId: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

---

## PausedStateBreakpoint
**Extends:** PausedState
**Tags:** NotCreatable, NotReplicated

### Properties
```
Breakpoint: Breakpoint [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

---

## PausedStateException
**Extends:** PausedState
**Tags:** NotCreatable, NotReplicated

### Properties
```
ExceptionText: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

---

## PerformanceControlService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
IsCrossExperienceLaunchFeasible(type: string) → bool [RobloxScriptSecurity]
```

---

## PermissionsService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
GetIsThirdPartyAssetAllowed() → bool [RobloxScriptSecurity]
GetIsThirdPartyPurchaseAllowed() → bool [RobloxScriptSecurity]
GetIsThirdPartyTeleportAllowed() → bool [RobloxScriptSecurity]
GetPermissions(assetId: string) → Array [RobloxScriptSecurity]
SetPermissions(assetId: string, permissions: Array) → null [RobloxScriptSecurity]
```

---

## PhysicsService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
CollisionGroupContainsPart(name: string, part: BasePart) → bool [Deprecated]
CollisionGroupSetCollidable(name1: string, name2: string, collidable: bool) → null
CollisionGroupsAreCollidable(name1: string, name2: string) → bool
CreateCollisionGroup(name: string) → int [Deprecated]
GetCollisionGroupId(name: string) → int [Deprecated]
GetCollisionGroupName(name: int) → string [Deprecated]
GetCollisionGroups() → Array [Deprecated]
GetMaxCollisionGroups() → int
GetRegisteredCollisionGroups() → Array
IkSolve(part: BasePart, target: CFrame, translateStiffness: float, rotateStiffness: float) → null [RobloxScriptSecurity]
IsCollisionGroupRegistered(name: string) → bool
LocalIkSolve(part: BasePart, target: CFrame, translateStiffness: float, rotateStiffness: float) → null [LocalUserSecurity]
RegisterCollisionGroup(name: string) → null
RemoveCollisionGroup(name: string) → null [Deprecated]
RenameCollisionGroup(from: string, to: string) → null
SetPartCollisionGroup(part: BasePart, name: string) → null [Deprecated]
UnregisterCollisionGroup(name: string) → null
```

---

## PhysicsSettings
**Extends:** Instance
**Tags:** NotCreatable, Settings, NotReplicated

### Properties
```
AllowSleep: bool
AreAnchorsShown: bool
AreAssembliesShown: bool
AreAssemblyCentersOfMassShown: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AreAwakePartsHighlighted: bool
AreBodyTypesShown: bool
AreCollisionCostsShown: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AreConstraintForcesShownForSelectedOrHoveredInstances: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AreConstraintTorquesShownForSelectedOrHoveredInstances: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AreContactForcesShownForSelectedOrHoveredAssemblies: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AreContactIslandsShown: bool
AreContactPointsShown: bool
AreGravityForcesShownForSelectedOrHoveredAssemblies: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AreJointCoordinatesShown: bool
AreMagnitudesShownForDrawnForcesAndTorques: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AreMechanismsShown: bool
AreModelCoordsShown: bool
AreNonAnchorsShown: bool
AreOwnersShown: bool
ArePartCoordsShown: bool
AreRegionsShown: bool
AreSolverIslandsShown: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AreTerrainReplicationRegionsShown: bool
AreTimestepsShown: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AreUnalignedPartsShown: bool
AreWorldCoordsShown: bool
DisableCSGv2: bool
DisableCSGv3ForPlugins: bool
DrawConstraintsNetForce: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DrawContactsNetForce: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DrawTotalNetForce: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
EnableForceVisualizationSmoothing: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
FluidForceDrawScale: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ForceCSGv2: bool
ForceDrawScale: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ForceVisualizationSmoothingSteps: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
IsInterpolationThrottleShown: bool
IsReceiveAgeShown: bool
IsTreeShown: bool
PhysicsEnvironmentalThrottle: EnviromentalPhysicsThrottle
ShowDecompositionGeometry: bool
ShowFluidForcesForSelectedOrHoveredMechanisms: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ShowInstanceNamesForDrawnForcesAndTorques: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
SolverConvergenceMetricType: SolverConvergenceMetricType [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
SolverConvergenceVisualizationMode: SolverConvergenceVisualizationMode [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ThrottleAdjustTime: double
TorqueDrawScale: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
UseCSGv2: bool
```

---

## PlaceAssetIdsService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## PlaceStatsService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## PlacesService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
StartPlaySolo() → null [RobloxScriptSecurity]
StopPlaySolo() → null [RobloxScriptSecurity]
```

---

## PlatformCloudStorageService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
IsUserDataAvailable() → bool [RobloxScriptSecurity]
GetUserDataAsync(key: string) → Dictionary [RobloxScriptSecurity]
SetUserDataAsync(key: string, data: Dictionary) → null [RobloxScriptSecurity]
```

---

## PlatformFriendsService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
IsInviteFriendsEnabled() → bool [RobloxScriptSecurity]
IsProfileEnabled() → bool [RobloxScriptSecurity]
ShowInviteFriendsUI() → null [RobloxScriptSecurity]
ShowProfile(platformUserId: string) → null [RobloxScriptSecurity]
GetPartyMembers() → Array [RobloxScriptSecurity]
```

---

## Player
**Extends:** Instance

### Properties
```
AccountAge: int [ReadOnly]
AccountAgeReplicate: int
AppearanceDidLoad: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly] [Deprecated]
AutoJumpEnabled: bool
CameraMaxZoomDistance: float
CameraMinZoomDistance: float
CameraMode: CameraMode
CanLoadCharacterAppearance: bool
Character: Model
CharacterAppearance: string [Deprecated]
CharacterAppearanceId: int64
ChararacterRegionId: Vector3 [Read:RobloxSecurity] [Write:RobloxSecurity]
ChatMode: ChatMode [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
ChatPrivacyMode: ChatPrivacyMode [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CloudEditCameraCoordinateFrame: CFrame
CloudEditPlayerActive: bool
CountryRegionCodeReplicate: string
DataComplexity: int [ReadOnly] [Deprecated]
DataComplexityLimit: int [Read:LocalUserSecurity] [Write:LocalUserSecurity] [Deprecated]
DataReady: bool [ReadOnly] [Deprecated]
DevCameraOcclusionMode: DevCameraOcclusionMode
DevComputerCameraMode: DevComputerCameraMovementMode
DevComputerMovementMode: DevComputerMovementMode
DevEnableMouseLock: bool
DevTouchCameraMode: DevTouchCameraMovementMode
DevTouchMovementMode: DevTouchMovementMode
DisplayName: string
FollowUserId: int64 [ReadOnly]
FollowUserIdReplicated: int64
GameplayPaused: bool [Write:NotAccessibleSecurity]
Guest: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
HasVerifiedBadge: bool
HealthDisplayDistance: float
InternalCharacterAppearanceLoaded: bool
LocaleId: string [ReadOnly]
MaxSimulationRadius: float [Read:LocalUserSecurity] [Write:LocalUserSecurity]
MaximumSimulationRadius: float [Read:LocalUserSecurity] [Write:LocalUserSecurity]
MembershipType: MembershipType [ReadOnly]
MembershipTypeReplicate: MembershipType
NameDisplayDistance: float
Neutral: bool
OsPlatform: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
PartyId: string [Write:RobloxSecurity]
PlatformName: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
RawJoinData: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
ReplicationFocus: Instance
RespawnLocation: SpawnLocation
SimulationRadius: float [Read:LocalUserSecurity] [Write:LocalUserSecurity]
StepIdOffset: int [Read:RobloxSecurity] [Write:RobloxSecurity]
SuperSafeChatReplicate: bool [Read:LocalUserSecurity] [Write:LocalUserSecurity]
Team: Team
TeamColor: BrickColor
Teleported: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
TeleportedIn: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ThirdPartyTextChatRestrictionStatus: ChatRestrictionStatus [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
UnfilteredChat: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
UserId: int64
VRDevice: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
VREnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
userId: int64 [Deprecated]
```

### Functions
```
AddReplicationFocus(part: BasePart) → null
AddReplicationFocusPosition(center: Vector3, radius: int) → null [RobloxSecurity]
AddToBlockList(userIds: Array) → null [RobloxScriptSecurity]
ClearCharacterAppearance() → null
DistanceFromCharacter(point: Vector3) → float
GetData() → PlayerData
GetFriendStatus(player: Player) → FriendStatus [RobloxScriptSecurity]
GetGameSessionID() → string [RobloxSecurity]
GetJoinData() → Dictionary
GetMouse() → Mouse
GetNetworkPing() → float
GetUnder13() → bool [RobloxScriptSecurity]
HasAppearanceLoaded() → bool
IsVerified() → bool
Kick(message: string) → null
LoadBoolean(key: string) → bool [Deprecated]
LoadCharacterAppearance(assetInstance: Instance) → null [Deprecated]
LoadData() → null [LocalUserSecurity] [Deprecated]
LoadInstance(key: string) → Instance [Deprecated]
LoadNumber(key: string) → double [Deprecated]
LoadString(key: string) → string [Deprecated]
Move(walkDirection: Vector3, relativeToCamera: bool) → null
OverrideStreamingRadii(minRadius: int, targetRadius: int) → null [RobloxSecurity]
PinStreamingForInstance(instance: Instance, depth: int) → null [RobloxScriptSecurity]
RemoveCharacter() → null [LocalUserSecurity]
RemoveReplicationFocus(part: BasePart) → null
RemoveReplicationFocusPosition(center: Vector3, radius: int) → null [RobloxSecurity]
RequestFriendship(player: Player) → null [RobloxScriptSecurity]
RevokeFriendship(player: Player) → null [RobloxScriptSecurity]
SaveBoolean(key: string, value: bool) → null [Deprecated]
SaveData() → null [LocalUserSecurity] [Deprecated]
SaveInstance(key: string, value: Instance) → null [Deprecated]
SaveNumber(key: string, value: double) → null [Deprecated]
SaveString(key: string, value: string) → null [Deprecated]
SetAccountAge(accountAge: int) → null [PluginSecurity]
SetBlockListInitialized() → null [RobloxScriptSecurity]
SetCharacterAppearanceJson(jsonBlob: string) → null [RobloxScriptSecurity]
SetChatTranslationSettingsLocaleId(locale: string) → null [RobloxScriptSecurity]
SetExperienceSettingsLocaleId(locale: string) → null [RobloxScriptSecurity]
SetMembershipType(membershipType: MembershipType) → null [RobloxScriptSecurity]
SetModerationAccessKey(moderationAccessKey: string) → null [RobloxScriptSecurity]
SetSuperSafeChat(value: bool) → null [PluginSecurity]
SetUnder13(value: bool) → null [RobloxSecurity] [Deprecated]
UnpinStreamingForInstance(instance: Instance, depth: int) → null [RobloxScriptSecurity]
UpdatePlayerBlocked(userId: int64, blocked: bool) → null [RobloxScriptSecurity]
loadBoolean(key: string) → bool [Deprecated]
loadInstance(key: string) → Instance [Deprecated]
loadNumber(key: string) → double [Deprecated]
loadString(key: string) → string [Deprecated]
saveBoolean(key: string, value: bool) → null [Deprecated]
saveInstance(key: string, value: Instance) → null [Deprecated]
saveNumber(key: string, value: double) → null [Deprecated]
saveString(key: string, value: string) → null [Deprecated]
GetFriendsOnline(maxFriends: int) → Array
GetRankInGroup(groupId: int64) → int
GetRoleInGroup(groupId: int64) → string
IsBestFriendsWith(userId: int64) → bool [Deprecated]
IsFriendsWith(userId: int64) → bool
IsInGroup(groupId: int64) → bool
LoadCharacter() → null
LoadCharacterBlocking() → null [LocalUserSecurity]
LoadCharacterWithAvatarRules(avatarRules: AvatarRules) → null [RobloxScriptSecurity]
LoadCharacterWithHumanoidDescription(humanoidDescription: HumanoidDescription) → null
RequestStreamAroundAsync(position: Vector3, timeOut: double) → null
WaitForDataReady() → bool [Deprecated]
isFriendsWith(userId: int64) → bool [Deprecated]
waitForDataReady() → bool [Deprecated]
```

### Events
```
CharacterAdded(character: Model)
CharacterAppearanceLoaded(character: Model)
CharacterRemoving(character: Model)
Chatted(message: string, recipient: Player)
CloudEditSelectionChanged(newSelection: Array) [RobloxScriptSecurity]
ConnectDiedSignalBackend() [RobloxSecurity]
FriendStatusChanged(player: Player, friendStatus: FriendStatus) [RobloxScriptSecurity]
Idled(time: double)
Kill() [LocalUserSecurity]
NotifyStreamingUnpinned(instance: Instance, depth: int) [RobloxSecurity]
OnTeleport(teleportState: TeleportState, placeId: int64, spawnName: string)
OnTeleportInternal(teleportState: TeleportState, teleportInfo: Dictionary, customLoadingScreen: Instance) [RobloxSecurity]
OverrideStreamRadii(minRadius: int, targetRadius: int) [RobloxSecurity]
PlayerCharacterLoaded(metrics: Dictionary) [RobloxSecurity]
PlayerChatTranslationSettingsLocaleSetFromLua(newLocaleId: string) [RobloxSecurity]
PlayerExperienceSettingsLocaleSetFromLua(newLocaleId: string) [RobloxSecurity]
RemoteFriendRequestSignal(otherUserId: int64, eventType: FriendRequestEvent) [RobloxScriptSecurity]
RemoteInsert(url: string, position: Vector3) [LocalUserSecurity]
RequestStreamingPin(instance: Instance, depth: int) [RobloxSecurity]
ScopeCheckInitiated(guid: string, serializedScopes: Array, metadata: Dictionary) [RobloxSecurity]
ScriptSecurityError(hash: string, error: string, stack: string) [LocalUserSecurity]
ServerToClientUnfilteredChatReplicate(value: bool) [RobloxSecurity]
ServerUpdatedHead(assetType: AssetType, assetId: int64) [RobloxSecurity]
SetShutdownMessage(message: string) [RobloxSecurity]
SimulationRadiusChanged(radius: float) [LocalUserSecurity]
StatsAvailable(info: string) [LocalUserSecurity]
StreamingPinComplete(instance: Instance) [RobloxScriptSecurity]
UnpinStreaming(instance: Instance, depth: int) [RobloxSecurity]
```

---

## PlayerData
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
GetPlayer() → Player
GetRecordAsync(recordName: string) → PlayerDataRecord
```

---

## PlayerDataRecord
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
CreatedTime: int64 = 0 [ReadOnly]
DefaultRecordName: bool = true [ReadOnly]
Dirty: bool = false [ReadOnly]
Error: PlayerDataErrorState = None [ReadOnly]
FlushedTime: int64 = 0 [ReadOnly]
LoadedTime: int64 = 0 [ReadOnly]
ModifiedTime: int64 = 0 [ReadOnly]
NewRecord: bool = false [ReadOnly]
Readable: bool = false [ReadOnly]
RecordName: string = Default [ReadOnly]
Writable: bool = false [ReadOnly]
```

### Functions
```
GetPlayer() → Player
GetValue(key: string) → Variant
GetValueChangedSignal(key: string) → RBXScriptSignal
RemoveValue(key: string) → null
SetValue(key: string, value: Variant) → null
ReleaseAsync() → null
RequestFlushAsync() → null
```

### Events
```
Changed(key: string, value: Variant)
Flushed(flushState: bool, error: string?)
Loaded(success: bool, error: string?)
```

---

## PlayerDataRecordConfig
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
RecordName: string [ReadOnly]
```

### Functions
```
GetDefaultValue(key: string) → Variant
SetDefaultValue(key: string, value: Variant) → null
```

---

## PlayerDataService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
LoadFailureBehavior: PlayerDataLoadFailureBehavior = Failure
```

### Functions
```
GetRecordConfig(recordName: string) → PlayerDataRecordConfig
```

---

## PlayerEmulatorService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
CustomPoliciesEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
EmulatedCountryCode: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
EmulatedGameLocale: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
PlayerEmulationEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
PseudolocalizationEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
SerializedEmulatedPolicyInfo: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
TextElongationFactor: int = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
GetEmulatedPolicyInfo() → Dictionary [RobloxScriptSecurity]
RegionCodeWillHaveAutomaticNonCustomPolicies(regionCode: string) → bool [RobloxScriptSecurity]
SetEmulatedPolicyInfo(emulatedPolicyInfo: Dictionary) → null [RobloxScriptSecurity]
```

---

## PlayerHydrationService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Events
```
PlayerHydration(userId: int64, playerHydrationBlob: string, playerHydrationSignature: string) [RobloxSecurity]
```

---

## PlayerScripts
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
ClearComputerCameraMovementModes() → null
ClearComputerMovementModes() → null
ClearTouchCameraMovementModes() → null
ClearTouchMovementModes() → null
GetRegisteredComputerCameraMovementModes() → Array [RobloxScriptSecurity]
GetRegisteredComputerMovementModes() → Array [RobloxScriptSecurity]
GetRegisteredTouchCameraMovementModes() → Array [RobloxScriptSecurity]
GetRegisteredTouchMovementModes() → Array [RobloxScriptSecurity]
RegisterComputerCameraMovementMode(cameraMovementMode: ComputerCameraMovementMode) → null
RegisterComputerMovementMode(movementMode: ComputerMovementMode) → null
RegisterTouchCameraMovementMode(cameraMovementMode: TouchCameraMovementMode) → null
RegisterTouchMovementMode(movementMode: TouchMovementMode) → null
```

### Events
```
ComputerCameraMovementModeRegistered() [RobloxScriptSecurity]
ComputerMovementModeRegistered() [RobloxScriptSecurity]
TouchCameraMovementModeRegistered() [RobloxScriptSecurity]
TouchMovementModeRegistered() [RobloxScriptSecurity]
```

---

## PlayerViewService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetDeviceCameraCFrame(player: Player) → CFrame
GetDeviceCameraCFrameForSelfView() → CFrame [RobloxScriptSecurity]
OnCameraCFrameReplicationRequest() → null [RobloxScriptSecurity]
UpdateDeviceCFrame(player: Player, cframe: CFrame, timestamp: int64) → null [RobloxScriptSecurity]
```

---

## Players
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
BanningEnabled: bool
BubbleChat: bool [ReadOnly]
CharacterAutoLoads: bool
ClassicChat: bool [ReadOnly]
LocalPlayer: Player [ReadOnly]
MaxPlayers: int [ReadOnly]
MaxPlayersInternal: int [Read:LocalUserSecurity] [Write:LocalUserSecurity]
NumPlayers: int [ReadOnly] [Deprecated]
PreferredPlayers: int [ReadOnly]
PreferredPlayersInternal: int [Read:LocalUserSecurity] [Write:LocalUserSecurity]
RespawnTime: float
ServerGitHash: string [Read:RobloxSecurity] [Write:RobloxSecurity]
ServerLogPrefix: string [Read:RobloxSecurity] [Write:RobloxSecurity]
UseStrafingAnimations: bool
localPlayer: Player [ReadOnly] [Deprecated]
numPlayers: int [ReadOnly] [Deprecated]
```

### Functions
```
Chat(message: string) → null [PluginSecurity]
CreateLocalPlayer() → Player [LocalUserSecurity]
GetPlayerByUserId(userId: int64) → Player
GetPlayerFromCharacter(character: Model) → Player
GetPlayers() → Instances
ReportAbuse(player: Player, reason: string, optionalMessage: string) → null [LocalUserSecurity]
ReportAbuseV3(player: Player, jsonTags: string) → null [RobloxScriptSecurity]
ReportChatAbuse(eligibleChatLines: Array, targetChatLines: Array, tags: Dictionary) → null [RobloxScriptSecurity]
ResetLocalPlayer() → null [LocalUserSecurity]
SetChatStyle(style: ChatStyle) → null [PluginSecurity]
SetLocalPlayerInfo(userId: int64, userName: string, displayName: string, membershipType: MembershipType, isUnder13: bool) → null [RobloxScriptSecurity]
TeamChat(message: string) → null [PluginSecurity]
WhisperChat(message: string, player: Instance) → null [LocalUserSecurity]
getPlayers() → Instances [Deprecated]
playerFromCharacter(character: Model) → Player [Deprecated]
players() → Instances [Deprecated]
BanAsync(config: Dictionary) → null
CreateHumanoidModelFromDescription(description: HumanoidDescription, rigType: HumanoidRigType, assetTypeVerification: AssetTypeVerification) → Model
CreateHumanoidModelFromUserId(userId: int64) → Model
GetBanHistoryAsync(userId: int64) → BanHistoryPages
GetCharacterAppearanceAsync(userId: int64) → Model [Deprecated]
GetCharacterAppearanceInfoAsync(userId: int64) → Dictionary
GetFriendsAsync(userId: int64) → FriendPages
GetHumanoidDescriptionFromOutfitId(outfitId: int64) → HumanoidDescription
GetHumanoidDescriptionFromUserId(userId: int64) → HumanoidDescription
GetNameFromUserIdAsync(userId: int64) → string
GetUserIdFromNameAsync(userName: string) → int64
GetUserThumbnailAsync(userId: int64, thumbnailType: ThumbnailType, thumbnailSize: ThumbnailSize) → Tuple
UnbanAsync(config: Dictionary) → null
```

### Events
```
CloudEditApplyEditsMessage(playerName: string, scriptName: string) [RobloxSecurity]
FriendRequestEvent(player: Player, player: Player, friendRequestEvent: FriendRequestEvent) [RobloxScriptSecurity]
GameAnnounce(message: string) [RobloxScriptSecurity]
PlayerAdded(player: Player)
PlayerChatted(chatType: PlayerChatType, player: Player, message: string, targetPlayer: Player) [LocalUserSecurity]
PlayerConnecting(player: Player) [LocalUserSecurity]
PlayerDisconnecting(player: Player) [LocalUserSecurity]
PlayerMembershipChanged(player: Player)
PlayerRejoining(player: Player) [LocalUserSecurity]
PlayerRemoving(player: Player)
PromptGameServerReportEnrichment(reportId: string) [RobloxSecurity]
PromptGameServerTargetedChatReportEnrichment(reportId: string, eligibleChatLines: Array, targetChatLines: Array) [RobloxSecurity]
PromptReportServerEnrichmentAndScan(v1comment: string, submitterId: int64, abuserId: int64, reportId: string) [RobloxSecurity]
RequestCloudEditImmediatePublishWithContext(spanContext: string) [RobloxSecurity]
RequestCloudEditKick(playerId: int64) [RobloxSecurity]
RequestCloudEditShutdown() [RobloxSecurity]
RequestTeamCreateImmediateSaveWithContext(spanContext: string) [RobloxSecurity]
TeamCreatePublishFinished(publishSuccessful: bool) [RobloxSecurity]
TeamCreateSaveFinished(saveSuccessful: bool) [RobloxSecurity]
TeamCreateServerMessage(messageType: MessageType, message: string, printToStatusBar: bool) [RobloxSecurity]
UserSubscriptionStatusChanged(user: Player, subscriptionId: string)
```

---

## Plugin
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
CollisionEnabled: bool [ReadOnly]
DisableUIDragDetectorDrags: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GridSize: float [ReadOnly]
HostDataModelType: StudioDataModelType [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
HostDataModelTypeIsCurrent: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
IsDebuggable: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
MultipleDocumentInterfaceInstance: MultipleDocumentInterfaceInstance [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
UsesAssetInsertionDrag: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
Activate(exclusiveMouse: bool) → null [PluginSecurity]
CreatePluginAction(actionId: string, text: string, statusTip: string, iconName: string, allowBinding: bool) → PluginAction [PluginSecurity]
CreatePluginMenu(id: string, title: string, icon: string) → PluginMenu [PluginSecurity]
CreateToolbar(name: string) → PluginToolbar [PluginSecurity]
Deactivate() → null [PluginSecurity]
GetItem(key: string, defaultValue: Variant) → Variant [RobloxScriptSecurity]
GetJoinMode() → JointCreationMode [PluginSecurity]
GetMouse() → PluginMouse [PluginSecurity]
GetPluginComponent(name: string) → Variant [RobloxScriptSecurity]
GetSelectedRibbonTool() → RibbonTool [PluginSecurity]
GetSetting(key: string) → Variant [PluginSecurity]
GetStudioUserId() → int64 [PluginSecurity] [Deprecated]
GetUri() → Dictionary [RobloxScriptSecurity]
Intersect(objects: Instances) → Instance [PluginSecurity]
Invoke(key: string, arguments: Tuple) → null [RobloxScriptSecurity]
IsActivated() → bool [PluginSecurity]
IsActivatedWithExclusiveMouse() → bool [PluginSecurity]
IsLoadedFromProject() → bool [RobloxScriptSecurity]
Negate(objects: Instances) → Instances [PluginSecurity]
OnInvoke(key: string, callback: Function) → Instance [RobloxScriptSecurity]
OnInvokeSuspendOverride(key: string, callback: Function) → Instance [RobloxScriptSecurity]
OnSetItem(key: string, callback: Function) → Instance [RobloxScriptSecurity]
OpenScript(script: LuaSourceContainer, lineNumber: int) → null [PluginSecurity]
OpenWikiPage(url: string) → null [PluginSecurity]
PauseSound(sound: Instance) → null [RobloxScriptSecurity]
PlaySound(sound: Instance, normalizedTimePosition: double) → null [RobloxScriptSecurity]
ResumeSound(sound: Instance) → null [RobloxScriptSecurity]
SaveSelectedToRoblox() → null [PluginSecurity]
SelectRibbonTool(tool: RibbonTool, position: UDim2) → null [PluginSecurity]
Separate(objects: Instances) → Instances [PluginSecurity]
SetItem(key: string, value: Variant) → null [RobloxScriptSecurity]
SetReady() → null [RobloxScriptSecurity]
SetSetting(key: string, value: Variant) → null [PluginSecurity]
StartDecalDrag(decal: Instance) → null [RobloxScriptSecurity]
StartDrag(dragData: Dictionary) → null [PluginSecurity]
StopAllSounds() → null [RobloxScriptSecurity]
Union(objects: Instances) → Instance [PluginSecurity]
CreateDockWidgetPluginGui(pluginGuiId: string, dockWidgetPluginGuiInfo: DockWidgetPluginGuiInfo) → DockWidgetPluginGui [PluginSecurity]
CreateQWidgetPluginGui(pluginGuiId: string, pluginGuiOptions: Dictionary) → QWidgetPluginGui [RobloxScriptSecurity]
ImportFbxAnimation(rigModel: Instance, isR15: bool) → Instance [PluginSecurity]
ImportFbxRig(isR15: bool) → Instance [PluginSecurity]
PromptForExistingAssetId(assetType: string) → int64 [PluginSecurity]
PromptSaveSelection(suggestedFileName: string) → bool [PluginSecurity]
```

### Events
```
Deactivation() [PluginSecurity]
Ready() [RobloxScriptSecurity]
Unloading() [PluginSecurity]
```

---

## PluginAction
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
ActionId: string [ReadOnly]
AllowBinding: bool = true [ReadOnly]
Checked: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DefaultShortcut: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Enabled: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
StatusTip: string [ReadOnly]
Text: string [Write:RobloxScriptSecurity]
```

### Events
```
Triggered() [PluginSecurity]
```

---

## PluginCapabilities
**Extends:** Instance

### Properties
```
Manifest: string = {"Metadata":{"TargetDataModels": ["Edit", "Server", "Client"]},"Permissions":{}} [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

---

## PluginDebugService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## PluginDragEvent
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
Data: string [ReadOnly]
MimeType: string [ReadOnly]
Position: Vector2 [ReadOnly]
Sender: string [ReadOnly]
```

---

## PluginGuiService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## PluginManagementService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
SetAutoUpdate(pluginId: int64, state: bool) → null [RobloxScriptSecurity]
GetOTAPluginVersion(pluginName: string) → int64 [RobloxScriptSecurity]
```

---

## PluginManager
**Extends:** Instance
**Tags:** NotCreatable

### Functions
```
CreatePlugin() → Instance [PluginSecurity] [Deprecated]
ExportPlace(filePath: string) → null [PluginSecurity]
ExportSelection(filePath: string) → null [PluginSecurity]
```

---

## PluginManagerInterface
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
CreatePlugin() → Instance [PluginSecurity] [Deprecated]
ExportPlace(filePath: string) → null [PluginSecurity]
ExportSelection(filePath: string) → null [PluginSecurity]
```

---

## PluginMenu
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
Icon: string
Title: string
```

### Functions
```
AddAction(action: Instance) → null [PluginSecurity]
AddMenu(menu: Instance) → null [PluginSecurity]
AddNewAction(actionId: string, text: string, icon: string) → Instance [PluginSecurity]
AddSeparator() → null [PluginSecurity]
Clear() → null [PluginSecurity]
ShowAsync() → Instance [PluginSecurity]
```

---

## PluginPolicyService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetPluginPolicy(pluginName: string) → Dictionary [RobloxScriptSecurity]
```

---

## PluginToolbar
**Extends:** Instance
**Tags:** NotCreatable

### Functions
```
CreateButton(buttonId: string, tooltip: string, iconname: string, text: string) → PluginToolbarButton [PluginSecurity]
CreatePopupButton(buttonId: string, tooltip: string, iconname: string, text: string) → PluginToolbarButton [RobloxScriptSecurity]
```

---

## PluginToolbarButton
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
ClickableWhenViewportHidden: bool
Enabled: bool
Icon: ContentId
```

### Functions
```
SetActive(active: bool) → null [PluginSecurity]
SetDropdownActive(active: bool) → null [RobloxScriptSecurity]
```

### Events
```
Click() [PluginSecurity]
DropdownClick() [RobloxScriptSecurity]
```

---

## PointsService
**Extends:** Instance
**Tags:** NotCreatable, Service, Deprecated

### Functions
```
GetAwardablePoints() → int [Deprecated]
AwardPoints(userId: int64, amount: int) → Tuple [Deprecated]
GetGamePointBalance(userId: int64) → int [Deprecated]
GetPointBalance(userId: int64) → int [Deprecated]
```

### Events
```
PointsAwarded(userId: int64, pointsAwarded: int, userBalanceInGame: int, userTotalBalance: int)
```

---

## PolicyService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
IsLuobuServer: TriStateBoolean = Unknown [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LuobuWhitelisted: TriStateBoolean = Unknown [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
CanViewBrandProjectAsync(player: Player, brandProjectId: string) → bool
GetPolicyInfoForPlayerAsync(player: Instance) → Dictionary
GetPolicyInfoForServerRobloxOnlyAsync() → Dictionary [RobloxScriptSecurity]
```

---

## PoseBase
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
EasingDirection: PoseEasingDirection
EasingStyle: PoseEasingStyle
Weight: float
```

---

## NumberPose
**Extends:** PoseBase

### Properties
```
Value: double = 0
```

---

## Pose
**Extends:** PoseBase

### Properties
```
CFrame: CFrame
MaskWeight: float = 0 [Deprecated]
```

### Functions
```
AddSubPose(pose: Instance) → null
GetSubPoses() → Instances
RemoveSubPose(pose: Instance) → null
```

---

## PostEffect
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
Enabled: bool
```

---

## BloomEffect
**Extends:** PostEffect

### Properties
```
Intensity: float = 0.400000006
Size: float = 24
Threshold: float = 0.949999988
```

---

## BlurEffect
**Extends:** PostEffect

### Properties
```
Size: float = 24
```

---

## ColorCorrectionEffect
**Extends:** PostEffect

### Properties
```
Brightness: float = 0
Contrast: float = 0
Saturation: float = 0
TintColor: Color3 = 1, 1, 1
```

---

## ColorGradingEffect
**Extends:** PostEffect

### Properties
```
TonemapperPreset: TonemapperPreset = Default
```

---

## DepthOfFieldEffect
**Extends:** PostEffect

### Properties
```
FarIntensity: float = 0.75
FocusDistance: float = 0.0500000007
InFocusRadius: float = 10
NearIntensity: float = 0.75
```

---

## SunRaysEffect
**Extends:** PostEffect

### Properties
```
Intensity: float = 0.25
Spread: float = 1
```

---

## ProcessInstancePhysicsService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## ProximityPrompt
**Extends:** Instance

### Properties
```
ActionText: string = Interact
AutoLocalize: bool = true
ClickablePrompt: bool = true
Enabled: bool = true
Exclusivity: ProximityPromptExclusivity = OnePerButton
GamepadKeyCode: KeyCode = ButtonX
HoldDuration: float = 0
KeyboardKeyCode: KeyCode = E
MaxActivationDistance: float = 10
MaxIndicatorDistance: float = 0
ObjectText: string
RequiresLineOfSight: bool = true
RootLocalizationTable: LocalizationTable
Style: ProximityPromptStyle = Default
UIOffset: Vector2 = 0, 0
```

### Functions
```
InputHoldBegin() → null
InputHoldEnd() → null
```

### Events
```
ButtonHoldBeganActionReplicated(player: Player) [RobloxSecurity]
ButtonHoldEndedActionReplicated(player: Player) [RobloxSecurity]
IndicatorHidden()
IndicatorShown()
PromptButtonHoldBegan(playerWhoTriggered: Player)
PromptButtonHoldEnded(playerWhoTriggered: Player)
PromptHidden()
PromptShown(inputType: ProximityPromptInputType)
TriggerEnded(playerWhoTriggered: Player)
TriggerEndedActionReplicated(player: Player) [RobloxSecurity]
Triggered(playerWhoTriggered: Player)
TriggeredActionReplicated(player: Instance) [RobloxSecurity]
```

---

## ProximityPromptService
**Extends:** Instance
**Tags:** Service, NotBrowsable

### Properties
```
Enabled: bool = true
MaxIndicatorsVisible: int = 16
MaxPromptsVisible: int = 16
```

### Events
```
IndicatorHidden(prompt: ProximityPrompt)
IndicatorShown(prompt: ProximityPrompt)
PromptButtonHoldBegan(prompt: ProximityPrompt, playerWhoTriggered: Player)
PromptButtonHoldEnded(prompt: ProximityPrompt, playerWhoTriggered: Player)
PromptHidden(prompt: ProximityPrompt)
PromptShown(prompt: ProximityPrompt, inputType: ProximityPromptInputType)
PromptTriggerEnded(prompt: ProximityPrompt, playerWhoTriggered: Player)
PromptTriggered(prompt: ProximityPrompt, playerWhoTriggered: Player)
```

---

## PublishService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
PublishDescendantAssets(instance: Instance) → bool [RobloxScriptSecurity]
CreateAssetAndWaitForAssetId(instances: Instances, operationId: string, creatorType: AssetCreatorType, creatorId: int64, assetType: string, name: string, description: string, expectedPrice: int) → int64 [RobloxScriptSecurity]
CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsync(serializedInstance: string, creatorType: AssetCreatorType, creatorId: int64, assetType: string, assetId: int64, name: string, description: string, token: string, contentType: string, expectedPrice: int) → Dictionary [RobloxScriptSecurity]
CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsyncWithAddParam(serializedInstance: string, publishInfo: Dictionary) → Dictionary [RobloxScriptSecurity]
CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsyncWithAddParamErrorJson(serializedInstance: string, publishInfo: Dictionary) → Dictionary [RobloxScriptSecurity]
PublishCageMeshAsync(wrap: Instance, cageType: CageType) → ContentId [RobloxScriptSecurity]
PublishDescendantAssetsAsync(instance: Instance) → bool [RobloxScriptSecurity]
```

---

## RTAnimationTracker
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
Active: bool = false
EnableFallbackAudioInput: bool = false
SessionName: string
TrackerMode: TrackerMode = None [ReadOnly]
TrackerType: TrackerType = Face
```

### Functions
```
Step() → null [RobloxScriptSecurity]
```

### Events
```
TrackerError(errorCode: TrackerError, msg: string)
TrackerPrompt(prompt: TrackerPromptEvent)
```

---

## RbxAnalyticsService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
AddGlobalPointsField(key: string, value: int) → null [RobloxScriptSecurity]
AddGlobalPointsTag(key: string, value: string) → null [RobloxScriptSecurity]
DEPRECATED_TrackEvent(category: string, action: string, label: string, value: int64) → null [RobloxScriptSecurity]
DEPRECATED_TrackEventWithArgs(category: string, action: string, label: string, args: Dictionary, value: int64) → null [RobloxScriptSecurity]
GetClientId() → string [RobloxScriptSecurity]
GetPlaySessionId() → string [RobloxScriptSecurity]
GetSessionId() → string [RobloxScriptSecurity]
ReleaseRBXEventStream(target: string) → null [RobloxScriptSecurity]
RemoveGlobalPointsField(key: string) → null [RobloxScriptSecurity]
RemoveGlobalPointsTag(key: string) → null [RobloxScriptSecurity]
ReportCounter(counterName: string, amount: int) → null [RobloxScriptSecurity]
ReportInfluxSeries(seriesName: string, points: Dictionary, throttlingPercentage: int) → null [RobloxScriptSecurity]
ReportStats(category: string, value: float) → null [RobloxScriptSecurity]
ReportToDiagByCountryCode(featureName: string, measureName: string, seconds: double) → null [RobloxScriptSecurity]
SendEventDeferred(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null [RobloxScriptSecurity]
SendEventImmediately(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null [RobloxScriptSecurity]
SetRBXEvent(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null [RobloxScriptSecurity]
SetRBXEventStream(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null [RobloxScriptSecurity]
TrackEvent(category: string, action: string, label: string, value: int64) → null [RobloxScriptSecurity]
TrackEventWithArgs(category: string, action: string, label: string, args: Dictionary, value: int64) → null [RobloxScriptSecurity]
UpdateHeartbeatObject(args: Dictionary) → null [RobloxScriptSecurity]
```

---

## RecommendationService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
LogActionEvent(actionType: RecommendationActionType, itemId: string, tracingId: string, actionEventDetails: Dictionary) → null
LogImpressionEvent(impressionType: RecommendationImpressionType, itemId: string, tracingId: string, impressionEventDetails: Dictionary) → null
GenerateItemListAsync(generateRecommendationItemListRequest: Dictionary) → RecommendationPages
RegisterItemAsync(player: Player, registerRecommendationItemsRequest: Dictionary) → Dictionary
RemoveItemAsync(itemId: string) → null
UpdateItemAsync(updateRecommendationItemRequest: Dictionary) → null
```

---

## ReflectionMetadata
**Extends:** Instance

---

## ReflectionMetadataCallbacks
**Extends:** Instance

---

## ReflectionMetadataClasses
**Extends:** Instance

---

## ReflectionMetadataEnums
**Extends:** Instance

---

## ReflectionMetadataEvents
**Extends:** Instance

---

## ReflectionMetadataFunctions
**Extends:** Instance

---

## ReflectionMetadataItem
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
Browsable: bool
ClassCategory: string
ClientOnly: bool
Constraint: string
Deprecated: bool
EditingDisabled: bool
EditorType: string
FFlag: string
IsBackend: bool
PropertyOrder: int
ScriptContext: string
ServerOnly: bool
SliderScaling: string
UIMaximum: double
UIMinimum: double
UINumTicks: double
```

---

## ReflectionMetadataClass
**Extends:** ReflectionMetadataItem

### Properties
```
ExplorerImageIndex: int = 0
ExplorerOrder: int = 2147483647
Insertable: bool = true
PreferredParent: string
ServiceVisibility: ServiceVisibility = Always [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## ReflectionMetadataEnum
**Extends:** ReflectionMetadataItem

---

## ReflectionMetadataEnumItem
**Extends:** ReflectionMetadataItem

---

## ReflectionMetadataMember
**Extends:** ReflectionMetadataItem

---

## ReflectionMetadataProperties
**Extends:** Instance

---

## ReflectionMetadataYieldFunctions
**Extends:** Instance

---

## ReflectionService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetClass(className: string, filter: Dictionary) → Dictionary?
GetClasses(filter: Dictionary) → Array
GetPropertiesOfClass(className: string, filter: Dictionary) → Array
GetPropertyNames(name: string) → Array [RobloxScriptSecurity]
GetStyledPropertyNames(name: string) → Array [RobloxScriptSecurity]
```

---

## RemoteCursorService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Events
```
BroadcastRemoteCursorPositions(script: string, remoteCursorPosition: string) [RobloxSecurity]
RequestAllRemoteCursorPositionForScript(script: string) [RobloxSecurity]
UpdateClientRemoteCursorPosition(script: string, remoteCursorPosition: string) [RobloxSecurity]
```

---

## RemoteDebuggerServer
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## RemoteFunction
**Extends:** Instance

### Functions
```
InvokeClient(player: Player, arguments: Tuple) → Tuple
InvokeServer(arguments: Tuple) → Tuple
```

### Events
```
RemoteOnInvokeClient(id: int, arguments: Tuple)
RemoteOnInvokeError(id: int, arguments: string)
RemoteOnInvokeServer(id: int, player: Player, arguments: Tuple)
RemoteOnInvokeSuccess(id: int, arguments: Tuple)
```

---

## RenderSettings
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated, NotBrowsable

### Properties
```
AutoFRMLevel: int
EagerBulkExecution: bool
EditQualityLevel: QualityLevel
Enable VR Mode: bool
EnableFRM: bool
ExportMergeByMaterial: bool
FrameRateManager: FramerateManagerMode
GraphicsMode: GraphicsMode
MeshCacheSize: int
MeshPartDetailLevel: MeshPartDetailLevel
QualityLevel: QualityLevel
ReloadAssets: bool
RenderCSGTrianglesDebug: bool
ShowBoundingBoxes: bool
ViewMode: ViewMode
```

### Functions
```
GetMaxQualityLevel() → int
```

---

## RenderingTest
**Extends:** Instance

### Properties
```
CFrame: CFrame
ComparisonDiffThreshold: int = 10
ComparisonMethod: RenderingTestComparisonMethod = psnr
ComparisonPsnrThreshold: float = 50
Description: string
FieldOfView: float = 70
Orientation: Vector3 = -0, 0, 0
PerfTest: bool = false
Position: Vector3 = 0, 0, 0
QualityAuto: bool = false
QualityLevel: int = 21
RenderingTestFrameCount: int = 20
ShouldSkip: bool = false
Ticket: string
Timeout: int = 30
```

### Functions
```
RenderdocTriggerCapture() → null
```

---

## ReplicatedFirst
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
IsDefaultLoadingGuiRemoved() → bool [RobloxScriptSecurity]
IsFinishedReplicating() → bool [RobloxScriptSecurity]
RemoveDefaultLoadingScreen() → null
SetDefaultLoadingGuiRemoved() → null [RobloxScriptSecurity]
```

### Events
```
DefaultLoadingGuiRemoved() [RobloxScriptSecurity]
FinishedReplicating() [RobloxScriptSecurity]
RemoveDefaultLoadingGuiSignal() [RobloxScriptSecurity]
```

---

## ReplicatedStorage
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## RibbonNotificationService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
OnNotificationUpdateFromPlugin(newNotificationId: string, seenNotificationId: string) → null [RobloxScriptSecurity]
```

### Events
```
AllNotificationsReadFromRibbon() [RobloxScriptSecurity]
NewNotificationFromRibbon(newNotificationId: string) [RobloxScriptSecurity]
NotificationReadFromRibbon(newNotificationId: string) [RobloxScriptSecurity]
ToggleNotificationTray(checked: bool, newNotificationAvailable: bool) [RobloxScriptSecurity]
```

---

## RobloxPluginGuiService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## RobloxReplicatedStorage
**Extends:** Instance
**Tags:** NotCreatable, Service, NotBrowsable

---

## RobloxSerializableInstance
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
Data: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## RobloxServerStorage
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## RomarkRbxAnalyticsService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## RomarkService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
EndRemoteRomarkTest() → null
```

### Events
```
RomarkEndOfTest() [RobloxScriptSecurity]
```

---

## RotationCurve
**Extends:** Instance

### Properties
```
Length: int = 0 [ReadOnly]
ValuesAndTimes: BinaryString = 
```

### Functions
```
GetKeyAtIndex(index: int) → RotationCurveKey
GetKeyIndicesAtTime(time: float) → Array
GetKeys() → Array
GetValueAtTime(time: float) → CoordinateFrame?
InsertKey(key: RotationCurveKey) → Array
RemoveKeyAtIndex(startingIndex: int, count: int) → int
SetKeys(keys: Array) → int
```

---

## RtMessagingService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## RunService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
ClientGitHash: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
RunState: RunState [Read:PluginSecurity] [Write:PluginSecurity]
```

### Functions
```
BindToRenderStep(name: string, priority: int, function: Function) → null
GetCoreScriptVersion() → string [RobloxScriptSecurity]
GetRobloxClientChannel() → string [RobloxScriptSecurity]
GetRobloxGuiFocused() → bool [RobloxScriptSecurity]
GetRobloxVersion() → string [RobloxScriptSecurity]
IsClient() → bool
IsEdit() → bool [PluginSecurity]
IsRunMode() → bool
IsRunning() → bool
IsServer() → bool
IsStudio() → bool
Pause() → null [PluginSecurity]
Reset() → null [PluginSecurity] [Deprecated]
Run() → null [PluginSecurity]
Set3dRenderingEnabled(enable: bool) → null [RobloxScriptSecurity]
SetRobloxGuiFocused(focus: bool) → null [RobloxScriptSecurity]
Stop() → null [PluginSecurity]
UnbindFromRenderStep(name: string) → null
setThrottleFramerateEnabled(enable: bool) → null [RobloxScriptSecurity]
```

### Events
```
Heartbeat(deltaTime: double)
PostSimulation(deltaTimeSim: double)
PreAnimation(deltaTimeSim: double)
PreRender(deltaTimeRender: double)
PreSimulation(deltaTimeSim: double)
RenderStepped(deltaTime: double)
RobloxGuiFocusedChanged(isRobloxGuiFocused: bool) [RobloxScriptSecurity]
Stepped(time: double, deltaTime: double)
```

---

## RuntimeScriptService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## SafetyService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
IsCaptureModeForReport: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
DecodeAvatarMovementProto(avatarMovementProtoString: string) → Dictionary [RobloxScriptSecurity]
ReportMenuTabClose() → null [RobloxScriptSecurity]
ReportMenuTabOpen() → null [RobloxScriptSecurity]
TakeScreenshot(screenshotOptions: Dictionary) → int64 [RobloxScriptSecurity]
```

### Events
```
FSTriggeredSignal(requestId: string, playerId: int64, mac: string, args: Tuple) [RobloxSecurity]
ScreenshotContentReady(screenshotJobId: int64, contentId: ContentId) [RobloxScriptSecurity]
ScreenshotUploaded(screenshotJobId: int64, screenshotId: string) [RobloxScriptSecurity]
```

---

## ScreenshotHud
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
CameraButtonIcon: ContentId
CameraButtonPosition: UDim2
CloseButtonPosition: UDim2
CloseWhenScreenshotTaken: bool
ExperienceNameOverlayEnabled: bool [Deprecated]
HideCoreGuiForCaptures: bool
HidePlayerGuiForCaptures: bool
OverlayFont: Font [Deprecated]
UsernameOverlayEnabled: bool [Deprecated]
Visible: bool
```

---

## ScriptBuilder
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

---

## SyncScriptBuilder
**Extends:** ScriptBuilder
**Tags:** NotCreatable, NotReplicated

### Properties
```
CompileTarget: CompileTarget = CoreScript
CoverageInfo: bool = false
DebugInfo: bool = false
PackAsSource: bool = false
RawBytecode: bool = false [Deprecated]
```

---

## ScriptChangeService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Events
```
ScriptAdded(script: LuaSourceContainer) [RobloxScriptSecurity]
ScriptBeingRemoved(script: LuaSourceContainer) [RobloxScriptSecurity]
ScriptChanged(script: LuaSourceContainer, property: string) [RobloxScriptSecurity]
ScriptFullNameChanged(script: LuaSourceContainer) [RobloxScriptSecurity]
ScriptSourceChanged(script: LuaSourceContainer) [RobloxScriptSecurity]
```

---

## ScriptCloneWatcher
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## ScriptCloneWatcherHelper
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## ScriptCommitService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## ScriptContext
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
ScriptsDisabled: bool = false [Read:LocalUserSecurity] [Write:LocalUserSecurity]
```

### Functions
```
AddCoreScriptLocal(name: string, parent: Instance) → null [RobloxScriptSecurity]
CompressLuaApp() → null [RobloxScriptSecurity]
GetCoverageStats() → Array [RobloxScriptSecurity]
GetLuauHeapInstanceReferenceReport(target: string) → Dictionary [RobloxScriptSecurity]
GetLuauHeapMemoryReport(target: string) → Dictionary [RobloxScriptSecurity]
ReportLuaRequireCount() → null [RobloxScriptSecurity]
SetTimeout(seconds: double) → null [PluginSecurity]
```

### Events
```
Error(message: string, stackTrace: string, script: Instance)
ErrorDetailed(message: string, stackTrace: string, script: Instance, details: string, securityLevel: int, messageId: string) [RobloxScriptSecurity]
```

---

## ScriptDebugger
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
CoreScriptIdentifier: string
CurrentLine: int = 0 [ReadOnly]
IsDebugging: bool = false [ReadOnly]
IsPaused: bool = false [ReadOnly]
Script: Instance [ReadOnly]
ScriptGuid: string
```

### Functions
```
AddWatch(expression: string) → Instance
GetBreakpoints() → Instances
GetGlobals(stackFrame: int) → Map
GetLocals(stackFrame: int) → Map
GetStack() → Array
GetUpvalues(stackFrame: int) → Map
GetWatchValue(watch: Instance) → Variant
GetWatches() → Instances
SetBreakpoint(line: int, isContextDependentBreakpoint: bool) → Instance
SetGlobal(name: string, value: Variant, stackFrame: int) → null
SetLocal(name: string, value: Variant, stackFrame: int) → null
SetUpvalue(name: string, value: Variant, stackFrame: int) → null
```

### Events
```
BreakpointAdded(breakpoint: Instance)
BreakpointRemoved(breakpoint: Instance)
EncounteredBreak(line: int, breakReason: BreakReason)
Resuming()
WatchAdded(watch: Instance)
WatchRemoved(watch: Instance)
```

---

## ScriptDocument
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
GetInternalUri() → string [RobloxScriptSecurity]
GetLine(lineIndex: int?) → string [PluginSecurity]
GetLineCount() → int [PluginSecurity]
GetScript() → LuaSourceContainer [PluginSecurity]
GetSelectedText() → string [PluginSecurity]
GetSelection() → Tuple [PluginSecurity]
GetSelectionEnd() → Tuple [PluginSecurity]
GetSelectionStart() → Tuple [PluginSecurity]
GetText(startLine: int?, startCharacter: int?, endLine: int?, endCharacter: int?) → string [PluginSecurity]
GetViewport() → Tuple [PluginSecurity]
HasSelectedText() → bool [PluginSecurity]
IsCommandBar() → bool [PluginSecurity]
CloseAsync() → Tuple [PluginSecurity]
EditTextAsync(newText: string, startLine: int, startCharacter: int, endLine: int, endCharacter: int) → Tuple [PluginSecurity]
ForceSetSelectionAsync(cursorLine: int, cursorCharacter: int, anchorLine: int?, anchorCharacter: int?) → Tuple [PluginSecurity]
MultiEditTextAsync(edits: Array) → Tuple [PluginSecurity]
RequestSetSelectionAsync(cursorLine: int, cursorCharacter: int, anchorLine: int?, anchorCharacter: int?) → Tuple [PluginSecurity]
```

### Events
```
SelectionChanged(positionLine: int64, positionCharacter: int64, anchorLine: int64, anchorCharacter: int64) [PluginSecurity]
ViewportChanged(startLine: int64, endLine: int64) [PluginSecurity]
```

---

## ScriptEditorService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
DeregisterAutocompleteCallback(name: string) → null [PluginSecurity]
DeregisterScriptAnalysisCallback(name: string) → null [PluginSecurity]
FindScriptDocument(script: LuaSourceContainer) → ScriptDocument [PluginSecurity]
ForceReloadSource(uri: string, newsrc: string) → null [RobloxScriptSecurity]
GetEditorSource(script: LuaSourceContainer) → string [PluginSecurity]
GetScriptDocuments() → Instances [PluginSecurity]
IsAutocompleteCallbackRegistered(name: string) → bool [RobloxScriptSecurity]
IsScriptAnalysisCallbackRegistered(name: string) → bool [RobloxScriptSecurity]
RegisterAutocompleteCallback(name: string, priority: int, callbackFunction: Function) → null [PluginSecurity]
RegisterScriptAnalysisCallback(name: string, priority: int, callbackFunction: Function) → null [PluginSecurity]
StripComments(code: string) → string [RobloxScriptSecurity]
EditSourceAsyncWithRanges(script: LuaSourceContainer, newText: string, startLine: int, startCharacter: int, endLine: int, endCharacter: int) → Tuple [RobloxScriptSecurity]
OpenScriptDocumentAsync(script: LuaSourceContainer, options: Dictionary) → Tuple [PluginSecurity]
UpdateSourceAsync(script: LuaSourceContainer, callback: Function) → null [PluginSecurity]
```

### Events
```
TextDocumentDidChange(document: ScriptDocument, changesArray: Variant) [PluginSecurity]
TextDocumentDidClose(oldDocument: ScriptDocument) [PluginSecurity]
TextDocumentDidOpen(newDocument: ScriptDocument) [PluginSecurity]
```

---

## ScriptProfilerService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
ClientRequestData(player: Player) → null [PluginSecurity]
ClientStart(player: Player, frequency: int?) → null [PluginSecurity]
ClientStop(player: Player) → null [PluginSecurity]
DeserializeJSON(jsonString: string?) → Dictionary [PluginSecurity]
SaveScriptProfilingData(jsonString: string, filename: string) → string [RobloxScriptSecurity]
ServerRequestData() → null [PluginSecurity]
ServerStart(frequency: int?) → null [PluginSecurity]
ServerStop() → null [PluginSecurity]
```

### Events
```
OnNewData(player: Player, jsonString: string) [PluginSecurity]
RequestData() [RobloxSecurity]
SetProfilingState(start: bool, frequency: int) [RobloxSecurity]
```

---

## ScriptRegistrationService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetSourceContainerByScriptGuid(guid: string) → LuaSourceContainer [RobloxScriptSecurity]
```

---

## ScriptRuntime
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

---

## ScriptService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## Selection
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
ActiveInstance: Instance [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
RenderMode: SelectionRenderMode [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
SelectionBoxThickness: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
SelectionLineThickness: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
SelectionThickness: float [ReadOnly]
ShowActiveInstanceHighlight: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
Add(instancesToAdd: Instances) → null [PluginSecurity]
AddFocusCallback(priority: int, function: Function) → RBXScriptConnection [RobloxScriptSecurity]
ClearTerrainSelectionHack() → null [RobloxScriptSecurity]
Get() → Instances [PluginSecurity]
Remove(instancesToRemove: Instances) → null [PluginSecurity]
Set(selection: Instances) → null [PluginSecurity]
SetTerrainSelectionHack(center: Vector3, size: Vector3) → null [RobloxScriptSecurity]
```

### Events
```
SelectionChanged()
SelectionChangedThisFrame() [RobloxScriptSecurity]
```

---

## SelectionHighlightManager
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## SensorBase
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
UpdateType: SensorUpdateType
```

### Functions
```
Sense() → null [Deprecated]
```

### Events
```
OnSensorOutputChanged()
```

---

## AtmosphereSensor
**Extends:** SensorBase

### Properties
```
AirDensity: float = 0 [ReadOnly]
RelativeWindVelocity: Vector3 = 0, 0, 0 [ReadOnly]
```

---

## BuoyancySensor
**Extends:** SensorBase

### Properties
```
FullySubmerged: bool = false
TouchingSurface: bool = false
```

---

## ControllerSensor
**Extends:** SensorBase
**Tags:** NotCreatable

---

## ControllerPartSensor
**Extends:** ControllerSensor

### Properties
```
HitFrame: CFrame
HitNormal: Vector3 = 0, 0, 0
SearchDistance: float = 0
SensedPart: BasePart
SensorMode: SensorMode = Floor
```

---

## FluidForceSensor
**Extends:** SensorBase

### Properties
```
CenterOfPressure: Vector3 = 0, 0, 0 [ReadOnly]
Force: Vector3 = 0, 0, 0 [ReadOnly]
Torque: Vector3 = 0, 0, 0 [ReadOnly]
```

### Functions
```
EvaluateAsync(linearVelocity: Vector3, angularVelocity: Vector3, cframe: CFrame) → Tuple
```

---

## SerializationService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
DeserializeInstancesAsync(buffer: buffer) → Instances
SerializeInstancesAsync(inputInstances: Instances) → buffer
```

---

## ServerScriptService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
LoadStringEnabled: bool = false
```

---

## ServerStorage
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## ServiceProvider
**Extends:** Instance
**Tags:** NotCreatable, NotBrowsable

### Functions
```
FindService(className: string) → Instance
GetService(className: string) → Instance
getService(className: string) → Instance [Deprecated]
service(className: string) → Instance [Deprecated]
```

### Events
```
Close()
CloseLate() [LocalUserSecurity]
ServiceAdded(service: Instance)
ServiceRemoving(service: Instance)
```

---

## DataModel
**Extends:** ServiceProvider
**Tags:** NotCreatable

### Properties
```
CreatorId: int64 [ReadOnly]
CreatorType: CreatorType [ReadOnly]
Environment: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
ForceR15: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
GameAvatarType: GameAvatarType [Read:RobloxSecurity] [Write:RobloxSecurity] [Deprecated]
GameId: int64 [ReadOnly]
GearGenreSetting: GearGenreSetting [ReadOnly] [Deprecated]
Genre: Genre [ReadOnly]
IsSFFlagsLoaded: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
JobId: string [ReadOnly]
MatchmakingType: MatchmakingType [ReadOnly]
PlaceId: int64 [ReadOnly]
PlaceVersion: int [ReadOnly]
PrivateServerId: string [ReadOnly]
PrivateServerOwnerId: int64 [ReadOnly]
R15CollisionType: R15CollisionType [Read:RobloxSecurity] [Write:RobloxSecurity] [Deprecated]
VIPServerId: string [ReadOnly] [Deprecated]
VIPServerOwnerId: int64 [ReadOnly] [Deprecated]
Workspace: Workspace [ReadOnly]
lighting: Instance [ReadOnly] [Deprecated]
workspace: Workspace [ReadOnly] [Deprecated]
```

### Functions
```
BindToClose(function: Function) → null
DefineFastFlag(name: string, defaultValue: bool) → bool [RobloxScriptSecurity]
DefineFastInt(name: string, defaultValue: int) → int [RobloxScriptSecurity]
DefineFastString(name: string, defaultValue: string) → string [RobloxScriptSecurity]
GetEngineFeature(name: string) → bool [LocalUserSecurity]
GetFastFlag(name: string) → bool [LocalUserSecurity]
GetFastInt(name: string) → int [LocalUserSecurity]
GetFastString(name: string) → string [LocalUserSecurity]
GetJobsInfo() → Array [PluginSecurity]
GetMessage() → string [Deprecated]
GetObjects(url: ContentId) → Instances [PluginSecurity]
GetObjectsAllOrNone(url: ContentId, binaryFormatOnly: bool) → Instances [RobloxScriptSecurity]
GetObjectsList(urls: Array) → Array [RobloxScriptSecurity]
GetPlaySessionId() → string [RobloxScriptSecurity]
GetRemoteBuildMode() → bool [Deprecated]
IsContentLoaded() → bool [RobloxScriptSecurity]
IsGearTypeAllowed(gearType: GearType) → bool [Deprecated]
IsLoaded() → bool
IsUniverseMetadataLoaded() → bool [RobloxScriptSecurity]
Load(url: ContentId) → null [LocalUserSecurity]
OpenScreenshotsFolder() → null [RobloxScriptSecurity]
OpenVideosFolder() → null [RobloxScriptSecurity]
ReportInGoogleAnalytics(category: string, action: string, label: string, value: int) → null [RobloxScriptSecurity]
SetFastFlagForTesting(name: string, newValue: bool) → bool [RobloxScriptSecurity]
SetFastIntForTesting(name: string, newValue: int) → int [RobloxScriptSecurity]
SetFastStringForTesting(name: string, newValue: string) → string [RobloxScriptSecurity]
SetFlagVersion(name: string, version: int) → null [RobloxScriptSecurity]
SetIsLoaded(value: bool, placeSizeInBytes: int?) → null [RobloxScriptSecurity]
SetPlaceId(placeId: int64) → null [PluginSecurity]
SetUniverseId(universeId: int64) → null [PluginSecurity]
Shutdown() → null [LocalUserSecurity]
GetObjectsAsync(url: ContentId) → Instances [RobloxScriptSecurity]
HttpGetAsync(url: string, httpRequestType: HttpRequestType) → string [RobloxScriptSecurity]
HttpPostAsync(url: string, data: string, contentType: string, httpRequestType: HttpRequestType) → string [RobloxScriptSecurity]
InsertObjectsAndJoinIfLegacyAsync(url: ContentId) → Instances [RobloxScriptSecurity]
SavePlace(saveFilter: SaveFilter) → bool [Deprecated]
```

### Events
```
AllowedGearTypeChanged()
GraphicsQualityChangeRequest(betterQuality: bool)
ItemChanged(object: Instance, descriptor: string)
Loaded()
ScreenshotReady(path: string) [RobloxScriptSecurity]
ScreenshotSavedToAlbum(filename: string, success: bool, message: string) [RobloxScriptSecurity]
UniverseMetadataLoaded() [RobloxScriptSecurity]
```

---

## GenericSettings
**Extends:** ServiceProvider
**Tags:** NotCreatable

---

## GlobalSettings
**Extends:** GenericSettings
**Tags:** NotCreatable, NotBrowsable

### Functions
```
GetFFlag(name: string) → bool
GetFFlagOverrides() → string [RobloxScriptSecurity]
GetFFlags() → string [RobloxScriptSecurity]
GetFVariable(name: string) → string
SetFFlagOverrides(overrides: string) → bool [RobloxScriptSecurity]
```

---

## UserSettings
**Extends:** GenericSettings
**Tags:** NotCreatable

### Functions
```
IsUserFeatureEnabled(name: string) → bool
Reset() → null
SaveState() → null [RobloxScriptSecurity]
```

---

## ServiceVisibilityService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
HiddenServices: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
VisibleServices: BinaryString [Read:RobloxSecurity] [Write:RobloxSecurity]
```

### Functions
```
SetServiceVisibilityPreference(service: Instance, visible: bool) → null [RobloxScriptSecurity]
```

### Events
```
ServiceVisibilityChanged(serviceName: string) [RobloxScriptSecurity]
```

---

## SessionCheckService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## SessionService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
AcquireContextFocus(context: string) → null [RobloxScriptSecurity]
GenerateSessionInfoString(includeArbitrarySessions: bool, includeTag: bool, includeTimestamps: bool, includeMetadata: bool) → string [RobloxScriptSecurity]
GetCreatedTimestampUtcMs(sid: string) → int64 [RobloxScriptSecurity]
GetMetadata(sid: string, key: string) → Variant [RobloxScriptSecurity]
GetRootSID() → string [RobloxScriptSecurity]
GetSessionID(structuralId: string) → string [RobloxScriptSecurity]
GetSessionTag(sid: string) → string [RobloxScriptSecurity]
IsContextFocused(context: string) → bool [RobloxScriptSecurity]
ReleaseContextFocus(context: string) → null [RobloxScriptSecurity]
RemoveMetadata(sid: string, key: string, context: string) → null [RobloxScriptSecurity]
RemoveSession(sid: string, context: string) → null [RobloxScriptSecurity]
RemoveSessionsWithMetadataKey(key: string) → null [RobloxScriptSecurity]
ReplaceSession(sid: string, tag: string) → null [RobloxScriptSecurity]
SessionExists(sid: string) → bool [RobloxScriptSecurity]
SetMetadata(sid: string, key: string, value: Variant, context: string) → null [RobloxScriptSecurity]
SetSession(parentSid: string, childSid: string, tag: string, context: string) → null [RobloxScriptSecurity]
```

---

## SharedTableRegistry
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetSharedTable(name: string) → SharedTable
SetSharedTable(name: string, st: SharedTable?) → null
```

---

## Sky
**Extends:** Instance

### Properties
```
CelestialBodiesShown: bool = true
MoonAngularSize: float = 11
MoonTextureId: ContentId = rbxasset://sky/moon.jpg
SkyboxBk: ContentId = rbxasset://textures/sky/sky512_bk.tex
SkyboxDn: ContentId = rbxasset://textures/sky/sky512_dn.tex
SkyboxFt: ContentId = rbxasset://textures/sky/sky512_ft.tex
SkyboxLf: ContentId = rbxasset://textures/sky/sky512_lf.tex
SkyboxOrientation: Vector3 = 0, 0, 0
SkyboxRt: ContentId = rbxasset://textures/sky/sky512_rt.tex
SkyboxUp: ContentId = rbxasset://textures/sky/sky512_up.tex
StarCount: int = 3000
SunAngularSize: float = 21
SunTextureId: ContentId = rbxasset://sky/sun.jpg
```

---

## SlimService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## Smoke
**Extends:** Instance

### Properties
```
Color: Color3 = 1, 1, 1
Enabled: bool = true
LocalTransparencyModifier: float = 0
Opacity: float = 0.5
RiseVelocity: float = 1
Size: float = 1
TimeScale: float = 1
opacity_xml: float = 0.5
riseVelocity_xml: float = 1
size_xml: float = 1
```

### Functions
```
FastForward(numFrames: int) → null [RobloxScriptSecurity]
```

---

## SmoothVoxelsUpgraderService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
Cancel() → null [RobloxScriptSecurity]
Start() → null [RobloxScriptSecurity]
```

### Events
```
Status(progressRatio: float) [RobloxScriptSecurity]
```

---

## SnippetService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## SocialService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetPlayersByPartyId(partyId: string) → Instances
HideSelfView() → null
InvokeGameInvitePromptClosed(player: Instance, recipientIds: Array) → null [RobloxScriptSecurity]
InvokeIrisInvite(player: Instance, tag: string, irisParticipants: Array) → null [RobloxScriptSecurity]
InvokeIrisInvitePromptClosed(player: Instance) → null [RobloxScriptSecurity]
InvokeShareSheetClosed() → null [RobloxScriptSecurity]
PromptGameInvite(player: Instance, experienceInviteOptions: Instance) → null
PromptPhoneBook(player: Instance, tag: string) → null
PromptRsvpToEventCompleted(eventId: string, success: bool, rsvpStatus: RsvpStatus) → null [RobloxScriptSecurity]
ShowSelfView(selfViewPosition: SelfViewPosition) → null
UpdatePlayerPartyData(partyId: string) → null [RobloxScriptSecurity]
CanSendCallInviteAsync(player: Instance) → bool
CanSendGameInviteAsync(player: Instance, recipientId: int64) → bool
GetEventRsvpStatusAsync(eventId: string) → RsvpStatus
GetPartyAsync(partyId: string) → Array
PromptLinkSharing(player: Player, options: Dictionary) → Tuple
PromptRsvpToEventAsync(eventId: string) → RsvpStatus
```

### Events
```
CallInviteStateChanged(player: Instance, inviteState: InviteState)
GameInvitePromptClosed(player: Instance, recipientIds: Array)
IrisInviteInitiated(message: string) [RobloxSecurity]
OpenShareSheetWithLink(link: string) [RobloxScriptSecurity]
PhoneBookPromptClosed(player: Instance)
PlayerPartyDataChanged(partyId: string) [RobloxScriptSecurity]
PromptInviteRequested(player: Instance, experienceInviteOptions: Instance) [RobloxScriptSecurity]
PromptIrisInviteRequested(player: Instance, tag: string) [RobloxScriptSecurity]
SelfViewHidden() [RobloxScriptSecurity]
SelfViewVisible(selfViewPosition: SelfViewPosition) [RobloxScriptSecurity]
ShareSheetClosed(player: Player)
ShowPromptRsvpToEvent(eventId: string) [RobloxScriptSecurity]
```

---

## Sound
**Extends:** Instance

### Properties
```
ChannelCount: int = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
EmitterSize: float = 10 [Deprecated]
IsLoaded: bool = false [ReadOnly]
IsMutedForCapture: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
IsPaused: bool = true [ReadOnly]
IsPlaying: bool = false [ReadOnly]
IsSpatial: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
LoopRegion: NumberRange = 0 60000 
Looped: bool = false
MaxDistance: float = 10000 [Deprecated]
MinDistance: float = 10 [Deprecated]
Pitch: float = 1 [Deprecated]
PlayOnRemove: bool = false
PlaybackLoudness: double = 0 [ReadOnly]
PlaybackRegion: NumberRange = 0 60000 
PlaybackRegionsEnabled: bool = false
PlaybackSpeed: float = 1
Playing: bool = false
PlayingReplicator: bool = false
RollOffGain: float = 1 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
RollOffMaxDistance: float = 10000
RollOffMinDistance: float = 10
RollOffMode: RollOffMode = Inverse
SoundGroup: SoundGroup
SoundId: ContentId
TimeLength: double = 0 [ReadOnly]
TimePosition: double = 0
TimePositionReplicator: double = 0
UsageContextPermission: UsageContext = Default [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Volume: float = 0.5
isPlaying: bool = false [ReadOnly] [Deprecated]
xmlRead_MaxDistance_3: float = 10000 [Deprecated]
xmlRead_MinDistance_3: float = 10 [Deprecated]
```

### Functions
```
Pause() → null
Play() → null
Resume() → null
Stop() → null
pause() → null [Deprecated]
play() → null [Deprecated]
stop() → null [Deprecated]
```

### Events
```
DidLoop(soundId: string, numOfTimesLooped: int)
Ended(soundId: string)
Loaded(soundId: string)
Paused(soundId: string)
Played(soundId: string)
PlayingUpdatedFromClient(value: bool) [RobloxSecurity]
PlayingUpdatedFromServer(value: bool) [RobloxSecurity]
Resumed(soundId: string)
Stopped(soundId: string)
TimePositionUpdatedFromClient(newPositionSeconds: double, lastLuaSetTimePosition: double) [RobloxSecurity]
TimePositionUpdatedFromServer(newPositionSeconds: double, lastLuaSetTimePosition: double) [RobloxSecurity]
playbackActionSync(action: int) [RobloxSecurity]
```

---

## SoundEffect
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
Enabled: bool
Priority: int
```

---

## ChorusSoundEffect
**Extends:** SoundEffect

### Properties
```
Depth: float = 0.150000006
Mix: float = 0.5
Rate: float = 0.5
```

---

## CompressorSoundEffect
**Extends:** SoundEffect

### Properties
```
Attack: float = 0.100000001
GainMakeup: float = 0
Ratio: float = 40
Release: float = 0.100000001
SideChain: Instance
Threshold: float = -40
```

---

## CustomSoundEffect
**Extends:** SoundEffect
**Tags:** NotCreatable

---

## AssetSoundEffect
**Extends:** CustomSoundEffect
**Tags:** NotCreatable

---

## ChannelSelectorSoundEffect
**Extends:** CustomSoundEffect
**Tags:** NotCreatable, NotBrowsable

### Properties
```
Channel: int = 1
```

---

## DistortionSoundEffect
**Extends:** SoundEffect

### Properties
```
Level: float = 0.75
```

---

## EchoSoundEffect
**Extends:** SoundEffect

### Properties
```
Delay: float = 1
DryLevel: float = 0
Feedback: float = 0.5
WetLevel: float = 0
```

---

## EqualizerSoundEffect
**Extends:** SoundEffect

### Properties
```
HighGain: float = 0
LowGain: float = -20
MidGain: float = -10
```

---

## FlangeSoundEffect
**Extends:** SoundEffect

### Properties
```
Depth: float = 0.449999988
Mix: float = 0.850000024
Rate: float = 5
```

---

## PitchShiftSoundEffect
**Extends:** SoundEffect

### Properties
```
Octave: float = 1.25
```

---

## ReverbSoundEffect
**Extends:** SoundEffect

### Properties
```
DecayTime: float = 1.5
Density: float = 1
Diffusion: float = 1
DryLevel: float = -6
WetLevel: float = 0
```

---

## TremoloSoundEffect
**Extends:** SoundEffect

### Properties
```
Depth: float = 1
Duty: float = 0.5
Frequency: float = 5
```

---

## SoundGroup
**Extends:** Instance

### Properties
```
Volume: float = 0.5
```

---

## SoundService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
AmbientReverb: ReverbType = NoReverb
AudioApiByDefault: RolloutState = Default [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CharacterSoundsUseNewApi: RolloutState = Default [Write:PluginSecurity]
DefaultListenerLocation: ListenerLocation = Default [Read:PluginSecurity] [Write:PluginSecurity]
DistanceFactor: float = 3.32999992
DopplerScale: float = 1
IsNewExpForAudioApiByDefault: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
RespectFilteringEnabled: bool = false
RolloffScale: float = 1
VolumetricAudio: VolumetricAudio = Automatic
```

### Functions
```
BeginRecording() → bool [RobloxScriptSecurity]
GetAudioApiByDefault() → bool [RobloxScriptSecurity]
GetAudioInstances() → Array [RobloxScriptSecurity]
GetInputDevice() → Tuple [RobloxScriptSecurity]
GetInputDevices() → Tuple [RobloxScriptSecurity]
GetListener() → Tuple
GetOutputDevice() → Tuple [RobloxScriptSecurity]
GetOutputDevices() → Tuple [RobloxScriptSecurity]
GetSoundMemoryData() → Dictionary [RobloxScriptSecurity]
InsertAsset(assetId: ContentId, assetName: string, useSelection: bool) → Instances [RobloxScriptSecurity]
OpenAttenuationCurveEditor(selectedCurveObjects: Instances) → null [PluginSecurity]
OpenDirectionalCurveEditor(selectedCurveObjects: Instances) → null [PluginSecurity]
PlayLocalSound(sound: Instance) → null
SetAudioApiByDefault(enabled: bool) → null [RobloxScriptSecurity]
SetInputDevice(name: string, guid: string) → null [RobloxScriptSecurity]
SetListener(listenerType: ListenerType, listener: Tuple) → null
SetOutputDevice(name: string, guid: string) → null [RobloxScriptSecurity]
SetRecordingDevice(deviceIndex: int) → bool [RobloxScriptSecurity]
SetSoundEnabled(enabled: bool) → null [RobloxScriptSecurity]
EndRecording() → Dictionary [RobloxScriptSecurity]
GetRecordingDevices() → Dictionary [RobloxScriptSecurity]
```

### Events
```
AudioInstanceAdded(instance: Instance) [RobloxScriptSecurity]
ClientLoggedEvent(sessionIdRaw: string) [RobloxSecurity]
DeviceListChanged(newDevices: Tuple) [RobloxScriptSecurity]
OpenAttenuationCurveEditorSignal(selectedCurveObjects: Instances) [RobloxScriptSecurity]
OpenAudioCompressorEditorSignal(selectedCompressorObjects: Instances) [RobloxScriptSecurity]
OpenAudioEqualizerEditorSignal(selectedEqualizerObjects: Instances) [RobloxScriptSecurity]
OpenDirectionalCurveEditorSignal(selectedCurveObjects: Instances) [RobloxScriptSecurity]
```

---

## Sparkles
**Extends:** Instance

### Properties
```
Color: Color3 = 1, 1, 1
Enabled: bool = true
LocalTransparencyModifier: float = 0
SparkleColor: Color3 = 0.564706, 0.0980392, 1
TimeScale: float = 1
```

### Functions
```
FastForward(numFrames: int) → null [RobloxScriptSecurity]
```

---

## SpawnerService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## StackFrame
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
FrameId: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
FrameName: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
FrameType: DebuggerFrameType [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Globals: DebuggerVariable [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Line: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Locals: DebuggerVariable [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Populated: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Script: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Upvalues: DebuggerVariable [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

---

## StandalonePluginScripts
**Extends:** Instance

---

## StartPageService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
generateTempUrlInContentProvider(url: string) → null [RobloxScriptSecurity]
getDaysSinceFirstUserLogin() → int [RobloxScriptSecurity]
getLocalGamesFromRegistry() → Array [RobloxScriptSecurity]
getRecentAPIGamesFromRegistry() → Array [RobloxScriptSecurity]
getTempUrlInContentProvider(url: string) → string [RobloxScriptSecurity]
isTutorialBannerClosed() → bool [RobloxScriptSecurity]
isTutorialPopupClosed() → bool [RobloxScriptSecurity]
openLink(link: string) → null [RobloxScriptSecurity]
openLocalFile(filePath: string) → null [RobloxScriptSecurity]
openPlace(placeId: int64, universeId: int64, launchTutorial: bool) → null [RobloxScriptSecurity]
removeAPIGameFromRegistry(gameId: int64) → null [RobloxScriptSecurity]
removeLocalFileFromRegistry(fileName: string) → null [RobloxScriptSecurity]
setTutorialBannerClosed(closed: bool) → null [RobloxScriptSecurity]
setTutorialPopupClosed(closed: bool) → null [RobloxScriptSecurity]
shouldShowMacOSDeprecationWarning() → bool [RobloxScriptSecurity]
shouldShowWinOSDeprecationWarning() → bool [RobloxScriptSecurity]
startTutorial() → null [RobloxScriptSecurity]
```

### Events
```
ImageImportedSignal(urlImported: string, temporaryId: string) [RobloxScriptSecurity]
LocalGamesFromRegistryUpdatedSignal(localGames: Array) [RobloxScriptSecurity]
RecentApiGamesFromRegistryUpdatedSignal(recentGames: Array) [RobloxScriptSecurity]
```

---

## StarterGear
**Extends:** Instance

---

## StarterPack
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## StarterPlayer
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
AllowCustomAnimations: bool = true [Write:RobloxScriptSecurity]
AutoJumpEnabled: bool = true
AvatarJointUpgrade: RolloutState = Default
AvatarJointUpgrade_SerializedRollout: RolloutState = Default
CameraMaxZoomDistance: float = 400
CameraMinZoomDistance: float = 0.5
CameraMode: CameraMode = Classic
CharacterJumpHeight: float = 7.19999981
CharacterJumpPower: float = 50
CharacterMaxSlopeAngle: float = 89
CharacterUseJumpPower: bool = true
CharacterWalkSpeed: float = 16
ClassicDeath: bool = true
DevCameraOcclusionMode: DevCameraOcclusionMode = Zoom
DevComputerCameraMovementMode: DevComputerCameraMovementMode = UserChoice
DevComputerMovementMode: DevComputerMovementMode = UserChoice
DevTouchCameraMovementMode: DevTouchCameraMovementMode = UserChoice
DevTouchMovementMode: DevTouchMovementMode = UserChoice
EnableDynamicHeads: LoadDynamicHeads = Default
EnableMouseLockOption: bool = true
GameSettingsAssetIDFace: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsAssetIDHead: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsAssetIDLeftArm: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsAssetIDLeftLeg: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsAssetIDPants: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsAssetIDRightArm: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsAssetIDRightLeg: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsAssetIDShirt: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsAssetIDTeeShirt: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsAssetIDTorso: int64 = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsAvatar: GameAvatarType = R15 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsR15Collision: R15CollisionType = OuterBox [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsScaleRangeBodyType: NumberRange = 0 1  [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsScaleRangeHead: NumberRange = 0.95 1  [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsScaleRangeHeight: NumberRange = 0.9 1.05  [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsScaleRangeProportion: NumberRange = 0 1  [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GameSettingsScaleRangeWidth: NumberRange = 0.7 1  [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
HealthDisplayDistance: float = 100
LoadCharacterAppearance: bool = true
LoadCharacterLayeredClothing: LoadCharacterLayeredClothing = Default
LoadCharacterLayeredClothing : LoadCharacterLayeredClothing = Default
LuaCharacterController: CharacterControlMode = Default
NameDisplayDistance: float = 100
RagdollDeath: bool = true
UserEmotesEnabled: bool = true
```

### Functions
```
ClearDefaults() → null [RobloxScriptSecurity]
```

---

## StarterPlayerScripts
**Extends:** Instance
**Tags:** NotCreatable

---

## StarterCharacterScripts
**Extends:** StarterPlayerScripts
**Tags:** NotCreatable

---

## StartupMessageService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetStartupMessage() → Variant [RobloxScriptSecurity]
```

---

## Stats
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
ContactsCount: int [ReadOnly]
DataReceiveKbps: float [ReadOnly]
DataSendKbps: float [ReadOnly]
FrameTime: float [ReadOnly]
HeartbeatTime: float [ReadOnly]
HeartbeatTimeMs: float [ReadOnly] [Deprecated]
InstanceCount: int [ReadOnly]
MovingPrimitivesCount: int [ReadOnly]
PhysicsReceiveKbps: float [ReadOnly]
PhysicsSendKbps: float [ReadOnly]
PhysicsStepTime: float [ReadOnly]
PhysicsStepTimeMs: float [ReadOnly] [Deprecated]
PrimitivesCount: int [ReadOnly]
RenderCPUFrameTime: float [ReadOnly]
RenderGPUFrameTime: float [ReadOnly]
SceneDrawcallCount: int [ReadOnly]
SceneTriangleCount: int [ReadOnly]
ShadowsDrawcallCount: int [ReadOnly]
ShadowsTriangleCount: int [ReadOnly]
UI2DDrawcallCount: int [ReadOnly]
UI2DTriangleCount: int [ReadOnly]
UI3DDrawcallCount: int [ReadOnly]
UI3DTriangleCount: int [ReadOnly]
```

### Functions
```
GetBrowserTrackerId() → string [RobloxScriptSecurity]
GetHarmonyQualityLevel() → int
GetMemoryCategoryNames() → Array
GetMemoryUsageMbAllCategories() → Array
GetMemoryUsageMbForTag(tag: DeveloperMemoryTag) → float
GetTotalMemoryUsageMb() → float
ResetHarmonyMemoryTarget() → null
SetHarmonyMemoryTarget(targetMB: int) → null
GetPaginatedMemoryByTexture(queryType: TextureQueryType, pageIndex: int, pageSize: int) → Dictionary [RobloxScriptSecurity]
```

---

## StatsItem
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
DisplayName: string [Read:PluginSecurity] [Write:PluginSecurity] [ReadOnly]
```

### Functions
```
GetValue() → double [PluginSecurity]
GetValueString() → string [PluginSecurity]
```

---

## RunningAverageItemDouble
**Extends:** StatsItem
**Tags:** NotCreatable

---

## RunningAverageItemInt
**Extends:** StatsItem
**Tags:** NotCreatable

---

## RunningAverageTimeIntervalItem
**Extends:** StatsItem
**Tags:** NotCreatable

---

## TotalCountTimeIntervalItem
**Extends:** StatsItem
**Tags:** NotCreatable

---

## StopWatchReporter
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
FinishTask(taskId: int) → null [RobloxScriptSecurity]
SendReport(reportName: string) → null [RobloxScriptSecurity]
StartTask(reportName: string, taskName: string) → int [RobloxScriptSecurity]
```

---

## StreamingService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetEphemeralVariable(key: string) → Variant [RobloxScriptSecurity]
GetInstance(requestId: string, instanceId: string) → Instance [RobloxScriptSecurity]
InvokeCommand(requestId: string, commandName: string, arg: Variant) → null [RobloxScriptSecurity]
RegisterCommandInternal(commandName: string, function: Function, isSequential: bool, isPublic: bool) → null [RobloxScriptSecurity]
RegisterContextCollector(collectorName: string, function: Function) → null [RobloxScriptSecurity]
SetEphemeralVariable(key: string, value: Variant, timeToLive: int) → null [RobloxScriptSecurity]
SetPluginInfoCallback(function: Function) → null [RobloxScriptSecurity]
UnregisterCommand(commandName: string) → null [RobloxScriptSecurity]
UnregisterContextCollector(collectorName: string) → null [RobloxScriptSecurity]
AttemptSaveAndSendPlaceTelemetry(requestId: string, toolSource: string) → null [RobloxScriptSecurity]
BindCodeToGuid(runCodeGuid: string, code: string) → Tuple [RobloxScriptSecurity]
ExecuteCommandAsync(requestId: string, commandName: string, arg: Variant) → Variant
GetRequiredScripts(script: Instance) → Variant [RobloxScriptSecurity]
RunSandboxedCode(runCodeGuid: string, requestId: string) → Tuple [RobloxScriptSecurity]
SearchForAssets(body: Variant) → Variant [RobloxScriptSecurity]
```

### Events
```
ConversationCleared() [RobloxScriptSecurity]
RequestEnded(requestId: string) [RobloxScriptSecurity]
RequestError(requestId: string, errorType: string, errorMessage: string) [RobloxScriptSecurity]
RequestStarted(requestId: string, queryToProcess: string) [RobloxScriptSecurity]
SequentialCommandsFinished(requestId: string, success: bool) [RobloxScriptSecurity]
Stream(requestId: string, commandName: string, streamContent: string) [RobloxScriptSecurity]
```

---

## Studio
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
"TODO" Color: Color3
"function" Color: Color3
"local" Color: Color3
"nil" Color: Color3
"self" Color: Color3
ActionOnAutoResumeSync: ActionOnAutoResumeSync [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ActionOnStopSync: ActionOnStopSync
Active Color: Color3
Active Hover Over Color: Color3
Always Save Script Changes: bool
Animate Hover Over: bool
Auto Clean Empty Line: bool
Auto Closing Brackets: bool
Auto Closing Quotes: bool
Auto Delete Closing Brackets and Quotes: bool
Auto Indent Rule: AutoIndentRule
Auto-Recovery Enabled: bool
Auto-Recovery Interval (Minutes): int
AutoResumeSyncOnPlaceOpen: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
AutocompleteAcceptanceBehavior: CompletionAcceptanceBehavior [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Automatically trigger AI Code Completion: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Background Color: Color3
Basic Objects Display Mode: ListDisplayMode
Bool Color: Color3
Bracket Color: Color3
Built-in Function Color: Color3
Camera Mouse Wheel Speed: float
Camera Pan Speed: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Camera Shift Speed: float
Camera Speed: float
Camera Speed Adjust Binding: CameraSpeedAdjustBinding
Camera Zoom to Mouse Position: bool
CameraAdaptiveSpeed: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CameraOrbitSensitivity: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CameraPanSensitivity: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CameraShiftFactor: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CameraSpeedLockDefault: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CameraTweenFocus: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CameraZoomSpeed: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Clear Output On Start: bool
CommandBarLocalState: bool
Comment Color: Color3
Current Line Highlight Color: Color3
Debugger Current Line Color: Color3
Debugger Error Line Color: Color3
DeprecatedObjectsShown: bool
DisplayLanguage: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Doc View Code Background Color: Color3 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DraggerActiveColor: Color3 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DraggerMajorGridIncrement: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DraggerMaxSoftSnaps: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DraggerPassiveColor: Color3 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DraggerShowHoverRuler: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DraggerShowMeasurement: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DraggerShowTargetSnap: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DraggerSoftSnapMarginFactor: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DraggerSummonMarginFactor: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DraggerTiltRotateDuration: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Enable Autocomplete: bool
Enable Autocomplete Doc View: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Enable CoreScript Debugger: bool
Enable Http Sandboxing: bool
Enable Internal Beta Features: bool
Enable Internal Features: bool
Enable Script Analysis: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Enable Scrollbar Markers: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Enable Signature Help: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Enable Signature Help Doc View: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Enable Temporary Tabs: bool
Enable Temporary Tabs In Explorer: bool
Enable Type Hover: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
EnableCodeAssist: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
EnableIndentationRulers: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
EnableOnTypeAutocomplete: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
EnableSelectionTooltips: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Error Color: Color3
Find Selection Background Color: Color3
Font: QFont
Format On Paste: bool
Format On Type: bool
Function Name Color: Color3
Highlight Current Line: bool
Highlight Occurances: bool
HintColor: Color3
Hover Animate Speed: HoverAnimateSpeed
Hover Box Thickness: float [Read:RobloxSecurity] [Write:RobloxSecurity]
Hover Line Thickness: int [Read:RobloxSecurity] [Write:RobloxSecurity]
Hover Over Color: Color3
IconOverrideDir: QDir [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Indent Using Spaces: bool
IndentationRulerColor: Color3 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
InformationColor: Color3
Keyword Color: Color3
LargeFileLineCountThreshold: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LargeFileThreshold: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Line Thickness: float
LoadAllBuiltinPluginsInRunModes: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LoadInternalPlugins: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
LoadUserPluginsInRunModes: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
LocalAssetsFolder: QDir [Write:RobloxScriptSecurity]
LuaDebuggerEnabled: bool
LuaDebuggerEnabledAtStartup: bool [ReadOnly]
Luau Keyword Color: Color3
Main Volume: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Matching Word Background Color: Color3
Maximum Output Lines: int
Menu Item Background Color: Color3
Method Color: Color3
Number Color: Color3
Only Play Audio from Window in Focus: bool
Operator Color: Color3
Output Font: QFont
Output Layout Mode: OutputLayoutMode
PermissionLevelShown: PermissionLevelShown
Physical Draggers Select Scope By Default: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Pivot Snap To Geometry Color: Color3 [Read:RobloxSecurity] [Write:RobloxSecurity]
PluginDebuggingEnabled: bool
PluginsDir: QDir
Primary Text Color: Color3
Property Color: Color3
ReloadBuiltinPluginsOnChange: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
ReloadLocalPluginsOnChange: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
Respect Studio shortcuts when game has focus: bool
Ruler Color: Color3
Rulers: string
RuntimeUndoBehavior: RuntimeUndoBehavior
Script Editor Color Preset: StudioScriptEditorColorPresets
Script Editor Scrollbar Background Color: Color3
Script Editor Scrollbar Handle Color: Color3
ScriptEditorMenuBorderColor: Color3 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ScriptEditorShouldShowPluginMethods: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ScriptTimeoutLength: int
Scroll Past Last Line: bool
Secondary Text Color: Color3
Select Color: Color3
Select/Hover Color: Color3
Selected Menu Item Background Color: Color3
Selected Text Color: Color3
Selection Background Color: Color3
Selection Box Thickness: float [Read:RobloxSecurity] [Write:RobloxSecurity]
Selection Color: Color3
Selection Line Thickness: int [Read:RobloxSecurity] [Write:RobloxSecurity]
Set Pivot of Imported Parts: bool
Show Core GUI in Explorer while Playing: bool
Show Diagnostics Bar: bool
Show FileSyncService: bool
Show Hidden Objects in Explorer: bool
Show Hover Over: bool
Show Light Guides: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Show Navigation Labels: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Show Navigation Mesh: bool
Show Pathfinding Links: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Show Plugin GUI Service in Explorer: bool
Show Singly Selected Attachment Parent Frame: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Show Whitespace: bool
Show plus button on hover in Explorer: bool
ShowCorePackagesInExplorer: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Skip Closing Brackets and Quotes: bool
String Color: Color3
Tab Width: int
Text Color: Color3
Text Wrapping: bool
Theme: Instance
TypeColor: Color3
UI Theme: UITheme [ReadOnly] [Deprecated]
Use Bounding Box Move Handles: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Warning Color: Color3
Whitespace Color: Color3
```

### Functions
```
GetAvailableThemes() → Array [PluginSecurity]
```

### Events
```
ThemeChanged() [PluginSecurity]
```

---

## StudioAssetService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
ConvertToPackageUpload(uploadUrl: string, cloneInstances: Instances, originalInstances: Instances) → null [RobloxScriptSecurity]
FireOnUGCSubmitCompleted(cancelled: bool) → null [RobloxScriptSecurity]
PublishPackage(instance: Instance, publishInfo: Dictionary) → null [RobloxScriptSecurity]
ShowSaveToRoblox(instances: Instances, assetType: Variant, hasSubsequent: bool) → null [RobloxScriptSecurity]
UpdatePublishedPackage(assetmetadata: Dictionary, rootInstance: Instance, isConvert: bool, addUndoWaypoint: bool) → null [RobloxScriptSecurity]
AutoSetupAvatarAsync(modelId: ContentId, progressCallback: Function, notificationCallback: Function?) → Instance [RobloxScriptSecurity]
AutoSetupSerializedAvatarAsync(serializedInstance: string, publishInfo: Dictionary, telemetryMetadata: Dictionary, progressCallback: Function, notificationCallback: Function?) → Instance [RobloxScriptSecurity]
CancelAutoSetupAvatarAsync(jobId: string) → null [RobloxScriptSecurity]
DEPRECATED_SerializeInstances(instances: Instances) → string [RobloxScriptSecurity]
RequestAvatarAutosetupAsync(meshId: ContentId, textureId: ContentId, progressCallback: Function) → Instance [RobloxScriptSecurity]
SerializeInstances(instances: Instances, groupId: int64, isPackage: bool) → string [RobloxScriptSecurity]
```

### Events
```
OnConvertToPackageResult(isSuccessful: bool, errorMessage: string) [RobloxScriptSecurity]
OnPublishPackageResult(result: Dictionary, errorMessage: string) [RobloxScriptSecurity]
OnSaveToRoblox(instances: Instances, assetType: Variant, hasSubsequent: bool) [RobloxScriptSecurity]
OnUGCSubmitCompleted(cancelled: bool) [RobloxScriptSecurity]
```

---

## StudioAttachment
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
AutoHideParent: bool = false
IsArrowVisible: bool = false
Offset: Vector2 = 0, 0
SourceAnchorPoint: Vector2 = 0, 0
TargetAnchorPoint: Vector2 = 0, 0
```

---

## StudioCallout
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
AnchorPoint: Vector2 = 0.5, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
IsArrowVisible: bool = true [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
IsNextVisible: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
RowName: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Text: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Title: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
SetOnNextClicked(onClick: Function) → null [RobloxScriptSecurity]
```

---

## StudioCameraService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
LockCameraSpeed: bool = false
```

### Events
```
ShowCameraSpeed(speed: float)
```

---

## StudioData
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
EnableScriptCollabByDefaultOnLoad: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

---

## StudioDeviceEmulatorService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
HasMultiTouchStarted: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
IsMultiTouchEmulationOn: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
IsMultiTouchEnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
PivotPosition: Vector2 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Functions
```
GetMaxNumTouches() → int [RobloxScriptSecurity]
GetTouchInBounds(index: int) → bool [RobloxScriptSecurity]
GetTouchPosition(index: int) → Vector2 [RobloxScriptSecurity]
EmulatePCDeviceWithResolution(deviceId: string, resolution: Vector2) → bool [RobloxScriptSecurity]
GetCurrentDeviceId() → string [RobloxScriptSecurity]
GetCurrentOrientation() → ScreenOrientation [RobloxScriptSecurity]
HasDeviceWithId(deviceId: string) → bool [RobloxScriptSecurity]
SetCurrentDeviceId(deviceId: string) → null [RobloxScriptSecurity]
SetCurrentOrientation(orientation: ScreenOrientation) → null [RobloxScriptSecurity]
```

### Events
```
CurrentDeviceIdChanged() [RobloxScriptSecurity]
OrientationChanged() [RobloxScriptSecurity]
TouchInBoundsChanged() [RobloxScriptSecurity]
TouchPositionsChanged() [RobloxScriptSecurity]
```

---

## StudioObjectBase
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

---

## StudioWidget
**Extends:** StudioObjectBase
**Tags:** NotCreatable, NotReplicated

### Functions
```
SetFixedSize(width: int, height: int) → null [RobloxScriptSecurity]
```

---

## StudioPublishService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
PublishLocked: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
ClearUploadNames() → null [RobloxScriptSecurity]
CloseAfterPublish(closeMode: StudioCloseMode) → null [RobloxScriptSecurity]
PublishAs(universeId: int64, placeId: int64, groupId: int64, isPublish: bool, publishParameters: Variant, willRetryOnConflict: bool, allowOpeningNewPlace: bool) → null [RobloxScriptSecurity]
PublishThenTurnOnTeamCreate() → null [RobloxScriptSecurity]
RefreshDocumentDisplayName() → null [RobloxScriptSecurity]
RegisterPublishHold(priority: int, callback: Function) → RBXScriptConnection [RobloxScriptSecurity]
SetTeamCreateOnPublishInfo(shouldTurnOnTcOnPublish: bool, newPlaceName: string) → null [RobloxScriptSecurity]
SetUniverseDisplayName(newName: string) → null [RobloxScriptSecurity]
SetUploadNames(placeName: string, universeName: string) → null [RobloxScriptSecurity]
ShowSaveOrPublishPlaceToRoblox(showGameSelect: bool, isPublish: bool, closeMode: StudioCloseMode) → null [RobloxScriptSecurity]
```

### Events
```
GameNameUpdated(name: string) [RobloxScriptSecurity]
GamePublishCancelled() [RobloxScriptSecurity]
GamePublishFinished(success: bool, gameId: int64, message: string, reason: StudioPlaceUpdateFailureReason) [RobloxScriptSecurity]
OnPublishAttempt(isPublishAs: bool) [RobloxScriptSecurity]
OnSaveOrPublishPlaceToRoblox(showGameSelect: bool, isPublish: bool, closeMode: StudioCloseMode) [RobloxScriptSecurity]
```

---

## StudioScriptDebugEventListener
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## StudioSdkService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetSdk() → Instance [RobloxScriptSecurity]
SetSdk(sdk: Instance) → null [RobloxScriptSecurity]
```

---

## StudioService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
ActiveScript: Instance [ReadOnly]
AlignDraggedObjects: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
DraggerSolveConstraints: bool [ReadOnly]
DrawConstraintsOnTop: bool [ReadOnly] [Deprecated]
GridSize: float [ReadOnly]
HoverInstance: Instance [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
InstalledPluginData: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
PivotSnapToGeometry: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
RotateIncrement: float [ReadOnly]
Secrets: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ShowConstraintDetails: bool [ReadOnly]
ShowWeldDetails: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
StudioLocaleId: string [ReadOnly]
UseLocalSpace: bool
```

### Functions
```
AnimationIdSelected(id: int64) → null [RobloxScriptSecurity]
CopyToClipboard(stringToCopy: string) → null [RobloxScriptSecurity]
GetBadgeConfigureUrl(badgeId: int64) → string [RobloxScriptSecurity]
GetBadgeUploadUrl() → string [RobloxScriptSecurity]
GetClassIcon(className: string) → Dictionary [PluginSecurity]
GetPlaceIsPersistedToCloud() → bool [RobloxScriptSecurity]
GetResourceByCategory(category: string) → Dictionary [RobloxScriptSecurity]
GetStartupAssetId() → string [RobloxScriptSecurity]
GetStartupPluginId() → string [RobloxScriptSecurity]
GetTermsOfUseUrl() → string [RobloxScriptSecurity]
GetUserId() → int64 [PluginSecurity]
GizmoRaycast(origin: Vector3, direction: Vector3, raycastParams: RaycastParams) → RaycastResult? [PluginSecurity]
HasInternalPermission() → bool [RobloxScriptSecurity]
IsPluginInstalled(assetId: int64) → bool [RobloxScriptSecurity]
IsPluginUpToDate(assetId: int64, currentAssetVersion: int64) → bool [RobloxScriptSecurity]
OpenInBrowser_DONOTUSE(url: string) → null [RobloxScriptSecurity]
SetPluginEnabled(assetId: int64, state: bool) → null [RobloxScriptSecurity]
ShowPlaceVersionHistoryDialog(placeId: int64) → null [RobloxScriptSecurity] [Deprecated]
ShowPublishToRoblox() → null [RobloxScriptSecurity]
UninstallPlugin(assetId: int64) → null [RobloxScriptSecurity]
UpdatePluginManagement() → null [RobloxScriptSecurity]
PromptImportFile(fileTypeFilter: Array) → Instance [PluginSecurity]
PromptImportFiles(fileTypeFilter: Array) → Instances [PluginSecurity]
TryInstallPlugin(assetId: int64, assetVersionId: int64) → null [RobloxScriptSecurity]
```

### Events
```
OnImportFromRoblox() [RobloxScriptSecurity]
OnOpenGameSettings(pageIdentifier: string) [RobloxScriptSecurity]
OnOpenManagePackagePlugin(userId: int64, assetId: int64) [RobloxScriptSecurity]
OnPluginInstalledFromToolbox() [RobloxScriptSecurity]
OnPluginInstalledFromWeb(pluginId: string) [RobloxScriptSecurity]
OnPublishAsPlugin(instances: Instances) [RobloxScriptSecurity]
OnSaveToRoblox(instances: Instances) [RobloxScriptSecurity]
PromptTransformPluginCheckEnable() [RobloxScriptSecurity]
SaveLocallyAsComplete(success: bool) [RobloxScriptSecurity]
```

---

## StudioTheme
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
GetColor(styleguideitem: StudioStyleGuideColor, modifier: StudioStyleGuideModifier) → Color3 [PluginSecurity]
```

---

## StudioUserService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
IsLoggedIn: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

---

## StudioWidgetsService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
ApplyFillInBox(target: StudioWidget) → null [RobloxScriptSecurity]
ApplyHighlight(target: StudioWidget, rowName: string?) → null [RobloxScriptSecurity]
ApplyShadows() → null [RobloxScriptSecurity]
ApplySpotlight(target: StudioWidget, rowName: string?) → null [RobloxScriptSecurity]
GetWidgetFromLabel(label: string) → StudioWidget [RobloxScriptSecurity]
GetWidgetFromPluginGui(gui: PluginGui) → StudioWidget [RobloxScriptSecurity]
HideSpotlight() → null [RobloxScriptSecurity]
```

---

## StyleBase
**Extends:** Instance
**Tags:** NotCreatable

### Functions
```
GetStyleRules() → Instances
InsertStyleRule(rule: StyleRule, priority: int?) → null
SetStyleRules(rules: Instances) → null
```

### Events
```
StyleRulesChanged()
```

---

## StyleRule
**Extends:** StyleBase

### Properties
```
Index: int = -1
Priority: int = 0
PropertiesSerialize: BinaryString
Selector: string
SelectorError: string [ReadOnly]
```

### Functions
```
GetProperties() → Dictionary
GetPropertiesResolved() → Dictionary [RobloxScriptSecurity]
GetProperty(name: string) → Variant
GetPropertyResolved(name: string) → Variant [RobloxScriptSecurity]
SetProperties(styleProperties: Dictionary) → null
SetProperty(name: string, value: Variant) → null
```

### Events
```
StyleRulePropertyChanged(styleProperty: string) [RobloxScriptSecurity]
```

---

## StyleSheet
**Extends:** StyleBase

### Functions
```
GetDerives() → Instances
SetDerives(derives: Instances) → null
```

---

## StyleDerive
**Extends:** Instance

### Properties
```
Index: int = -1
Priority: int = 0
StyleSheet: StyleSheet
```

---

## StyleLink
**Extends:** Instance

### Properties
```
StyleSheet: StyleSheet
```

---

## StylingService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetAppliedStyles(instance: Instance) → Array [RobloxScriptSecurity]
GetStyleInfo(style: StyleRule) → Dictionary [RobloxScriptSecurity]
GetStyleSheetDerivesChain(styleSheet: StyleSheet) → Instances [RobloxScriptSecurity]
GetStyleSheetInfo(styleSheet: StyleSheet) → Dictionary [RobloxScriptSecurity]
UpdateUnitTestOnly() → null [RobloxScriptSecurity]
```

---

## SurfaceAppearance
**Extends:** Instance

### Properties
```
AlphaMode: AlphaMode = Overlay
Color: Color3 = 1, 1, 1
ColorMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
ColorMapContent: Content [Write:PluginSecurity]
MetalnessMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
MetalnessMapContent: Content [Write:PluginSecurity]
NormalMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
NormalMapContent: Content [Write:PluginSecurity]
RoughnessMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
RoughnessMapContent: Content [Write:PluginSecurity]
TexturePack: ContentId [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## SystemThemeService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
isSystemThemeAvailable() → bool [RobloxScriptSecurity]
setTheme(theme: SystemThemeValue) → null [RobloxScriptSecurity]
getSystemThemeAsync() → SystemThemeValue [RobloxScriptSecurity]
```

### Events
```
OnLuaThemeUpdated(theme: SystemThemeValue) [RobloxScriptSecurity]
```

---

## TaskScheduler
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
SchedulerDutyCycle: double [ReadOnly]
SchedulerRate: double [ReadOnly]
ThreadPoolConfig: ThreadPoolConfig
ThreadPoolSize: int [ReadOnly]
```

---

## Team
**Extends:** Instance

### Properties
```
AutoAssignable: bool = true
AutoColorCharacters: bool = true [Deprecated]
ChildOrder: int = -1 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Score: int = 0 [Deprecated]
TeamColor: BrickColor
```

### Functions
```
GetPlayers() → Instances
```

### Events
```
PlayerAdded(player: Player)
PlayerRemoved(player: Player)
```

---

## TeamCreateData
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
InitialCameraCFrame: CFrame [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## TeamCreatePublishService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Events
```
TeamCreateErrorStatus(result: TeamCreateErrorState, teamCreateSaveData: Dictionary) [RobloxScriptSecurity]
TeamCreatePlaceUploadRequest(metadata: Dictionary) [RobloxSecurity]
TeamCreatePlaceUploadResponse(success: bool, metadata: Dictionary) [RobloxSecurity]
```

---

## TeamCreateService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
CloseGameIfUserDoesntHavePerms() → null [RobloxScriptSecurity]
```

---

## Teams
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
GetTeams() → Instances
RebalanceTeams() → null [Deprecated]
```

---

## TelemetryService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
LogCounter(config: Dictionary, data: Dictionary?, value: float) → Variant [RobloxScriptSecurity]
LogDurationEvent(key: string) → Variant [RobloxScriptSecurity]
LogDurationEventWithTimestamp(key: string, timestamp: int64) → Variant [RobloxScriptSecurity]
LogEvent(config: Dictionary, data: Dictionary) → Variant [RobloxScriptSecurity]
LogStat(config: Dictionary, data: Dictionary?, value: float) → Variant [RobloxScriptSecurity]
```

---

## TeleportAsyncResult
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
PrivateServerId: string [ReadOnly]
ReservedServerAccessCode: string [ReadOnly]
```

---

## TeleportOptions
**Extends:** Instance

### Properties
```
ReservedServerAccessCode: string
ServerInstanceId: string
ShouldReserveServer: bool = false
```

### Functions
```
GetTeleportData() → Variant
SetTeleportData(teleportData: Variant) → null
```

---

## TeleportService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
CustomizedTeleportUI: bool [Deprecated]
```

### Functions
```
Block() → null [RobloxScriptSecurity]
GetArrivingTeleportGui() → Instance
GetLocalPlayerTeleportData() → Variant
GetTeleportSetting(setting: string) → Variant
GetThirdPartyTeleportInfo(goForth: bool) → Tuple [RobloxScriptSecurity]
SetTeleportGui(gui: Instance) → null
SetTeleportSetting(setting: string, value: Variant) → null
Teleport(placeId: int64, player: Instance, teleportData: Variant, customLoadingScreen: Instance) → null
TeleportCancel() → null [RobloxScriptSecurity]
TeleportToPlaceInstance(placeId: int64, instanceId: string, player: Instance, spawnName: string, teleportData: Variant, customLoadingScreen: Instance) → null
TeleportToPrivateServer(placeId: int64, reservedServerAccessCode: string, players: Instances, spawnName: string, teleportData: Variant, customLoadingScreen: Instance) → null
TeleportToSpawnByName(placeId: int64, spawnName: string, player: Instance, teleportData: Variant, customLoadingScreen: Instance) → null
TeleportTrustedBackForth(goForth: bool) → null [RobloxScriptSecurity]
GetPlayerPlaceInstanceAsync(userId: int64) → Tuple
ReserveServer(placeId: int64) → Tuple
TeleportAsync(placeId: int64, players: Instances, teleportOptions: Instance) → Instance
TeleportPartyAsync(placeId: int64, players: Instances, teleportData: Variant, customLoadingScreen: Instance) → string
UnblockAsync() → Tuple [RobloxScriptSecurity]
```

### Events
```
LocalPlayerArrivedFromTeleport(loadingGui: Instance, dataTable: Variant)
MenuTeleportAttempt() [RobloxScriptSecurity]
SendVIPData(player: Instance, vipServerCode: string, dmPlaceID: int64) [RobloxSecurity]
TeleportInProgress(player: Instance, teleportInfo: Dictionary) [RobloxSecurity]
TeleportInitFailed(player: Instance, teleportResult: TeleportResult, errorMessage: string, placeId: int64, teleportOptions: Instance)
TeleportInitFailedInternal(player: Instance, teleportResult: TeleportResult, errorMessage: string, guid: string) [RobloxSecurity]
```

---

## TemporaryCageMeshProvider
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## TemporaryScriptService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## TerrainDetail
**Extends:** Instance

### Properties
```
ColorMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
ColorMapContent: Content [Read:PluginSecurity] [Write:PluginSecurity]
Face: TerrainFace = Side
MaterialPattern: MaterialPattern = Regular
MetalnessMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
MetalnessMapContent: Content [Read:PluginSecurity] [Write:PluginSecurity]
NormalMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
NormalMapContent: Content [Read:PluginSecurity] [Write:PluginSecurity]
RoughnessMap: ContentId [Read:PluginSecurity] [Write:PluginSecurity]
RoughnessMapContent: Content [Read:PluginSecurity] [Write:PluginSecurity]
StudsPerTile: float = 10
TexturePack: ContentId
```

---

## TerrainRegion
**Extends:** Instance

### Properties
```
ExtentsMax: Vector3int16 = 0, 0, 0
ExtentsMin: Vector3int16 = 0, 0, 0
GridV3: BinaryString = __api_dump_write_only_property__
IsSmooth: bool = true [ReadOnly] [Deprecated]
SizeInCells: Vector3 = 1, 1, 1 [ReadOnly]
SmoothGrid: BinaryString = 
```

### Functions
```
ApplyTransform(rotation: CFrame, size: Vector3) → null [RobloxScriptSecurity]
ApplyTransformSubregion(rotation: CFrame, size: Vector3, region: Region3int16) → TerrainRegion [RobloxScriptSecurity]
ConvertToSmooth() → null [PluginSecurity] [Deprecated]
GetRegionWireframe() → Array [RobloxScriptSecurity]
```

---

## TestService
**Extends:** Instance
**Tags:** Service

### Properties
```
AutoRuns: bool = true
Description: string
ErrorCount: int = 0 [ReadOnly]
ExecuteWithStudioRun: bool = false
Is30FpsThrottleEnabled: bool = true [Deprecated]
IsPhysicsEnvironmentalThrottled: bool = true
IsSleepAllowed: bool = true
NumberOfPlayers: int = 0
SimulateSecondsLag: double = 0
TestCount: int = 0 [ReadOnly]
ThrottlePhysicsToRealtime: bool = true
Timeout: double = 10
WarnCount: int = 0 [ReadOnly]
```

### Functions
```
Check(condition: bool, description: string, source: Instance, line: int) → null
Checkpoint(text: string, source: Instance, line: int) → null
CreateAndSavePropertySet(source: Instance, fileName: string) → null [RobloxScriptSecurity]
Done() → null
Error(description: string, source: Instance, line: int) → null
Fail(description: string, source: Instance, line: int) → null
Message(text: string, source: Instance, line: int) → null
Require(condition: bool, description: string, source: Instance, line: int) → null
ScopeTime() → Dictionary
TakeSnapshot(snapshotname: string) → null
Warn(condition: bool, description: string, source: Instance, line: int) → null
isFeatureEnabled(name: string) → bool
Run() → null [PluginSecurity]
```

### Events
```
ServerCollectConditionalResult(condition: bool, text: string, script: Instance, line: int)
ServerCollectResult(text: string, script: Instance, line: int)
```

---

## TextBoxService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## TextChannel
**Extends:** Instance

### Properties
```
DirectChatRequester: Player [ReadOnly]
```

### Functions
```
DisplaySystemMessage(systemMessage: string, metadata: string) → TextChatMessage
SetDirectChatRequester(requester: Player) → null
AddUserAsync(userId: int64) → Tuple
SendAsync(message: string, metadata: string) → TextChatMessage
```

### Events
```
MessageReceived(incomingMessage: TextChatMessage)
```

---

## TextChatCommand
**Extends:** Instance

### Properties
```
AutocompleteVisible: bool = true
Enabled: bool = true
PrimaryAlias: string
SecondaryAlias: string
```

### Events
```
Triggered(originTextSource: TextSource, unfilteredText: string)
```

---

## TextChatConfigurations
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

---

## BubbleChatConfiguration
**Extends:** TextChatConfigurations
**Tags:** NotCreatable

### Properties
```
AdorneeName: string = HumanoidRootPart
BackgroundColor3: Color3 = 0.980392, 0.980392, 0.980392
BackgroundTransparency: double = 0.10000000000000000555
BubbleDuration: float = 15
BubblesSpacing: float = 6
Enabled: bool = true
Font: Font = GothamMedium
FontFace: Font
LocalPlayerStudsOffset: Vector3 = 0, 0, 0
MaxBubbles: float = 3
MaxDistance: float = 100
MinimizeDistance: float = 40
TailVisible: bool = true
TextColor3: Color3 = 0.223529, 0.231373, 0.239216
TextSize: int64 = 16
VerticalStudsOffset: float = 0
```

---

## ChannelTabsConfiguration
**Extends:** TextChatConfigurations
**Tags:** NotCreatable

### Properties
```
AbsolutePosition: Vector2 = 0, 0 [ReadOnly]
AbsoluteSize: Vector2 = 0, 0 [ReadOnly]
BackgroundColor3: Color3 = 0.0980392, 0.105882, 0.113725
BackgroundTransparency: double = 0
Enabled: bool = false
FontFace: Font
HoverBackgroundColor3: Color3 = 0.490196, 0.490196, 0.490196
SelectedTabTextColor3: Color3 = 1, 1, 1
TextColor3: Color3 = 0.686275, 0.686275, 0.686275
TextSize: int64 = 18
TextStrokeColor3: Color3 = 0, 0, 0
TextStrokeTransparency: double = 1
```

### Functions
```
SetAbsolutePosition(value: Vector2) → null [RobloxScriptSecurity]
SetAbsoluteSize(value: Vector2) → null [RobloxScriptSecurity]
```

---

## ChatInputBarConfiguration
**Extends:** TextChatConfigurations
**Tags:** NotCreatable

### Properties
```
AbsolutePosition: Vector2 = 0, 0 [ReadOnly]
AbsolutePositionWrite: Vector2 = 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AbsoluteSize: Vector2 = 0, 0 [ReadOnly]
AbsoluteSizeWrite: Vector2 = 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AutocompleteEnabled: bool = true
BackgroundColor3: Color3 = 0.0980392, 0.105882, 0.113725
BackgroundTransparency: double = 0.2000000000000000111
Enabled: bool = true
FontFace: Font
IsFocused: bool = false [ReadOnly]
IsFocusedWrite: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
KeyboardKeyCode: KeyCode = Slash
PlaceholderColor3: Color3 = 0.698039, 0.698039, 0.698039
TargetTextChannel: TextChannel
TextBox: TextBox
TextColor3: Color3 = 1, 1, 1
TextSize: int64 = 14
TextStrokeColor3: Color3 = 0, 0, 0
TextStrokeTransparency: double = 0.5
```

---

## ChatWindowConfiguration
**Extends:** TextChatConfigurations
**Tags:** NotCreatable

### Properties
```
AbsolutePosition: Vector2 = 0, 0 [ReadOnly]
AbsolutePositionWrite: Vector2 = 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
AbsoluteSize: Vector2 = 0, 0 [ReadOnly]
AbsoluteSizeWrite: Vector2 = 0, 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
BackgroundColor3: Color3 = 0.0980392, 0.105882, 0.113725
BackgroundTransparency: double = 0.2999999999999999889
Enabled: bool = true
FontFace: Font
HeightScale: float = 1
HorizontalAlignment: HorizontalAlignment = Left
TextColor3: Color3 = 1, 1, 1
TextSize: int64 = 14
TextStrokeColor3: Color3 = 0, 0, 0
TextStrokeTransparency: double = 0.5
VerticalAlignment: VerticalAlignment = Top
WidthScale: float = 1
```

### Functions
```
DeriveNewMessageProperties() → ChatWindowMessageProperties
```

---

## TextChatMessage
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
BubbleChatMessageProperties: BubbleChatMessageProperties
ChatWindowMessageProperties: ChatWindowMessageProperties
MessageId: string
Metadata: string
PrefixText: string
Status: TextChatMessageStatus
Text: string
TextChannel: TextChannel
TextSource: TextSource
Timestamp: DateTime
Translation: string
Verified: bool = false [Read:RobloxSecurity] [Write:RobloxSecurity]
```

---

## TextChatMessageProperties
**Extends:** Instance

### Properties
```
PrefixText: string
Text: string
Translation: string
```

---

## BubbleChatMessageProperties
**Extends:** TextChatMessageProperties

### Properties
```
BackgroundColor3: Color3 = 0.980392, 0.980392, 0.980392
BackgroundTransparency: double = 0.10000000000000000555
FontFace: Font
TailVisible: bool = true
TextColor3: Color3 = 0.223529, 0.231373, 0.239216
TextSize: int64 = 16
```

---

## ChatWindowMessageProperties
**Extends:** TextChatMessageProperties
**Tags:** NotCreatable

### Properties
```
FontFace: Font
PrefixTextProperties: ChatWindowMessageProperties
TextColor3: Color3 = 1, 1, 1
TextSize: int = 18
TextStrokeColor3: Color3 = 0, 0, 0
TextStrokeTransparency: double = 0.5
```

---

## TextChatService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
ChatTranslationEnabled: bool = true [Write:RobloxScriptSecurity]
ChatTranslationFTUXShown: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ChatTranslationToggleEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ChatVersion: ChatVersion = LegacyChatService [Write:RobloxScriptSecurity]
CreateDefaultCommands: bool = true [Write:PluginSecurity]
CreateDefaultTextChannels: bool = true [Write:PluginSecurity]
HasSeenDeprecationDialog: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
IsLegacyChatDisabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
DisplayBubble(partOrCharacter: Instance, message: string) → null
CanUserChatAsync(userId: int64) → bool
CanUsersChatAsync(userIdFrom: int64, userIdTo: int64) → bool
CanUsersDirectChatAsync(requesterUserId: int64, userIds: Array) → Array
CanUsersWhisperAsync(fromUserId: int64, toUserId: int64) → bool [RobloxScriptSecurity]
```

### Events
```
BubbleDisplayed(partOrCharacter: Instance, textChatMessage: TextChatMessage)
ClientToServerMessageReplicateSignalV2(text: string, metadata: string, messageId: string, textSource: TextSource, textChannel: TextChannel) [RobloxSecurity]
ClientToServerMessageReplicateSignalV3(text: string, metadata: string, messageId: string, textSource: TextSource, textChannel: TextChannel, verified: bool, isEscapedFlagEnabled: bool) [RobloxSecurity]
MessageReceived(textChatMessage: TextChatMessage)
SendingMessage(textChatMessage: TextChatMessage)
ServerToClientMessageReplicateSignal(text: string, prefixText: string, metadata: string, messageId: string, textSource: TextSource, textChannel: TextChannel, timestamp: int64, status: TextChatMessageStatus) [RobloxSecurity]
ServerToClientMessageReplicateSignalV2(data: Dictionary) [RobloxSecurity]
UpdateChatTimeout(userId: int64, startTime: int64, duration: int64) [RobloxSecurity]
```

---

## TextFilterResult
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
GetChatForUserAsync(toUserId: int64) → string [Deprecated]
GetNonChatStringForBroadcastAsync() → string
GetNonChatStringForUserAsync(toUserId: int64) → string
```

---

## TextFilterTranslatedResult
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
SourceLanguage: string [ReadOnly]
SourceText: TextFilterResult [ReadOnly]
```

### Functions
```
GetTranslationForLocale(locale: string) → TextFilterResult
GetTranslations() → Dictionary
```

---

## TextService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetFontMemoryData() → Dictionary [RobloxScriptSecurity]
GetTextSize(string: string, fontSize: int, font: Font, frameSize: Vector2) → Vector2
SetResolutionScale(scale: float) → null [RobloxScriptSecurity]
FilterAndTranslateStringAsync(stringToFilter: string, fromUserId: int64, targetLocales: Array, textContext: TextFilterContext) → TextFilterTranslatedResult
FilterStringAsync(stringToFilter: string, fromUserId: int64, textContext: TextFilterContext) → TextFilterResult
GetFamilyInfoAsync(assetId: ContentId) → Dictionary
GetTextBoundsAsync(params: GetTextBoundsParams) → Vector2
GetTextSizeOffsetAsync(fontSize: int, font: Font) → float
```

---

## TextSource
**Extends:** Instance
**Tags:** NotCreatable

### Properties
```
CanSend: bool = true
UserId: int64 = 0 [ReadOnly]
UserIdReplicated: int64 = 0
```

---

## TextureGenerationPartGroup
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
GetInstances() → Instances [RobloxScriptSecurity]
GetMeshIdsHash() → string [RobloxScriptSecurity]
```

---

## TextureGenerationService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
CancelGenerationRequest(jobUuid: string) → null [RobloxScriptSecurity]
CreatePartGroup(instances: Instances) → TextureGenerationPartGroup [RobloxScriptSecurity]
GenerateTexture(previewJobId: string) → Dictionary [RobloxScriptSecurity]
PreviewTexture(partGroup: TextureGenerationPartGroup, prompt: string, options: Dictionary) → Dictionary [RobloxScriptSecurity]
GetQuotasAsync() → Dictionary [RobloxScriptSecurity]
```

### Events
```
GenerationNotificationSignal(notificationData: Dictionary) [RobloxScriptSecurity]
PreviewNotificationSignal(notificationData: Dictionary) [RobloxScriptSecurity]
```

---

## TextureGenerationUnwrappingRequest
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Functions
```
ApplyToDataModel(partGroup: TextureGenerationPartGroup) → TextureGenerationPartGroup [RobloxScriptSecurity]
GetPartGroup() → TextureGenerationPartGroup [RobloxScriptSecurity]
```

---

## ThirdPartyUserService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
FriendCommunicationRestrictionStatus: ChatRestrictionStatus [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Functions
```
GetUserPlatformName() → string [RobloxScriptSecurity]
GetVoiceChatRestrictionStatus() → ChatRestrictionStatus [RobloxScriptSecurity]
HaveActiveUser() → bool [RobloxScriptSecurity]
IsChatRestrictionSupported() → bool [RobloxScriptSecurity]
ShowAccountPicker() → null [RobloxScriptSecurity]
RegisterActiveUser(gamepadId: UserInputType) → int [RobloxScriptSecurity]
```

### Events
```
ActiveUserSignedOut(signOutStatus: int) [RobloxScriptSecurity]
```

---

## ThreadState
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
FrameCount: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
Populated: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
ThreadId: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
ThreadName: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Functions
```
GetFrame(index: int) → Instance [RobloxScriptSecurity]
```

---

## TimerService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## ToastNotificationService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
HideNotification(notificationId: string) → null [RobloxScriptSecurity]
ShowNotification(message: string, notificationId: string) → null [RobloxScriptSecurity]
```

---

## TouchInputService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## TouchTransmitter
**Extends:** Instance
**Tags:** NotCreatable, NotBrowsable

---

## TracerService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
FinishSpan(spanId: string) → null [RobloxScriptSecurity]
StartSpan(name: string, parentId: string) → string [RobloxScriptSecurity]
```

---

## TrackerLodController
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
AudioMode: TrackerLodFlagMode
VideoExtrapolationMode: TrackerExtrapolationFlagMode
VideoLodMode: TrackerLodValueMode
VideoMode: TrackerLodFlagMode
```

### Functions
```
getExtrapolation() → int [RobloxScriptSecurity]
getVideoLod() → int [RobloxScriptSecurity]
isAudioEnabled() → bool [RobloxScriptSecurity]
isVideoEnabled() → bool [RobloxScriptSecurity]
```

### Events
```
UpdateState() [RobloxScriptSecurity]
```

---

## TrackerStreamAnimation
**Extends:** Instance
**Tags:** NotReplicated

---

## Trail
**Extends:** Instance

### Properties
```
Attachment0: Attachment
Attachment1: Attachment
Brightness: float = 1
Color: ColorSequence = 0 1 1 1 0 1 1 1 1 0 
Enabled: bool = true
FaceCamera: bool = false
Lifetime: float = 2
LightEmission: float = 0
LightInfluence: float = 0
LocalTransparencyModifier: float = 0
MaxLength: float = 0
MinLength: float = 0.100000001
Texture: ContentId
TextureLength: float = 1
TextureMode: TextureMode = Stretch
Transparency: NumberSequence = 0 0.5 0 1 0.5 0 
WidthScale: NumberSequence = 0 1 0 1 1 0 
```

### Functions
```
Clear() → null
```

### Events
```
OnClearRequested()
```

---

## Translator
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
LocaleId: string [ReadOnly]
```

### Functions
```
FormatByKey(key: string, args: Variant) → string
RobloxOnlyTranslate(context: Instance, text: string) → string [RobloxScriptSecurity]
Translate(context: Instance, text: string) → string
```

---

## TutorialService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
GetMainViewSessionId() → string [RobloxScriptSecurity]
HasUserCompletedTutorial() → bool [RobloxScriptSecurity]
HideWidgets(commaSeparatedNames: string) → bool [RobloxScriptSecurity]
PromptClosePlace() → null [RobloxScriptSecurity]
SetTutorialCompletionStatus(completed: bool) → null [RobloxScriptSecurity]
ShouldLaunchTutorial() → bool [RobloxScriptSecurity]
ShowWidgets(commaSeparatedNames: string) → bool [RobloxScriptSecurity]
```

---

## TweenBase
**Extends:** Instance
**Tags:** NotCreatable, NotBrowsable

### Properties
```
PlaybackState: PlaybackState [ReadOnly]
```

### Functions
```
Cancel() → null
Pause() → null
Play() → null
```

### Events
```
Completed(playbackState: PlaybackState)
```

---

## Tween
**Extends:** TweenBase

### Properties
```
Instance: Instance [ReadOnly]
TweenInfo: TweenInfo = Time:1 DelayTime:0 RepeatCount:0 Reverses:False EasingDirection:Out EasingStyle:Quad [ReadOnly]
```

---

## TweenService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
Create(instance: Instance, tweenInfo: TweenInfo, propertyTable: Dictionary) → Tween
GetValue(alpha: float, easingStyle: EasingStyle, easingDirection: EasingDirection) → float
SmoothDamp(current: Variant, target: Variant, velocity: Variant, smoothTime: float, maxSpeed: float?, dt: float?) → void
```

---

## UGCAvatarService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## UGCValidationService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
CalculateAverageEditableCageMeshDistance(innerCage: EditableMesh, outerCage: EditableMesh, refMesh: EditableMesh, innerTransform: CFrame, outerTransform: CFrame) → float [RobloxScriptSecurity]
CalculateBodyPartMaxCageDistance(outerCage: EditableMesh, renderMesh: EditableMesh, outerTransform: CFrame, scale: Vector3) → float [RobloxScriptSecurity]
CalculateEditableMeshInsideMeshPercentage(editableMeshRoot: EditableMesh, editableMeshQuery: EditableMesh, meshQueryTransform: CFrame, meshQueryScale: Vector3) → float [RobloxScriptSecurity]
CalculateEditableMeshModifiedCageBoundingBox(referenceUVValues: Array, innerCage: EditableMesh, innerTransform: CFrame, outerCage: EditableMesh, outerTransform: CFrame) → Tuple [RobloxScriptSecurity]
CalculateEditableMeshNumModifiedCageUVsInSet(referenceUVValues: Array, innerCage: EditableMesh, innerTransform: CFrame, outerCage: EditableMesh, outerTransform: CFrame) → Tuple [RobloxScriptSecurity]
CalculateEditableMeshTotalSurfaceArea(editableMesh: EditableMesh, meshScale: Vector3) → float [RobloxScriptSecurity]
CalculateEditableMeshUniqueUVCount(editableMesh: EditableMesh) → int [RobloxScriptSecurity]
CheckEditableMeshInCameraFrustum(editableMesh: EditableMesh, meshScale: Vector3, handleWorldCF: CFrame, cameraWorldCF: CFrame) → bool [RobloxScriptSecurity]
CreateEditableImageFromBinaryStringRobloxOnly(value: BinaryStringValue) → EditableImage [RobloxScriptSecurity]
CreateEditableMeshFromBinaryStringRobloxOnly(value: BinaryStringValue) → EditableMesh [RobloxScriptSecurity]
GetBoundingBoxManipulationData(partMeshObjects: Array, partCFs: Array, meshScales: Array) → Map [RobloxScriptSecurity]
GetDynamicHeadEditableMeshInactiveControls(editableMesh: EditableMesh, controlNames: Array) → Tuple [RobloxScriptSecurity]
GetEditableCagingRelevancyMetrics(innerCage: EditableMesh, outerCage: EditableMesh, refMesh: EditableMesh, offsetInner: Vector3, offsetOuter: Vector3) → Tuple [RobloxScriptSecurity]
GetEditableImageData(editableImage: EditableImage) → BinaryStringValue [RobloxScriptSecurity]
GetEditableImageSize(editableImage: EditableImage) → Vector2 [RobloxScriptSecurity]
GetEditableMeshMaxNearbyVerticesCollisions(editableMesh: EditableMesh, meshScale: Vector3) → int [RobloxScriptSecurity]
GetEditableMeshTriCount(editableMesh: EditableMesh) → int [RobloxScriptSecurity]
GetEditableMeshVertColors(editableMesh: EditableMesh) → Array [RobloxScriptSecurity]
GetEditableMeshVerticesSimilarityRate(editableMesh: EditableMesh, meshScale: Vector3) → float [RobloxScriptSecurity]
GetEditableMeshVerts(editableMesh: EditableMesh) → Array [RobloxScriptSecurity]
GetFacsDrivenJointNamesFromEditableMesh(editableMesh: EditableMesh) → Tuple [RobloxScriptSecurity]
GetImageTransparencyWithByteString(textureId: string) → float [RobloxScriptSecurity]
GetPropertyValue(instance: Instance, property: string) → Variant [RobloxScriptSecurity]
GetSkinnedJointNamesFromEditableMesh(editableMesh: EditableMesh) → Tuple [RobloxScriptSecurity]
IsEditableMeshNumCoplanarIntersectionsOverLimit(editableMesh: EditableMesh, limit: int, meshScale: Vector3, intersectBackFaces: bool) → bool [RobloxScriptSecurity]
RegisterAlternateMesh(alternateId: string, binaryStringValue: BinaryStringValue) → null [RobloxScriptSecurity]
RegisterUGCValidationFunction(setFunction: Function) → null [RobloxScriptSecurity]
ReportUGCValidationCounter(success: bool, validationType: string) → null [RobloxScriptSecurity]
ReportUGCValidationFailureTelemetry(errorType: string) → null [RobloxScriptSecurity]
ReportUGCValidationTelemetry(assetType: string, data: Dictionary) → null [RobloxScriptSecurity]
ResetCollisionFidelity(meshPart: Instance, collisionFidelity: CollisionFidelity) → null [RobloxScriptSecurity]
ResetCollisionFidelityWithEditableMeshDataLua(meshPart: MeshPart, editableMesh: EditableMesh, collisionFidelity: CollisionFidelity) → null [RobloxScriptSecurity]
SetMeshIdBlocking(meshPart: Instance, meshId: string) → null [RobloxScriptSecurity]
ValidateDynamicHeadEditableMesh(editableMesh: EditableMesh) → bool [RobloxScriptSecurity]
ValidateEditableImageSize(editableImage: EditableImage) → bool [RobloxScriptSecurity]
ValidateEditableMeshCageMeshIntersection(innerCage: EditableMesh, outerCage: EditableMesh, refMesh: EditableMesh) → Tuple [RobloxScriptSecurity]
ValidateEditableMeshCageNonManifoldAndHoles(editableMesh: EditableMesh) → Tuple [RobloxScriptSecurity]
ValidateEditableMeshCageUVCoincident(editableMesh: EditableMesh) → bool [RobloxScriptSecurity]
ValidateEditableMeshCageUVTriangleArea(editableMesh: EditableMesh) → bool [RobloxScriptSecurity]
ValidateEditableMeshFacialBounds(editableMesh: EditableMesh, boundsScale: float, partSize: Vector3) → bool [RobloxScriptSecurity]
ValidateEditableMeshFacialExpressiveness(editableMesh: EditableMesh, minDelta: float, partSize: Vector3) → float [RobloxScriptSecurity]
ValidateEditableMeshFullBodyCageDeletion(editableMesh: EditableMesh) → bool [RobloxScriptSecurity]
ValidateEditableMeshMisMatchUV(innerCage: EditableMesh, outerCage: EditableMesh) → bool [RobloxScriptSecurity]
ValidateEditableMeshOverlappingVertices(editableMesh: EditableMesh) → bool [RobloxScriptSecurity]
ValidateEditableMeshTriangleArea(editableMesh: EditableMesh) → bool [RobloxScriptSecurity]
ValidateEditableMeshTriangles(editableMesh: EditableMesh) → bool [RobloxScriptSecurity]
ValidateEditableMeshUVDuplicates(referenceValues: Array, editableMesh: EditableMesh) → int [RobloxScriptSecurity]
ValidateEditableMeshUVSpace(editableMesh: EditableMesh) → bool [RobloxScriptSecurity]
ValidateEditableMeshUVValuesInReference(referenceValues: Array, editableMesh: EditableMesh) → bool [RobloxScriptSecurity]
ValidateEditableMeshUniqueUVCount(editableMesh: EditableMesh, numRequired: int) → bool [RobloxScriptSecurity]
ValidateEditableMeshVertColors(editableMesh: EditableMesh, includeAlpha: bool) → bool [RobloxScriptSecurity]
ValidatePartBBoxAfterFullFacs(headEditableMesh: EditableMesh, partEditableMesh: EditableMesh, headScale: Vector3, partScale: Vector3, boundsMaxMultiplier: float) → bool [RobloxScriptSecurity]
ValidateSkinnedEditableMesh(editableMesh: EditableMesh) → bool [RobloxScriptSecurity]
CalculateBodyMaxCageDistance(inputBodyParts: Array) → Tuple [RobloxScriptSecurity]
CanLoadAsset(assetId: string) → bool [RobloxScriptSecurity]
CompareTextureOverlapByteString(byteStringBaseline: string, byteStringFollowup: string) → Array [RobloxScriptSecurity]
CompareTextureOverlapTextureId(textureIdBaseline: string, textureIdFollowup: string) → Array [RobloxScriptSecurity]
DoesMeshHaveSkinningData(meshId: string) → bool [RobloxScriptSecurity]
FetchAssetWithFormat(url: ContentId, assetFormat: string) → Instances [RobloxScriptSecurity]
GetCagingRelevancyMetrics(innerCageMeshId: string, outerCageMeshId: string, refMeshId: string, offsetInner: Vector3, offsetOuter: Vector3) → Tuple [RobloxScriptSecurity]
GetDynamicHeadMeshInactiveControls(meshId: string, controlNames: Array) → Tuple [RobloxScriptSecurity]
GetFacsDrivenJointNamesFromMeshId(meshId: string) → Tuple [RobloxScriptSecurity]
GetImageTransparencyWithTextureID(textureId: string) → float [RobloxScriptSecurity]
GetMaxNearbyVerticesCollisions(meshId: string, meshScale: Vector3) → int [RobloxScriptSecurity]
GetMeshDataBinaryString(meshId: string) → BinaryStringValue [RobloxScriptSecurity]
GetMeshTriCount(meshId: string) → int [RobloxScriptSecurity]
GetMeshVertColors(meshId: string) → Array [RobloxScriptSecurity]
GetMeshVerts(meshId: string) → Array [RobloxScriptSecurity]
GetSkinnedJointNamesFromMeshId(meshId: string) → Tuple [RobloxScriptSecurity]
GetTextureSize(textureId: string) → Vector2 [RobloxScriptSecurity]
IsDeformedLayeredClothingOutOfRenderBounds(accessory: Accessory) → bool [RobloxScriptSecurity]
ValidateCageMeshIntersection(innerCageMeshId: string, outerCageMeshId: string, refMeshId: string) → Tuple [RobloxScriptSecurity]
ValidateCageUVCoincident(meshId: string) → bool [RobloxScriptSecurity]
ValidateCageUVTriangleArea(meshId: string) → bool [RobloxScriptSecurity]
ValidateDynamicHeadMesh(meshId: string) → bool [RobloxScriptSecurity]
ValidateFacialBounds(meshId: string, boundsScale: float, partSize: Vector3) → bool [RobloxScriptSecurity]
ValidateFacialExpressiveness(meshId: string, minDelta: float, partSize: Vector3) → float [RobloxScriptSecurity]
ValidateImageTransparencyThresholdByteString(image: string, threshold: float) → bool [RobloxScriptSecurity]
ValidateImageTransparencyThresholdByteString_V2(image: string, threshold: float) → bool [RobloxScriptSecurity]
ValidateImageTransparencyThresholdTextureID(textureId: string, threshold: float) → bool [RobloxScriptSecurity]
ValidateImageTransparencyThresholdTextureID_V2(textureId: string, threshold: float) → bool [RobloxScriptSecurity]
ValidateMeshVertColors(meshId: string, includeAlpha: bool) → bool [RobloxScriptSecurity]
ValidateOverlappingVertices(meshId: string) → bool [RobloxScriptSecurity]
ValidatePartBBoxAfterFullFacsFromMeshIds(headMeshId: string, partMeshId: string, headScale: Vector3, partScale: Vector3, boundsMaxMultiplier: float) → bool [RobloxScriptSecurity]
ValidateSkinnedMesh(meshId: string) → bool [RobloxScriptSecurity]
ValidateTextureAlpha(textureId: string, pixelWidth: int) → bool [RobloxScriptSecurity]
ValidateTextureAlphaByteString(byteString: string, pixelWidth: int) → bool [RobloxScriptSecurity]
ValidateUVValuesInReference(referenceValues: Array, meshId: string) → bool [RobloxScriptSecurity]
```

---

## UIBase
**Extends:** Instance
**Tags:** NotCreatable

---

## UIComponent
**Extends:** UIBase
**Tags:** NotCreatable

---

## UIConstraint
**Extends:** UIComponent
**Tags:** NotCreatable

---

## UIAspectRatioConstraint
**Extends:** UIConstraint

### Properties
```
AspectRatio: float = 1
AspectType: AspectType = FitWithinMaxSize
DominantAxis: DominantAxis = Width
```

---

## UISizeConstraint
**Extends:** UIConstraint

### Properties
```
MaxSize: Vector2 = INF, INF
MinSize: Vector2 = 0, 0
```

---

## UITextSizeConstraint
**Extends:** UIConstraint

### Properties
```
MaxTextSize: int = 100
MinTextSize: int = 1
```

---

## UIContainerQuery
**Extends:** UIComponent
**Tags:** NotReplicated, NotBrowsable

### Properties
```
AspectRatioRange: NumberRange = 0 inf 
IsActive: bool = true
MaxSize: Vector2 = INF, INF
MinSize: Vector2 = 0, 0
```

---

## UICorner
**Extends:** UIComponent

### Properties
```
CornerRadius: UDim = 0, 8
```

---

## UIDragDetector
**Extends:** UIComponent

### Properties
```
ActivatedCursorIcon: ContentId
BoundingBehavior: UIDragDetectorBoundingBehavior = Automatic
BoundingUI: GuiBase2d
CursorIcon: ContentId
DragAxis: Vector2 = 1, 0
DragRelativity: UIDragDetectorDragRelativity = Absolute
DragRotation: float = 0
DragSpace: UIDragDetectorDragSpace = Parent
DragStyle: UIDragDetectorDragStyle = TranslatePlane
DragUDim2: UDim2 = {0, 0}, {0, 0}
Enabled: bool = true
MaxDragAngle: float = 0
MaxDragTranslation: UDim2 = {0, 0}, {0, 0}
MinDragAngle: float = 0
MinDragTranslation: UDim2 = {0, 0}, {0, 0}
ReferenceUIInstance: GuiObject
ResponseStyle: UIDragDetectorResponseStyle = Offset
SelectionModeDragSpeed: UDim2 = {0, 300}, {0, 300}
SelectionModeRotateSpeed: float = 90
UIDragSpeedAxisMapping: UIDragSpeedAxisMapping = XY
```

### Functions
```
AddConstraintFunction(priority: int, function: Function) → RBXScriptConnection
GetReferencePosition() → UDim2
GetReferenceRotation() → float
SetDragStyleFunction(function: Function) → null
```

### Events
```
DragContinue(inputPosition: Vector2)
DragEnd(inputPosition: Vector2)
DragStart(inputPosition: Vector2)
```

---

## UIFlexItem
**Extends:** UIComponent

### Properties
```
FlexMode: UIFlexMode = None
GrowRatio: float = 0
ItemLineAlignment: ItemLineAlignment = Automatic
ShrinkRatio: float = 0
```

---

## UIGradient
**Extends:** UIComponent

### Properties
```
Color: ColorSequence = 0 1 1 1 0 1 1 1 1 0 
Enabled: bool = true
Offset: Vector2 = 0, 0
Rotation: float = 0
Transparency: NumberSequence = 0 0 0 1 0 0 
```

---

## UILayout
**Extends:** UIComponent
**Tags:** NotCreatable

---

## UIGridStyleLayout
**Extends:** UILayout
**Tags:** NotCreatable, NotBrowsable

### Properties
```
AbsoluteContentSize: Vector2 [ReadOnly]
FillDirection: FillDirection
HorizontalAlignment: HorizontalAlignment
SortOrder: SortOrder
VerticalAlignment: VerticalAlignment
```

### Functions
```
ApplyLayout() → null [Deprecated]
SetCustomSortFunction(function: Function) → null [Deprecated]
```

---

## UIGridLayout
**Extends:** UIGridStyleLayout

### Properties
```
AbsoluteCellCount: Vector2 = 0, 0 [ReadOnly]
AbsoluteCellSize: Vector2 = 100, 100 [ReadOnly]
CellPadding: UDim2 = {0, 5}, {0, 5}
CellSize: UDim2 = {0, 100}, {0, 100}
FillDirectionMaxCells: int = 0
StartCorner: StartCorner = TopLeft
```

---

## UIListLayout
**Extends:** UIGridStyleLayout

### Properties
```
HorizontalFlex: UIFlexAlignment = None
HorizontalPadding: UDim = 0, 0
ItemLineAlignment: ItemLineAlignment = Automatic
Padding: UDim = 0, 0
VerticalFlex: UIFlexAlignment = None
VerticalPadding: UDim = 0, 0
Wraps: bool = false
```

---

## UIPageLayout
**Extends:** UIGridStyleLayout

### Properties
```
Animated: bool = true
Circular: bool = false
CurrentPage: GuiObject [ReadOnly]
EasingDirection: EasingDirection = Out
EasingStyle: EasingStyle = Back
GamepadInputEnabled: bool = true
Padding: UDim = 0, 0
ScrollWheelInputEnabled: bool = true
TouchInputEnabled: bool = true
TweenTime: float = 1
```

### Functions
```
JumpTo(page: Instance) → null
JumpToIndex(index: int) → null
Next() → null
Previous() → null
```

### Events
```
PageEnter(page: Instance)
PageLeave(page: Instance)
Stopped(currentPage: Instance)
```

---

## UITableLayout
**Extends:** UIGridStyleLayout

### Properties
```
FillEmptySpaceColumns: bool = false
FillEmptySpaceRows: bool = false
MajorAxis: TableMajorAxis = RowMajor
Padding: UDim2 = {0, 0}, {0, 0}
```

---

## UIPadding
**Extends:** UIComponent

### Properties
```
PaddingBottom: UDim = 0, 0
PaddingLeft: UDim = 0, 0
PaddingRight: UDim = 0, 0
PaddingTop: UDim = 0, 0
```

---

## UIScale
**Extends:** UIComponent

### Properties
```
Scale: float = 1
```

---

## UIStroke
**Extends:** UIComponent

### Properties
```
ApplyStrokeMode: ApplyStrokeMode = Contextual
BorderOffset: UDim = 0, 0
BorderStrokePosition: BorderStrokePosition = Outer
Color: Color3 = 0, 0, 0
Enabled: bool = true
LineJoinMode: LineJoinMode = Round
StrokeSizingMode: StrokeSizingMode = FixedSize
Thickness: float = 1
Transparency: float = 0
ZIndex: int = 1
```

---

## UIDragDetectorService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## UniqueIdLookupService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
GetInstanceByRfc4122String(id: string) → Instance [RobloxScriptSecurity]
```

---

## UnvalidatedAssetService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
CachedData: string = {"lastSaveTime":0,"lastKnownPublishRequest":0,"users":[]} [Read:RobloxSecurity] [Write:RobloxSecurity]
```

### Functions
```
AppendTempAssetId(userId: int64, id: int64, lookAt: Vector3, camPos: Vector3, usage: string) → null [RobloxScriptSecurity]
AppendVantagePoint(userId: int64, id: int64, lookAt: Vector3, camPos: Vector3) → bool [RobloxScriptSecurity]
UpgradeTempAssetId(userId: int64, tempId: int64, assetId: int64) → bool [RobloxScriptSecurity]
```

---

## UserGameSettings
**Extends:** Instance
**Tags:** NotCreatable, UserSettings, NotReplicated

### Properties
```
AllTutorialsDisabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CameraMode: CustomCameraMode [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CameraYInverted: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ChatTranslationEnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ChatTranslationFTUXShown: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ChatTranslationLocale: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ChatTranslationToggleEnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ChatVisible: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CompletedTutorials: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ComputerCameraMovementChanged: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
ComputerCameraMovementMode: ComputerCameraMovementMode
ComputerMovementChanged: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
ComputerMovementMode: ComputerMovementMode
ControlMode: ControlMode
DefaultCameraID: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
FramerateCap: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Fullscreen: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GamepadCameraSensitivity: float
GraphicsOptimizationMode: GraphicsOptimizationMode [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
GraphicsQualityLevel: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
HapticStrength: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
HasEverUsedVR: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
IsUsingCameraYInverted: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
IsUsingGamepadCameraSensitivity: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
MasterVolume: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
MasterVolumeStudio: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
MaxQualityEnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
MicroProfilerWebServerEnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
MicroProfilerWebServerIP: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
MicroProfilerWebServerPort: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
MouseSensitivity: float
MouseSensitivityFirstPerson: Vector2 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
MouseSensitivityThirdPerson: Vector2 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
OnScreenProfilerEnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
OnboardingsCompleted: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
PartyVoiceVolume: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
PerformanceStatsVisible: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
PlayerHeight: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
PreferredTextSize: PreferredTextSize [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
PreferredTransparency: float [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
QualityResetLevel: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
RCCProfilerRecordFrameRate: int
RCCProfilerRecordTimeFrame: int
ReadAloud: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ReducedMotion: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
RotationType: RotationType
SavedQualityLevel: SavedQualitySetting
StartMaximized: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
StartScreenPosition: Vector2 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
StartScreenSize: Vector2 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
TouchCameraMovementChanged: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
TouchCameraMovementMode: TouchCameraMovementMode
TouchMovementChanged: bool [Read:RobloxSecurity] [Write:RobloxSecurity]
TouchMovementMode: TouchMovementMode
UiNavigationKeyBindEnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
UsedCoreGuiIsVisibleToggle: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
UsedCustomGuiIsVisibleToggle: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
UsedHideHudShortcut: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
VRComfortSetting: VRComfortSetting [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
VREnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
VRRotationIntensity: int [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
VRSafetyBubbleMode: VRSafetyBubbleMode [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
VRSmoothRotationEnabled: bool [Write:RobloxScriptSecurity]
VRSmoothRotationEnabledCustomOption: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
VRThirdPersonFollowCamEnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
VRThirdPersonFollowCamEnabledCustomOption: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
VignetteEnabled: bool [Write:RobloxScriptSecurity]
VignetteEnabledCustomOption: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
gaID: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
GetCameraYInvertValue() → int
GetDefaultFramerateCap() → int [RobloxScriptSecurity]
GetOnboardingCompleted(onboardingId: string) → bool
GetTutorialState(tutorialId: string) → bool [RobloxScriptSecurity]
InFullScreen() → bool
InStudioMode() → bool
ResetOnboardingCompleted(onboardingId: string) → null [RobloxScriptSecurity]
SetCameraYInvertVisible() → null
SetGamepadCameraSensitivityVisible() → null
SetOnboardingCompleted(onboardingId: string) → null
SetTutorialState(tutorialId: string, value: bool) → null [RobloxScriptSecurity]
```

### Events
```
FullscreenChanged(isFullscreen: bool)
PerformanceStatsVisibleChanged(isPerformanceStatsVisible: bool) [RobloxScriptSecurity]
StudioModeChanged(isStudioMode: bool)
```

---

## UserInputService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Properties
```
AccelerometerEnabled: bool [ReadOnly]
BottomBarSize: Vector2 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
GamepadEnabled: bool [ReadOnly]
GyroscopeEnabled: bool [ReadOnly]
KeyboardEnabled: bool [ReadOnly]
LegacyInputEventsEnabled: bool [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [Deprecated]
ModalEnabled: bool [Deprecated]
MouseBehavior: MouseBehavior
MouseDeltaSensitivity: float
MouseEnabled: bool [ReadOnly]
MouseIcon: ContentId
MouseIconEnabled: bool
NavBarSize: Vector2 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
OnScreenKeyboardAnimationDuration: double [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
OnScreenKeyboardPosition: Vector2 [ReadOnly]
OnScreenKeyboardSize: Vector2 [ReadOnly]
OnScreenKeyboardVisible: bool [ReadOnly]
OverrideMouseIconBehavior: OverrideMouseIconBehavior [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
PreferredInput: PreferredInput [ReadOnly]
RightBarSize: Vector2 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
StatusBarSize: Vector2 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
TouchEnabled: bool [ReadOnly]
UserHeadCFrame: CFrame [ReadOnly] [Deprecated]
VREnabled: bool [ReadOnly]
```

### Functions
```
GamepadSupports(gamepadNum: UserInputType, gamepadKeyCode: KeyCode) → bool
GetConnectedGamepads() → Array
GetDeviceAcceleration() → InputObject
GetDeviceGravity() → InputObject
GetDeviceLevel() → DeviceLevel [RobloxScriptSecurity]
GetDeviceRotation() → Tuple
GetDeviceType() → DeviceType [RobloxScriptSecurity]
GetFocusedTextBox() → TextBox
GetGamepadConnected(gamepadNum: UserInputType) → bool
GetGamepadState(gamepadNum: UserInputType) → Array
GetImageForKeyCode(keyCode: KeyCode) → ContentId
GetKeysPressed() → Array
GetLastInputType() → UserInputType
GetMouseButtonsPressed() → Array
GetMouseDelta() → Vector2
GetMouseLocation() → Vector2
GetNavigationGamepads() → Array
GetPasteText() → string [RobloxScriptSecurity]
GetPlatform() → Platform [RobloxScriptSecurity]
GetStringForKeyCode(keyCode: KeyCode) → string
GetSupportedGamepadKeyCodes(gamepadNum: UserInputType) → Array
GetUserCFrame(type: UserCFrame) → CFrame [Deprecated]
IsGamepadButtonDown(gamepadNum: UserInputType, gamepadKeyCode: KeyCode) → bool
IsKeyDown(keyCode: KeyCode) → bool
IsMouseButtonPressed(mouseButton: UserInputType) → bool
IsNavigationGamepad(gamepadEnum: UserInputType) → bool
RecenterUserHeadCFrame() → null
SendAppUISizes(statusBarSize: Vector2, navBarSize: Vector2, bottomBarSize: Vector2, rightBarSize: Vector2) → null [RobloxScriptSecurity]
SetNavigationGamepad(gamepadEnum: UserInputType, enabled: bool) → null
```

### Events
```
DeviceAccelerationChanged(acceleration: InputObject)
DeviceGravityChanged(gravity: InputObject)
DeviceRotationChanged(rotation: InputObject, cframe: CFrame)
GamepadConnected(gamepadNum: UserInputType)
GamepadDisconnected(gamepadNum: UserInputType)
InputBegan(input: InputObject, gameProcessedEvent: bool)
InputChanged(input: InputObject, gameProcessedEvent: bool)
InputEnded(input: InputObject, gameProcessedEvent: bool)
JumpRequest()
LastInputTypeChanged(lastInputType: UserInputType)
PointerAction(wheel: float, pan: Vector2, pinch: float, gameProcessedEvent: bool)
StatusBarTapped(position: Vector2) [RobloxScriptSecurity]
TextBoxFocusReleased(textboxReleased: TextBox)
TextBoxFocused(textboxFocused: TextBox)
TouchDrag(dragDirection: SwipeDirection, numberOfTouches: int, gameProcessedEvent: bool)
TouchEnded(touch: InputObject, gameProcessedEvent: bool)
TouchLongPress(touchPositions: Array, state: UserInputState, gameProcessedEvent: bool)
TouchMoved(touch: InputObject, gameProcessedEvent: bool)
TouchPan(touchPositions: Array, totalTranslation: Vector2, velocity: Vector2, state: UserInputState, gameProcessedEvent: bool)
TouchPinch(touchPositions: Array, scale: float, velocity: float, state: UserInputState, gameProcessedEvent: bool)
TouchRotate(touchPositions: Array, rotation: float, velocity: float, state: UserInputState, gameProcessedEvent: bool)
TouchStarted(touch: InputObject, gameProcessedEvent: bool)
TouchSwipe(swipeDirection: SwipeDirection, numberOfTouches: int, gameProcessedEvent: bool)
TouchTap(touchPositions: Array, gameProcessedEvent: bool)
TouchTapInWorld(position: Vector2, processedByUI: bool)
UserCFrameChanged(type: UserCFrame, value: CFrame)
WindowFocusReleased()
WindowFocused()
```

---

## UserService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Functions
```
GetUserInfosByUserIdsAsync(userIds: Array) → Array
```

---

## VRService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
AutomaticScaling: VRScaling = World
AvatarGestures: bool = false
ControllerModels: VRControllerModelMode = Transparent
DidPointerHit: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
FadeOutViewOnCollision: bool = true
GuiInputUserCFrame: UserCFrame = Head
LaserDistance: float = 50 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
LaserPointer: VRLaserPointerMode = Pointer
PointerHitCFrame: CFrame [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
QuestASWState: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
QuestDisplayRefreshRate: float = 0 [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ThirdPersonFollowCamEnabled: bool = true [ReadOnly]
VRDeviceAvailable: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
VRDeviceName: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
VREnabled: bool = false [ReadOnly]
VRSessionState: VRSessionState = Undefined [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity] [ReadOnly]
```

### Functions
```
GetTouchpadMode(pad: VRTouchpad) → VRTouchpadMode
GetUserCFrame(type: UserCFrame) → CFrame
GetUserCFrameEnabled(type: UserCFrame) → bool
IsMaquettes() → bool [RobloxScriptSecurity]
IsVRAppBuild() → bool [RobloxScriptSecurity]
RecenterUserHeadCFrame() → null
RequestNavigation(cframe: CFrame, inputUserCFrame: UserCFrame) → null
SetTouchpadMode(pad: VRTouchpad, mode: VRTouchpadMode) → null
```

### Events
```
LaserPointerTriggered(input: InputObject) [RobloxScriptSecurity]
NavigationRequested(cframe: CFrame, inputUserCFrame: UserCFrame)
TouchpadModeChanged(pad: VRTouchpad, mode: VRTouchpadMode)
UserCFrameChanged(type: UserCFrame, value: CFrame)
UserCFrameEnabled(type: UserCFrame, enabled: bool)
```

---

## VRStatusService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## ValueBase
**Extends:** Instance
**Tags:** NotCreatable

---

## BinaryStringValue
**Extends:** ValueBase

### Properties
```
Value: BinaryString
```

### Events
```
Changed(value: BinaryString)
```

---

## BoolValue
**Extends:** ValueBase

### Properties
```
Value: bool = false
```

### Events
```
Changed(value: bool)
changed(value: bool)
```

---

## BrickColorValue
**Extends:** ValueBase

### Properties
```
Value: BrickColor
```

### Events
```
Changed(value: BrickColor)
changed(value: BrickColor)
```

---

## CFrameValue
**Extends:** ValueBase

### Properties
```
Value: CFrame
```

### Events
```
Changed(value: CFrame)
changed(value: CFrame)
```

---

## Color3Value
**Extends:** ValueBase

### Properties
```
Value: Color3 = 0, 0, 0
```

### Events
```
Changed(value: Color3)
changed(value: Color3)
```

---

## DoubleConstrainedValue
**Extends:** ValueBase
**Tags:** Deprecated

### Properties
```
ConstrainedValue: double = 0
MaxValue: double = 1
MinValue: double = 0
Value: double = 0
value: double = 0
```

### Events
```
Changed(value: double)
changed(value: double)
```

---

## IntConstrainedValue
**Extends:** ValueBase
**Tags:** Deprecated

### Properties
```
ConstrainedValue: int64 = 0
MaxValue: int64 = 10
MinValue: int64 = 0
Value: int64 = 0
value: int64 = 0
```

### Events
```
Changed(value: int64)
changed(value: int64)
```

---

## IntValue
**Extends:** ValueBase

### Properties
```
Value: int64 = 0
```

### Events
```
Changed(value: int64)
changed(value: int64)
```

---

## NumberValue
**Extends:** ValueBase

### Properties
```
Value: double = 0
```

### Events
```
Changed(value: double)
changed(value: double)
```

---

## ObjectValue
**Extends:** ValueBase

### Properties
```
Value: Instance
```

### Events
```
Changed(value: Instance)
changed(value: Instance)
```

---

## RayValue
**Extends:** ValueBase

### Properties
```
Value: Ray = {0, 0, 0}, {0, 0, 0}
```

### Events
```
Changed(value: Ray)
changed(value: Ray)
```

---

## StringValue
**Extends:** ValueBase

### Properties
```
Value: string
```

### Events
```
Changed(value: string)
changed(value: string)
```

---

## Vector3Value
**Extends:** ValueBase

### Properties
```
Value: Vector3 = 0, 0, 0
```

### Events
```
Changed(value: Vector3)
changed(value: Vector3)
```

---

## Vector3Curve
**Extends:** Instance

### Functions
```
GetValueAtTime(time: float) → Array
X() → FloatCurve
Y() → FloatCurve
Z() → FloatCurve
```

---

## VersionControlService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
ScriptCollabEnabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ScriptCollabVersionHistoryEnabled: bool = false [Read:RobloxSecurity] [Write:RobloxSecurity]
```

### Events
```
BroadcastScriptChangesSubmitted(scriptGuid: string) [RobloxSecurity]
CommitRejectedInfo(reason: int) [LocalUserSecurity]
LockedScriptBatchCommit(scriptGuidTuple: Tuple, scriptTextTuple: Tuple, commitMessage: string) [LocalUserSecurity]
RequestAllEditorsSignal() [LocalUserSecurity]
ScriptBatchCommit(scriptGuidTuple: Tuple, scriptHashBaseTuple: Tuple, scriptTextTuple: Tuple, commitMessage: string) [LocalUserSecurity]
ScriptChangesSubmitted(scriptGuid: string, submitted: bool) [LocalUserSecurity]
ScriptEditorAdded(scriptGuid: string, editor: Instance) [LocalUserSecurity]
ScriptEditorRemoved(scriptGuid: string, editor: Instance) [LocalUserSecurity]
ScriptStartEdit(scriptGuid: string) [LocalUserSecurity]
ScriptStopEdit(scriptGuid: string) [LocalUserSecurity]
```

---

## VideoCaptureService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
Active: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
CameraID: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
GetCameraDevices() → Map [RobloxScriptSecurity]
```

### Events
```
DevicesChanged() [RobloxScriptSecurity]
Error(cameraid: string, errorcode: string) [RobloxScriptSecurity]
Started(cameraid: string) [RobloxScriptSecurity]
Stopped(cameraid: string) [RobloxScriptSecurity]
```

---

## VideoDeviceInput
**Extends:** Instance
**Tags:** NotReplicated

### Properties
```
Active: bool = false
CameraId: string
CaptureQuality: VideoDeviceCaptureQuality = Default
IsReady: bool = false [ReadOnly]
```

---

## VideoPlayer
**Extends:** Instance
**Tags:** NotBrowsable

### Properties
```
Asset: ContentId
AutoLoadInStudio: bool = false [Write:RobloxScriptSecurity]
AutoPlayInStudio: bool = false [Write:RobloxScriptSecurity]
IsLoaded: bool = false [ReadOnly]
IsPlaying: bool = false [ReadOnly]
Looping: bool = false
PlaybackSpeed: float = 1
Resolution: Vector2 = 0, 0 [ReadOnly]
TimeLength: double = 0 [ReadOnly]
TimePosition: double = 0
Volume: float = 1
```

### Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
Pause() → null
Play() → null
SetStudioPreview(isPreview: bool) → null [RobloxScriptSecurity]
Unload() → null
LoadAsync() → AssetFetchStatus
```

### Events
```
DidEnd()
DidLoop()
PlayFailed(error: AssetFetchStatus)
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

## VideoService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## VirtualInputManager
**Extends:** Instance
**Tags:** Service

### Properties
```
AdditionalLuaState: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
Dump() → null [RobloxScriptSecurity]
HandleGamepadAxisInput(objectId: int, keyCode: KeyCode, x: float, y: float, z: float) → null [RobloxScriptSecurity]
HandleGamepadButtonInput(deviceId: int, keyCode: KeyCode, buttonState: int) → null [RobloxScriptSecurity]
HandleGamepadConnect(deviceId: int) → null [RobloxScriptSecurity]
HandleGamepadDisconnect(deviceId: int) → null [RobloxScriptSecurity]
SendAccelerometerEvent(x: float, y: float, z: float) → null [RobloxScriptSecurity]
SendGravityEvent(x: float, y: float, z: float) → null [RobloxScriptSecurity]
SendGyroscopeEvent(quatX: float, quatY: float, quatZ: float, quatW: float) → null [RobloxScriptSecurity]
SendKeyEvent(isPressed: bool, keyCode: KeyCode, isRepeatedKey: bool, layerCollector: Instance) → null [RobloxScriptSecurity]
SendMouseButtonEvent(x: int, y: int, mouseButton: int, isDown: bool, layerCollector: Instance, repeatCount: int) → null [RobloxScriptSecurity]
SendMouseMoveDeltaEvent(deltaX: float, deltaY: float, layerCollector: Instance) → null [RobloxScriptSecurity]
SendMouseMoveEvent(x: float, y: float, layerCollector: Instance) → null [RobloxScriptSecurity]
SendMouseWheelEvent(x: float, y: float, isForwardScroll: bool, layerCollector: Instance) → null [RobloxScriptSecurity]
SendScroll(x: float, y: float, deltaX: float, deltaY: float, options: Dictionary, layerCollector: Instance) → null [RobloxScriptSecurity]
SendTextInputCharacterEvent(str: string, layerCollector: Instance) → null [RobloxScriptSecurity]
SendTouchEvent(touchId: int64, state: int, x: float, y: float) → null [RobloxScriptSecurity]
SetInputTypesToIgnore(inputTypesToIgnore: Variant) → null [RobloxScriptSecurity]
StartPlaying(fileName: string) → null [RobloxScriptSecurity]
StartPlayingJSON(string: string) → null [RobloxScriptSecurity]
StartRecording() → null [RobloxScriptSecurity]
StopPlaying() → null [RobloxScriptSecurity]
StopRecording() → null [RobloxScriptSecurity]
sendRobloxEvent(namespace: string, detail: string, detailType: string) → null [RobloxScriptSecurity]
sendThemeChangeEvent(themeName: string) → null [RobloxScriptSecurity]
WaitForInputEventsProcessed() → null [RobloxScriptSecurity]
```

### Events
```
PlaybackCompleted(additionalLuaState: string) [RobloxScriptSecurity]
RecordingCompleted(result: string) [RobloxScriptSecurity]
```

---

## VirtualUser
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
Button1Down(position: Vector2, camera: CFrame) → null [LocalUserSecurity]
Button1Up(position: Vector2, camera: CFrame) → null [LocalUserSecurity]
Button2Down(position: Vector2, camera: CFrame) → null [LocalUserSecurity]
Button2Up(position: Vector2, camera: CFrame) → null [LocalUserSecurity]
CaptureController() → null [LocalUserSecurity]
ClickButton1(position: Vector2, camera: CFrame) → null [LocalUserSecurity]
ClickButton2(position: Vector2, camera: CFrame) → null [LocalUserSecurity]
MoveMouse(position: Vector2, camera: CFrame) → null [LocalUserSecurity]
SetKeyDown(key: string) → null [LocalUserSecurity]
SetKeyUp(key: string) → null [LocalUserSecurity]
StartRecording() → null [LocalUserSecurity]
StopRecording() → string [LocalUserSecurity]
TypeKey(key: string) → null [LocalUserSecurity]
```

---

## VisibilityCheckDispatcher
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## Visit
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

---

## VisualizationMode
**Extends:** Instance

### Properties
```
Enabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Title: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
ToolTip: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

---

## VisualizationModeCategory
**Extends:** Instance

### Properties
```
Enabled: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
Title: string [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

---

## VisualizationModeService
**Extends:** Instance
**Tags:** NotCreatable, Service

---

## VoiceChatInternal
**Extends:** Instance
**Tags:** NotCreatable, Service, NotBrowsable

### Properties
```
VoiceChatState: VoiceChatState = Idle [ReadOnly] [Deprecated]
```

### Functions
```
GetAndClearCallFailureMessage() → string [RobloxScriptSecurity] [Deprecated]
GetAudioProcessingSettings() → Tuple [Deprecated]
GetChannelId() → string [RobloxScriptSecurity]
GetGroupId() → string [RobloxScriptSecurity]
GetMicDevices() → Tuple [Deprecated]
GetParticipants() → Array [Deprecated]
GetSessionId() → string [RobloxScriptSecurity]
GetSpeakerDevices() → Tuple [Deprecated]
GetVoiceChatApiVersion() → int [Deprecated]
GetVoiceChatAvailable() → int [Deprecated]
GetVoiceExperienceId() → string [RobloxScriptSecurity]
IsContextVoiceEnabled() → bool [RobloxScriptSecurity]
IsPublishPaused() → bool [Deprecated]
IsSubscribePaused(userId: int64) → bool [Deprecated]
JoinByGroupId(groupId: string, isMicMuted: bool) → bool [Deprecated]
JoinByGroupIdToken(groupId: string, isMicMuted: bool, isRetry: bool) → bool [Deprecated]
Leave() → null [Deprecated]
LogPublisherWebRTCStats() → bool [RobloxScriptSecurity]
LogSubscriptionWebRTCStats() → bool [RobloxScriptSecurity]
PublishPause(paused: bool) → bool [Deprecated]
SetMicDevice(micDeviceName: string, micDeviceGuid: string) → null [Deprecated]
SetSpeakerDevice(speakerDeviceName: string, speakerDeviceGuid: string) → null [Deprecated]
SubscribeBlock(userId: int64) → bool [RobloxScriptSecurity]
SubscribePause(userId: int64, paused: bool) → bool [Deprecated]
SubscribePauseAll(paused: bool) → bool [Deprecated]
SubscribeRetry(userId: int64) → bool [RobloxScriptSecurity]
SubscribeUnblock(userId: int64) → bool [RobloxScriptSecurity]
IsVoiceEnabledForUserIdAsync(userId: int64) → bool
```

### Events
```
LocalPlayerModerated() [RobloxScriptSecurity]
ParticipantsStateChanged(participantsLeft: Array, participantsJoined: Array, updatedStates: Array) [RobloxScriptSecurity]
PlayerMicActivitySignalChange(activityInfo: Dictionary) [RobloxScriptSecurity]
StateChanged(old: VoiceChatState, new: VoiceChatState)
TempSetMicMutedToggleMic() [RobloxScriptSecurity]
```

---

## VoiceChatService
**Extends:** Instance
**Tags:** NotCreatable, Service

### Properties
```
DefaultDistanceAttenuation: VoiceChatDistanceAttenuationType = Inverse [Read:PluginSecurity] [Write:PluginSecurity]
EnableDefaultVoice: bool = true [Read:PluginSecurity] [Write:PluginSecurity]
UseAudioApi: AudioApiRollout = Automatic [Read:PluginSecurity] [Write:PluginSecurity]
UseNewAudioApi: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
UseNewControlPaths: bool = false [Read:RobloxSecurity] [Write:RobloxSecurity]
UseNewJoinFlow: bool = false [Read:RobloxSecurity] [Write:RobloxSecurity]
UseStreamSwitching: bool = false [Read:RobloxSecurity] [Write:RobloxSecurity]
VoiceChatEnabledForPlaceOnRcc: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
VoiceChatEnabledForUniverseOnRcc: bool = false [Read:RobloxScriptSecurity] [Write:RobloxScriptSecurity]
```

### Functions
```
getInternalChannelId() → string [RobloxScriptSecurity]
getInternalGroupId() → string [RobloxScriptSecurity]
getInternalPublishPause() → bool [RobloxScriptSecurity]
getInternalSessionId() → string [RobloxScriptSecurity]
getInternalSubscribePause(userId: int64) → bool [RobloxScriptSecurity]
getInternalSubscribePauseAll() → bool [RobloxScriptSecurity]
getInternalVoiceChatApiVersion() → int [RobloxScriptSecurity]
isInternalPublishPaused() → bool [RobloxScriptSecurity]
joinVoice() → null [RobloxScriptSecurity]
lastVoiceChatStats() → Dictionary [RobloxScriptSecurity]
leaveVoice() → null [RobloxScriptSecurity]
rejoinVoice() → null [RobloxScriptSecurity]
IsVoiceEnabledForUserIdAsync(userId: int64) → bool
```

### Events
```
ClientRetryJoin() [RobloxSecurity]
ClientRetryJoinWithConfig(sessionConfigFlags: int64) [RobloxSecurity]
FetchUserTurnAuthOperationFailed(sessionId: string) [RobloxSecurity]
JoinedVoice(channelName: string, participantId: int64, sessionId: string, channelId: string) [RobloxSecurity]
PublishStateChange(muteState: MuteState, sessionId: string) [RobloxSecurity]
PublishingHandshakeAcked(handshakeAnswer: string, sessionId: string) [RobloxSecurity]
PublishingHandshakeAckedWithBothSdp(fullHandshakeAnswer: string, compressedHandshakeAnswer: string, sessionId: string, compressMode: int) [RobloxSecurity]
PublishingHandshakeAckedWithCompressedSdp(compressedHandshakeAnswer: string, sessionId: string, compressMode: int) [RobloxSecurity]
PublishingHandshakeCompleted(sessionId: string) [RobloxSecurity]
PublishingHandshakeInitiated(handshakeOffer: string, muteState: MuteState, sessionId: string) [RobloxSecurity]
PublishingHandshakeInitiatedWithBothSdp(fullHandshakeOffer: string, compressedHandshakeOffer: string, muteState: MuteState, sessionId: string, compressMode: int) [RobloxSecurity]
PublishingHandshakeInitiatedWithCompressedSdp(compressedHandshakeOffer: string, muteState: MuteState, sessionId: string, compressMode: int) [RobloxSecurity]
ReJoinedVoice(channelName: string, participantId: int64, sessionId: string, channelId: string) [RobloxSecurity]
RelayCandidatesGathered(voiceControlPath: VoiceControlPath, serializedIceCandidates: string, isLast: bool, sessionId: string, clientIp: string, clientPort: int) [RobloxSecurity]
RuppInitialToken(sessionId: string, token: string, destinationIpAddress: string, destinationPort: int) [RobloxSecurity]
RuppPeriodicToken(sessionId: string, token: string, destinationIpAddress: string, destinationPort: int, sourceIpAddress: string, sourcePort: int) [RobloxSecurity]
SubscribeStateChange(muteState: MuteState, userIds: string, sessionId: string) [RobloxSecurity]
SubscriptionDropped(sessionId: string) [RobloxSecurity]
SubscriptionFeedStarted(eventTag: int64, sessionId: string) [RobloxSecurity]
SubscriptionHandshakeAcked(eventTag: int64, handshakeAnswer: string, usersToMute: string, sessionId: string) [RobloxSecurity]
SubscriptionHandshakeAckedWithBothSdp(eventTag: int64, fullHandshakeAnswer: string, compressedSdpAnswer: string, usersToMute: string, sessionId: string, compressMode: int) [RobloxSecurity]
SubscriptionHandshakeAckedWithCompressedSdp(eventTag: int64, compressedSdpAnswer: string, usersToMute: string, sessionId: string, compressMode: int) [RobloxSecurity]
SubscriptionHandshakeCompleted(sessionId: string, eventTag: int64) [RobloxSecurity]
SubscriptionHandshakeInitiated(handshakeOffer: string, newSubscriptionStates: string, isNewConnection: bool, sessionId: string, eventTag: int64) [RobloxSecurity]
SubscriptionHandshakeInitiatedWithBothSdp(fullHandshakeOffer: string, compressedHandshakeOffer: string, newSubscriptionStates: string, isNewConnection: bool, sessionId: string, eventTag: int64, compressMode: int) [RobloxSecurity]
SubscriptionHandshakeInitiatedWithCompressedSdp(compressedHandshakeOffer: string, newSubscriptionStates: string, isNewConnection: bool, sessionId: string, eventTag: int64, compressMode: int) [RobloxSecurity]
SubscriptionReset(sessionId: string) [RobloxSecurity]
UpdateTurnAuthInfoRequest() [RobloxSecurity]
UserTurnAuth(sessionId: string, userName: string, password: string, ttl: int, uris: Array) [RobloxSecurity]
VoiceChatClientVoiceCapability() [RobloxSecurity]
VoiceChatClientVoiceCapabilityWithConfig(sessionConfigFlags: int64) [RobloxSecurity]
VoiceChatPlayerMuteStateChangedClientToServer(muteState: MuteState) [RobloxSecurity]
VoiceChatPlayerMuteStateChangedServerToClient(muteState: MuteState) [RobloxSecurity]
VoiceChatSampleTaggedEventClientToServer(tag: int64, value: string) [RobloxSecurity]
VoiceChatSampleTaggedEventServerToClient(tag: int64, value: string) [RobloxSecurity]
VoiceChatStatsCollected() [RobloxScriptSecurity]
VoiceChatSubscriptionInitialBatchEmpty(sessionId: string) [RobloxSecurity]
VoiceChatplayerMuteStatusChangedEvent(userId: int64, muted: bool, sessionId: string) [RobloxSecurity]
VoiceSetupFailed(voiceControlPath: VoiceControlPath, serializedFailure: string, sessionId: string) [RobloxSecurity]
VoiceUdmuxVip(sessionId: string, udmuxVipAddress: string) [RobloxSecurity]
```

---

## WebSocketClient
**Extends:** Instance
**Tags:** NotCreatable, NotReplicated

### Properties
```
ConnectionState: WebSocketState [ReadOnly]
```

### Functions
```
Close() → null
Send(data: string) → null
```

### Events
```
Closed()
MessageReceived(data: string)
Opened()
```

---

## WebSocketService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
CreateClient(uri: string) → WebSocketClient
```

---

## WebViewService
**Extends:** Instance
**Tags:** NotCreatable, Service, NotReplicated

### Functions
```
CloseWindow() → null [RobloxScriptSecurity]
MutateWindow(url: string, title: string?, isVisible: bool?, searchType: string?, transitionAnimation: string?, showDomainAsTitle: bool?) → null [RobloxScriptSecurity]
OpenWindow(url: string, title: string?, isVisible: bool?, searchType: string?, transitionAnimation: string?, showDomainAsTitle: bool?) → null [RobloxScriptSecurity]
IsAvailable() → bool [RobloxScriptSecurity]
```

### Events
```
OnJavaScriptCall(content: string) [RobloxScriptSecurity]
OnWindowClosed() [RobloxScriptSecurity]
```

---

## WeldConstraint
**Extends:** Instance

### Properties
```
Active: bool = false [ReadOnly]
CFrame0: CFrame
CFrame1: CFrame
Enabled: bool = true
Part0: BasePart
Part0Internal: BasePart
Part1: BasePart
Part1Internal: BasePart
State: int = 3
```

---

## Wire
**Extends:** Instance

### Properties
```
Connected: bool = false [ReadOnly]
SourceInstance: Instance
SourceName: string = Output
TargetInstance: Instance
TargetName: string = Input
```

### Functions
```
RenameToDefault() → null [RobloxScriptSecurity]
```

---

## MLSession
**Extends:** Object
**Tags:** NotCreatable, NotReplicated

### Functions
```
ForwardAsync(data: Dictionary) → Dictionary
```

---

## TerrainIterateOperation
**Extends:** Object
**Tags:** NotCreatable, NotReplicated

### Functions
```
CommitBlock(block: Dictionary) → RBXScriptSignal
```

### Events
```
Ready(block: Dictionary)
```

---

## TerrainModifyOperation
**Extends:** Object
**Tags:** NotCreatable, NotReplicated

### Functions
```
CommitBlock(block: Dictionary) → RBXScriptSignal
```

### Events
```
Ready(block: Dictionary)
```

---

## TerrainReadOperation
**Extends:** Object
**Tags:** NotCreatable, NotReplicated

### Events
```
Ready(block: Dictionary)
```

---

## TerrainWriteOperation
**Extends:** Object
**Tags:** NotCreatable, NotReplicated

### Functions
```
CommitBlock(block: Dictionary) → RBXScriptSignal
GetBlock() → Dictionary
```

---


# ENUMS

## AccessModifierType
```
Allow = 0
Deny = 1
```

---

## AccessoryType
```
Unknown = 0
Hat = 1
Hair = 2
Face = 3
Neck = 4
Shoulder = 5
Front = 6
Back = 7
Waist = 8
TShirt = 9
Shirt = 10
Pants = 11
Jacket = 12
Sweater = 13
Shorts = 14
LeftShoe = 15
RightShoe = 16
DressSkirt = 17
Eyebrow = 18
Eyelash = 19
```

---

## ActionOnAutoResumeSync
```
DontResume = 0
KeepStudio = 1
KeepLocal = 2
```

---

## ActionOnStopSync
```
AlwaysAsk = 0
KeepLocalFiles = 1
DeleteLocalFiles = 2
```

---

## ActionType
```
Nothing = 0
Pause = 1
Lose = 2
Draw = 3
Win = 4
```

---

## ActuatorRelativeTo
```
Attachment0 = 0
Attachment1 = 1
World = 2
```

---

## ActuatorType
```
None = 0
Motor = 1
Servo = 2
```

---

## AdAvailabilityResult
```
IsAvailable = 1
DeviceIneligible = 2
ExperienceIneligible = 3
InternalError = 4
NoFill = 5
PlayerIneligible = 6
PublisherIneligible = 7
```

---

## AdEventType
```
RewardedAdLoaded = 3
RewardedAdGrant = 4
RewardedAdUnloaded = 5
VideoLoaded = 0 [Deprecated]
VideoRemoved = 1 [Deprecated]
UserCompletedVideo = 2 [Deprecated]
```

---

## AdFormat
```
RewardedVideo = 0
```

---

## AdShape
```
HorizontalRectangle = 1
```

---

## AdTeleportMethod
```
Undefined = 0
PortalForward = 1
InGameMenuBackButton = 2
UIBackButton = 3
```

---

## AdUIEventType
```
AdLabelClicked = 0
VolumeButtonClicked = 1
FullscreenButtonClicked = 2
PlayButtonClicked = 3
PauseButtonClicked = 4
CloseButtonClicked = 5
WhyThisAdClicked = 6
PlayEventTriggered = 7
PauseEventTriggered = 8
```

---

## AdUIType
```
None = 0
Image = 1
Video = 2
```

---

## AdUnitStatus
```
Inactive = 0
Active = 1
```

---

## AdornCullingMode
```
Automatic = 0
Never = 1
```

---

## AlignType
```
PrimaryAxisParallel = 2
PrimaryAxisPerpendicular = 3
PrimaryAxisLookAt = 4
AllAxes = 5
Parallel = 0 [Deprecated]
Perpendicular = 1 [Deprecated]
```

---

## AlphaMode
```
Overlay = 0
Transparency = 1
TintMask = 2
```

---

## AnalyticsCustomFieldKeys
```
CustomField01 = 0
CustomField02 = 1
CustomField03 = 2
```

---

## AnalyticsEconomyAction
```
Default = 0
Acquire = 1
Spend = 2
```

---

## AnalyticsEconomyFlowType
```
Sink = 0
Source = 1
```

---

## AnalyticsEconomyTransactionType
```
IAP = 0
Shop = 1
Gameplay = 2
ContextualPurchase = 3
TimedReward = 4
Onboarding = 5
```

---

## AnalyticsLogLevel
```
Trace = 0
Debug = 1
Information = 2
Warning = 3
Error = 4
Fatal = 5
```

---

## AnalyticsProgressionStatus
```
Default = 0
Begin = 1
Complete = 2
Abandon = 3
Fail = 4
```

---

## AnalyticsProgressionType
```
Custom = 0
Start = 1
Fail = 2
Complete = 3
```

---

## AnimationClipFromVideoStatus
```
Initializing = 0
Pending = 1
Processing = 2
ErrorGeneric = 4
Success = 6
ErrorVideoTooLong = 7
ErrorNoPersonDetected = 8
ErrorVideoUnstable = 9
Timeout = 10
Cancelled = 11
ErrorMultiplePeople = 12
ErrorUploadingVideo = 2001
```

---

## AnimationPriority
```
Core = 1000
Idle = 0
Movement = 1
Action = 2
Action2 = 3
Action3 = 4
Action4 = 5
```

---

## AnimatorRetargetingMode
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## AnnotationEditingMode
```
None = 0
PlacingNew = 1
WritingNew = 2
```

---

## AnnotationRequestStatus
```
Success = 0
Loading = 1
ErrorInternalFailure = 2
ErrorNotFound = 3
ErrorModerated = 4
```

---

## AnnotationRequestType
```
Unknown = 0
Create = 1
Resolve = 2
Delete = 3
Edit = 4
```

---

## AppLifecycleManagerState
```
Detached = 0
Active = 1
Inactive = 2
Hidden = 3
```

---

## AppShellActionType
```
None = 0
OpenApp = 1
TapChatTab = 2
TapConversationEntry = 3
TapAvatarTab = 4
ReadConversation = 5
TapGamePageTab = 6
TapHomePageTab = 7
GamePageLoaded = 8
HomePageLoaded = 9
AvatarEditorPageLoaded = 10
```

---

## AppShellFeature
```
None = 0
Chat = 1
AvatarEditor = 2
GamePage = 3
HomePage = 4
More = 5
Landing = 6
```

---

## AppUpdateStatus
```
Unknown = 0
NotSupported = 1
Failed = 2
NotAvailable = 3
Available = 4
AvailableBoundChannel = 5
```

---

## ApplyStrokeMode
```
Contextual = 0
Border = 1
```

---

## AspectType
```
FitWithinMaxSize = 0
ScaleWithParentSize = 1
```

---

## AssetCreatorType
```
User = 0
Group = 1
```

---

## AssetFetchStatus
```
Success = 0
Failure = 1
None = 2
Loading = 3
TimedOut = 4
```

---

## AssetType
```
Image = 1
TShirt = 2
Audio = 3
Mesh = 4
Lua = 5
Hat = 8
Place = 9
Model = 10
Shirt = 11
Pants = 12
Decal = 13
Head = 17
Face = 18
Gear = 19
Badge = 21
Animation = 24
Torso = 27
RightArm = 28
LeftArm = 29
LeftLeg = 30
RightLeg = 31
Package = 32
GamePass = 34
Plugin = 38
MeshPart = 40
HairAccessory = 41
FaceAccessory = 42
NeckAccessory = 43
ShoulderAccessory = 44
FrontAccessory = 45
BackAccessory = 46
WaistAccessory = 47
ClimbAnimation = 48
DeathAnimation = 49
FallAnimation = 50
IdleAnimation = 51
JumpAnimation = 52
RunAnimation = 53
SwimAnimation = 54
WalkAnimation = 55
PoseAnimation = 56
EarAccessory = 57
EyeAccessory = 58
EmoteAnimation = 61
Video = 62
TShirtAccessory = 64
ShirtAccessory = 65
PantsAccessory = 66
JacketAccessory = 67
SweaterAccessory = 68
ShortsAccessory = 69
LeftShoeAccessory = 70
RightShoeAccessory = 71
DressSkirtAccessory = 72
FontFamily = 73
EyebrowAccessory = 76
EyelashAccessory = 77
MoodAnimation = 78
DynamicHead = 79
```

---

## AssetTypeVerification
```
Default = 1
ClientOnly = 2
Always = 3
```

---

## AudioApiRollout
```
Disabled = 0
Automatic = 1
Enabled = 2
```

---

## AudioCaptureMode
```
```

---

## AudioChannelLayout
```
Mono = 0
Stereo = 1
Quad = 2
Surround_5 = 3
Surround_5_1 = 4
Surround_7_1 = 5
Surround_7_1_4 = 6
```

---

## AudioFilterType
```
Peak = 0
LowShelf = 1
HighShelf = 2
Lowpass12dB = 3
Lowpass24dB = 4
Lowpass48dB = 5
Highpass12dB = 6
Highpass24dB = 7
Highpass48dB = 8
Bandpass = 9
Notch = 10
Lowpass6dB = 11
```

---

## AudioSimulationFidelity
```
None = 0
Automatic = 1
```

---

## AudioSubType
```
Music = 1
SoundEffect = 2
```

---

## AudioWindowSize
```
Small = 0
Medium = 1
Large = 2
```

---

## AuthorityMode
```
Server = 0
Automatic = 1
```

---

## AutoIndentRule
```
Off = 0
Absolute = 1
Relative = 2
```

---

## AutomaticSize
```
None = 0
X = 1
Y = 2
XY = 3
```

---

## AvatarAssetType
```
TShirt = 2
Hat = 8
Shirt = 11
Pants = 12
Head = 17
Face = 18
Gear = 19
Torso = 27
RightArm = 28
LeftArm = 29
LeftLeg = 30
RightLeg = 31
HairAccessory = 41
FaceAccessory = 42
NeckAccessory = 43
ShoulderAccessory = 44
FrontAccessory = 45
BackAccessory = 46
WaistAccessory = 47
ClimbAnimation = 48
FallAnimation = 50
IdleAnimation = 51
JumpAnimation = 52
RunAnimation = 53
SwimAnimation = 54
WalkAnimation = 55
MoodAnimation = 78
EmoteAnimation = 61
TShirtAccessory = 64
ShirtAccessory = 65
PantsAccessory = 66
JacketAccessory = 67
SweaterAccessory = 68
ShortsAccessory = 69
LeftShoeAccessory = 70
RightShoeAccessory = 71
DressSkirtAccessory = 72
EyebrowAccessory = 76
EyelashAccessory = 77
DynamicHead = 79
```

---

## AvatarChatServiceFeature
```
None = 0
UniverseAudio = 1
UniverseVideo = 2
PlaceAudio = 4
PlaceVideo = 8
UserAudioEligible = 16
UserAudio = 32
UserVideoEligible = 64
UserVideo = 128
UserBanned = 256
UserVerifiedForVoice = 512
```

---

## AvatarContextMenuOption
```
Friend = 0
Chat = 1
Emote = 2
InspectMenu = 3
```

---

## AvatarGenerationError
```
None = 0
Unknown = 1
DownloadFailed = 2
Canceled = 3
Offensive = 4
Timeout = 5
JobNotFound = 6
```

---

## AvatarItemType
```
Asset = 1
Bundle = 2
```

---

## AvatarPromptResult
```
Success = 1
PermissionDenied = 2
Failed = 3
```

---

## AvatarSettingsAccessoryLimitMethod
```
Scale = 0
Remove = 1
PreviewScale = 2
PreviewRemove = 3
```

---

## AvatarSettingsAccessoryMode
```
PlayerChoice = 0
CustomLimit = 1
```

---

## AvatarSettingsAnimationClipsMode
```
PlayerChoice = 0
CustomClips = 1
```

---

## AvatarSettingsAnimationPacksMode
```
PlayerChoice = 0
StandardR15 = 1
StandardR6 = 2
```

---

## AvatarSettingsAppearanceMode
```
PlayerChoice = 0
CustomParts = 1
CustomBody = 2
```

---

## AvatarSettingsBuildMode
```
PlayerChoice = 0
CustomBuild = 1
```

---

## AvatarSettingsClothingMode
```
PlayerChoice = 0
CustomLimit = 1
```

---

## AvatarSettingsCollisionMode
```
Default = 0
SingleCollider = 1
Legacy = 2
```

---

## AvatarSettingsCustomAccessoryMode
```
PlayerChoice = 0
CustomAccessories = 1
```

---

## AvatarSettingsCustomBodyType
```
AvatarReference = 0
BundleId = 1
```

---

## AvatarSettingsCustomClothingMode
```
PlayerChoice = 0
CustomClothing = 1
```

---

## AvatarSettingsHitAndTouchDetectionMode
```
UseParts = 0
UseCollider = 1
```

---

## AvatarSettingsJumpMode
```
JumpHeight = 0
JumpPower = 1
```

---

## AvatarSettingsLegacyCollisionMode
```
R6Colliders = 0
InnerBoxColliders = 1
```

---

## AvatarSettingsScaleMode
```
PlayerChoice = 0
CustomScale = 1
```

---

## AvatarThumbnailCustomizationType
```
Closeup = 1
FullBody = 2
```

---

## AvatarUnificationMode
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## Axis
```
X = 0
Y = 1
Z = 2
```

---

## BenefitType
```
DeveloperProduct = 0
AvatarAsset = 1
AvatarBundle = 2
```

---

## BinType
```
Script = 0
GameTool = 1
Grab = 2
Clone = 3
Hammer = 4
```

---

## BodyPart
```
Head = 0
Torso = 1
LeftArm = 2
RightArm = 3
LeftLeg = 4
RightLeg = 5
```

---

## BodyPartR15
```
Head = 0
UpperTorso = 1
LowerTorso = 2
LeftFoot = 3
LeftLowerLeg = 4
LeftUpperLeg = 5
RightFoot = 6
RightLowerLeg = 7
RightUpperLeg = 8
LeftHand = 9
LeftLowerArm = 10
LeftUpperArm = 11
RightHand = 12
RightLowerArm = 13
RightUpperArm = 14
RootPart = 15
Unknown = 17
```

---

## BorderMode
```
Outline = 0
Middle = 1
Inset = 2
```

---

## BorderStrokePosition
```
Outer = 0
Center = 1
Inner = 2
```

---

## BreakReason
```
Other = 0
Error = 1
SpecialBreakpoint = 2
UserBreakpoint = 3
```

---

## BreakpointRemoveReason
```
Requested = 0
ScriptChanged = 1
ScriptRemoved = 2
```

---

## BulkMoveMode
```
FireAllEvents = 0
FireCFrameChanged = 1
```

---

## BundleType
```
BodyParts = 1
Animations = 2
Shoes = 3
DynamicHead = 4
DynamicHeadAvatar = 5
```

---

## Button
```
Jump = 32
Dismount = 8
```

---

## ButtonStyle
```
Custom = 0
RobloxButtonDefault = 1
RobloxButton = 2
RobloxRoundButton = 3
RobloxRoundDefaultButton = 4
RobloxRoundDropdownButton = 5
```

---

## CageType
```
Inner = 0
Outer = 1
```

---

## CameraMode
```
Classic = 0
LockFirstPerson = 1
```

---

## CameraPanMode
```
Classic = 0
EdgeBump = 1
```

---

## CameraSpeedAdjustBinding
```
None = 0
RmbScroll = 1
AltScroll = 2
```

---

## CameraType
```
Fixed = 0
Attach = 1
Watch = 2
Track = 3
Follow = 4
Custom = 5
Scriptable = 6
Orbital = 7
```

---

## CaptureGalleryPermission
```
ReadAndUpload = 0
```

---

## CaptureType
```
Screenshot = 1
Video = 2
```

---

## CatalogCategoryFilter
```
None = 1
Featured = 2
Collectibles = 3
CommunityCreations = 4
Premium = 5
Recommended = 6
```

---

## CatalogSortAggregation
```
Past12Hours = 1
PastDay = 2
Past3Days = 3
PastWeek = 4
PastMonth = 5
AllTime = 6
```

---

## CatalogSortType
```
Relevance = 1
PriceHighToLow = 2
PriceLowToHigh = 3
MostFavorited = 5
RecentlyCreated = 6
Bestselling = 7
```

---

## CellBlock
```
Solid = 0
VerticalWedge = 1
CornerWedge = 2
InverseCornerWedge = 3
HorizontalWedge = 4
```

---

## CellMaterial
```
Empty = 0
Grass = 1
Sand = 2
Brick = 3
Granite = 4
Asphalt = 5
Iron = 6
Aluminum = 7
Gold = 8
WoodPlank = 9
WoodLog = 10
Gravel = 11
CinderBlock = 12
MossyStone = 13
Cement = 14
RedPlastic = 15
BluePlastic = 16
Water = 17
```

---

## CellOrientation
```
NegZ = 0
X = 1
Z = 2
NegX = 3
```

---

## CenterDialogType
```
UnsolicitedDialog = 1
PlayerInitiatedDialog = 2
ModalDialog = 3
QuitDialog = 4
```

---

## CharacterControlMode
```
Default = 0
Legacy = 1
NoCharacterController = 2
LuaCharacterController = 3
```

---

## ChatCallbackType
```
OnCreatingChatWindow = 1
OnClientSendingMessage = 2
OnClientFormattingMessage = 3
OnServerReceivingMessage = 17
```

---

## ChatColor
```
Blue = 0
Green = 1
Red = 2
White = 3
```

---

## ChatMode
```
Menu = 0
TextAndMenu = 1
```

---

## ChatPrivacyMode
```
AllUsers = 0
NoOne = 1
Friends = 2
```

---

## ChatRestrictionStatus
```
Unknown = 0
NotRestricted = 1
Restricted = 2
```

---

## ChatStyle
```
Classic = 0
Bubble = 1
ClassicAndBubble = 2
```

---

## ChatVersion
```
LegacyChatService = 0
TextChatService = 1
```

---

## ClientAnimatorThrottlingMode
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## CloseReason
```
Unknown = 0
RobloxMaintenance = 1
DeveloperShutdown = 2
DeveloperUpdate = 3
ServerEmpty = 4
OutOfMemory = 5
```

---

## CollaboratorStatus
```
None = 0
Editing3D = 1
Scripting = 2
PrivateScripting = 3
```

---

## CollisionFidelity
```
Default = 0
Hull = 1
Box = 2
PreciseConvexDecomposition = 3
```

---

## CommandPermission
```
Plugin = 0
LocalUser = 1
```

---

## CompileTarget
```
Client = 0
CoreScript = 1
Studio = 2
CoreScriptRaw = 3
```

---

## CompletionAcceptanceBehavior
```
Insert = 0
Replace = 1
ReplaceOnEnterInsertOnTab = 2
InsertOnEnterReplaceOnTab = 3
```

---

## CompletionItemKind
```
Text = 1
Method = 2
Function = 3
Constructor = 4
Field = 5
Variable = 6
Class = 7
Interface = 8
Module = 9
Property = 10
Unit = 11
Value = 12
Enum = 13
Keyword = 14
Snippet = 15
Color = 16
File = 17
Reference = 18
Folder = 19
EnumMember = 20
Constant = 21
Struct = 22
Event = 23
Operator = 24
TypeParameter = 25
```

---

## CompletionItemTag
```
Deprecated = 1
IncorrectIndexType = 2
PluginPermissions = 3
CommandLinePermissions = 4
RobloxPermissions = 5
AddParens = 6
PutCursorInParens = 7
TypeCorrect = 8
ClientServerBoundaryViolation = 9
Invalidated = 10
PutCursorBeforeEnd = 11
```

---

## CompletionTriggerKind
```
Invoked = 1
TriggerCharacter = 2
TriggerForIncompleteCompletions = 3
```

---

## ComputerCameraMovementMode
```
Default = 0
Classic = 1
Follow = 2
Orbital = 3
CameraToggle = 4
```

---

## ComputerMovementMode
```
Default = 0
KeyboardMouse = 1
ClickToMove = 2
```

---

## ConfigSnapshotErrorState
```
None = 0
LoadFailed = 1
```

---

## ConnectionError
```
OK = 0
Unknown = 1
DisconnectErrors = 256
DisconnectBadhash = 257
DisconnectSecurityKeyMismatch = 258
DisconnectProtocolMismatch = 259
DisconnectReceivePacketError = 260
DisconnectReceivePacketStreamError = 261
DisconnectSendPacketError = 262
DisconnectIllegalTeleport = 263
DisconnectDuplicatePlayer = 264
DisconnectDuplicateTicket = 265
DisconnectTimeout = 266
DisconnectLuaKick = 267
DisconnectOnRemoteSysStats = 268
DisconnectHashTimeout = 269
DisconnectCloudEditKick = 270
DisconnectPlayerless = 271
DisconnectNewSecurityKeyMismatch = 272
DisconnectEvicted = 273
DisconnectDevMaintenance = 274
DisconnectRobloxMaintenance = 275
DisconnectRejoin = 276
DisconnectConnectionLost = 277
DisconnectIdle = 278
DisconnectRaknetErrors = 279
DisconnectWrongVersion = 280
DisconnectBySecurityPolicy = 281
DisconnectBlockedIP = 282
DisconnectClientFailure = 284
DisconnectClientRequest = 285
DisconnectPrivateServerKickout = 286
DisconnectModeratedGame = 287
ServerShutdown = 288
ReplicatorTimeout = 290
PlayerRemoved = 291
DisconnectOutOfMemoryKeepPlayingLeave = 292
DisconnectRomarkEndOfTest = 293
DisconnectCollaboratorPermissionRevoked = 294
DisconnectCollaboratorUnderage = 295
NetworkInternal = 296
NetworkSend = 297
NetworkTimeout = 298
NetworkMisbehavior = 299
NetworkSecurity = 300
ReplacementReady = 301
ServerEmpty = 302
PhantomFreeze = 303
AndroidAnticheatKick = 304
AndroidEmulatorKick = 305
AndroidRootedKick = 306
PlacelaunchErrors = 512
PlacelaunchDisabled = 515
PlacelaunchError = 516
PlacelaunchGameEnded = 517
PlacelaunchGameFull = 518
PlacelaunchUserLeft = 522
PlacelaunchRestricted = 523
PlacelaunchUnauthorized = 524
PlacelaunchFlooded = 525
PlacelaunchHashExpired = 526
PlacelaunchHashException = 527
PlacelaunchPartyCannotFit = 528
PlacelaunchHttpError = 529
PlacelaunchUserPrivacyUnauthorized = 533
PlacelaunchCreatorBan = 600
PlacelaunchCustomMessage = 610
PlacelaunchOtherError = 611
TeleportErrors = 768
TeleportFailure = 769
TeleportGameNotFound = 770
TeleportGameEnded = 771
TeleportGameFull = 772
TeleportUnauthorized = 773
TeleportFlooded = 774
TeleportIsTeleporting = 775
```

---

## ConnectionState
```
Connected = 0
Disconnected = 1
```

---

## ContentSourceType
```
None = 0
Uri = 1
Object = 2
```

---

## ContextActionPriority
```
Low = 1000
Medium = 2000
High = 3000
```

---

## ContextActionResult
```
Sink = 0
Pass = 1
```

---

## ControlMode
```
Classic = 0
MouseLockSwitch = 1
```

---

## CoreGuiType
```
PlayerList = 0
Health = 1
Backpack = 2
Chat = 3
All = 4
EmotesMenu = 5
SelfView = 6
Captures = 7
```

---

## CreateAssetResult
```
Success = 1
PermissionDenied = 2
UploadFailed = 3
Unknown = 4
```

---

## CreateOutfitFailure
```
InvalidName = 1
OutfitLimitReached = 2
Other = 3
```

---

## CreatorType
```
User = 0
Group = 1
```

---

## CreatorTypeFilter
```
User = 0
Group = 1
All = 2
```

---

## CurrencyType
```
Default = 0
Robux = 1
Tix = 2
```

---

## CustomCameraMode
```
Default = 0
Classic = 1
Follow = 2
```

---

## DataStoreRequestType
```
GetAsync = 0
SetIncrementAsync = 1
UpdateAsync = 2
GetSortedAsync = 3
SetIncrementSortedAsync = 4
OnUpdate = 5
ListAsync = 6
GetVersionAsync = 7
RemoveVersionAsync = 8
```

---

## DebuggerEndReason
```
ClientRequest = 0
Timeout = 1
InvalidHost = 2
Disconnected = 3
ServerShutdown = 4
ServerProtocolMismatch = 5
ConfigurationFailed = 6
RpcError = 7
```

---

## DebuggerExceptionBreakMode
```
Never = 0
Always = 1
Unhandled = 2
```

---

## DebuggerFrameType
```
C = 0
Lua = 1
```

---

## DebuggerPauseReason
```
Unknown = 0
Requested = 1
Breakpoint = 2
Exception = 3
SingleStep = 4
Entrypoint = 5
```

---

## DebuggerStatus
```
Success = 0
Timeout = 1
ConnectionLost = 2
InvalidResponse = 3
InternalError = 4
InvalidState = 5
RpcError = 6
InvalidArgument = 7
ConnectionClosed = 8
```

---

## DevCameraOcclusionMode
```
Zoom = 0
Invisicam = 1
```

---

## DevComputerCameraMovementMode
```
UserChoice = 0
Classic = 1
Follow = 2
Orbital = 3
CameraToggle = 4
```

---

## DevComputerMovementMode
```
UserChoice = 0
KeyboardMouse = 1
ClickToMove = 2
Scriptable = 3
```

---

## DevTouchCameraMovementMode
```
UserChoice = 0
Classic = 1
Follow = 2
Orbital = 3
```

---

## DevTouchMovementMode
```
UserChoice = 0
Thumbstick = 1
DPad = 2
Thumbpad = 3
ClickToMove = 4
Scriptable = 5
DynamicThumbstick = 6
```

---

## DeveloperMemoryTag
```
Internal = 0
HttpCache = 1
Instances = 2
Signals = 3
LuaHeap = 4
Script = 5
PhysicsCollision = 6
PhysicsParts = 7
GraphicsSolidModels = 8
GraphicsMeshParts = 10
GraphicsParticles = 11
GraphicsParts = 12
GraphicsSpatialHash = 13
GraphicsTerrain = 14
GraphicsTexture = 15
GraphicsTextureCharacter = 16
Sounds = 17
StreamingSounds = 18
TerrainVoxels = 19
Gui = 21
Animation = 22
Navigation = 23
GeometryCSG = 24
GraphicsSlimModels = 25
```

---

## DeviceFeatureType
```
DeviceCapture = 0
```

---

## DeviceForm
```
Console = 0
Phone = 1
Tablet = 2
Desktop = 3
VR = 4
```

---

## DeviceLevel
```
Low = 0
Medium = 1
High = 2
```

---

## DeviceType
```
Unknown = 0
Desktop = 1
Tablet = 2
Phone = 3
```

---

## DialogBehaviorType
```
SinglePlayer = 0
MultiplePlayers = 1
```

---

## DialogPurpose
```
Quest = 0
Help = 1
Shop = 2
```

---

## DialogTone
```
Neutral = 0
Friendly = 1
Enemy = 2
```

---

## DisplaySize
```
Small = 0
Medium = 1
Large = 2
```

---

## DominantAxis
```
Width = 0
Height = 1
```

---

## DraftStatusCode
```
OK = 0
DraftOutdated = 1
ScriptRemoved = 2
DraftCommitted = 3
```

---

## DragDetectorDragStyle
```
TranslateLine = 0
TranslatePlane = 1
TranslatePlaneOrLine = 2
TranslateLineOrPlane = 3
TranslateViewPlane = 4
RotateAxis = 5
RotateTrackball = 6
Scriptable = 7
BestForDevice = 8
```

---

## DragDetectorPermissionPolicy
```
Nobody = 0
Everybody = 1
Scriptable = 2
```

---

## DragDetectorResponseStyle
```
Geometric = 0
Physical = 1
Custom = 2
```

---

## DraggerCoordinateSpace
```
Object = 0
World = 1
```

---

## DraggerMovementMode
```
Geometric = 0
Physical = 1
```

---

## DraggingScrollBar
```
None = 0
Horizontal = 1
Vertical = 2
```

---

## EasingDirection
```
In = 0
Out = 1
InOut = 2
```

---

## EasingStyle
```
Linear = 0
Sine = 1
Back = 2
Quad = 3
Quart = 4
Quint = 5
Bounce = 6
Elastic = 7
Exponential = 8
Circular = 9
Cubic = 10
```

---

## EditableStatus
```
Unknown = 0
Allowed = 1
Disallowed = 2
```

---

## ElasticBehavior
```
WhenScrollable = 0
Always = 1
Never = 2
```

---

## EnviromentalPhysicsThrottle
```
DefaultAuto = 0
Disabled = 1
Always = 2
Skip2 = 3
Skip4 = 4
Skip8 = 5
Skip16 = 6
```

---

## ExperienceAuthScope
```
DefaultScope = 0
CreatorAssetsCreate = 1
```

---

## ExplosionType
```
NoCraters = 0
Craters = 1
```

---

## FACSDataLod
```
LOD0 = 0
LOD1 = 1
LODCount = 2
```

---

## FacialAgeEstimationResultType
```
Complete = 0
Cancel = 1
Error = 2
```

---

## FacialAnimationStreamingState
```
None = 0
Audio = 1
Video = 2
Place = 4
Server = 8
```

---

## FacsActionUnit
```
ChinRaiserUpperLip = 0
ChinRaiser = 1
FlatPucker = 2
Funneler = 3
LowerLipSuck = 4
LipPresser = 5
LipsTogether = 6
MouthLeft = 7
MouthRight = 8
Pucker = 9
UpperLipSuck = 10
LeftCheekPuff = 11
LeftDimpler = 12
LeftLipCornerDown = 13
LeftLowerLipDepressor = 14
LeftLipCornerPuller = 15
LeftLipStretcher = 16
LeftUpperLipRaiser = 17
RightCheekPuff = 18
RightDimpler = 19
RightLipCornerDown = 20
RightLowerLipDepressor = 21
RightLipCornerPuller = 22
RightLipStretcher = 23
RightUpperLipRaiser = 24
JawDrop = 25
JawLeft = 26
JawRight = 27
Corrugator = 28
LeftBrowLowerer = 29
LeftOuterBrowRaiser = 30
LeftNoseWrinkler = 31
LeftInnerBrowRaiser = 32
RightBrowLowerer = 33
RightOuterBrowRaiser = 34
RightInnerBrowRaiser = 35
RightNoseWrinkler = 36
EyesLookDown = 37
EyesLookLeft = 38
EyesLookUp = 39
EyesLookRight = 40
LeftCheekRaiser = 41
LeftEyeUpperLidRaiser = 42
LeftEyeClosed = 43
RightCheekRaiser = 44
RightEyeUpperLidRaiser = 45
RightEyeClosed = 46
TongueDown = 47
TongueOut = 48
TongueUp = 49
```

---

## FieldOfViewMode
```
Vertical = 0
Diagonal = 1
MaxAxis = 2
```

---

## FillDirection
```
Horizontal = 0
Vertical = 1
```

---

## FilterErrorType
```
BackslashNotEscapingAnything = 0
BadBespokeFilter = 1
BadName = 2
IncompleteOr = 3
IncompleteParenthesis = 4
InvalidDoubleStar = 5
InvalidTilde = 6
PropertyBadOperator = 7
PropertyDoesNotExist = 8
PropertyInvalidField = 9
PropertyInvalidValue = 10
PropertyUnsupportedFields = 11
PropertyUnsupportedProperty = 12
UnexpectedNameIndex = 13
UnexpectedToken = 14
UnfinishedBinaryOperator = 15
UnfinishedQuote = 16
UnknownBespokeFilter = 17
WildcardInProperty = 18
```

---

## FilterResult
```
Accepted = 0
Rejected = 1
```

---

## FinishRecordingOperation
```
Cancel = 0
Commit = 1
Append = 2
```

---

## FluidFidelity
```
Automatic = 0
UseCollisionGeometry = 1
UsePreciseGeometry = 2
```

---

## FluidForces
```
Default = 0
Experimental = 1
```

---

## Font
```
Legacy = 0
Arial = 1
ArialBold = 2
SourceSans = 3
SourceSansBold = 4
SourceSansLight = 5
SourceSansItalic = 6
Bodoni = 7
Garamond = 8
Cartoon = 9
Code = 10
Highway = 11
SciFi = 12
Arcade = 13
Fantasy = 14
Antique = 15
SourceSansSemibold = 16
Gotham = 17
GothamMedium = 18
GothamBold = 19
GothamBlack = 20
AmaticSC = 21
Bangers = 22
Creepster = 23
DenkOne = 24
Fondamento = 25
FredokaOne = 26
GrenzeGotisch = 27
IndieFlower = 28
JosefinSans = 29
Jura = 30
Kalam = 31
LuckiestGuy = 32
Merriweather = 33
Michroma = 34
Nunito = 35
Oswald = 36
PatrickHand = 37
PermanentMarker = 38
Roboto = 39
RobotoCondensed = 40
RobotoMono = 41
Sarpanch = 42
SpecialElite = 43
TitilliumWeb = 44
Ubuntu = 45
BuilderSans = 46
BuilderSansMedium = 47
BuilderSansBold = 48
BuilderSansExtraBold = 49
Arimo = 50
ArimoBold = 51
Unknown = 100
```

---

## FontSize
```
Size8 = 0
Size9 = 1
Size10 = 2
Size11 = 3
Size12 = 4
Size14 = 5
Size18 = 6
Size24 = 7
Size36 = 8
Size48 = 9
Size28 = 10
Size32 = 11
Size42 = 12
Size60 = 13
Size96 = 14
```

---

## FontStyle
```
Normal = 0
Italic = 1
```

---

## FontWeight
```
Thin = 100
ExtraLight = 200
Light = 300
Regular = 400
Medium = 500
SemiBold = 600
Bold = 700
ExtraBold = 800
Heavy = 900
```

---

## ForceLimitMode
```
Magnitude = 0
PerAxis = 1
```

---

## FormFactor
```
Symmetric = 0
Brick = 1
Plate = 2
Custom = 3
```

---

## FrameStyle
```
Custom = 0
ChatBlue = 1
RobloxSquare = 2
RobloxRound = 3
ChatGreen = 4
ChatRed = 5
DropShadow = 6
```

---

## FramerateManagerMode
```
Automatic = 0
On = 1
Off = 2
```

---

## FriendRequestEvent
```
Issue = 0
Revoke = 1
Accept = 2
Deny = 3
```

---

## FriendStatus
```
Unknown = 0
NotFriend = 1
Friend = 2
FriendRequestSent = 3
FriendRequestReceived = 4
```

---

## FunctionalTestResult
```
Passed = 0
Warning = 1
Error = 2
```

---

## GameAvatarType
```
R6 = 0
R15 = 1
PlayerChoice = 2
```

---

## GamepadType
```
Unknown = 0
PS4 = 1
PS5 = 2
XboxOne = 3
```

---

## GearGenreSetting
**Tags:** Deprecated
```
AllGenres = 0 [Deprecated]
MatchingGenreOnly = 1 [Deprecated]
```

---

## GearType
**Tags:** Deprecated
```
MeleeWeapons = 0 [Deprecated]
RangedWeapons = 1 [Deprecated]
Explosives = 2 [Deprecated]
PowerUps = 3 [Deprecated]
NavigationEnhancers = 4 [Deprecated]
MusicalInstruments = 5 [Deprecated]
SocialItems = 6 [Deprecated]
BuildingTools = 7 [Deprecated]
Transport = 8 [Deprecated]
```

---

## Genre
**Tags:** Deprecated
```
All = 0
TownAndCity = 1
Fantasy = 2
SciFi = 3
Ninja = 4
Scary = 5
Pirate = 6
Adventure = 7
Sports = 8
Funny = 9
WildWest = 10
War = 11
SkatePark = 12
Tutorial = 13
```

---

## GraphicsMode
```
Automatic = 1
Direct3D11 = 2
OpenGL = 4
Metal = 5
Vulkan = 6
NoGraphics = 9
```

---

## GraphicsOptimizationMode
```
Performance = 0
Balanced = 1
Quality = 2
```

---

## GuiState
```
Idle = 0
Hover = 1
Press = 2
NonInteractable = 3
```

---

## GuiType
```
Core = 0
Custom = 1
PlayerNameplates = 2
CustomBillboards = 3
CoreBillboards = 4
```

---

## HandRigDescriptionSide
```
None = 0
Left = 1
Right = 2
```

---

## HandlesStyle
```
Resize = 0
Movement = 1
```

---

## HapticEffectType
```
Custom = 0
UIHover = 1
UIClick = 2
UINotification = 3
GameplayExplosion = 4
GameplayCollision = 5
```

---

## HighlightDepthMode
```
AlwaysOnTop = 0
Occluded = 1
```

---

## HorizontalAlignment
```
Center = 0
Left = 1
Right = 2
```

---

## HoverAnimateSpeed
```
VerySlow = 0
Slow = 1
Medium = 2
Fast = 3
VeryFast = 4
```

---

## HttpCachePolicy
```
None = 0
Full = 1
DataOnly = 2
Default = 3
InternalRedirectRefresh = 4
```

---

## HttpCompression
```
None = 0
Gzip = 1
```

---

## HttpContentType
```
ApplicationJson = 0
ApplicationXml = 1
ApplicationUrlEncoded = 2
TextPlain = 3
TextXml = 4
```

---

## HttpError
```
OK = 0
InvalidUrl = 1
DnsResolve = 2
ConnectFail = 3
OutOfMemory = 4
TimedOut = 5
TooManyRedirects = 6
InvalidRedirect = 7
NetFail = 8
Aborted = 9
SslConnectFail = 10
SslVerificationFail = 11
Unknown = 12
ConnectionClosed = 13
ServerProtocolError = 14
CreatorEnvironmentsNotSupportedByService = 15
```

---

## HttpRequestType
```
Default = 0
MarketplaceService = 2
Players = 7
Chat = 15
Avatar = 16
Analytics = 23
Localization = 25
```

---

## HumanoidCollisionType
```
OuterBox = 0
InnerBox = 1
```

---

## HumanoidDisplayDistanceType
```
Viewer = 0
Subject = 1
None = 2
```

---

## HumanoidHealthDisplayType
```
DisplayWhenDamaged = 0
AlwaysOn = 1
AlwaysOff = 2
```

---

## HumanoidRigType
```
R6 = 0
R15 = 1
```

---

## HumanoidStateType
```
FallingDown = 0
Ragdoll = 1
GettingUp = 2
Jumping = 3
Swimming = 4
Freefall = 5
Flying = 6
Landed = 7
Running = 8
RunningNoPhysics = 10
StrafingNoPhysics = 11
Climbing = 12
Seated = 13
PlatformStanding = 14
Dead = 15
Physics = 16
None = 18
```

---

## IKCollisionsMode
```
NoCollisions = 0
OtherMechanismsAnchored = 1
IncludeContactedMechanisms = 2
```

---

## IKControlConstraintSupport
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## IKControlType
```
Transform = 0
Position = 1
Rotation = 2
LookAt = 3
```

---

## IXPLoadingStatus
```
None = 0
Pending = 1
Initialized = 2
ErrorInvalidUser = 3
ErrorConnection = 4
ErrorJsonParse = 5
ErrorTimedOut = 6
```

---

## ImageAlphaType
```
Default = 1
LockCanvasAlpha = 2
LockCanvasColor = 3
```

---

## ImageCombineType
```
BlendSourceOver = 1
Overwrite = 2
Add = 3
Multiply = 4
AlphaBlend = 5
```

---

## InOut
```
Edge = 0
Inset = 1
Center = 2
```

---

## InfoType
```
Asset = 0
Product = 1
GamePass = 2
Subscription = 3
Bundle = 4
```

---

## InitialDockState
```
Top = 0
Bottom = 1
Left = 2
Right = 3
Float = 4
```

---

## InputActionType
```
Bool = 0
Direction1D = 1
Direction2D = 2
Direction3D = 3
```

---

## InputType
```
NoInput = 0
Constant = 12
Sin = 13
```

---

## IntermediateMeshGenerationResult
```
HighQualityMesh = 0
```

---

## InterpolationThrottlingMode
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## InviteState
```
Placed = 0
Accepted = 1
Declined = 2
Missed = 3
```

---

## ItemLineAlignment
```
Automatic = 0
Start = 1
Center = 2
End = 3
Stretch = 4
```

---

## JoinSource
```
CreatedItemAttribution = 1
```

---

## JointCreationMode
```
All = 0
Surface = 1
None = 2
```

---

## KeyCode
```
Unknown = 0
Backspace = 8
Tab = 9
Clear = 12
Return = 13
Pause = 19
Escape = 27
Space = 32
QuotedDouble = 34
Hash = 35
Dollar = 36
Percent = 37
Ampersand = 38
Quote = 39
LeftParenthesis = 40
RightParenthesis = 41
Asterisk = 42
Plus = 43
Comma = 44
Minus = 45
Period = 46
Slash = 47
Zero = 48
One = 49
Two = 50
Three = 51
Four = 52
Five = 53
Six = 54
Seven = 55
Eight = 56
Nine = 57
Colon = 58
Semicolon = 59
LessThan = 60
Equals = 61
GreaterThan = 62
Question = 63
At = 64
LeftBracket = 91
BackSlash = 92
RightBracket = 93
Caret = 94
Underscore = 95
Backquote = 96
A = 97
B = 98
C = 99
D = 100
E = 101
F = 102
G = 103
H = 104
I = 105
J = 106
K = 107
L = 108
M = 109
N = 110
O = 111
P = 112
Q = 113
R = 114
S = 115
T = 116
U = 117
V = 118
W = 119
X = 120
Y = 121
Z = 122
LeftCurly = 123
Pipe = 124
RightCurly = 125
Tilde = 126
Delete = 127
KeypadZero = 256
KeypadOne = 257
KeypadTwo = 258
KeypadThree = 259
KeypadFour = 260
KeypadFive = 261
KeypadSix = 262
KeypadSeven = 263
KeypadEight = 264
KeypadNine = 265
KeypadPeriod = 266
KeypadDivide = 267
KeypadMultiply = 268
KeypadMinus = 269
KeypadPlus = 270
KeypadEnter = 271
KeypadEquals = 272
Up = 273
Down = 274
Right = 275
Left = 276
Insert = 277
Home = 278
End = 279
PageUp = 280
PageDown = 281
F1 = 282
F2 = 283
F3 = 284
F4 = 285
F5 = 286
F6 = 287
F7 = 288
F8 = 289
F9 = 290
F10 = 291
F11 = 292
F12 = 293
F13 = 294
F14 = 295
F15 = 296
NumLock = 300
CapsLock = 301
ScrollLock = 302
RightShift = 303
LeftShift = 304
RightControl = 305
LeftControl = 306
RightAlt = 307
LeftAlt = 308
RightMeta = 309
LeftMeta = 310
LeftSuper = 311
RightSuper = 312
Mode = 313
Compose = 314
Help = 315
Print = 316
SysReq = 317
Break = 318
Menu = 319
Power = 320
Euro = 321
Undo = 322
ButtonX = 1000
ButtonY = 1001
ButtonA = 1002
ButtonB = 1003
ButtonR1 = 1004
ButtonL1 = 1005
ButtonR2 = 1006
ButtonL2 = 1007
ButtonR3 = 1008
ButtonL3 = 1009
ButtonStart = 1010
ButtonSelect = 1011
DPadLeft = 1012
DPadRight = 1013
DPadUp = 1014
DPadDown = 1015
Thumbstick1 = 1016
Thumbstick2 = 1017
MouseLeftButton = 1018
MouseRightButton = 1019
MouseMiddleButton = 1020
World0 = 160 [Deprecated]
World1 = 161 [Deprecated]
World2 = 162 [Deprecated]
World3 = 163 [Deprecated]
World4 = 164 [Deprecated]
World5 = 165 [Deprecated]
World6 = 166 [Deprecated]
World7 = 167 [Deprecated]
World8 = 168 [Deprecated]
World9 = 169 [Deprecated]
World10 = 170 [Deprecated]
World11 = 171 [Deprecated]
World12 = 172 [Deprecated]
World13 = 173 [Deprecated]
World14 = 174 [Deprecated]
World15 = 175 [Deprecated]
World16 = 176 [Deprecated]
World17 = 177 [Deprecated]
World18 = 178 [Deprecated]
World19 = 179 [Deprecated]
World20 = 180 [Deprecated]
World21 = 181 [Deprecated]
World22 = 182 [Deprecated]
World23 = 183 [Deprecated]
World24 = 184 [Deprecated]
World25 = 185 [Deprecated]
World26 = 186 [Deprecated]
World27 = 187 [Deprecated]
World28 = 188 [Deprecated]
World29 = 189 [Deprecated]
World30 = 190 [Deprecated]
World31 = 191 [Deprecated]
World32 = 192 [Deprecated]
World33 = 193 [Deprecated]
World34 = 194 [Deprecated]
World35 = 195 [Deprecated]
World36 = 196 [Deprecated]
World37 = 197 [Deprecated]
World38 = 198 [Deprecated]
World39 = 199 [Deprecated]
World40 = 200 [Deprecated]
World41 = 201 [Deprecated]
World42 = 202 [Deprecated]
World43 = 203 [Deprecated]
World44 = 204 [Deprecated]
World45 = 205 [Deprecated]
World46 = 206 [Deprecated]
World47 = 207 [Deprecated]
World48 = 208 [Deprecated]
World49 = 209 [Deprecated]
World50 = 210 [Deprecated]
World51 = 211 [Deprecated]
World52 = 212 [Deprecated]
World53 = 213 [Deprecated]
World54 = 214 [Deprecated]
World55 = 215 [Deprecated]
World56 = 216 [Deprecated]
World57 = 217 [Deprecated]
World58 = 218 [Deprecated]
World59 = 219 [Deprecated]
World60 = 220 [Deprecated]
World61 = 221 [Deprecated]
World62 = 222 [Deprecated]
World63 = 223 [Deprecated]
World64 = 224 [Deprecated]
World65 = 225 [Deprecated]
World66 = 226 [Deprecated]
World67 = 227 [Deprecated]
World68 = 228 [Deprecated]
World69 = 229 [Deprecated]
World70 = 230 [Deprecated]
World71 = 231 [Deprecated]
World72 = 232 [Deprecated]
World73 = 233 [Deprecated]
World74 = 234 [Deprecated]
World75 = 235 [Deprecated]
World76 = 236 [Deprecated]
World77 = 237 [Deprecated]
World78 = 238 [Deprecated]
World79 = 239 [Deprecated]
World80 = 240 [Deprecated]
World81 = 241 [Deprecated]
World82 = 242 [Deprecated]
World83 = 243 [Deprecated]
World84 = 244 [Deprecated]
World85 = 245 [Deprecated]
World86 = 246 [Deprecated]
World87 = 247 [Deprecated]
World88 = 248 [Deprecated]
World89 = 249 [Deprecated]
World90 = 250 [Deprecated]
World91 = 251 [Deprecated]
World92 = 252 [Deprecated]
World93 = 253 [Deprecated]
World94 = 254 [Deprecated]
World95 = 255 [Deprecated]
MouseBackButton = 1021 [Deprecated]
MouseNoButton = 1022 [Deprecated]
MouseX = 1023 [Deprecated]
MouseY = 1024 [Deprecated]
```

---

## KeyInterpolationMode
```
Constant = 0
Linear = 1
Cubic = 2
```

---

## KeywordFilterType
```
Include = 0
Exclude = 1
```

---

## Language
```
Default = 0
```

---

## LeftRight
```
Left = 0
Center = 1
Right = 2
```

---

## LexemeType
```
Eof = 0
Name = 1
QuotedString = 2
Number = 3
And = 4
Or = 5
Equal = 6
TildeEqual = 7
GreaterThan = 8
GreaterThanEqual = 9
LessThan = 10
LessThanEqual = 11
Colon = 12
Dot = 13
LeftParenthesis = 14
RightParenthesis = 15
Star = 16
DoubleStar = 17
ReservedSpecial = 18
```

---

## LightingStyle
```
Realistic = 0
Soft = 1
```

---

## Limb
```
Head = 0
Torso = 1
LeftArm = 2
RightArm = 3
LeftLeg = 4
RightLeg = 5
Unknown = 6
```

---

## LineJoinMode
```
Round = 0
Bevel = 1
Miter = 2
```

---

## ListDisplayMode
```
Horizontal = 0
Vertical = 1
```

---

## ListenerLocation
```
Default = 0
None = 1
Character = 2
Camera = 3
```

---

## ListenerType
```
Camera = 0
CFrame = 1
ObjectPosition = 2
ObjectCFrame = 3
```

---

## LiveEditingAtomicUpdateResponse
```
Success = 0
FailureGuidNotFound = 1
FailureHashMismatch = 2
FailureOperationIllegal = 3
```

---

## LiveEditingBroadcastMessageType
```
Normal = 0
Warning = 1
Error = 2
```

---

## LoadCharacterLayeredClothing
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## LoadDynamicHeads
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## LocationType
```
Character = 0
Camera = 1
ObjectPosition = 2
```

---

## LuauTypeCheckMode
```
NoCheck = 0
Nonstrict = 1
Strict = 2
```

---

## MarketplaceBulkPurchasePromptStatus
```
Completed = 1
Aborted = 2
Error = 3
```

---

## MarketplaceItemPurchaseStatus
```
Success = 1
SystemError = 2
AlreadyOwned = 3
InsufficientRobux = 4
QuantityLimitExceeded = 5
QuotaExceeded = 6
NotForSale = 7
NotAvailableForPurchaser = 8
PriceMismatch = 9
SoldOut = 10
PurchaserIsSeller = 11
InsufficientMembership = 12
PlaceInvalid = 13
```

---

## MarketplaceProductType
```
AvatarAsset = 1
AvatarBundle = 2
```

---

## MarkupKind
```
PlainText = 0
Markdown = 1
```

---

## MatchmakingType
```
Default = 1
XboxOnly = 2
PlayStationOnly = 3
```

---

## Material
```
Plastic = 256
SmoothPlastic = 272
Neon = 288
Wood = 512
WoodPlanks = 528
Marble = 784
Slate = 800
Concrete = 816
Granite = 832
Brick = 848
Pebble = 864
Cobblestone = 880
Rock = 896
Sandstone = 912
Basalt = 788
CrackedLava = 804
Limestone = 820
Pavement = 836
CorrodedMetal = 1040
DiamondPlate = 1056
Foil = 1072
Metal = 1088
Grass = 1280
LeafyGrass = 1284
Sand = 1296
Fabric = 1312
Snow = 1328
Mud = 1344
Ground = 1360
Asphalt = 1376
Salt = 1392
Ice = 1536
Glacier = 1552
Glass = 1568
ForceField = 1584
Air = 1792
Water = 2048
Cardboard = 2304
Carpet = 2305
CeramicTiles = 2306
ClayRoofTiles = 2307
RoofShingles = 2308
Leather = 2309
Plaster = 2310
Rubber = 2311
```

---

## MaterialPattern
```
Regular = 0
Organic = 1
```

---

## MembershipType
```
None = 0
BuildersClub = 1
TurboBuildersClub = 2
OutrageousBuildersClub = 3
Premium = 4
```

---

## MeshPartDetailLevel
```
DistanceBased = 0
Level00 = 1
Level01 = 2
Level02 = 3
Level03 = 4
Level04 = 5
```

---

## MeshPartHeadsAndAccessories
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## MeshScaleUnit
```
Stud = 0
Meter = 1
CM = 2
MM = 3
Foot = 4
Inch = 5
```

---

## MeshType
```
Head = 0
Torso = 1
Wedge = 2
Sphere = 3
Cylinder = 4
FileMesh = 5
Brick = 6
Prism = 7 [Deprecated]
Pyramid = 8 [Deprecated]
ParallelRamp = 9 [Deprecated]
RightAngleRamp = 10 [Deprecated]
CornerWedge = 11 [Deprecated]
```

---

## MessageType
```
MessageOutput = 0
MessageInfo = 1
MessageWarning = 2
MessageError = 3
```

---

## ModelLevelOfDetail
```
Automatic = 0
StreamingMesh = 1
Disabled = 2
```

---

## ModelStreamingBehavior
```
Default = 0
Legacy = 1
Improved = 2
```

---

## ModelStreamingMode
```
Default = 0
Atomic = 1
Persistent = 2
PersistentPerPlayer = 3
Nonatomic = 4
```

---

## ModerationStatus
```
ReviewedApproved = 1
ReviewedRejected = 2
NotReviewed = 3
NotApplicable = 4
Invalid = 5
```

---

## ModifierKey
```
Shift = 0
Ctrl = 1
Alt = 2
Meta = 3
```

---

## MouseBehavior
```
Default = 0
LockCenter = 1
LockCurrentPosition = 2
```

---

## MoveState
```
Stopped = 0
Coasting = 1
Pushing = 2
Stopping = 3
AirFree = 4
```

---

## MoverConstraintRootBehaviorMode
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## MuteState
```
Unmuted = 0
Muted = 1
```

---

## NameOcclusion
```
NoOcclusion = 0
EnemyOcclusion = 1
OccludeAll = 2
```

---

## NegateOperationHiddenHistory
```
None = 0
NegatedUnion = 1
NegatedIntersection = 2
```

---

## NetworkOwnership
```
Automatic = 0
Manual = 1
OnContact = 2
```

---

## NetworkStatus
```
Unknown = 0
Connected = 1
Disconnected = 2
```

---

## NoiseType
```
SimplexGabor = 0
```

---

## NormalId
```
Right = 0
Top = 1
Back = 2
Left = 3
Bottom = 4
Front = 5
```

---

## NotificationButtonType
```
Primary = 0
Secondary = 1
```

---

## OperationType
```
Null = 0
Union = 1
Subtraction = 2
Intersection = 3
Primitive = 4
```

---

## OrientationAlignmentMode
```
OneAttachment = 0
TwoAttachment = 1
```

---

## OutfitSource
```
All = 1
Created = 2
Purchased = 3
```

---

## OutfitType
```
All = 1
Avatar = 2
DynamicHead = 3
```

---

## OutputLayoutMode
```
Horizontal = 0
Vertical = 1
```

---

## OverrideMouseIconBehavior
```
None = 0
ForceShow = 1
ForceHide = 2
```

---

## PackagePermission
```
None = 0
NoAccess = 1
Revoked = 2
UseView = 3
Edit = 4
Own = 5
```

---

## PartType
```
Ball = 0
Block = 1
Cylinder = 2
Wedge = 3
CornerWedge = 4
```

---

## ParticleEmitterShape
```
Box = 0
Sphere = 1
Cylinder = 2
Disc = 3
```

---

## ParticleEmitterShapeInOut
```
Outward = 0
Inward = 1
InAndOut = 2
```

---

## ParticleEmitterShapeStyle
```
Volume = 0
Surface = 1
```

---

## ParticleFlipbookLayout
```
None = 0
Grid2x2 = 1
Grid4x4 = 2
Grid8x8 = 3
```

---

## ParticleFlipbookMode
```
Loop = 0
OneShot = 1
PingPong = 2
Random = 3
```

---

## ParticleFlipbookTextureCompatible
```
NotCompatible = 0
Compatible = 1
Unknown = 2
```

---

## ParticleOrientation
```
FacingCamera = 0
FacingCameraWorldUp = 1
VelocityParallel = 2
VelocityPerpendicular = 3
```

---

## PathStatus
```
Success = 0
NoPath = 5
ClosestNoPath = 1 [Deprecated]
ClosestOutOfRange = 2 [Deprecated]
FailStartNotEmpty = 3 [Deprecated]
FailFinishNotEmpty = 4 [Deprecated]
```

---

## PathWaypointAction
```
Walk = 0
Jump = 1
Custom = 2
```

---

## PathfindingUseImprovedSearch
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## PerformanceOverlayMode
```
Overdraw = 0
Transparent = 1
Decals = 2
Lights = 3
```

---

## PermissionLevelShown
```
Game = 0
RobloxGame = 1
RobloxScript = 2
Studio = 3
Roblox = 4
```

---

## PhysicsSimulationRate
```
Fixed240Hz = 0
Fixed120Hz = 1
Fixed60Hz = 2
```

---

## PhysicsSteppingMethod
```
Default = 0
Fixed = 1
Adaptive = 2
```

---

## PlacePublishType
```
None = 0
Publish = 1
Save = 2
```

---

## Platform
```
Windows = 0
OSX = 1
IOS = 2
Android = 3
XBoxOne = 4
PS4 = 5
PS3 = 6
XBox360 = 7
WiiU = 8
NX = 9
Ouya = 10
AndroidTV = 11
Chromecast = 12
Linux = 13
SteamOS = 14
WebOS = 15
DOS = 16
BeOS = 17
UWP = 18
PS5 = 19
MetaOS = 20
None = 21
```

---

## PlaybackState
```
Begin = 0
Delayed = 1
Playing = 2
Paused = 3
Completed = 4
Cancelled = 5
```

---

## PlayerActions
```
CharacterForward = 0
CharacterBackward = 1
CharacterLeft = 2
CharacterRight = 3
CharacterJump = 4
```

---

## PlayerCharacterDestroyBehavior
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## PlayerChatType
```
All = 0
Team = 1
Whisper = 2
```

---

## PlayerDataErrorState
```
LoadFailed = 0
FlushFailed = 1
ReleaseFailed = 2
None = 3
```

---

## PlayerDataLoadFailureBehavior
```
Failure = 0
FallbackToDefault = 1
Kick = 2
```

---

## PoseEasingDirection
```
In = 0
Out = 1
InOut = 2
```

---

## PoseEasingStyle
```
Linear = 0
Constant = 1
Elastic = 2
Cubic = 3
Bounce = 4
CubicV2 = 5
```

---

## PositionAlignmentMode
```
OneAttachment = 0
TwoAttachment = 1
```

---

## PredictionMode
```
Auto = 0
None = 1
Forced = 2 [Deprecated]
```

---

## PreferredInput
```
KeyboardAndMouse = 0
Gamepad = 1
Touch = 2
```

---

## PreferredTextSize
```
Medium = 1
Large = 2
Larger = 3
Largest = 4
```

---

## PrimalPhysicsSolver
```
Default = 0
Experimental = 1
Disabled = 2
```

---

## PrimitiveType
```
Null = 0
Ball = 1
Cylinder = 2
Block = 3
Wedge = 4
CornerWedge = 5
```

---

## PrivilegeType
**Tags:** Deprecated
```
Owner = 255
Admin = 240
Member = 128
Visitor = 10
Banned = 0
```

---

## ProductLocationRestriction
```
AvatarShop = 0
AllowedGames = 1
AllGames = 2
```

---

## ProductPurchaseChannel
```
InExperience = 1
ExperienceDetailsPage = 2
AdReward = 3
CommerceProduct = 4
```

---

## ProductPurchaseDecision
```
NotProcessedYet = 0
PurchaseGranted = 1
```

---

## PromptCreateAssetResult
```
Success = 1
PermissionDenied = 2
Timeout = 3
UploadFailed = 4
NoUserInput = 5
UnknownFailure = 6
```

---

## PromptCreateAvatarResult
```
Success = 1
PermissionDenied = 2
Timeout = 3
UploadFailed = 4
NoUserInput = 5
InvalidHumanoidDescription = 6
UGCValidationFailed = 7
ModeratedName = 8
MaxOutfits = 9
PurchaseFailure = 10
UnknownFailure = 11
TokenInvalid = 12
```

---

## PromptLinkSharingResult
```
Success = 1
PlayerLeft = 2
InvalidLaunchData = 3
```

---

## PromptPublishAssetResult
```
Success = 1
PermissionDenied = 2
Timeout = 3
UploadFailed = 4
NoUserInput = 5
UnknownFailure = 6
```

---

## PropertyStatus
```
Ok = 0
Warning = 1
Error = 2
```

---

## ProximityPromptExclusivity
```
OnePerButton = 0
OneGlobally = 1
AlwaysShow = 2
```

---

## ProximityPromptInputType
```
Keyboard = 0
Gamepad = 1
Touch = 2
```

---

## ProximityPromptStyle
```
Default = 0
Custom = 1
```

---

## QualityLevel
```
Automatic = 0
Level01 = 1
Level02 = 2
Level03 = 3
Level04 = 4
Level05 = 5
Level06 = 6
Level07 = 7
Level08 = 8
Level09 = 9
Level10 = 10
Level11 = 11
Level12 = 12
Level13 = 13
Level14 = 14
Level15 = 15
Level16 = 16
Level17 = 17
Level18 = 18
Level19 = 19
Level20 = 20
Level21 = 21
```

---

## R15CollisionType
```
OuterBox = 0
InnerBox = 1
```

---

## RaycastFilterType
```
Exclude = 0
Include = 1
```

---

## ReadCapturesFromGalleryResult
```
Success = 0
NeedPermission = 1
```

---

## RecommendationActionType
```
AddReaction = 0
RemoveReaction = 1
Share = 2
Report = 3
Comment = 4
Play = 5
Purchase = 6
```

---

## RecommendationImpressionType
```
View = 0
```

---

## RecommendationItemVisibility
```
Private = 0
Public = 1
```

---

## RejectCharacterDeletions
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## RenderFidelity
```
Automatic = 0
Precise = 1
Performance = 2
```

---

## RenderPriority
```
First = 0
Input = 100
Camera = 200
Character = 300
Last = 2000
```

---

## RenderingCacheOptimizationMode
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## RenderingTestComparisonMethod
```
psnr = 0
diff = 1
```

---

## ReplicateInstanceDestroySetting
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## ResamplerMode
```
Default = 0
Pixelated = 1
```

---

## ReservedHighlightId
```
Standard = 0
Selection = 524288
Hover = 262144
Active = 131072
```

---

## RestPose
```
Default = 0
RotationsReset = 1
Custom = 2
```

---

## ReturnKeyType
```
Default = 0
Done = 1
Go = 2
Next = 3
Search = 4
Send = 5
```

---

## ReverbType
```
NoReverb = 0
GenericReverb = 1
PaddedCell = 2
Room = 3
Bathroom = 4
LivingRoom = 5
StoneRoom = 6
Auditorium = 7
ConcertHall = 8
Cave = 9
Arena = 10
Hangar = 11
CarpettedHallway = 12
Hallway = 13
StoneCorridor = 14
Alley = 15
Forest = 16
City = 17
Mountains = 18
Quarry = 19
Plain = 20
ParkingLot = 21
SewerPipe = 22
UnderWater = 23
```

---

## RibbonTool
```
Select = 0
Scale = 1
Rotate = 2
Move = 3
Transform = 4
ColorPicker = 5
MaterialPicker = 6
Group = 7
Ungroup = 8
None = 9
PivotEditor = 10
```

---

## RigScale
```
Default = 0
Rthro = 1
RthroNarrow = 2
```

---

## RigType
```
R15 = 0
Custom = 1
None = 2
```

---

## RollOffMode
```
Inverse = 0
Linear = 1
LinearSquare = 2
InverseTapered = 3
```

---

## RolloutState
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## RotationOrder
```
XYZ = 0
XZY = 1
YZX = 2
YXZ = 3
ZXY = 4
ZYX = 5
```

---

## RotationType
```
MovementRelative = 0
CameraRelative = 1
```

---

## RsvpStatus
```
None = 0
Going = 1
NotGoing = 2
```

---

## RtlTextSupport
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## RunContext
```
Legacy = 0
Server = 1
Client = 2
Plugin = 3
```

---

## RunState
```
Stopped = 0
Running = 1
Paused = 2
```

---

## RuntimeUndoBehavior
```
Aggregate = 0
Snapshot = 1
Hybrid = 2
```

---

## SafeAreaCompatibility
```
None = 0
FullscreenExtension = 1
```

---

## SalesTypeFilter
```
All = 1
Collectibles = 2
Premium = 3
```

---

## SandboxedInstanceMode
```
Default = 0
Experimental = 1
```

---

## SaveAvatarThumbnailCustomizationFailure
```
BadThumbnailType = 1
BadYRotDeg = 2
BadFieldOfViewDeg = 3
BadDistanceScale = 4
Other = 5
Throttled = 6
```

---

## SaveFilter
**Tags:** Deprecated
```
SaveWorld = 0
SaveGame = 1
SaveAll = 2
```

---

## SavedQualitySetting
```
Automatic = 0
QualityLevel1 = 1
QualityLevel2 = 2
QualityLevel3 = 3
QualityLevel4 = 4
QualityLevel5 = 5
QualityLevel6 = 6
QualityLevel7 = 7
QualityLevel8 = 8
QualityLevel9 = 9
QualityLevel10 = 10
```

---

## ScaleType
```
Stretch = 0
Slice = 1
Tile = 2
Fit = 3
Crop = 4
```

---

## ScopeCheckResult
```
ConsentAccepted = 0
InvalidScopes = 1
Timeout = 2
NoUserInput = 3
BackendError = 4
UnexpectedError = 5
InvalidArgument = 6
ConsentDenied = 7
```

---

## ScreenInsets
```
None = 0
DeviceSafeInsets = 1
CoreUISafeInsets = 2
TopbarSafeInsets = 3
```

---

## ScreenOrientation
```
LandscapeLeft = 0
LandscapeRight = 1
LandscapeSensor = 2
Portrait = 3
Sensor = 4
```

---

## ScrollBarInset
```
None = 0
ScrollBar = 1
Always = 2
```

---

## ScrollingDirection
```
X = 1
Y = 2
XY = 4
```

---

## SecurityCapability
```
RunClientScript = 0
RunServerScript = 1
AccessOutsideWrite = 2
AssetRequire = 3
LoadString = 4
ScriptGlobals = 5
CreateInstances = 6
Basic = 7
Audio = 8
DataStore = 9
Network = 10
Physics = 11
UI = 12
CSG = 13
Chat = 14
Animation = 15
Avatar = 16
Input = 17
Environment = 18
RemoteEvent = 19
LegacySound = 20
Players = 21
CapabilityControl = 22
```

---

## SelectionBehavior
```
Escape = 0
Stop = 1
```

---

## SelectionRenderMode
```
Outlines = 0
BoundingBoxes = 1
Both = 2
```

---

## SelfViewPosition
```
LastPosition = 0
TopLeft = 1
TopRight = 2
BottomLeft = 3
BottomRight = 4
```

---

## SensorMode
```
Floor = 0
Ladder = 1
```

---

## SensorUpdateType
```
OnRead = 0
Manual = 1
```

---

## ServerLiveEditingMode
```
Uninitialized = 0
Enabled = 1
Disabled = 2
```

---

## ServiceVisibility
```
Always = 0
Off = 1
WithChildren = 2
```

---

## Severity
```
Error = 1
Warning = 2
Information = 3
Hint = 4
```

---

## ShowAdResult
```
ShowCompleted = 1
AdNotReady = 2
AdAlreadyShowing = 3
InternalError = 4
ShowInterrupted = 5
InsufficientMemory = 6
```

---

## SignalBehavior
```
Default = 0
Immediate = 1
Deferred = 2
AncestryDeferred = 3
```

---

## SizeConstraint
```
RelativeXY = 0
RelativeXX = 1
RelativeYY = 2
```

---

## SolverConvergenceMetricType
```
IterationBased = 0
AlgorithmAgnostic = 1
```

---

## SolverConvergenceVisualizationMode
```
Disabled = 0
PerIsland = 1
PerEdge = 2
```

---

## SortDirection
```
Ascending = 0
Descending = 1
```

---

## SortOrder
```
Name = 0
Custom = 1 [Deprecated]
LayoutOrder = 2
```

---

## SpecialKey
```
Insert = 0
Home = 1
End = 2
PageUp = 3
PageDown = 4
ChatHotkey = 5
```

---

## StartCorner
```
TopLeft = 0
TopRight = 1
BottomLeft = 2
BottomRight = 3
```

---

## StateObjectFieldType
```
Boolean = 0 [Deprecated]
CFrame = 1 [Deprecated]
Color3 = 2 [Deprecated]
Float = 3 [Deprecated]
Instance = 4 [Deprecated]
Random = 5 [Deprecated]
Vector2 = 6 [Deprecated]
Vector3 = 7 [Deprecated]
INVALID = 8 [Deprecated]
```

---

## Status
**Tags:** Deprecated
```
Poison = 0 [Deprecated]
Confusion = 1 [Deprecated]
```

---

## StreamOutBehavior
```
Default = 0
LowMemory = 1
Opportunistic = 2
```

---

## StreamingIntegrityMode
```
Default = 0
Disabled = 1
MinimumRadiusPause = 2
PauseOutsideLoadedArea = 3
```

---

## StreamingPauseMode
```
Default = 0 [Deprecated]
Disabled = 1 [Deprecated]
ClientPhysicsPause = 2 [Deprecated]
```

---

## StrokeSizingMode
```
FixedSize = 0
ScaledSize = 1
```

---

## StudioCloseMode
```
None = 0
CloseStudio = 1
CloseDoc = 2
LogOut = 3
```

---

## StudioDataModelType
```
Edit = 0
PlayClient = 1
PlayServer = 2
Standalone = 3
None = 4
```

---

## StudioPlaceUpdateFailureReason
```
Other = 0
TeamCreateConflict = 1
```

---

## StudioScriptEditorColorCategories
```
Default = 0
Operator = 1
Number = 2
String = 3
Comment = 4
Keyword = 5
Builtin = 6
Method = 7
Property = 8
Nil = 9
Bool = 10
Function = 11
Local = 12
Self = 13
LuauKeyword = 14
FunctionName = 15
TODO = 16
Background = 17
SelectionText = 18
SelectionBackground = 19
FindSelectionBackground = 20
MatchingWordBackground = 21
Warning = 22
Error = 23
Info = 24
Hint = 25
Whitespace = 26
ActiveLine = 27
DebuggerCurrentLine = 28
DebuggerErrorLine = 29
Ruler = 30
Bracket = 31
Type = 32
MenuPrimaryText = 33
MenuSecondaryText = 34
MenuSelectedText = 35
MenuBackground = 36
MenuSelectedBackground = 37
MenuScrollbarBackground = 38
MenuScrollbarHandle = 39
MenuBorder = 40
DocViewCodeBackground = 41
AICOOverlayText = 42
AICOOverlayButtonBackground = 43
AICOOverlayButtonBackgroundHover = 44
AICOOverlayButtonBackgroundPressed = 45
IndentationRuler = 46
```

---

## StudioScriptEditorColorPresets
```
RobloxDefault = 0
Extra1 = 1
Extra2 = 2
Custom = 3
```

---

## StudioStyleGuideColor
```
MainBackground = 0
Titlebar = 1
Dropdown = 2
Tooltip = 3
Notification = 4
ScrollBar = 5
ScrollBarBackground = 6
TabBar = 7
Tab = 8
FilterButtonDefault = 9
FilterButtonHover = 10
FilterButtonChecked = 11
FilterButtonAccent = 12
FilterButtonBorder = 13
FilterButtonBorderAlt = 14
RibbonTab = 15
RibbonTabTopBar = 16
Button = 17
MainButton = 18
RibbonButton = 19
ViewPortBackground = 20
InputFieldBackground = 21
Item = 22
TableItem = 23
CategoryItem = 24
GameSettingsTableItem = 25
GameSettingsTooltip = 26
EmulatorBar = 27
EmulatorDropDown = 28
ColorPickerFrame = 29
CurrentMarker = 30
Border = 31
DropShadow = 32
Shadow = 33
Light = 34
Dark = 35
Mid = 36
MainText = 37
SubText = 38
TitlebarText = 39
BrightText = 40
DimmedText = 41
LinkText = 42
WarningText = 43
ErrorText = 44
InfoText = 45
SensitiveText = 46
ScriptSideWidget = 47
ScriptBackground = 48
ScriptText = 49
ScriptSelectionText = 50
ScriptSelectionBackground = 51
ScriptFindSelectionBackground = 52
ScriptMatchingWordSelectionBackground = 53
ScriptOperator = 54
ScriptNumber = 55
ScriptString = 56
ScriptComment = 57
ScriptKeyword = 58
ScriptBuiltInFunction = 59
ScriptWarning = 60
ScriptError = 61
ScriptInformation = 62
ScriptHint = 63
ScriptWhitespace = 64
ScriptRuler = 65
DocViewCodeBackground = 66
DebuggerCurrentLine = 67
DebuggerErrorLine = 68
DiffFilePathText = 69
DiffTextHunkInfo = 70
DiffTextNoChange = 71
DiffTextAddition = 72
DiffTextDeletion = 73
DiffTextSeparatorBackground = 74
DiffTextNoChangeBackground = 75
DiffTextAdditionBackground = 76
DiffTextDeletionBackground = 77
DiffLineNum = 78
DiffLineNumSeparatorBackground = 79
DiffLineNumNoChangeBackground = 80
DiffLineNumAdditionBackground = 81
DiffLineNumDeletionBackground = 82
DiffFilePathBackground = 83
DiffFilePathBorder = 84
ChatIncomingBgColor = 85
ChatIncomingTextColor = 86
ChatOutgoingBgColor = 87
ChatOutgoingTextColor = 88
ChatModeratedMessageColor = 89
Separator = 90
ButtonBorder = 91
ButtonText = 92
InputFieldBorder = 93
CheckedFieldBackground = 94
CheckedFieldBorder = 95
CheckedFieldIndicator = 96
HeaderSection = 97
Midlight = 98
StatusBar = 99
DialogButton = 100
DialogButtonText = 101
DialogButtonBorder = 102
DialogMainButton = 103
DialogMainButtonText = 104
InfoBarWarningBackground = 105
InfoBarWarningText = 106
ScriptEditorCurrentLine = 107
ScriptMethod = 108
ScriptProperty = 109
ScriptNil = 110
ScriptBool = 111
ScriptFunction = 112
ScriptLocal = 113
ScriptSelf = 114
ScriptLuauKeyword = 115
ScriptFunctionName = 116
ScriptTodo = 117
ScriptBracket = 118
AttributeCog = 119
AICOOverlayText = 128
AICOOverlayButtonBackground = 129
AICOOverlayButtonBackgroundHover = 130
AICOOverlayButtonBackgroundPressed = 131
OnboardingCover = 132
OnboardingHighlight = 133
OnboardingShadow = 134
BreakpointMarker = 136
DiffLineNumHover = 137
DiffLineNumSeparatorBackgroundHover = 138
```

---

## StudioStyleGuideModifier
```
Default = 0
Selected = 1
Pressed = 2
Disabled = 3
Hover = 4
```

---

## Style
```
AlternatingSupports = 0
BridgeStyleSupports = 1
NoSupports = 2
```

---

## SubscriptionExpirationReason
```
ProductInactive = 0
ProductDeleted = 1
SubscriberCancelled = 2
SubscriberRefunded = 3
Lapsed = 4
```

---

## SubscriptionPaymentStatus
```
Paid = 0
Refunded = 1
```

---

## SubscriptionPeriod
```
Month = 0
```

---

## SubscriptionState
```
NeverSubscribed = 0
SubscribedWillRenew = 1
SubscribedWillNotRenew = 2
SubscribedRenewalPaymentPending = 3
Expired = 4
```

---

## SurfaceConstraint
```
None = 0
Hinge = 1
SteppingMotor = 2
Motor = 3
```

---

## SurfaceGuiShape
```
Flat = 0
CurvedHorizontally = 1
```

---

## SurfaceGuiSizingMode
```
FixedSize = 0
PixelsPerStud = 1
```

---

## SurfaceType
```
Smooth = 0
Glue = 1
Weld = 2
Studs = 3
Inlet = 4
Universal = 5
Hinge = 6
Motor = 7
SteppingMotor = 8
SmoothNoOutlines = 10
```

---

## SwipeDirection
```
Right = 0
Left = 1
Up = 2
Down = 3
None = 4
```

---

## SystemThemeValue
```
error = 0
light = 1
dark = 2
systemLight = 3
systemDark = 4
```

---

## TableMajorAxis
```
RowMajor = 0
ColumnMajor = 1
```

---

## TeamCreateErrorState
```
PlaceSizeTooLarge = 0
PlaceSizeApproachingLimit = 1
NoError = 2
```

---

## Technology
```
Voxel = 1
Compatibility = 2
ShadowMap = 3
Future = 4
Legacy = 0 [Deprecated]
Unified = 5 [Deprecated]
```

---

## TeleportMethod
```
TeleportToSpawnByName = 0
TeleportToPlaceInstance = 1
TeleportToPrivateServer = 2
TeleportPartyAsync = 3
TeleportToVIPServer = 4
TeleportToInstanceBack = 5
TeleportUnknown = 6
```

---

## TeleportResult
```
Success = 0
Failure = 1
GameNotFound = 2
GameEnded = 3
GameFull = 4
Unauthorized = 5
Flooded = 6
IsTeleporting = 7
```

---

## TeleportState
```
RequestedFromServer = 0
Started = 1
WaitingForServer = 2
Failed = 3
InProgress = 4
```

---

## TeleportType
```
ToPlace = 0
ToInstance = 1
ToReservedServer = 2
ToVIPServer = 3
ToInstanceBack = 4
```

---

## TerrainAcquisitionMethod
```
None = 0
Legacy = 1
Template = 2
Generate = 3
Import = 4
Convert = 5
EditAddTool = 6
EditSeaLevelTool = 7
EditReplaceTool = 8
RegionFillTool = 9
RegionPasteTool = 10
Other = 11
```

---

## TerrainFace
```
Top = 0
Side = 1
Bottom = 2
```

---

## TextChatMessageStatus
```
Unknown = 1
Success = 2
Sending = 3
TextFilterFailed = 4
Floodchecked = 5
InvalidPrivacySettings = 6
InvalidTextChannelPermissions = 7
MessageTooLong = 8
ModerationTimeout = 9
```

---

## TextDirection
```
Auto = 0
LeftToRight = 1
RightToLeft = 2
```

---

## TextFilterContext
```
PublicChat = 1
PrivateChat = 2
```

---

## TextInputType
```
Default = 0
NoSuggestions = 1
Number = 2
Email = 3
Phone = 4
Password = 5
PasswordShown = 6
Username = 7
OneTimePassword = 8
```

---

## TextTruncate
```
None = 0
AtEnd = 1
SplitWord = 2
```

---

## TextXAlignment
```
Left = 0
Right = 1
Center = 2
```

---

## TextYAlignment
```
Top = 0
Center = 1
Bottom = 2
```

---

## TextureMode
```
Stretch = 0
Wrap = 1
Static = 2
```

---

## TextureQueryType
```
NonHumanoid = 0
NonHumanoidOrphaned = 1
Humanoid = 2
HumanoidOrphaned = 3
```

---

## ThreadPoolConfig
```
PerCore4 = 104
PerCore3 = 103
PerCore2 = 102
PerCore1 = 101
Auto = 0
Threads1 = 1
Threads2 = 2
Threads3 = 3
Threads4 = 4
Threads8 = 8
Threads16 = 16
```

---

## ThrottlingPriority
```
Extreme = 2
ElevatedOnServer = 1
Default = 0
```

---

## ThumbnailSize
```
Size48x48 = 0
Size180x180 = 1
Size420x420 = 2
Size60x60 = 3
Size100x100 = 4
Size150x150 = 5
Size352x352 = 6
```

---

## ThumbnailType
```
HeadShot = 0
AvatarBust = 1
AvatarThumbnail = 2
```

---

## TickCountSampleMethod
```
Fast = 0
Benchmark = 1
Precise = 2
```

---

## TonemapperPreset
```
Default = 0
Retro = 1
```

---

## TopBottom
```
Top = 0
Center = 1
Bottom = 2
```

---

## TouchCameraMovementMode
```
Default = 0
Classic = 1
Follow = 2
Orbital = 3
```

---

## TouchMovementMode
```
Default = 0
Thumbstick = 1
DPad = 2
Thumbpad = 3
ClickToMove = 4
DynamicThumbstick = 5
```

---

## TrackerError
```
Ok = 0
NoService = 1
InitFailed = 2
NoVideo = 3
VideoError = 4
VideoNoPermission = 5
VideoUnsupported = 6
NoAudio = 7
AudioError = 8
AudioNoPermission = 9
UnsupportedDevice = 10
```

---

## TrackerExtrapolationFlagMode
```
Auto = 3
ForceDisabled = 0
ExtrapolateFacsAndPose = 1
ExtrapolateFacsOnly = 2
```

---

## TrackerFaceTrackingStatus
```
FaceTrackingSuccess = 0
FaceTrackingNoFaceFound = 1
FaceTrackingUnknown = 2
FaceTrackingLost = 3
FaceTrackingHasTrackingError = 4
FaceTrackingIsOccluded = 5
FaceTrackingUninitialized = 6
```

---

## TrackerLodFlagMode
```
Auto = 2
ForceFalse = 0
ForceTrue = 1
```

---

## TrackerLodValueMode
```
Auto = 2
Force0 = 0
Force1 = 1
```

---

## TrackerMode
```
None = 0
Audio = 1
Video = 2
AudioVideo = 3
```

---

## TrackerPromptEvent
```
LODCameraRecommendDisable = 0
```

---

## TrackerType
```
None = 0
Face = 1
UpperBody = 2
```

---

## TriStateBoolean
```
False = 2
True = 1
Unknown = 0
```

---

## TweenStatus
```
Canceled = 0
Completed = 1
```

---

## UICaptureMode
```
All = 0
None = 1
```

---

## UIDragDetectorBoundingBehavior
```
Automatic = 0
EntireObject = 1
HitPoint = 2
```

---

## UIDragDetectorDragRelativity
```
Absolute = 0
Relative = 1
```

---

## UIDragDetectorDragSpace
```
Parent = 0
LayerCollector = 1
Reference = 2
```

---

## UIDragDetectorDragStyle
```
TranslatePlane = 0
TranslateLine = 1
Rotate = 2
Scriptable = 3
```

---

## UIDragDetectorResponseStyle
```
Offset = 0
Scale = 1
CustomOffset = 2
CustomScale = 3
```

---

## UIDragSpeedAxisMapping
```
XY = 0
XX = 1
YY = 2
```

---

## UIFlexAlignment
```
None = 0
Fill = 1
SpaceAround = 2
SpaceBetween = 3
SpaceEvenly = 4
```

---

## UIFlexMode
```
None = 0
Grow = 1
Shrink = 2
Fill = 3
Custom = 4
```

---

## UITheme
```
Light = 0 [Deprecated]
Dark = 1 [Deprecated]
```

---

## UiMessageType
```
UiMessageError = 0
UiMessageInfo = 1
```

---

## UploadCaptureResult
```
Success = 0
NeedPermission = 1
CaptureModerated = 2
CaptureNotInGallery = 3
IneligibleCapture = 4
```

---

## UsageContext
```
Default = 0
Preview = 1
```

---

## UserCFrame
```
Head = 0
LeftHand = 1
RightHand = 2
Floor = 3
```

---

## UserInputState
```
Begin = 0
Change = 1
End = 2
Cancel = 3
None = 4
```

---

## UserInputType
```
MouseButton1 = 0
MouseButton2 = 1
MouseButton3 = 2
MouseWheel = 3
MouseMovement = 4
Touch = 7
Keyboard = 8
Focus = 9
Accelerometer = 10
Gyro = 11
Gamepad1 = 12
Gamepad2 = 13
Gamepad3 = 14
Gamepad4 = 15
Gamepad5 = 16
Gamepad6 = 17
Gamepad7 = 18
Gamepad8 = 19
TextInput = 20
InputMethod = 21
None = 22
```

---

## VRComfortSetting
```
Comfort = 0
Normal = 1
Expert = 2
Custom = 3
```

---

## VRControllerModelMode
```
Disabled = 0
Transparent = 1
```

---

## VRDeviceType
```
Unknown = 0
OculusRift = 1
HTCVive = 2
ValveIndex = 3
OculusQuest = 4
```

---

## VRLaserPointerMode
```
Disabled = 0
Pointer = 1
DualPointer = 2
```

---

## VRSafetyBubbleMode
```
NoOne = 0
OnlyFriends = 1
Anyone = 2
```

---

## VRScaling
```
World = 0
Off = 1
```

---

## VRSessionState
```
Undefined = 0
Idle = 1
Visible = 2
Focused = 3
Stopping = 4
```

---

## VRTouchpad
```
Left = 0
Right = 1
```

---

## VRTouchpadMode
```
Touch = 0
VirtualThumbstick = 1
ABXY = 2
```

---

## VelocityConstraintMode
```
Line = 0
Plane = 1
Vector = 2
```

---

## VerticalAlignment
```
Center = 0
Top = 1
Bottom = 2
```

---

## VerticalScrollBarPosition
```
Right = 0
Left = 1
```

---

## VibrationMotor
```
Large = 0
Small = 1
LeftTrigger = 2
RightTrigger = 3
LeftHand = 4
RightHand = 5
```

---

## VideoCaptureResult
```
Success = 0
OtherError = 1
ScreenSizeChanged = 2
TimeLimitReached = 3
```

---

## VideoCaptureStartedResult
```
Success = 0
OtherError = 1
CapturingAlready = 2
NoDeviceSupport = 3
NoSpaceOnDevice = 4
```

---

## VideoDeviceCaptureQuality
```
Default = 0
Low = 1
Medium = 2
High = 3
```

---

## VideoError
```
Ok = 0
Eof = 1
EAgain = 2
BadParameter = 3
AllocFailed = 4
CodecInitFailed = 5
CodecCloseFailed = 6
DecodeFailed = 7
ParsingFailed = 8
Unsupported = 9
Generic = 10
DownloadFailed = 11
StreamNotFound = 12
EncodeFailed = 13
CreateFailed = 14
NoPermission = 15
NoService = 16
ReleaseFailed = 17
Unknown = 18
```

---

## ViewMode
```
None = 0
GeometryComplexity = 1
Transparent = 2
Decal = 3
```

---

## VirtualCursorMode
```
Default = 0
Disabled = 1
Enabled = 2
```

---

## VirtualInputMode
```
None = 0
Recording = 1
Playing = 2
```

---

## VoiceChatDistanceAttenuationType
```
Inverse = 0
Legacy = 1
```

---

## VoiceChatState
```
Idle = 0
Joining = 1
JoiningRetry = 2
Joined = 3
Leaving = 4
Ended = 5
Failed = 6
```

---

## VoiceControlPath
```
Publish = 0
Subscribe = 1
Join = 2
```

---

## VolumetricAudio
```
Disabled = 0
Automatic = 1
Enabled = 2
```

---

## WaterDirection
```
NegX = 0
X = 1
NegY = 2
Y = 3
NegZ = 4
Z = 5
```

---

## WaterForce
```
None = 0
Small = 1
Medium = 2
Strong = 3
Max = 4
```

---

## WebSocketState
```
Connecting = 0
Open = 1
Closing = 2
Closed = 3
```

---

## WeldConstraintPreserve
```
All = 0
None = 1
Touching = 2
```

---

## WhisperChatPrivacyMode
```
AllUsers = 0
NoOne = 1
```

---

## WrapLayerAutoSkin
```
Disabled = 0
EnabledPreserve = 1
EnabledOverride = 2
```

---

## WrapLayerDebugMode
```
None = 0
BoundCage = 1
LayerCage = 2
BoundCageAndLinks = 3
Reference = 4
Rbf = 5
OuterCage = 6
ReferenceMeshAfterMorph = 7
HSROuterDetail = 8
HSROuter = 9
HSRInner = 10
HSRInnerReverse = 11
LayerCageFittedToBase = 12
LayerCageFittedToPrev = 13
PreWrapDeformerOuterCage = 14
```

---

## WrapTargetDebugMode
```
None = 0
TargetCageOriginal = 1
TargetCageCompressed = 2
TargetCageInterface = 3
TargetLayerCageOriginal = 4
TargetLayerCageCompressed = 5
TargetLayerInterface = 6
Rbf = 7
OuterCageDetail = 8
PreWrapDeformerCage = 9
```

---

## ZIndexBehavior
```
Global = 0
Sibling = 1
```

---
