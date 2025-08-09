# Object

## Properties
```
ClassName: string [ReadOnly]
className: string [ReadOnly] [Deprecated]
```

## Functions
```
GetPropertyChangedSignal(property: string) → RBXScriptSignal
IsA(className: string) → bool
isA(className: string) → bool [Deprecated]
```

## Events
```
Changed(property: string)
```

---

# Capture
**Extends:** Object

## Properties
```
CaptureTime: DateTime [ReadOnly]
CaptureType: CaptureType [ReadOnly]
LocalId: string [ReadOnly]
SourcePlaceId: int64 [ReadOnly]
SourceUniverseId: int64 [ReadOnly]
```

---

# ScreenshotCapture
**Extends:** Capture

---

# VideoCapture
**Extends:** Capture

## Properties
```
FilePath: string [ReadOnly]
TimeLength: double [ReadOnly]
```

---

# ConfigSnapshot
**Extends:** Object

## Properties
```
Error: ConfigSnapshotErrorState [ReadOnly]
Outdated: bool [ReadOnly]
```

## Functions
```
GetValue(key: string, defaultValue: Variant) → Variant
GetValueChangedSignal(key: string) → RBXScriptSignal
Refresh() → null
```

## Events
```
UpdateAvailable()
```

---

# EditableImage
**Extends:** Object

## Properties
```
ImageData: BinaryString
IsReplicatedCopy: bool
Size: Vector2 [ReadOnly]
```

## Functions
```
Destroy() → null
DrawCircle(center: Vector2, radius: int, color: Color3, transparency: float, combineType: ImageCombineType) → null
DrawImage(position: Vector2, image: EditableImage, combineType: ImageCombineType) → null
DrawImageProjected(mesh: EditableMesh, projection: Dictionary, brushConfig: Dictionary) → null
DrawImageTransformed(position: Vector2, scale: Vector2, rotation: float, image: EditableImage, options: Dictionary?) → null
DrawLine(p1: Vector2, p2: Vector2, color: Color3, transparency: float, combineType: ImageCombineType) → null
DrawRectangle(position: Vector2, size: Vector2, color: Color3, transparency: float, combineType: ImageCombineType) → null
DrawTriangle(p1: Vector2, p2: Vector2, p3: Vector2, color: Color3, transparency: float) → null
ReadPixelsBuffer(position: Vector2, size: Vector2) → buffer
WritePixelsBuffer(position: Vector2, size: Vector2, buffer: buffer) → null
```

---

# EditableMesh
**Extends:** Object

## Properties
```
FixedSize: bool [ReadOnly]
IsReplicatedCopy: bool
MeshData: SharedString
SkinningEnabled: bool [Deprecated]
```

## Functions
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

# Instance
**Extends:** Object

## Properties
```
Archivable: bool
Attributes: string [ReadOnly]
AttributesReplicate: string
AttributesSerialize: BinaryString
Capabilities: SecurityCapabilities
DataCost: int [ReadOnly] [Deprecated]
DefinesCapabilities: bool
HistoryId: UniqueId
Name: string
Parent: Instance
PropertyStatusStudio: PropertyStatus [ReadOnly]
RobloxLocked: bool
Sandboxed: bool
SourceAssetId: int64
Tags: BinaryString
UniqueId: UniqueId
archivable: bool [Deprecated]
numExpectedDirectChildren: int
```

## Functions
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
GetDebugId(scopeLength: int) → string
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

## Events
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

# AccessoryDescription
**Extends:** Instance

## Properties
```
AccessoryType: AccessoryType
AssetId: int64
Instance: Instance
IsLayered: bool
Order: int
Position: Vector3
Puffiness: float
Rotation: Vector3
Scale: Vector3
```

## Functions
```
GetAppliedInstance() → Instance
```

---

# AccountService
**Extends:** Instance

## Functions
```
DeviceAccessTokenAvailable() → bool
DeviceIntegrityAvailable() → bool
GetDeviceIntegrityToken(data: string) → string
MagicLogin(data: string) → null
GetCredentialsHeaders() → string
GetDeviceAccessToken() → string
GetDeviceIntegrityTokenYield(data: string) → string
```

## Events
```
MagicLoginEvent(data: string)
```

---

# Accoutrement
**Extends:** Instance

## Properties
```
AttachmentForward: Vector3
AttachmentPoint: CFrame
AttachmentPos: Vector3
AttachmentRight: Vector3
AttachmentUp: Vector3
BackendAccoutrementState: int
```

## Events
```
ServerEquipAccoutrement(character: Instance)
ServerUnequipAccoutrement(oldCharacter: Instance)
```

---

# Accessory
**Extends:** Accoutrement

## Properties
```
AccessoryType: AccessoryType
```

---

# Hat
**Extends:** Accoutrement

---

# AchievementService
**Extends:** Instance

## Functions
```
IsAvailable() → bool
GrantAchievement(achievementName: string) → bool
HasAchieved(achievementName: string) → bool
```

---

# ActivityHistoryEventService
**Extends:** Instance

## Events
```
WriteActivityHistoryEventFromStudio(eventType: int, resourceId: int64, metadata: string)
```

---

# AdPortal
**Extends:** Instance

## Properties
```
PortalInvalidReason: string [ReadOnly]
PortalVersion: int64 [ReadOnly]
Status: AdUnitStatus [ReadOnly]
```

## Functions
```
TeleportConfirmed(placeId: int64, player: Player) → null
TeleportRejected(shouldCooldown: bool, rejectedByDistance: bool) → null
```

---

# AdService
**Extends:** Instance

## Functions
```
CreateAdRewardFromDevProductId(devProductId: int64) → AdReward
GetAdTeleportInfo() → Tuple
GetReportAdInfo() → Array
HandleWhyThisAdClicked(advertiserName: string, payerName: string) → null
HideEudsaDisclosure() → null
OnDemandVideoCompleteFromUI(result: ShowAdResult, encryptedAdTrackingData: string, encryptionMetadata: string, rewardDetails: string) → null
ReturnToPublisherExperience(adTeleportMethod: AdTeleportMethod) → null
SetAdGuiInteractivityHandlerInitialized() → null
ShowVideoAd() → null [Deprecated]
UnregisterAdOpportunity(instance: Instance) → null
GetAdAvailabilityNowAsync(adFormat: AdFormat) → Variant
RegisterAdOpportunityAsync(instance: Instance, placementId: int64?) → null
ShowRewardedVideoAdAsync(player: Player, reward: AdReward, placementId: int64?) → ShowAdResult
```

## Events
```
AdTeleportEnded()
AdTeleportInitiated()
PortalPrompt(destinationId: int64, portal: Instance, requiresNoButton: bool)
ReportImpressionSignal(ad_instance_name: string, encrypted_ad_tracking_data: string, encryption_metadata: string)
ReportTeleportSignal(ad_instance_name: string, encrypted_ad_tracking_data: string, encryption_metadata: string, teleport_type: string, teleport_source_universe_id: int64, teleport_source_place_id: int64, teleport_dest_place_id: int64)
RewardedVideoAdEnded()
RewardedVideoAdStarted()
ServeAdResponseSignal(uuid: string, response: string, isError: bool)
ServeAdSignal(uuid: string, request: string)
ShowDynamicEudsaDisclosure(advertiserName: string, payerName: string)
ShowReportAdPopup(adInfo: Dictionary)
VideoAdClosed(adShown: bool)
adGuiRegisterUI(adGui: Instance)
rewardedVideoAdPlayServerToClient(rewardDetails: string)
rewardedVideoAdPlayServerToClientWithPlacement(rewardDetails: string, placementId: int64)
rewardedVideoAdResultClientToServer(result: ShowAdResult, encryptedAdTrackingData: string, encryptionMetadata: string)
```

---

# AdvancedDragger
**Extends:** Instance

---

# AnalyticsService
**Extends:** Instance

## Properties
```
ApiKey: string [Deprecated]
```

## Functions
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

# Animation
**Extends:** Instance

## Properties
```
AnimationId: ContentId
```

---

# AnimationClip
**Extends:** Instance

## Properties
```
Guid: string
GuidBinaryString: BinaryString
Loop: bool
Priority: AnimationPriority
```

---

# CurveAnimation
**Extends:** AnimationClip

---

# KeyframeSequence
**Extends:** AnimationClip

## Properties
```
AuthoredHipHeight: float
```

## Functions
```
AddKeyframe(keyframe: Instance) → null
GetKeyframes() → Instances
RemoveKeyframe(keyframe: Instance) → null
```

---

# AnimationClipProvider
**Extends:** Instance

## Functions
```
GetAnimationClip(assetId: ContentId) → AnimationClip [Deprecated]
GetAnimationClipById(assetId: int64, useCache: bool) → AnimationClip [Deprecated]
GetMemStats() → Dictionary
RegisterActiveAnimationClip(animationClip: AnimationClip) → ContentId
RegisterAnimationClip(animationClip: AnimationClip) → ContentId
GetAnimationClipAsync(assetId: ContentId) → AnimationClip
GetAnimations(userId: int64) → Instance
GetClipEvaluatorAsync(assetId: ContentId) → ClipEvaluator
```

---

# AnimationController
**Extends:** Instance

## Functions
```
GetPlayingAnimationTracks() → Array [Deprecated]
LoadAnimation(animation: Animation) → AnimationTrack [Deprecated]
```

## Events
```
AnimationPlayed(animationTrack: AnimationTrack)
```

---

# AnimationFromVideoCreatorService
**Extends:** Instance

## Functions
```
CreateJob(filePath: string) → string
DownloadJobResult(jobId: string, outputFilePath: string) → string
FullProcess(videoFilePath: string, progressCallback: Function) → string
GetJobStatus(jobId: string) → string
```

---

# AnimationFromVideoCreatorStudioService
**Extends:** Instance

## Functions
```
IsAgeRestricted() → bool
CreateAnimationByUploadingVideo(progressCallback: Function) → string
ImportVideoWithPrompt() → string
```

---

# AnimationRigData
**Extends:** Instance

## Properties
```
label: BinaryString
name: BinaryString
parent: BinaryString
postTransform: BinaryString
preTransform: BinaryString
transform: BinaryString
```

## Functions
```
LoadFromHumanoid(humanoid: Instance) → bool
LoadFromModel(model: Instance) → bool
```

---

# AnimationStreamTrack
**Extends:** Instance

## Properties
```
Animation: TrackerStreamAnimation [ReadOnly]
FACSDataLod: FACSDataLod [ReadOnly]
IsPlaying: bool [ReadOnly]
Priority: AnimationPriority
WeightCurrent: float [ReadOnly]
WeightTarget: float [ReadOnly]
```

## Functions
```
AdjustWeight(weight: float, fadeTime: float) → null
GetActive() → bool
GetTrackerData() → Tuple
Play(fadeTime: float, weight: float) → null
Stop(fadeTime: float) → null
TogglePause(paused: bool) → null
```

## Events
```
Stopped()
```

---

# AnimationTrack
**Extends:** Instance

## Properties
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

## Functions
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

## Events
```
DidLoop()
Ended()
KeyframeReached(keyframeName: string)
Stopped()
```

---

# Animator
**Extends:** Instance

## Properties
```
EvaluationThrottled: bool [ReadOnly]
FacsReplicationData: FacsReplicationData
PreferLodEnabled: bool
RootMotion: CFrame [ReadOnly]
RootMotionWeight: float [ReadOnly]
```

## Functions
```
ApplyJointVelocities(motors: Variant) → null
GetPlayingAnimationTracks() → Array
GetPlayingAnimationTracksCoreScript() → Array
LoadAnimation(animation: Animation) → AnimationTrack
LoadAnimationCoreScript(animation: Animation) → AnimationTrack
LoadStreamAnimation(animation: TrackerStreamAnimation) → AnimationStreamTrack
LoadStreamAnimationForSelfieView_deprecated(animation: TrackerStreamAnimation, player: Player) → AnimationStreamTrack
LoadStreamAnimationV2(animation: TrackerStreamAnimation, player: Player, shouldLookupPlayer: bool, shouldReplicate: bool) → AnimationStreamTrack
RegisterEvaluationParallelCallback(callback: Function) → null
StepAnimations(deltaTime: float) → null
SynchronizeWith(otherAnimator: Animator) → null
```

## Events
```
AnimationPlayed(animationTrack: AnimationTrack)
AnimationPlayedCoreScript(animationTrack: AnimationTrack)
AnimationStreamTrackPlayed(animationTrack: AnimationStreamTrack)
OnCombinedUpdate(animation: ContentId, playState: bool, fadeTime: float, weight: float, speed: float, timePosition: float, priority: AnimationPriority, looping: bool, valuesUpdated: int)
OnCombinedUpdate2(animation: ContentId, playState: bool, fadeTime: float, weight: float, speed: float, timePosition: float, priority: AnimationPriority, valuesUpdated: int)
OnStreamingUpdated(fadeTime: float, weight: float, priority: AnimationPriority, valuesUpdated: int)
OnStreamingUpdated2(fadeTime: float, weight: float, priority: AnimationPriority, maskEnabled: bool, valuesUpdated: int)
StreamSyncRequest(player: Player)
```

---

# Annotation
**Extends:** Instance

## Properties
```
AuthorColor3: Color3
AuthorId: int64
ChannelId: string
Contents: string
CreationTimeUnix: int64
LastModifiedTimeUnix: int64
LoadingReplies: bool
MessageId: string
ReplyCount: int64
Resolved: bool
TaggedUsers: string
```

## Functions
```
GetRequests() → Dictionary
GetStringUniqueId() → string
IsThreadParent() → bool
```

## Events
```
RequestCompleted(requestId: string, requestType: AnnotationRequestType, result: AnnotationRequestStatus)
RequestInitiated(requestId: string, requestType: AnnotationRequestType)
```

---

# WorkspaceAnnotation
**Extends:** Annotation

## Properties
```
Adornee: PVInstance
AdorneeOffset: Vector3
```

## Functions
```
GetAbsolutePosition() → Vector3
SetAdorneeOffsetFromAbsolutePosition(position: Vector3) → null
```

---

# AnnotationsService
**Extends:** Instance

## Properties
```
AnnotationsLoadingStatus: AnnotationRequestStatus
AnnotationsVisible: bool
Hovered: Annotation
Mode: AnnotationEditingMode
ResolvedLoadingStatus: AnnotationRequestStatus
Selected: Annotation
```

## Functions
```
CreateAnnotation(annotation: Annotation) → null
DeleteAnnotation(annotation: Annotation) → null
EditAnnotation(uniqueId: string, contents: string, taggedUsers: string) → null
GetAnnotationThreads() → Instances
LoadAnnotationReplies(annotation: Annotation, reverseOrder: bool, loadAll: bool) → null
LoadAnnotations(resolved: bool) → null
LoadResolvedAnnotations(count: int) → null [Deprecated]
ResolveAnnotation(annotation: Annotation, resolved: bool) → null
```

## Events
```
AnnotationAdded(requestId: string, annotation: Annotation, channelId: string)
AnnotationDeleted(requestId: string, annotation: Annotation)
AnnotationEdited(requestId: string, uniqueId: string, contents: string, taggedUsers: string)
AnnotationResolved(requestId: string, annotation: Annotation, resolved: bool)
ServerLoadAnnotationReplies(annotation: Annotation, reverseOrder: bool, loadAll: bool)
ServerLoadAnnotations(resolved: bool)
ServerLoadResolvedAnnotations(count: int)
```

---

# AppLifecycleObserverService
**Extends:** Instance

## Functions
```
GetCurrentState() → AppLifecycleManagerState
IsDidDetachSupported() → bool
TriggerOnLandingPageMount() → null
TriggerOnLuaAppInteractive() → null
```

## Events
```
OnBecomeActive()
OnDetach()
OnHide()
OnResignActive()
OnStart()
OnUnhide()
```

---

# AppUpdateService
**Extends:** Instance

## Functions
```
CanPerformBinaryUpdate() → bool
CheckForUpdate(handler: Function) → null
PerformManagedUpdate() → bool
```

---

# AssetCounterService
**Extends:** Instance

---

# AssetDeliveryProxy
**Extends:** Instance

## Properties
```
Interface: string
Port: int
StartServer: bool
```

---

# AssetImportService
**Extends:** Instance

## Functions
```
GetAllPresets() → Dictionary
GetPreset(name: string) → Dictionary
RemovePreset(name: string) → null
SavePreset(name: string, preset: Dictionary) → bool
StartSessionWithPath(filePath: string) → AssetImportSession
PickImageFileWithPrompt() → string
PickMeshFileWithPrompt() → string
PickMultipleFilesWithPrompt() → Array
StartSessionWithPathAsync(filePath: string) → AssetImportSession
```

---

# AssetManagerService
**Extends:** Instance

## Functions
```
GetMeshIdFromAliasName(aliasName: string) → int64
GetMeshIdFromAssetId(assetId: int64) → int64
GetTextureIdFromAliasName(aliasName: string) → int64
GetTextureIdFromAssetId(assetId: int64) → int64
InsertAudio(assetId: int64, assetName: string) → null
InsertImage(assetId: int64) → null
InsertImages(assetIds: Array) → null
InsertMesh(aliasName: string, insertWithLocation: bool, sourceAssetId: int64) → null
InsertMeshesWithLocation(aliasNames: Array, meshIds: Array) → null
InsertModel(modelId: int64) → null
InsertPackage(packageId: int64) → null
InsertVideo(assetId: int64, assetName: string) → null
OpenPlace(placeId: int64) → null
ShowPackageDetails(packageId: int64) → null
UpdateAllPackages(packageId: int64) → null
ViewPackageOnWebsite(packageId: int64) → null
AddNewPlace() → int64
CreateAlias(assetType: int, assetId: int64, aliasName: string) → null
DeleteAlias(aliasName: string) → null
RemovePlace(placeId: int64) → null
RenameAlias(assetType: int, assetId: int64, oldAliasName: string, newAliasName: string) → null
RenameModel(modelId: int64, newName: string) → null
RenamePlace(placeId: int64, newName: string) → null
```

## Events
```
AssetImportedSignal(assetType: AssetType, assetId: string, assetName: int64)
ImportSessionFinished()
ImportSessionStarted()
```

---

# AssetPatchSettings
**Extends:** Instance

## Properties
```
ContentId: string
OutputPath: string
PatchId: string
```

---

# AssetService
**Extends:** Instance

## Functions
```
CreateEditableImage(editableImageOptions: Dictionary?) → EditableImage
CreateEditableMesh(editableMeshOptions: Dictionary?) → EditableMesh
DeserializeInstance(serializedInstance: string) → Instance
GetBundleDetailsSync(bundleId: int64) → Dictionary
RegisterUGCValidationFunction(function: Function) → null
CanEditAssetAsync(content: Content) → bool
CreateAssetAsync(object: Object, assetType: AssetType, requestParameters: Dictionary) → Tuple
CreateAssetVersionAsync(object: Object, assetType: AssetType, assetId: int64, requestParameters: Dictionary) → Tuple
CreateEditableImageAsync(content: Content, editableImageOptions: Dictionary?) → EditableImage
CreateEditableMeshAsync(content: Content, editableMeshOptions: Dictionary?) → EditableMesh
CreateEditableMeshStripSkinningAsync(meshId: ContentId) → EditableMesh
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

## Events
```
AudioMetadataFailedResponse(requestid: int64)
AudioMetadataRequest(requestid: int64, request: Array)
AudioMetadataResponse(requestid: int64, response: Array)
OpenCreateResultModal(resultType: PromptCreateAssetResult)
OpenPublishResultModal(resultType: PromptPublishAssetResult)
```

---

# Atmosphere
**Extends:** Instance

## Properties
```
Color: Color3
Decay: Color3
Density: float
Glare: float
Haze: float
Offset: float
```

---

# Attachment
**Extends:** Instance

## Properties
```
Axis: Vector3
CFrame: CFrame
Orientation: Vector3
Position: Vector3
Rotation: Vector3 [Deprecated]
SecondaryAxis: Vector3
Visible: bool
WorldAxis: Vector3
WorldCFrame: CFrame
WorldOrientation: Vector3
WorldPosition: Vector3
WorldRotation: Vector3 [ReadOnly] [Deprecated]
WorldSecondaryAxis: Vector3
```

## Functions
```
GetAxis() → Vector3 [Deprecated]
GetConstraints() → Instances
GetSecondaryAxis() → Vector3 [Deprecated]
SetAxis(axis: Vector3) → null [Deprecated]
SetSecondaryAxis(axis: Vector3) → null [Deprecated]
```

---

# Bone
**Extends:** Attachment

## Properties
```
Transform: CFrame
TransformedCFrame: CFrame [ReadOnly]
TransformedWorldCFrame: CFrame [ReadOnly]
```

---

# AudioAnalyzer
**Extends:** Instance

## Properties
```
PeakLevel: float [ReadOnly]
RmsLevel: float [ReadOnly]
SpectrumEnabled: bool
WindowSize: AudioWindowSize
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
GetSpectrum() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioChannelMixer
**Extends:** Instance

## Properties
```
Layout: AudioChannelLayout
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioChannelSplitter
**Extends:** Instance

## Properties
```
Layout: AudioChannelLayout
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioChorus
**Extends:** Instance

## Properties
```
Bypass: bool
Depth: float
Mix: float
Rate: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioCompressor
**Extends:** Instance

## Properties
```
Attack: float
Bypass: bool
Editor: bool
MakeupGain: float
Ratio: float
Release: float
Threshold: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioDeviceInput
**Extends:** Instance

## Properties
```
AccessList: BinaryString
AccessType: AccessModifierType
Active: bool
IsReady: bool [ReadOnly]
Muted: bool
MutedByLocalUser: bool
Player: Player
Volume: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
GetUserIdAccessList() → Array
SetUserIdAccessList(userIds: Array) → null
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioDeviceOutput
**Extends:** Instance

## Properties
```
Player: Player
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioDistortion
**Extends:** Instance

## Properties
```
Bypass: bool
Level: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioEcho
**Extends:** Instance

## Properties
```
Bypass: bool
DelayTime: float
DryLevel: float
Feedback: float
RampTime: float
WetLevel: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
Reset() → null
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioEmitter
**Extends:** Instance

## Properties
```
AngleAttenuation: BinaryString
AudioInteractionGroup: string
DistanceAttenuation: BinaryString
PositionOverride: Instance
SimulationFidelity: AudioSimulationFidelity
```

## Functions
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

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioEqualizer
**Extends:** Instance

## Properties
```
Bypass: bool
Editor: bool
HighGain: float
LowGain: float
MidGain: float
MidRange: NumberRange
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioFader
**Extends:** Instance

## Properties
```
Bypass: bool
Volume: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioFilter
**Extends:** Instance

## Properties
```
Bypass: bool
Editor: bool
FilterType: AudioFilterType
Frequency: float
Gain: float
Q: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetGainAt(frequency: float) → float
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioFlanger
**Extends:** Instance

## Properties
```
Bypass: bool
Depth: float
Mix: float
Rate: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioFocusService
**Extends:** Instance

## Functions
```
AcquireFocus(contextId: int) → bool
GetFocusedContextId() → int
GetRegisteredContexts() → Array
RegisterContextIdFromLua(contextId: int) → null
RequestFocus(contextId: int, priority: int) → bool
```

## Events
```
OnContextRegistered(contextId: int)
OnContextUnregistered(contextId: int)
OnDeafenVoiceAudio(contextId: int)
OnUndeafenVoiceAudio(contextId: int)
```

---

# AudioGate
**Extends:** Instance

## Properties
```
Attack: float
Bypass: bool
Release: float
Threshold: NumberRange
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
Reset() → null
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioLimiter
**Extends:** Instance

## Properties
```
Bypass: bool
Editor: bool
MaxLevel: float
Release: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioListener
**Extends:** Instance

## Properties
```
AngleAttenuation: BinaryString
AudioInteractionGroup: string
DistanceAttenuation: BinaryString
PositionOverride: Instance
SimulationFidelity: AudioSimulationFidelity
```

## Functions
```
GetAngleAttenuation() → Dictionary
GetAudibilityFor(emitter: AudioEmitter) → float
GetConnectedWires(pin: string) → Instances
GetDistanceAttenuation() → Dictionary
GetInputPins() → Array
GetInteractingEmitters() → Instances
GetOutputPins() → Array
Reset() → null
SetAngleAttenuation(curve: Dictionary) → null
SetDistanceAttenuation(curve: Dictionary) → null
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioPitchShifter
**Extends:** Instance

## Properties
```
Bypass: bool
Pitch: float
WindowSize: AudioWindowSize
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioPlayer
**Extends:** Instance

## Properties
```
Asset: ContentId
AssetId: string [Deprecated]
AutoLoad: bool
IsMutedForCapture: bool
IsPlaying: bool
IsReady: bool [ReadOnly]
LoopRegion: NumberRange
Looping: bool
PlaybackRegion: NumberRange
PlaybackSpeed: double
TimeLength: double [ReadOnly]
TimePosition: double
Volume: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
Play() → null
Stop() → null
GetWaveformAsync(timeRange: NumberRange, samples: int) → Array
```

## Events
```
Ended()
Looped()
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioRecorder
**Extends:** Instance

## Properties
```
IsRecording: bool
TimeLength: double [ReadOnly]
```

## Functions
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

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioReverb
**Extends:** Instance

## Properties
```
Bypass: bool
DecayRatio: float
DecayTime: float
Density: float
Diffusion: float
DryLevel: float
EarlyDelayTime: float
HighCutFrequency: float
LateDelayTime: float
LowShelfFrequency: float
LowShelfGain: float
ReferenceFrequency: float
WetLevel: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
Reset() → null
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioSearchParams
**Extends:** Instance

## Properties
```
Album: string
Artist: string
AudioSubType: AudioSubType
AudioSubtype: AudioSubType [Deprecated]
MaxDuration: int
MinDuration: int
SearchKeyword: string
Tag: string
Title: string
```

---

# AudioSpeechToText
**Extends:** Instance

## Properties
```
Enabled: bool
Text: string
VoiceDetected: bool [ReadOnly]
```

## Functions
```
GetConnectedWires(pin: string) → Instances
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AudioTextToSpeech
**Extends:** Instance

## Properties
```
IsLoaded: bool [ReadOnly]
IsPlaying: bool
Looping: bool
Pitch: float
PlaybackSpeed: float
Speed: float
Text: string
TimeLength: double [ReadOnly]
TimePosition: double
VoiceId: string
Volume: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
Pause() → null
Play() → null
Unload() → null
GetWaveformAsync(timeRange: NumberRange, samples: int) → Array
LoadAsync() → AssetFetchStatus
```

## Events
```
Ended()
Looped()
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# AuroraScriptObject
**Extends:** Instance

## Properties
```
BehaviorWeak: AuroraScript
BoundInstanceWeak: Instance
FrameId: int
LODLevel: int
MaxFrequency: int
PriorFrameInvoked: int
```

---

# AuroraScriptService
**Extends:** Instance

## Functions
```
GetLocalFrameId() → int
SendMessage(instance: Instance, behaviorName: string, functionName: string, args: Tuple) → null
```

---

# AuroraService
**Extends:** Instance

## Properties
```
BufferFullInputCount: int
HashRoundingPoint: double
IgnoreRotation: bool
InputDropRate: float
LockStepIdOffset: bool
OutOfOrderInputCount: int
RCCHeartbeatFPS: double
RollbackOffset: int
TooOldInputCount: int
```

## Functions
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

## Events
```
FixedRateTick(deltaTime: double, worldStepId: int)
Misprediction(worldStepId: int, mispredictedInstances: Array)
Rollback(worldStepId: int)
Step()
```

---

# AvatarAccessoryRules
**Extends:** Instance

## Properties
```
AccessoryMode: AvatarSettingsAccessoryMode
CustomAccessoryMode: AvatarSettingsCustomAccessoryMode
CustomBackAccessoryEnabled: bool
CustomBackAccessoryId: int64
CustomFaceAccessoryEnabled: bool
CustomFaceAccessoryId: int64
CustomFrontAccessoryEnabled: bool
CustomFrontAccessoryId: int64
CustomHairAccessoryEnabled: bool
CustomHairAccessoryId: int64
CustomHeadAccessoryEnabled: bool
CustomHeadAccessoryId: int64
CustomNeckAccessoryEnabled: bool
CustomNeckAccessoryId: int64
CustomShoulderAccessoryEnabled: bool
CustomShoulderAccessoryId: int64
CustomWaistAccessoryEnabled: bool
CustomWaistAccessoryId: int64
EnableSound: bool
EnableVFX: bool
LimitBounds: Vector3
LimitMethod: AvatarSettingsAccessoryLimitMethod
```

## Functions
```
willRemoveAccessory(humanoid: Humanoid, accessory: Accoutrement) → bool
```

---

# AvatarAnimationRules
**Extends:** Instance

## Properties
```
AnimationClipsMode: AvatarSettingsAnimationClipsMode
AnimationPacksMode: AvatarSettingsAnimationPacksMode
CustomClimbAnimationEnabled: bool
CustomClimbAnimationId: int64
CustomFallAnimationEnabled: bool
CustomFallAnimationId: int64
CustomIdleAlt1AnimationEnabled: bool
CustomIdleAlt1AnimationId: int64
CustomIdleAlt2AnimationEnabled: bool
CustomIdleAlt2AnimationId: int64
CustomIdleAnimationEnabled: bool
CustomIdleAnimationId: int64
CustomJumpAnimationEnabled: bool
CustomJumpAnimationId: int64
CustomRunAnimationEnabled: bool
CustomRunAnimationId: int64
CustomSwimAnimationEnabled: bool
CustomSwimAnimationId: int64
CustomSwimIdleAnimationEnabled: bool
CustomSwimIdleAnimationId: int64
CustomWalkAnimationEnabled: bool
CustomWalkAnimationId: int64
```

---

# AvatarBodyRules
**Extends:** Instance

## Properties
```
AppearanceMode: AvatarSettingsAppearanceMode
BuildMode: AvatarSettingsBuildMode
CustomBodyBundleId: int64
CustomBodyType: AvatarSettingsCustomBodyType
CustomBodyTypeScale: NumberRange
CustomEyebrowEnabled: bool
CustomEyebrowId: int64
CustomEyelashEnabled: bool
CustomEyelashId: int64
CustomFaceEnabled: bool
CustomFaceId: int64
CustomHeadEnabled: bool
CustomHeadId: int64
CustomHeadScale: NumberRange
CustomHeight: NumberRange
CustomHeightScale: NumberRange
CustomLeftArmEnabled: bool
CustomLeftArmId: int64
CustomLeftLegEnabled: bool
CustomLeftLegId: int64
CustomMoodEnabled: bool
CustomMoodId: int64
CustomProportionsScale: NumberRange
CustomRightArmEnabled: bool
CustomRightArmId: int64
CustomRightLegEnabled: bool
CustomRightLegId: int64
CustomTorsoEnabled: bool
CustomTorsoId: int64
CustomWidthScale: NumberRange
KeepPlayerHead: bool
ScaleMode: AvatarSettingsScaleMode
```

---

# AvatarChatService
**Extends:** Instance

## Properties
```
ClientFeatures: int [ReadOnly]
ClientFeaturesInitialized: bool [ReadOnly]
ServerFeatures: int
```

## Functions
```
DebugCounterGet(label: string, playerId: int64) → int64
EnableVoice() → bool
IsEnabled(mask: int, feature: AvatarChatServiceFeature) → bool
IsPlaceEnabled() → bool
IsUniverseEnabled() → bool
PollClientFeatures() → int
PollServerFeatures() → int
deviceMeetsRequirementsForFeature(feature: DeviceFeatureType) → bool
GetClientFeaturesAsync() → int
GetServerFeaturesAsync() → int
```

## Events
```
OnClientFeatures(features: int)
RefreshClientFeatures()
```

---

# AvatarClothingRules
**Extends:** Instance

## Properties
```
ClothingMode: AvatarSettingsClothingMode
CustomClassicPantsAccessoryEnabled: bool
CustomClassicPantsAccessoryId: int64
CustomClassicShirtsAccessoryEnabled: bool
CustomClassicShirtsAccessoryId: int64
CustomClassicTShirtsAccessoryEnabled: bool
CustomClassicTShirtsAccessoryId: int64
CustomClothingMode: AvatarSettingsCustomClothingMode
CustomDressSkirtAccessoryEnabled: bool
CustomDressSkirtAccessoryId: int64
CustomJacketAccessoryEnabled: bool
CustomJacketAccessoryId: int64
CustomLeftShoesAccessoryEnabled: bool
CustomLeftShoesAccessoryId: int64
CustomPantsAccessoryEnabled: bool
CustomPantsAccessoryId: int64
CustomRightShoesAccessoryEnabled: bool
CustomRightShoesAccessoryId: int64
CustomShirtAccessoryEnabled: bool
CustomShirtAccessoryId: int64
CustomShortsAccessoryEnabled: bool
CustomShortsAccessoryId: int64
CustomSweaterAccessoryEnabled: bool
CustomSweaterAccessoryId: int64
CustomTShirtAccessoryEnabled: bool
CustomTShirtAccessoryId: int64
LimitBounds: Vector3
```

---

# AvatarCollisionRules
**Extends:** Instance

## Properties
```
CollisionMode: AvatarSettingsCollisionMode
HitAndTouchDetectionMode: AvatarSettingsHitAndTouchDetectionMode
LegacyCollisionMode: AvatarSettingsLegacyCollisionMode
SingleColliderSize: Vector3
```

---

# AvatarCreationService
**Extends:** Instance

## Functions
```
DeserializeAvatarModel(serializedModel: string) → Instance
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

## Events
```
AvatarModerationCompleted(outfitId: int64, moderationStatus: ModerationStatus)
ReplicateAvatarGenerationImageId(fileId: string, error: string)
ReplicateAvatarModel(id: string, success: bool, serializedModel: string, bufferTable: Dictionary)
ReplicateAvatarPreviewUrl(id: string, downloadUrl: string)
RequestAvatarGenerationImage()
RequestAvatarModel(id: string)
RequestAvatarPreviewUrl(id: string)
UgcValidationFailure(guid: string, errorMessage: string)
UgcValidationSuccess(guid: string, serializedModel: string, price: int64)
```

---

# AvatarEditorService
**Extends:** Instance

## Functions
```
GetAccessoryType(avatarAssetType: AvatarAssetType) → AccessoryType
NoPromptCreateOutfit(humanoidDescription: HumanoidDescription, rigType: HumanoidRigType, name: string, gearAssetId: int64) → bool
NoPromptDeleteOutfit(outfitId: int64) → bool
NoPromptRenameOutfit(outfitId: int64, name: string) → bool
NoPromptSaveAvatar(humanoidDescription: HumanoidDescription, rigType: HumanoidRigType, saveDict: Dictionary, gearAssetId: int64) → bool
NoPromptSaveAvatarThumbnailCustomization(thumbnailType: AvatarThumbnailCustomizationType, emoteAssetId: int64, cameraDistanceScale: float, yRotDeg: float, fieldOfViewDeg: float) → bool
NoPromptSetFavorite(itemId: int64, itemType: AvatarItemType, shouldFavorite: bool) → bool
NoPromptUpdateOutfit(outfitId: int64, humanoidDescription: HumanoidDescription, rigType: HumanoidRigType, gearAssetId: int64) → bool
PerformCreateOutfitWithDescription(humanoidDescription: HumanoidDescription, name: string) → null
PerformDeleteOutfit() → null
PerformRenameOutfit(name: string) → null
PerformSaveAvatarWithDescription(humanoidDescription: HumanoidDescription, addedAssets: Array, removedAssets: Array) → null
PerformSetFavorite() → null
PerformUpdateOutfit(humanoidDescription: HumanoidDescription) → null
PromptAllowInventoryReadAccess() → null
PromptCreateOutfit(outfit: HumanoidDescription, rigType: HumanoidRigType) → null
PromptDeleteOutfit(outfitId: int64) → null
PromptRenameOutfit(outfitId: int64) → null
PromptSaveAvatar(humanoidDescription: HumanoidDescription, rigType: HumanoidRigType) → null
PromptSetFavorite(itemId: int64, itemType: AvatarItemType, shouldFavorite: bool) → null
PromptUpdateOutfit(outfitId: int64, updatedOutfit: HumanoidDescription, rigType: HumanoidRigType) → null
SetAllowInventoryReadAccess(inventoryReadAccessGranted: bool) → null
SignalCreateOutfitFailed() → null
SignalCreateOutfitPermissionDenied() → null
SignalDeleteOutfitFailed() → null
SignalDeleteOutfitPermissionDenied() → null
SignalRenameOutfitFailed() → null
SignalRenameOutfitPermissionDenied() → null
SignalSaveAvatarFailed() → null
SignalSaveAvatarPermissionDenied() → null
SignalSetFavoriteFailed() → null
SignalSetFavoritePermissionDenied() → null
SignalUpdateOutfitFailed() → null
SignalUpdateOutfitPermissionDenied() → null
refreshAvatarThumbnails(thumbnailTypes: Array) → null
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

## Events
```
OpenAllowInventoryReadAccess()
OpenPromptCreateOufit(humanoidDescription: HumanoidDescription, rigType: HumanoidRigType)
OpenPromptDeleteOutfit(outfitId: int64)
OpenPromptRenameOutfit(outfitId: int64)
OpenPromptSaveAvatar(humanoidDescription: HumanoidDescription, rigType: HumanoidRigType)
OpenPromptSetFavorite(itemId: int64, itemType: AvatarItemType, shouldFavorite: bool)
OpenPromptUpdateOutfit(outfitId: int64, humanoidDescription: HumanoidDescription, rigType: HumanoidRigType)
PromptAllowInventoryReadAccessCompleted(result: AvatarPromptResult)
PromptCreateOutfitCompleted(result: AvatarPromptResult, failureType: Variant)
PromptDeleteOutfitCompleted(result: AvatarPromptResult)
PromptRenameOutfitCompleted(result: AvatarPromptResult)
PromptSaveAvatarCompleted(result: AvatarPromptResult, humanoidDescription: HumanoidDescription)
PromptSaveAvatarThumbnailCustomizationCompleted(result: AvatarPromptResult, failureType: Variant)
PromptSetFavoriteCompleted(result: AvatarPromptResult)
PromptUpdateOutfitCompleted(result: AvatarPromptResult)
```

---

# AvatarImportService
**Extends:** Instance

## Functions
```
ImportFBXAnimationFromFilePathUserMayChooseModel(fbxFilePath: string, selectedRig: Instance, userChooseModelThenImportCB: Function) → Instance
ImportFBXAnimationUserMayChooseModel(selectedRig: Instance, userChooseModelThenImportCB: Function) → Instance
ImportFbxRigWithoutSceneLoad(isR15: bool) → Instance
ImportLoadedFBXAnimation(useFBXModel: bool) → Instance
LoadRigAndDetectType(promptR15Callback: Function) → Instance
```

---

# AvatarPreloader
**Extends:** Instance

## Functions
```
PreloadModelAssets(models: Instances) → Array
```

---

# AvatarRules
**Extends:** Instance

## Properties
```
AvatarType: GameAvatarType
```

---

# AvatarSettings
**Extends:** Instance

## Properties
```
Loaded: bool
```

## Functions
```
Discard() → null
Publish() → null
```

## Events
```
DiscardRequested()
RefreshPluginState()
```

---

# Backpack
**Extends:** Instance

---

# BadgeService
**Extends:** Instance

## Functions
```
AwardBadge(userId: int64, badgeId: int64) → bool
CheckUserBadgesAsync(userId: int64, badgeIds: Array) → Array
GetBadgeInfoAsync(badgeId: int64) → Dictionary
IsDisabled(badgeId: int64) → bool [Deprecated]
IsLegal(badgeId: int64) → bool [Deprecated]
UserHasBadge(userId: int64, badgeId: int64) → bool [Deprecated]
UserHasBadgeAsync(userId: int64, badgeId: int64) → bool
```

## Events
```
BadgeAwarded(message: string, userId: int64, badgeId: int64)
OnBadgeAwarded(userId: int64, creatorId: int64, badgeId: int64)
```

---

# BaseImportData
**Extends:** Instance

## Properties
```
Id: string [ReadOnly]
ImportName: string
ShouldImport: bool
```

## Functions
```
CreatePresetFromData() → Dictionary
GetPreview() → Instance
GetStatuses() → Dictionary
```

## Events
```
StatusRemoved(status: Dictionary)
StatusReported(status: Dictionary)
```

---

# AnimationImportData
**Extends:** BaseImportData

---

# FacsImportData
**Extends:** BaseImportData

---

# GroupImportData
**Extends:** BaseImportData

## Properties
```
Anchored: bool
ImportAsModelAsset: bool
InsertInWorkspace: bool
```

---

# JointImportData
**Extends:** BaseImportData

---

# MaterialImportData
**Extends:** BaseImportData

## Properties
```
DiffuseFilePath: string
IsPbr: bool [ReadOnly]
MetalnessFilePath: string
NormalFilePath: string
RoughnessFilePath: string
```

---

# MeshImportData
**Extends:** BaseImportData

## Properties
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

# RootImportData
**Extends:** BaseImportData

## Properties
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

# BasePlayerGui
**Extends:** Instance

## Functions
```
GetGuiObjectsAtPosition(x: int, y: int) → Instances
GetGuiObjectsInCircle(position: Vector2, radius: float) → Instances
```

---

# CoreGui
**Extends:** BasePlayerGui

## Properties
```
SelectionImageObject: GuiObject
Version: int [ReadOnly]
```

## Functions
```
SetUserGuiRendering(enabled: bool, guiAdornee: Instance, faceId: NormalId, horizontalCurvature: float) → null
TakeScreenshot() → null
ToggleRecording() → null
```

## Events
```
UserGuiRenderingChanged(enabled: bool, guiAdornee: Instance, faceId: NormalId, horizontalCurvature: float)
```

---

# PlayerGui
**Extends:** BasePlayerGui

## Properties
```
CurrentScreenOrientation: ScreenOrientation [ReadOnly]
ScreenOrientation: ScreenOrientation
SelectionImageObject: GuiObject
```

## Functions
```
GetTopbarTransparency() → float [Deprecated]
SetTopbarTransparency(transparency: float) → null [Deprecated]
```

## Events
```
TopbarTransparencyChangedSignal(transparency: float)
```

---

# StarterGui
**Extends:** BasePlayerGui

## Properties
```
ProcessUserInput: bool
ResetPlayerGuiOnSpawn: bool [Deprecated]
RtlTextSupport: RtlTextSupport
ScreenOrientation: ScreenOrientation
ShowDevelopmentGui: bool
StudioDefaultStyleSheet: StyleSheet
StudioInsertWidgetLayerCollectorAutoLinkStyleSheet: StyleSheet
VirtualCursorMode: VirtualCursorMode
```

## Functions
```
GetCoreGuiEnabled(coreGuiType: CoreGuiType) → bool
RegisterGetCore(parameterName: string, getFunction: Function) → null
RegisterSetCore(parameterName: string, setFunction: Function) → null
SetCore(parameterName: string, value: Variant) → null
SetCoreGuiEnabled(coreGuiType: CoreGuiType, enabled: bool) → null
GetCore(parameterName: string) → Variant
```

## Events
```
CoreGuiChangedSignal(coreGuiType: CoreGuiType, enabled: bool)
```

---

# BaseRemoteEvent
**Extends:** Instance

---

# RemoteEvent
**Extends:** BaseRemoteEvent

## Functions
```
FireAllClients(arguments: Tuple) → null
FireClient(player: Player, arguments: Tuple) → null
FireServer(arguments: Tuple) → null
```

## Events
```
OnClientEvent(arguments: Tuple)
OnRemoteServerEvent(arguments: Tuple)
OnServerEvent(player: Player, arguments: Tuple)
```

---

# UnreliableRemoteEvent
**Extends:** BaseRemoteEvent

## Functions
```
FireAllClients(arguments: Tuple) → null
FireClient(player: Player, arguments: Tuple) → null
FireServer(arguments: Tuple) → null
```

## Events
```
OnClientEvent(arguments: Tuple)
OnRemoteServerEvent(arguments: Tuple)
OnServerEvent(player: Player, arguments: Tuple)
```

---

# BaseWrap
**Extends:** Instance

## Properties
```
CageMeshContent: Content
CageMeshId: ContentId
CageOrigin: CFrame
CageOriginWorld: CFrame [ReadOnly]
HSRAssetId: ContentId
HSRData: SharedString
HSRMeshIdData: SharedString
ImportInProcess: bool
ImportOrigin: CFrame
ImportOriginWorld: CFrame [ReadOnly]
TemporaryCageMeshId: ContentId
```

## Functions
```
GetCageOffset() → Vector3
GetFaces(cageType: CageType) → Array
GetUVs(cageType: CageType) → Array
GetVertices(cageType: CageType) → Array
IsHSRReady() → bool
ModifyVertices(cageType: CageType, vertices: Array) → null
```

## Events
```
VerticesModified(vertices: Array)
```

---

# WrapDeformer
**Extends:** BaseWrap

## Functions
```
SetCageMeshContent(content: Content, cageOrigin: CoordinateFrame?) → null
CreateEditableMeshAsync() → EditableMesh
GetDeformedCFrameAsync(originalCFrame: CFrame) → CFrame
```

---

# WrapLayer
**Extends:** BaseWrap

## Properties
```
AutoSkin: WrapLayerAutoSkin
BindOffset: CFrame
Color: Color3
DebugMode: WrapLayerDebugMode
Enabled: bool
MaxSize: Vector3
Offset: Vector3
Order: int
Puffiness: float
ReferenceMeshContent: Content
ReferenceMeshId: ContentId
ReferenceOrigin: CFrame
ReferenceOriginWorld: CFrame [ReadOnly]
ShrinkFactor: float
TemporaryReferenceId: ContentId
```

---

# WrapTarget
**Extends:** BaseWrap

## Properties
```
Color: Color3
DebugMode: WrapTargetDebugMode
Stiffness: float
```

---

# Beam
**Extends:** Instance

## Properties
```
Attachment0: Attachment
Attachment1: Attachment
Brightness: float
Color: ColorSequence
CurveSize0: float
CurveSize1: float
Enabled: bool
FaceCamera: bool
LightEmission: float
LightInfluence: float
LocalTransparencyModifier: float
Segments: int
Texture: ContentId
TextureLength: float
TextureMode: TextureMode
TextureSpeed: float
Transparency: NumberSequence
Width0: float
Width1: float
ZOffset: float
```

## Functions
```
SetTextureOffset(offset: float) → null
```

---

# BindableEvent
**Extends:** Instance

## Functions
```
Fire(arguments: Tuple) → null
```

## Events
```
Event(arguments: Tuple)
```

---

# BindableFunction
**Extends:** Instance

## Functions
```
Invoke(arguments: Tuple) → Tuple
```

---

# BodyMover
**Extends:** Instance

---

# BodyAngularVelocity
**Extends:** BodyMover

## Properties
```
AngularVelocity: Vector3
MaxTorque: Vector3
P: float
angularvelocity: Vector3 [Deprecated]
maxTorque: Vector3 [Deprecated]
```

---

# BodyForce
**Extends:** BodyMover

## Properties
```
Force: Vector3
force: Vector3 [Deprecated]
```

---

# BodyGyro
**Extends:** BodyMover

## Properties
```
CFrame: CFrame
D: float
MaxTorque: Vector3
P: float
cframe: CFrame [Deprecated]
maxTorque: Vector3 [Deprecated]
```

---

# BodyPosition
**Extends:** BodyMover

## Properties
```
D: float
MaxForce: Vector3
P: float
Position: Vector3
maxForce: Vector3 [Deprecated]
position: Vector3 [Deprecated]
```

## Functions
```
GetLastForce() → Vector3
lastForce() → Vector3 [Deprecated]
```

## Events
```
ReachedTarget()
```

---

# BodyThrust
**Extends:** BodyMover

## Properties
```
Force: Vector3
Location: Vector3
force: Vector3 [Deprecated]
location: Vector3 [Deprecated]
```

---

# BodyVelocity
**Extends:** BodyMover

## Properties
```
MaxForce: Vector3
P: float
Velocity: Vector3
maxForce: Vector3 [Deprecated]
velocity: Vector3 [Deprecated]
```

## Functions
```
GetLastForce() → Vector3
lastForce() → Vector3
```

---

# RocketPropulsion
**Extends:** BodyMover

## Properties
```
Active: bool
CartoonFactor: float
MaxSpeed: float
MaxThrust: float
MaxTorque: Vector3
Target: BasePart
TargetOffset: Vector3
TargetRadius: float
ThrustD: float
ThrustP: float
TurnD: float
TurnP: float
```

## Functions
```
Abort() → null
Fire() → null
fire() → null [Deprecated]
```

## Events
```
ReachedTarget()
```

---

# BodyPartDescription
**Extends:** Instance

## Properties
```
AssetId: int64
BodyPart: BodyPart
Color: Color3
Instance: Instance
```

---

# Breakpoint
**Extends:** Instance

## Properties
```
Condition: string
ContinueExecution: bool
Enabled: bool
Id: int [ReadOnly]
Line: int [ReadOnly]
LogMessage: string
MetaBreakpointId: int [ReadOnly]
RemoveOnHit: bool
Script: string [ReadOnly]
Valid: bool [ReadOnly]
Verified: bool [ReadOnly]
```

---

# BrowserService
**Extends:** Instance

## Functions
```
CloseBrowserWindow() → null
CopyAuthCookieFromBrowserToEngine() → null
EmitHybridEvent(moduleName: string, eventName: string, params: string) → null
ExecuteJavaScript(javascript: string) → null
OpenBrowserWindow(url: string) → null
OpenNativeOverlay(title: string, url: string) → null
OpenWeChatAuthWindow() → null
ReturnToJavaScript(callbackId: string, success: bool, params: string) → null
SendCommand(command: string) → null
```

## Events
```
AuthCookieCopiedToEngine()
BrowserWindowClosed()
BrowserWindowWillNavigate(url: string)
JavaScriptCallback(content: string)
```

---

# BugReporterService
**Extends:** Instance

## Functions
```
IsAvailable() → bool
```

## Events
```
BugReportRequested(trigger: string)
```

---

# BulkImportService
**Extends:** Instance

## Functions
```
LaunchBulkImport(assetTypeToImport: int) → null
ShowBulkImportView() → null
```

## Events
```
AssetImported(assetType: AssetType, name: string, id: int64)
BulkImportFinished(state: int)
BulkImportStarted()
```

---

# CacheableContentProvider
**Extends:** Instance

---

# HSRDataContentProvider
**Extends:** CacheableContentProvider

---

# MeshContentProvider
**Extends:** CacheableContentProvider

## Functions
```
GetContentMemoryData() → Dictionary
```

---

# SlimContentProvider
**Extends:** CacheableContentProvider

## Functions
```
GetContentMemoryData() → Dictionary
```

---

# SolidModelContentProvider
**Extends:** CacheableContentProvider

---

# CalloutService
**Extends:** Instance

## Functions
```
AttachCallout(definitionId: string, locationId: string, target: Instance) → null
DefineCallout(definitionId: string, title: string, description: string, learnMoreURL: string) → null
DetachCalloutsByDefinitionId(definitionId: string) → null
```

---

# CaptureService
**Extends:** Instance

## Functions
```
CanCaptureVideo() → bool
CaptureScreenshot(onCaptureReady: Function) → null
DeleteCapture(capturePath: string) → null
DeleteVideoCapture(videoCapture: VideoCapture) → null
GetDeviceInfo() → Dictionary
IsCapturingVideo() → bool
OnCaptureBegan() → null
OnCaptureEnded() → null
OnCapturePermissionsPromptFinished(promptId: int64, wasAccepted: bool) → null
OnCaptureShared(capturePath: string) → null
OnSavePromptFinished(promptId: int64, results: Dictionary) → null
OnSharePromptFinished(promptId: int64, accepted: bool) → null
OnVideoCaptureShared(videoCapture: VideoCapture) → null
PreVideoCaptureShared(videoCapture: VideoCapture) → string
PromptCaptureGalleryPermission(captureGalleryPermission: CaptureGalleryPermission, onAcceptedCallback: Function, onDeniedCallback: Function) → null
PromptSaveCapturesToGallery(captures: Array, resultCallback: Function) → null
PromptShareCapture(captureContent: Content, launchData: string, onAcceptedCallback: Function, onDeniedCallback: Function) → null
RetrieveCaptures() → Array
SaveCaptureToExternalStorage(capturePath: string) → null
SaveScreenshotCapture(additionalInfo: string) → null
SaveVideoCaptureToExternalStorage(videoCapture: VideoCapture) → null
StopVideoCapture() → null
StopVideoCaptureInternal() → null
TakeCapture(onCaptureReady: Function, captureParams: Dictionary) → null
CreatePostAsync(pathArr: Array, caption: string) → Dictionary
DeleteCapturesAsync(pathArr: Array) → int64
DeleteVideoCaptureAsync(videoCapture: VideoCapture) → bool
GetCaptureFilePathAsync(captureContent: Content) → string
GetCaptureSizeAsync(captureContent: Content) → Vector2
GetCaptureStorageSizeAsync(pathArr: Array) → int64
GetCaptureUploadDataAsync(capturePath: string) → Dictionary
ReadCapturesFromGalleryAsync(captureTypeFilters: Array) → Tuple
SaveCapturesToExternalStorageAsync(pathArr: Array) → int64
StartVideoCaptureAsync(onCaptureReady: Function, captureParams: Dictionary) → VideoCaptureStartedResult
StartVideoCaptureInternalAsync() → VideoCaptureStartedResult
UploadCaptureAsync(capture: Capture) → Tuple
```

## Events
```
CaptureBegan(captureType: CaptureType)
CaptureEnded(captureType: CaptureType)
CaptureSaved(captureInfo: Dictionary)
CaptureSavedInternal(captureInfo: Dictionary, triggerSource: string)
OnCaptureAndMetadataSignatureResult(content: string, captureSignature: string, captureSignatureVersion: int, metadataSignature: string, metadataSignatureVersion: int)
OnCaptureSignatureResult(content: string, signature: string, signatureVersion: int)
OpenCapturePermissionsPrompt(promptId: int64, captureGalleryPermission: CaptureGalleryPermission)
OpenSaveCapturesPrompt(promptId: int64, captures: Array)
OpenShareCapturePrompt(promptId: int64, captureContent: Variant, launchData: string)
RequestCaptureAndMetadataSignature(content: string, audioAssetIds: string)
RequestCaptureSignature(content: string)
RequestCaptureSignatureV2(content: string)
UserCaptureSaved(captureContentId: ContentId)
UserVideoCaptureFailed(result: VideoCaptureResult)
UserVideoCaptureStartFailed(result: VideoCaptureStartedResult)
VideoCaptureInProgress(isInProgress: bool, captureTrigger: string)
```

---

# ChangeHistoryService
**Extends:** Instance

## Functions
```
FinishRecording(identifier: string, operation: FinishRecordingOperation, finalOptions: Dictionary?) → null
GetCanRedo() → Tuple
GetCanUndo() → Tuple
IsRecordingInProgress(identifier: string?) → bool
Redo() → null
ResetWaypoints() → null
SetEnabled(state: bool) → null
SetWaypoint(name: string) → null
TryBeginRecording(name: string, displayName: string?) → string?
Undo() → null
```

## Events
```
OnRecordingFinished(name: string, displayName: string?, identifier: string?, operation: FinishRecordingOperation, finalOptions: Dictionary?)
OnRecordingStarted(name: string, displayName: string?)
OnRedo(waypoint: string)
OnUndo(waypoint: string)
```

---

# CharacterAppearance
**Extends:** Instance

---

# BodyColors
**Extends:** CharacterAppearance

## Properties
```
HeadColor: BrickColor
HeadColor3: Color3
LeftArmColor: BrickColor
LeftArmColor3: Color3
LeftLegColor: BrickColor
LeftLegColor3: Color3
RightArmColor: BrickColor
RightArmColor3: Color3
RightLegColor: BrickColor
RightLegColor3: Color3
TorsoColor: BrickColor
TorsoColor3: Color3
```

---

# CharacterMesh
**Extends:** CharacterAppearance

## Properties
```
BaseTextureId: int64
BodyPart: BodyPart
MeshId: int64
OverlayTextureId: int64
```

---

# Clothing
**Extends:** CharacterAppearance

## Properties
```
Color3: Color3
Outfit1: ContentId
Outfit2: ContentId
```

---

# Pants
**Extends:** Clothing

## Properties
```
PantsTemplate: ContentId
```

---

# Shirt
**Extends:** Clothing

## Properties
```
ShirtTemplate: ContentId
```

---

# ShirtGraphic
**Extends:** CharacterAppearance

## Properties
```
Color3: Color3
Graphic: ContentId
```

---

# Skin
**Extends:** CharacterAppearance

## Properties
```
SkinColor: BrickColor
```

---

# Chat
**Extends:** Instance

## Properties
```
BubbleChatEnabled: bool
IsAutoMigrated: bool
LoadDefaultChat: bool
```

## Functions
```
Chat(partOrCharacter: Instance, message: string, color: ChatColor) → null
ChatLocal(partOrCharacter: Instance, message: string, color: ChatColor) → null
GetShouldUseLuaChat() → bool
InvokeChatCallback(callbackType: ChatCallbackType, callbackArguments: Tuple) → Tuple
RegisterChatCallback(callbackType: ChatCallbackType, callbackFunction: Function) → null
SetBubbleChatSettings(settings: Variant) → null
CanUserChatAsync(userId: int64) → bool
CanUsersChatAsync(userIdFrom: int64, userIdTo: int64) → bool
FilterStringAsync(stringToFilter: string, playerFrom: Player, playerTo: Player) → string
FilterStringForBroadcast(stringToFilter: string, playerFrom: Player) → string
FilterStringForPlayerAsync(stringToFilter: string, playerToFilterFor: Player) → string [Deprecated]
```

## Events
```
BubbleChatSettingsChanged(settings: Variant)
Chatted(part: Instance, message: string, color: ChatColor)
ClientToServerFilterMessageSignalV2(sender: Instance, receiver: Instance, unfilteredMessage: string)
ClientToServerReportUnfilteredSignal(unfilteredText: string, match: string, instancePath: string, instanceType: string)
ServerToClientUnderOver13FilteredResponseSignal(sender: Instance, unfilteredMessage: string, isError: bool, errorStr: string, under13: string, over13: string)
TimeoutChatAttempt(isPermanentTimeout: bool, endTime: int64)
```

---

# ChatbotUIService
**Extends:** Instance

## Functions
```
DisplayContent(contentType: string, data: Dictionary) → null
GetSettings() → Dictionary
```

## Events
```
ActionActivatedSignal(action: string)
FindVariationsSignal(action: string)
SetMaterialSettingsSignal(guid: string, studsPerTile: double, isOrganic: bool)
SettingChangedSignal(setting: string, value: Variant)
ShiftToAssetIdSignal(action: string, change: int64)
ShiftVariationSignal(action: string, change: int)
```

---

# ClickDetector
**Extends:** Instance

## Properties
```
CursorIcon: ContentId
MaxActivationDistance: float
```

## Events
```
MouseActionReplicated(player: Player, actionType: int)
MouseClick(playerWhoClicked: Player)
MouseHoverEnter(playerWhoHovered: Player)
MouseHoverLeave(playerWhoHovered: Player)
RightMouseClick(playerWhoClicked: Player)
mouseClick(playerWhoClicked: Player)
```

---

# DragDetector
**Extends:** ClickDetector

## Properties
```
ActivatedCursorIcon: ContentId
ApplyAtCenterOfMass: bool
Axis: Vector3
DragFrame: CFrame
DragStyle: DragDetectorDragStyle
Enabled: bool
GamepadModeSwitchKeyCode: KeyCode
KeyboardModeSwitchKeyCode: KeyCode
MaxDragAngle: float
MaxDragTranslation: Vector3
MaxForce: float
MaxTorque: float
MinDragAngle: float
MinDragTranslation: Vector3
Orientation: Vector3
PermissionPolicy: DragDetectorPermissionPolicy
PhysicalDragClickedPart: Instance
PhysicalDragHitPoint: Vector3
PhysicalDragIsInVR: bool
PhysicalDragTargetFrame: CFrame
ReferenceInstance: Instance
ResponseStyle: DragDetectorResponseStyle
Responsiveness: float
RunLocally: bool
SecondaryAxis: Vector3
TrackballRadialPullFactor: float
TrackballRollFactor: float
VRSwitchKeyCode: KeyCode
WorldAxis: Vector3
WorldSecondaryAxis: Vector3
```

## Functions
```
AddConstraintFunction(priority: int, function: Function) → RBXScriptConnection
GetReferenceFrame() → CFrame
RestartDrag() → null
SetDragStyleFunction(function: Function) → null
SetPermissionPolicyFunction(function: Function) → null
```

## Events
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

# CloudCRUDService
**Extends:** Instance

---

# Clouds
**Extends:** Instance

## Properties
```
Color: Color3
Cover: float
Density: float
Enabled: bool
```

---

# ClusterPacketCache
**Extends:** Instance

---

# Collaborator
**Extends:** Instance

## Properties
```
CFrame: CFrame
CollaboratorColor: int [Deprecated]
CollaboratorColor3: Color3
CurDocGUID: string
CurScriptLineNumber: int
IsIdle: bool
Status: CollaboratorStatus
UserId: int64
Username: string
```

---

# CollaboratorsService
**Extends:** Instance

## Functions
```
GetCollaboratorsList() → Instances
GetSelectionHighlightsEnabled() → bool
RequestFlyToCollaborator(collaboratorId: int64) → null
ToggleSelectionHighlights(showHighlights: bool) → null
ToggleTeamCreate(on: bool) → null
```

## Events
```
CollaboratorIdleUpdate(collaboratorId: int64, isIdle: bool)
CollaboratorInstanceCreatedSignal(collaboratorId: int64)
CollaboratorInstanceDestroyedSignal(collaboratorId: int64)
CollaboratorStatusUpdateRequestedSignal(collaboratorId: int64, newStatus: CollaboratorStatus)
CollaboratorStatusUpdatedSignal(collaboratorId: int64, newStatus: CollaboratorStatus)
ToggleSelectionHighlightsSignal(areHighlightsShown: bool)
```

---

# CollectionService
**Extends:** Instance

## Functions
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

## Events
```
ItemAdded(instance: Instance)
ItemRemoved(instance: Instance)
TagAdded(tag: string)
TagRemoved(tag: string)
```

---

# CommerceService
**Extends:** Instance

## Functions
```
PromptCommerceProductPurchase(user: Player, commerceProductId: string) → null
PromptRealWorldCommerceBrowser(player: Player, url: string) → null
SignalPromptCommerceProductPurchaseFinished(productId: string, didTryPurchase: bool, checkoutSessionId: string) → null
GetCommerceProductInfoAsync(commerceProductId: string) → Dictionary
PrepareCommerceProductPurchase(commerceProductId: string) → Dictionary
UserEligibleForRealWorldCommerceAsync() → bool
```

## Events
```
BenefitStatusReceived(isGranted: bool)
FetchReceipt()
InExperienceBrowserRequested(url: string)
PromptCommerceProductPurchaseFinished(user: Player, productId: string)
PromptCommerceProductPurchaseRequested(commerceProductId: string)
PurchaseBrowserClosed()
```

---

# ConfigService
**Extends:** Instance

## Functions
```
ClearTestingValue(key: string) → null
SetTestingValue(key: string, value: Variant) → null
GetConfigAsync() → ConfigSnapshot
GetConfigForPlayerAsync(player: Player) → ConfigSnapshot
```

---

# Configuration
**Extends:** Instance

---

# ConfigureServerService
**Extends:** Instance

---

# ConnectivityService
**Extends:** Instance

## Properties
```
NetworkStatus: NetworkStatus [ReadOnly]
```

## Functions
```
IsNetworkStateAvailable() → bool
```

---

# Constraint
**Extends:** Instance

## Properties
```
Active: bool [ReadOnly]
Attachment0: Attachment
Attachment1: Attachment
Color: BrickColor
Enabled: bool
Visible: bool
```

## Functions
```
GetDebugAppliedForce(bodyId: int) → Vector3 [Deprecated]
GetDebugAppliedTorque(bodyId: int) → Vector3 [Deprecated]
```

---

# AlignOrientation
**Extends:** Constraint

## Properties
```
AlignType: AlignType
CFrame: CFrame
LookAtPosition: Vector3
MaxAngularVelocity: float
MaxTorque: float
Mode: OrientationAlignmentMode
PrimaryAxis: Vector3
PrimaryAxisOnly: bool
ReactionTorqueEnabled: bool
Responsiveness: float
RigidityEnabled: bool
SecondaryAxis: Vector3
```

---

# AlignPosition
**Extends:** Constraint

## Properties
```
ApplyAtCenterOfMass: bool
ForceLimitMode: ForceLimitMode
ForceRelativeTo: ActuatorRelativeTo
MaxAxesForce: Vector3
MaxForce: float
MaxVelocity: float
Mode: PositionAlignmentMode
Position: Vector3
ReactionForceEnabled: bool
Responsiveness: float
RigidityEnabled: bool
```

---

# AngularVelocity
**Extends:** Constraint

## Properties
```
AngularVelocity: Vector3
MaxTorque: float
ReactionTorqueEnabled: bool
RelativeTo: ActuatorRelativeTo
```

---

# AnimationConstraint
**Extends:** Constraint

## Properties
```
C0: CFrame [ReadOnly] [Deprecated]
C1: CFrame [ReadOnly] [Deprecated]
IsKinematic: bool
MaxForce: float
MaxTorque: float
Part0: BasePart [ReadOnly] [Deprecated]
Part1: BasePart [ReadOnly] [Deprecated]
Transform: CFrame
```

---

# BallSocketConstraint
**Extends:** Constraint

## Properties
```
LimitsEnabled: bool
MaxFrictionTorque: float
MaxFrictionTorqueXml: float
Radius: float
Restitution: float
TwistLimitsEnabled: bool
TwistLowerAngle: float
TwistUpperAngle: float
UpperAngle: float
```

---

# HingeConstraint
**Extends:** Constraint

## Properties
```
ActuatorType: ActuatorType
AngularResponsiveness: float
AngularSpeed: float
AngularVelocity: float
CurrentAngle: float [ReadOnly]
LimitsEnabled: bool
LowerAngle: float
MotorMaxAcceleration: float
MotorMaxTorque: float
Radius: float
Restitution: float
ServoMaxTorque: float
SoftlockServoUponReachingTarget: bool [Deprecated]
TargetAngle: float
UpperAngle: float
```

---

# LineForce
**Extends:** Constraint

## Properties
```
ApplyAtCenterOfMass: bool
InverseSquareLaw: bool
Magnitude: float
MaxForce: float
ReactionForceEnabled: bool
```

---

# LinearVelocity
**Extends:** Constraint

## Properties
```
ForceLimitMode: ForceLimitMode
ForceLimitsEnabled: bool
LineDirection: Vector3
LineVelocity: float
MaxAxesForce: Vector3
MaxForce: float
MaxPlanarAxesForce: Vector2
PlaneVelocity: Vector2
PrimaryTangentAxis: Vector3
ReactionForceEnabled: bool
RelativeTo: ActuatorRelativeTo
SecondaryTangentAxis: Vector3
VectorVelocity: Vector3
VelocityConstraintMode: VelocityConstraintMode
```

---

# PlaneConstraint
**Extends:** Constraint

---

# Plane
**Extends:** PlaneConstraint

---

# RigidConstraint
**Extends:** Constraint

---

# RodConstraint
**Extends:** Constraint

## Properties
```
CurrentDistance: float [ReadOnly]
Length: float
LimitAngle0: float
LimitAngle1: float
LimitsEnabled: bool
Thickness: float
```

---

# RopeConstraint
**Extends:** Constraint

## Properties
```
CurrentDistance: float [ReadOnly]
Length: float
Restitution: float
Thickness: float
WinchEnabled: bool
WinchForce: float
WinchResponsiveness: float
WinchSpeed: float
WinchTarget: float
```

---

# SlidingBallConstraint
**Extends:** Constraint

## Properties
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

# CylindricalConstraint
**Extends:** SlidingBallConstraint

## Properties
```
AngularActuatorType: ActuatorType
AngularLimitsEnabled: bool
AngularResponsiveness: float
AngularRestitution: float
AngularSpeed: float
AngularVelocity: float
CurrentAngle: float [ReadOnly]
InclinationAngle: float
LowerAngle: float
MotorMaxAngularAcceleration: float
MotorMaxTorque: float
RotationAxisVisible: bool
ServoMaxTorque: float
SoftlockAngularServoUponReachingTarget: bool [Deprecated]
TargetAngle: float
UpperAngle: float
WorldRotationAxis: Vector3 [ReadOnly]
```

---

# PrismaticConstraint
**Extends:** SlidingBallConstraint

---

# SpringConstraint
**Extends:** Constraint

## Properties
```
Coils: float
CurrentLength: float [ReadOnly]
Damping: float
FreeLength: float
LimitsEnabled: bool
MaxForce: float
MaxLength: float
MinLength: float
Radius: float
Stiffness: float
Thickness: float
```

---

# Torque
**Extends:** Constraint

## Properties
```
RelativeTo: ActuatorRelativeTo
Torque: Vector3
```

---

# TorsionSpringConstraint
**Extends:** Constraint

## Properties
```
Coils: float
CurrentAngle: float [ReadOnly]
Damping: float
LimitEnabled: bool [Deprecated]
LimitsEnabled: bool
MaxAngle: float
MaxTorque: float
Radius: float
Restitution: float
Stiffness: float
```

---

# UniversalConstraint
**Extends:** Constraint

## Properties
```
LimitsEnabled: bool
MaxAngle: float
Radius: float
Restitution: float
```

---

# VectorForce
**Extends:** Constraint

## Properties
```
ApplyAtCenterOfMass: bool
Force: Vector3
RelativeTo: ActuatorRelativeTo
```

---

# ContentProvider
**Extends:** Instance

## Properties
```
BaseUrl: string [ReadOnly]
RequestQueueSize: int [ReadOnly]
```

## Functions
```
GetAssetFetchStatus(contentId: ContentId) → AssetFetchStatus
GetAssetFetchStatusChangedSignal(contentId: ContentId) → RBXScriptSignal
GetDependencyContentIds(root: Instance) → Array
GetFailedRequests() → Array
ListEncryptedAssets() → Array
Preload(contentId: ContentId) → null [Deprecated]
RegisterDefaultEncryptionKey(encryptionKey: string) → null
RegisterDefaultSessionKey(sessionKey: string) → null
RegisterEncryptedAsset(assetId: ContentId, encryptionKey: string) → null
RegisterSessionEncryptedAsset(contentId: ContentId, sessionKey: string) → null
SetBaseUrl(url: string) → null
UnregisterDefaultEncryptionKey() → null
UnregisterEncryptedAsset(assetId: ContentId) → null
PreloadAsync(contentIdList: Array, callbackFunction: Function) → null
```

## Events
```
AssetFetchFailed(assetId: ContentId)
```

---

# ContextActionService
**Extends:** Instance

## Functions
```
BindAction(actionName: string, functionToBind: Function, createTouchButton: bool, inputTypes: Tuple) → null
BindActionAtPriority(actionName: string, functionToBind: Function, createTouchButton: bool, priorityLevel: int, inputTypes: Tuple) → null
BindActionToInputTypes(actionName: string, functionToBind: Function, createTouchButton: bool, inputTypes: Tuple) → null [Deprecated]
BindActivate(userInputTypeForActivation: UserInputType, keyCodesForActivation: Tuple) → null
BindCoreAction(actionName: string, functionToBind: Function, createTouchButton: bool, inputTypes: Tuple) → null
BindCoreActionAtPriority(actionName: string, functionToBind: Function, createTouchButton: bool, priorityLevel: int, inputTypes: Tuple) → null
BindCoreActivate(userInputTypeForActivation: UserInputType, keyCodesForActivation: Tuple) → null
CallFunction(actionName: string, state: UserInputState, inputObject: Instance) → Tuple
FireActionButtonFoundSignal(actionName: string, actionButton: Instance) → null
GetAllBoundActionInfo() → Dictionary
GetAllBoundCoreActionInfo() → Dictionary
GetBoundActionInfo(actionName: string) → Dictionary
GetBoundCoreActionInfo(actionName: string) → Dictionary
GetCurrentLocalToolIcon() → string
SetDescription(actionName: string, description: string) → null
SetImage(actionName: string, image: string) → null
SetPosition(actionName: string, position: UDim2) → null
SetTitle(actionName: string, title: string) → null
UnbindAction(actionName: string) → null
UnbindActivate(userInputTypeForActivation: UserInputType, keyCodeForActivation: KeyCode) → null
UnbindAllActions() → null
UnbindCoreAction(actionName: string) → null
UnbindCoreActivate(userInputTypeForActivation: UserInputType, keyCodeForActivation: KeyCode) → null
GetButton(actionName: string) → Instance
```

## Events
```
BoundActionAdded(actionAdded: string, createTouchButton: bool, functionInfoTable: Dictionary, isCore: bool)
BoundActionChanged(actionChanged: string, changeName: string, changeTable: Dictionary)
BoundActionRemoved(actionRemoved: string, functionInfoTable: Dictionary, isCore: bool)
GetActionButtonEvent(actionName: string)
LocalToolEquipped(toolEquipped: Instance)
LocalToolUnequipped(toolUnequipped: Instance)
```

---

# Controller
**Extends:** Instance

## Functions
```
BindButton(button: Button, caption: string) → null
GetButton(button: Button) → bool
UnbindButton(button: Button) → null
bindButton(button: Button, caption: string) → null [Deprecated]
getButton(button: Button) → bool [Deprecated]
```

## Events
```
ButtonChanged(button: Button)
```

---

# HumanoidController
**Extends:** Controller

---

# SkateboardController
**Extends:** Controller

## Properties
```
Steer: float [ReadOnly]
Throttle: float [ReadOnly]
```

## Events
```
AxisChanged(axis: string)
```

---

# VehicleController
**Extends:** Controller

---

# ControllerBase
**Extends:** Instance

## Properties
```
Active: bool [ReadOnly]
BalanceRigidityEnabled: bool
MoveSpeedFactor: float
```

---

# AirController
**Extends:** ControllerBase

## Properties
```
BalanceMaxTorque: float
BalanceSpeed: float
LinearImpulse: Vector3
MaintainAngularMomentum: bool
MaintainLinearMomentum: bool
MoveMaxForce: float
TurnMaxTorque: float
TurnSpeedFactor: float
```

---

# ClimbController
**Extends:** ControllerBase

## Properties
```
AccelerationTime: float
BalanceMaxTorque: float
BalanceSpeed: float
MoveMaxForce: float
```

---

# GroundController
**Extends:** ControllerBase

## Properties
```
AccelerationLean: float
AccelerationTime: float
BalanceMaxTorque: float
BalanceSpeed: float
DecelerationTime: float
Friction: float
FrictionWeight: float
GroundOffset: float
StandForce: float
StandSpeed: float
TurnSpeedFactor: float
```

---

# SwimController
**Extends:** ControllerBase

## Properties
```
AccelerationTime: float
PitchMaxTorque: float
PitchSpeedFactor: float
RollMaxTorque: float
RollSpeedFactor: float
```

---

# ControllerManager
**Extends:** Instance

## Properties
```
ActiveController: ControllerBase
BaseMoveSpeed: float
BaseTurnSpeed: float
ClimbSensor: ControllerSensor
FacingDirection: Vector3
GroundSensor: ControllerSensor
MovingDirection: Vector3
RootPart: BasePart
UpDirection: Vector3
```

---

# ControllerService
**Extends:** Instance

---

# ConversationalAIAcceptanceService
**Extends:** Instance

## Functions
```
AlternativeAssetSelected(requestId: string, previousAssetId: int64, assetId: int64) → null
AssetInserted(requestId: string, assetId: int64) → null
CodeRunnerActivated(requestId: string, code: string, serverAutorun: bool, autorunEnabled: bool, autoExpandDropdowns: bool) → null
CodeRunnerCompleted(requestId: string, success: bool, errorMessage: string) → null
CodeRunnerUndone(requestId: string) → null
DataModelHierarchyLatency(requestId: string, latency: double) → null
ErrorTelemetry(requestId: string, errorId: string, errorType: string, errorMessage: string) → null
InstanceInserted(requestId: string) → null
RecordingActionEnded(requestId: string, waypointName: string) → null
ReportJSONEncodeFailure(instanceName: string, className: string) → null
SendCommandErrorTelemetry(requestId: string, commandName: string, errorMessage: string) → null
SendMeshGenActivatedTelemetry() → null
SendMeshGenCompletedTelemetry(requestId: string, generationId: string, success: bool, errorMessage: string, prompt: string) → null
SendMeshGenMeshInsertedTelemetry(requestId: string, generationId: string, success: bool, errorMessage: string) → null
SendMeshGenPublishedAssetsTelemetry(requestId: string, generationId: string, success: bool, errorMessage: string, meshId: int64?, imageId: int64?) → null
```

---

# CookiesService
**Extends:** Instance

---

# CorePackages
**Extends:** Instance

---

# CoreScriptDebuggingManagerHelper
**Extends:** Instance

---

# CoreScriptSyncService
**Extends:** Instance

## Functions
```
GetScriptFilePath(script: Instance) → Variant
```

---

# CreationDBService
**Extends:** Instance

---

# CreatorStoreService
**Extends:** Instance

## Functions
```
GetAssetInfoAsync(assetId: int64) → Dictionary
GetCreatorStoreProductInfoAsync(productTargetId: int64, assetType: string) → Dictionary
PerformCreatorStorePurchase(productTargetId: int64, assetType: string) → Dictionary
```

---

# CrossDMScriptChangeListener
**Extends:** Instance

## Functions
```
IsWatchingScriptLine(scriptRef: string, lineNumber: int) → bool
StartWatchingScriptLine(scriptRef: string, debuggerConnectionId: int, lineNumber: int) → null
```

## Events
```
GuidLineContentsChanged(guid: string, lineNumber: int, contents: string)
GuidNameChanged(guid: string, fullName: string)
```

---

# CustomEvent
**Extends:** Instance

## Properties
```
PersistedCurrentValue: float
```

## Functions
```
GetAttachedReceivers() → Instances
SetValue(newValue: float) → null
```

## Events
```
ReceiverConnected(receiver: Instance)
ReceiverDisconnected(receiver: Instance)
```

---

# CustomEventReceiver
**Extends:** Instance

## Properties
```
Source: Instance
```

## Functions
```
GetCurrentValue() → float
```

## Events
```
EventConnected(event: Instance)
EventDisconnected(event: Instance)
SourceValueChanged(newValue: float)
```

---

# CustomLog
**Extends:** Instance

## Functions
```
Close() → null
GetLogPath() → string
Open() → null
WriteAppend(append: string) → null
```

---

# DataModelMesh
**Extends:** Instance

## Properties
```
Offset: Vector3
Scale: Vector3
VertexColor: Vector3
```

---

# BevelMesh
**Extends:** DataModelMesh

## Properties
```
Bevel: float
Bevel Roundness: float
Bulge: float
```

---

# BlockMesh
**Extends:** BevelMesh

---

# CylinderMesh
**Extends:** BevelMesh

---

# FileMesh
**Extends:** DataModelMesh

## Properties
```
MeshId: ContentId
TextureId: ContentId
```

---

# SpecialMesh
**Extends:** FileMesh

## Properties
```
MeshType: MeshType
```

---

# DataModelPatchService
**Extends:** Instance

## Functions
```
GetLuaVersion(patchName: string) → string
GetPatch(patchName: string) → Instance
RegisterPatch(patchName: string, behaviorName: string, localConfigPath: string, userId: int64) → null
UpdatePatch(userId: int64, patchName: string, callbackFunction: Function) → null
```

---

# DataModelSession
**Extends:** Instance

## Properties
```
CurrentDataModelType: StudioDataModelType [ReadOnly]
SessionId: string [ReadOnly]
```

## Events
```
CurrentDataModelTypeAboutToChange(dataModelType: StudioDataModelType)
CurrentDataModelTypeChanged()
```

---

# DataStoreGetOptions
**Extends:** Instance

## Properties
```
UseCache: bool
```

---

# DataStoreIncrementOptions
**Extends:** Instance

## Functions
```
GetMetadata() → Dictionary
SetMetadata(attributes: Dictionary) → null
```

---

# DataStoreInfo
**Extends:** Instance

## Properties
```
CreatedTime: int64 [ReadOnly]
DataStoreName: string [ReadOnly]
UpdatedTime: int64 [ReadOnly]
```

---

# DataStoreKey
**Extends:** Instance

## Properties
```
KeyName: string [ReadOnly]
```

---

# DataStoreKeyInfo
**Extends:** Instance

## Properties
```
CreatedTime: int64 [ReadOnly]
UpdatedTime: int64 [ReadOnly]
Version: string [ReadOnly]
```

## Functions
```
GetMetadata() → Dictionary
GetUserIds() → Array
```

---

# DataStoreObjectVersionInfo
**Extends:** Instance

## Properties
```
CreatedTime: int64 [ReadOnly]
IsDeleted: bool [ReadOnly]
Version: string [ReadOnly]
```

---

# DataStoreOptions
**Extends:** Instance

## Properties
```
AllScopes: bool
```

## Functions
```
SetExperimentalFeatures(experimentalFeatures: Dictionary) → null
```

---

# DataStoreService
**Extends:** Instance

## Properties
```
AutomaticRetry: bool
LegacyNamingScheme: bool [Deprecated]
```

## Functions
```
GetDataStore(name: string, scope: string, options: Instance) → DataStore
GetGlobalDataStore() → DataStore
GetOrderedDataStore(name: string, scope: string) → OrderedDataStore
GetRequestBudgetForRequestType(requestType: DataStoreRequestType) → int
ListDataStoresAsync(prefix: string, pageSize: int, cursor: string) → DataStoreListingPages
```

---

# DataStoreSetOptions
**Extends:** Instance

## Functions
```
GetMetadata() → Dictionary
SetMetadata(attributes: Dictionary) → null
```

---

# Debris
**Extends:** Instance

## Properties
```
MaxItems: int [Deprecated]
```

## Functions
```
AddItem(item: Instance, lifetime: double) → null
SetLegacyMaxItems(enabled: bool) → null
addItem(item: Instance, lifetime: double) → null [Deprecated]
```

---

# DebugSettings
**Extends:** Instance

## Properties
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

# DebuggablePluginWatcher
**Extends:** Instance

---

# DebuggerBreakpoint
**Extends:** Instance

## Properties
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

# DebuggerConnection
**Extends:** Instance

## Properties
```
ErrorMessage: string [ReadOnly]
HasError: bool [ReadOnly]
Id: int [ReadOnly]
IsPaused: bool [ReadOnly]
```

## Functions
```
AddBreakpoint(script: string, line: int, breakpoint: Breakpoint) → null
Close() → null
EvaluateWatch(expression: string, frame: StackFrame, callback: Function) → int
GetFrameById(id: int) → StackFrame
GetSource(scriptRef: string, status: Function) → int
GetThreadById(id: int) → ThreadState
GetThreads(callback: Function) → int
GetVariableById(id: int) → DebuggerVariable
Pause(thread: ThreadState, status: Function) → int
Populate(instance: Instance, callback: Function) → int
RemoveBreakpoint(breakpoint: Breakpoint) → null
Resume(thread: ThreadState, status: Function) → int
SetExceptionBreakMode(breakMode: DebuggerExceptionBreakMode, callback: Function) → int
SetVariable(variable: DebuggerVariable, value: string, callback: Function) → int
Step(thread: ThreadState, callback: Function) → int
StepIn(thread: ThreadState, callback: Function) → int
StepOut(thread: ThreadState, callback: Function) → int
UpdateSelectedFrame(threadId: int, frameNumber: int) → null
```

## Events
```
BreakpointAdded(breakpoint: Breakpoint)
BreakpointChanged(breakpoint: Breakpoint)
BreakpointRemoved(breakpoint: Breakpoint, reason: BreakpointRemoveReason)
Paused(pausedState: PausedState, reason: DebuggerPauseReason)
Resumed(pausedState: PausedState)
```

---

# LocalDebuggerConnection
**Extends:** DebuggerConnection

---

# DebuggerConnectionManager
**Extends:** Instance

## Properties
```
Timeout: double
```

## Functions
```
ConnectLocal(dataModel: DataModel) → int
ConnectRemote(host: string, port: int) → int
FocusConnection(connection: DebuggerConnection) → null
GetAvailableConnection() → DebuggerConnection
GetConnectionById(id: int) → DebuggerConnection
```

## Events
```
ConnectionEnded(connection: DebuggerConnection, reason: DebuggerEndReason)
ConnectionStarted(connection: DebuggerConnection)
FocusChanged(connection: DebuggerConnection)
```

---

# DebuggerLuaResponse
**Extends:** Instance

## Properties
```
IsError: bool [ReadOnly]
IsSuccess: bool [ReadOnly]
Message: string [ReadOnly]
RequestId: int [ReadOnly]
Status: DebuggerStatus [ReadOnly]
```

## Functions
```
GetArg() → Variant
```

---

# DebuggerManager
**Extends:** Instance

## Properties
```
DebuggingEnabled: bool [ReadOnly]
```

## Functions
```
AddDebugger(script: Instance) → Instance
EnableDebugging() → null
GetDebuggers() → Instances
Resume() → null
StepIn() → null [Deprecated]
StepOut() → null [Deprecated]
StepOver() → null [Deprecated]
```

## Events
```
DebuggerAdded(debugger: Instance)
DebuggerRemoved(debugger: Instance)
```

---

# DebuggerUIService
**Extends:** Instance

## Functions
```
EditBreakpoint(metaBreakpointId: int) → null
EditWatch(expression: string) → null
IsConnectionForPlayDataModel(debuggerConnectionId: int) → bool
OpenExceptionMessagePopup(exceptionMessage: string, pausedLine: int) → null
OpenScriptAtLine(guid: string, debuggerConnectionId: int, line: int, showErrorOnFail: bool) → null
Pause() → null
RemoveScriptLineMarkers(debuggerConnectionId: int, allMarkers: bool) → null
Resume() → null
SetCurrentThreadId(debuggerThreadId: int) → null
SetScriptLineMarker(guid: string, debuggerConnectionId: int, line: int, lineMarkerType: bool) → null
SetWatchExpressions(expressions: Array) → null
```

## Events
```
ExpressionAdded(expression: string)
ExpressionsCleared()
```

---

# DebuggerVariable
**Extends:** Instance

## Properties
```
Name: string [ReadOnly]
Populated: bool [ReadOnly]
Type: string [ReadOnly]
Value: string [ReadOnly]
VariableId: int [ReadOnly]
VariablesCount: int [ReadOnly]
```

## Functions
```
GetVariableByIndex(index: int) → DebuggerVariable
GetVariableByName(name: string) → DebuggerVariable
```

---

# DebuggerWatch
**Extends:** Instance

## Properties
```
Expression: string
```

---

# DeviceIdService
**Extends:** Instance

## Functions
```
GetDeviceId() → string
```

---

# Dialog
**Extends:** Instance

## Properties
```
BehaviorType: DialogBehaviorType
ConversationDistance: float
GoodbyeChoiceActive: bool
GoodbyeDialog: string
InUse: bool
InitialPrompt: string
Purpose: DialogPurpose
Tone: DialogTone
TriggerDistance: float
TriggerOffset: Vector3
```

## Functions
```
GetCurrentPlayers() → Instances
SetGuiObject(gui: BillboardGui) → null
SetPlayerIsUsing(player: Instance, isUsing: bool) → null
SignalDialogChoiceSelected(player: Instance, dialogChoice: Instance) → null
```

## Events
```
DialogChoiceSelected(player: Instance, dialogChoice: Instance)
```

---

# DialogChoice
**Extends:** Instance

## Properties
```
GoodbyeChoiceActive: bool
GoodbyeDialog: string
ResponseDialog: string
UserDialog: string
```

---

# DraftsService
**Extends:** Instance

## Functions
```
DiscardEdits(scripts: Instances) → null
GetDraftStatus(script: Instance) → DraftStatusCode
GetEditors(script: Instance) → Instances
RestoreScripts(scripts: Instances) → null
ShowDiffsAgainstBase(scripts: Instances) → null
ShowDiffsAgainstServer(scripts: Instances) → null
ShowSourceDiffsAgainstCurrent(sources: Array, scripts: Instances) → null
CommitEdits(scripts: Instances) → null
GetDrafts() → Instances
UpdateToLatestVersion(scripts: Instances) → null
```

## Events
```
CommitStatusChanged(script: Instance, status: DraftStatusCode)
DraftAdded(script: Instance)
DraftRemoved(script: Instance)
DraftStatusChanged(script: Instance)
EditorsListChanged(script: Instance)
UpdateStatusChanged(script: Instance, status: DraftStatusCode)
```

---

# Dragger
**Extends:** Instance

## Functions
```
AxisRotate(axis: Axis) → null
MouseDown(mousePart: Instance, pointOnMousePart: Vector3, parts: Instances) → null
MouseMove(mouseRay: Ray) → null
MouseUp() → null
```

---

# DraggerService
**Extends:** Instance

## Properties
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
HoverLineThickness: int
HoverThickness: float
JointsEnabled: bool
LinearSnapEnabled: bool
LinearSnapIncrement: float
PartSnapEnabled: bool
PivotSnapToGeometry: bool
ShowHover: bool
ShowPivotIndicator: bool
```

---

# EditableService
**Extends:** Instance

## Properties
```
EditableStatus: EditableStatus
```

---

# EulerRotationCurve
**Extends:** Instance

## Properties
```
RotationOrder: RotationOrder
```

## Functions
```
GetAnglesAtTime(time: float) → Array
GetRotationAtTime(time: float) → CFrame
X() → FloatCurve
Y() → FloatCurve
Z() → FloatCurve
```

---

# EventIngestService
**Extends:** Instance

## Functions
```
SendEventDeferred(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null
SendEventImmediately(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null
SetRBXEvent(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null
SetRBXEventStream(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null
```

---

# ExampleService
**Extends:** Instance

## Functions
```
PrintHello() → null
```

## Events
```
OnPolo(message: string)
```

---

# ExampleV2Service
**Extends:** Instance

## Functions
```
PrintHello() → null
```

## Events
```
OnPolo(message: string)
```

---

# ExperienceAuthService
**Extends:** Instance

## Functions
```
ScopeCheckUIComplete(guid: string, scopes: Array, result: ScopeCheckResult, metadata: Dictionary) → null
```

## Events
```
OpenAuthPrompt(guid: string, scopes: Array, metadata: Dictionary)
ScopeCheckResult(guid: string, result: ScopeCheckResult, token: string, scopes: Array, metadata: Dictionary)
```

---

# ExperienceInviteOptions
**Extends:** Instance

## Properties
```
InviteMessageId: string
InviteUser: int64
LaunchData: string
PromptMessage: string
```

---

# ExperienceNotificationService
**Extends:** Instance

## Functions
```
InvokeOptInPromptClosed() → null
PromptOptIn() → null
CanPromptOptInAsync() → bool
```

## Events
```
OptInPromptClosed()
PromptOptInRequested()
```

---

# ExperienceService
**Extends:** Instance

## Functions
```
ExecuteCrossExperienceCall(callId: string, params: Dictionary, successCallback: Function, errorCallback: Function) → null
GetPendingJoinAttempt() → Dictionary
LaunchExperience(params: Dictionary) → string
LaunchExperienceFromSource(params: Dictionary, source: string) → string
LaunchExperienceFromSourceWithCallback(params: Dictionary, source: string, callback: Function) → null
RegisterForExperienceJoin(callback: Function) → RBXScriptConnection
RegisterForExperienceLeave(callback: Function) → RBXScriptConnection
StartCrossExperience(type: string, params: Dictionary) → null
StopCrossExperience(type: string, params: Dictionary) → null
```

## Events
```
OnCrossExperienceStarted(type: string, params: Dictionary)
OnCrossExperienceStopped(type: string, params: Dictionary)
OnNewJoinAttempt(params: Dictionary)
```

---

# ExperienceStateCaptureService
**Extends:** Instance

## Properties
```
HiddenSelectionEnabled: bool
IsInBackground: bool [ReadOnly]
IsInCaptureMode: bool [ReadOnly]
```

## Functions
```
CanEnterCaptureMode() → bool
ResetHighlight() → null
ToggleCaptureMode() → null
```

## Events
```
ItemSelectedInCaptureMode(instance: Instance)
```

---

# ExperienceStateRecordingService
**Extends:** Instance

---

# ExplorerFilter
**Extends:** Instance

## Functions
```
BeginSearch(root: Instance) → null
GetAutocompleter() → ExplorerFilterAutocompleter
GetErrors() → Array
GetLexemes() → Array
GetSearchResults(maxCandidatesToExplore: int) → Instances
HasMoreResults() → bool
InstancePassesFilter(instance: Instance) → bool
SetFilter(search: string) → null
```

---

# ExplorerFilterAutocompleter
**Extends:** Instance

## Properties
```
ReplaceRange: Vector2 [ReadOnly]
RequiresOutsideContext: bool [ReadOnly]
```

## Functions
```
GetSuggestions() → Array
```

---

# ExplorerServiceVisibilityService
**Extends:** Instance

## Functions
```
GetServiceVisibility(service: Instance) → bool
```

---

# Explosion
**Extends:** Instance

## Properties
```
BlastPressure: float
BlastRadius: float
DestroyJointRadiusPercent: float
ExplosionType: ExplosionType
LocalTransparencyModifier: float
Position: Vector3
TimeScale: float
Visible: bool
```

## Events
```
Hit(part: BasePart, distance: float)
```

---

# FaceAnimatorService
**Extends:** Instance

## Properties
```
AudioAnimationEnabled: bool
FaceTrackingStatusEnum: TrackerFaceTrackingStatus
FlipHeadOrientation: bool
VideoAnimationEnabled: bool
```

## Functions
```
GetTrackerLodController() → TrackerLodController
Init(videoEnabled: bool, audioEnabled: bool) → null
IsStarted() → bool
Start() → null
Step() → null
Stop() → null
```

## Events
```
TrackerError(error: TrackerError)
TrackerPrompt(prompt: TrackerPromptEvent)
```

---

# FaceControls
**Extends:** Instance

## Properties
```
ChinRaiser: float
ChinRaiserUpperLip: float
Corrugator: float
EyesLookDown: float
EyesLookLeft: float
EyesLookRight: float
EyesLookUp: float
FlatPucker: float
Funneler: float
JawDrop: float
JawLeft: float
JawRight: float
LeftBrowLowerer: float
LeftCheekPuff: float
LeftCheekRaiser: float
LeftDimpler: float
LeftEyeClosed: float
LeftEyeUpperLidRaiser: float
LeftInnerBrowRaiser: float
LeftLipCornerDown: float
LeftLipCornerPuller: float
LeftLipStretcher: float
LeftLowerLipDepressor: float
LeftNoseWrinkler: float
LeftOuterBrowRaiser: float
LeftUpperLipRaiser: float
LipPresser: float
LipsTogether: float
LowerLipSuck: float
MouthLeft: float
MouthRight: float
Pucker: float
RightBrowLowerer: float
RightCheekPuff: float
RightCheekRaiser: float
RightDimpler: float
RightEyeClosed: float
RightEyeUpperLidRaiser: float
RightInnerBrowRaiser: float
RightLipCornerDown: float
RightLipCornerPuller: float
RightLipStretcher: float
RightLowerLipDepressor: float
RightNoseWrinkler: float
RightOuterBrowRaiser: float
RightUpperLipRaiser: float
TongueDown: float
TongueOut: float
TongueUp: float
UpperLipSuck: float
```

---

# FaceInstance
**Extends:** Instance

## Properties
```
Face: NormalId
```

---

# Decal
**Extends:** FaceInstance

## Properties
```
Color3: Color3
LocalTransparencyModifier: float
MetalnessMap: ContentId
MetalnessMapContent: Content
NormalMap: ContentId
NormalMapContent: Content
RoughnessMap: ContentId
RoughnessMapContent: Content
Shiny: float [Deprecated]
Specular: float [Deprecated]
Texture: ContentId
TextureContent: Content
Transparency: float
UVOffset: Vector2
UVScale: Vector2
ZIndex: int
```

---

# Texture
**Extends:** Decal

## Properties
```
OffsetStudsU: float
OffsetStudsV: float
StudsPerTileU: float
StudsPerTileV: float
```

---

# FacialAgeEstimationService
**Extends:** Instance

## Functions
```
IsAvailable() → bool
InquiryAsync(inquiryRequest: Dictionary) → Dictionary
```

---

# FacialAnimationRecordingService
**Extends:** Instance

## Properties
```
BiometricDataConsent: bool
```

## Functions
```
IsAgeRestricted() → bool
CheckOrRequestCameraPermission() → string
```

---

# FacialAnimationStreamingServiceStats
**Extends:** Instance

## Functions
```
Get(label: string) → int64
GetWithPlayerId(label: string, playerId: int64) → int64
```

---

# FacialAnimationStreamingServiceV2
**Extends:** Instance

## Properties
```
ServiceState: int
```

## Functions
```
GetStats() → FacialAnimationStreamingServiceStats
IsAudioEnabled(mask: int) → bool
IsPlaceEnabled(mask: int) → bool
IsServerEnabled(mask: int) → bool
IsVideoEnabled(mask: int) → bool
ResolveStateForUser(userId: int64) → int
```

---

# FacialAnimationStreamingSubsessionStats
**Extends:** Instance

---

# Feature
**Extends:** Instance

## Properties
```
FaceId: NormalId
InOut: InOut
LeftRight: LeftRight
TopBottom: TopBottom
```

---

# Hole
**Extends:** Feature

---

# MotorFeature
**Extends:** Feature

---

# FeatureRestrictionManager
**Extends:** Instance

## Events
```
TimeoutChatAttempt(isPermanentTimeout: bool, endTime: int64)
UpdateExperienceChatTimeout(startTime: int64, duration: int64)
```

---

# File
**Extends:** Instance

## Properties
```
Size: int64 [ReadOnly]
```

## Functions
```
GetBinaryContents() → string
GetTemporaryId() → ContentId
```

---

# Fire
**Extends:** Instance

## Properties
```
Color: Color3
Enabled: bool
Heat: float
LocalTransparencyModifier: float
SecondaryColor: Color3
Size: float
TimeScale: float
heat_xml: float
size: float [Deprecated]
size_xml: float
```

## Functions
```
FastForward(numFrames: int) → null
```

---

# FlagStandService
**Extends:** Instance

---

# FloatCurve
**Extends:** Instance

## Properties
```
Length: int [ReadOnly]
ValuesAndTimes: BinaryString
```

## Functions
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

# FlyweightService
**Extends:** Instance

---

# CSGDictionaryService
**Extends:** FlyweightService

---

# NonReplicatedCSGDictionaryService
**Extends:** FlyweightService

---

# Folder
**Extends:** Instance

## Properties
```
ReplicatedGuiInsertionOrder: int
```

---

# ForceField
**Extends:** Instance

## Properties
```
Visible: bool
```

---

# FriendService
**Extends:** Instance

## Functions
```
GetPlatformFriends() → Array
```

## Events
```
FriendsUpdated(friendData: Array)
RemoteFriendEventSignal(userId: int64, userId: int64, event: FriendRequestEvent)
RemoteFriendStatusSignal(userId: int64, userId: int64, status: FriendStatus)
```

---

# FunctionalTest
**Extends:** Instance

## Properties
```
AllowSleep: bool
Description: string
HasMigratedSettingsToTestService: bool
Is30FpsThrottleEnabled: bool
PhysicsEnvironmentalThrottle: bool
Timeout: double
```

## Functions
```
Error(message: string) → null
Failed(message: string) → null
Pass(message: string) → null
Passed(message: string) → null
Warn(message: string) → null
```

---

# GamePassService
**Extends:** Instance

## Functions
```
PlayerHasPass(player: Player, gamePassId: int64) → bool [Deprecated]
```

---

# GameSettings
**Extends:** Instance

## Properties
```
VideoCaptureEnabled: bool
VideoRecording: bool
```

## Events
```
VideoRecordingChangeRequest(recording: bool)
```

---

# GamepadService
**Extends:** Instance

## Properties
```
GamepadCursorEnabled: bool
```

## Functions
```
DisableGamepadCursor() → null
EnableGamepadCursor(guiObject: Instance) → null
GetGamepadCursorPosition() → Vector2
SetGamepadCursorPosition(position: Vector2) → null
```

## Events
```
GamepadThumbstick1Changed(event: Vector2)
```

---

# GenerationService
**Extends:** Instance

## Functions
```
GenerateMeshAsync(inputs: Dictionary, player: Player, options: Dictionary, intermediateResultCallback: Function?) → Tuple
InternalGenerateMeshAsync(inputs: Dictionary, userId: int64, options: Dictionary, intermediateResultCallback: Function?) → Tuple
LoadGeneratedMeshAsync(generationId: string) → MeshPart
```

## Events
```
ReplicateGeneration(id: string, success: bool, serializedModel: string)
RequestGenerationReplication(id: string)
```

---

# GenericChallengeService
**Extends:** Instance

## Functions
```
SignalChallengeAbandoned(challengeID: string) → null
SignalChallengeCompleted(challengeID: string, challengeType: string, challengeMetadata: string) → null
SignalChallengeInvalidated(challengeID: string) → null
SignalChallengeLoaded(challengeID: string, success: bool) → null
SignalChallengeRequired(challengeID: string, challengeType: string, challengeMetadata: string) → null
```

## Events
```
ChallengeAbandonedEvent(challengeID: string)
ChallengeCompletedEvent(challengeID: string, challengeType: string, challengeMetadata: string)
ChallengeInvalidatedEvent(challengeID: string)
ChallengeLoadedEvent(challengeID: string, success: bool)
ChallengeRequiredEvent(challengeID: string, challengeType: string, challengeMetadata: string)
```

---

# Geometry
**Extends:** Instance

---

# GeometryService
**Extends:** Instance

## Functions
```
CalculateConstraintsToPreserve(source: Instance, destination: Array, options: Dictionary) → Array
HashMeshAsync(meshId: ContentId) → string
IntersectAsync(part: Instance, parts: Array, options: Dictionary) → Array
SubtractAsync(part: Instance, parts: Array, options: Dictionary) → Array
UnionAsync(part: Instance, parts: Array, options: Dictionary) → Array
```

---

# GetTextBoundsParams
**Extends:** Instance

## Properties
```
Font: Font
RichText: bool
Size: float
Text: string
Width: float
```

---

# GlobalDataStore
**Extends:** Instance

## Functions
```
OnUpdate(key: string, callback: Function) → RBXScriptConnection [Deprecated]
GetAsync(key: string, options: DataStoreGetOptions) → Tuple
IncrementAsync(key: string, delta: int, userIds: Array, options: DataStoreIncrementOptions) → Variant
RemoveAsync(key: string) → Tuple
SetAsync(key: string, value: Variant, userIds: Array, options: DataStoreSetOptions) → Variant
UpdateAsync(key: string, transformFunction: Function) → Tuple
```

---

# DataStore
**Extends:** GlobalDataStore

## Functions
```
GetVersionAsync(key: string, version: string) → Tuple
GetVersionAtTimeAsync(key: string, timestamp: int64) → Tuple
ListKeysAsync(prefix: string, pageSize: int, cursor: string, excludeDeleted: bool) → DataStoreKeyPages
ListVersionsAsync(key: string, sortDirection: SortDirection, minDate: int64, maxDate: int64, pageSize: int) → DataStoreVersionPages
RemoveVersionAsync(key: string, version: string) → null
```

---

# OrderedDataStore
**Extends:** GlobalDataStore

## Functions
```
GetSortedAsync(ascending: bool, pagesize: int, minValue: Variant, maxValue: Variant) → DataStorePages
```

---

# GroupService
**Extends:** Instance

## Functions
```
GetAlliesAsync(groupId: int64) → StandardPages
GetEnemiesAsync(groupId: int64) → StandardPages
GetGroupInfoAsync(groupId: int64) → Variant
GetGroupsAsync(userId: int64) → Array
```

---

# GuiBase
**Extends:** Instance

---

# GuiBase2d
**Extends:** GuiBase

## Properties
```
AbsolutePosition: Vector2 [ReadOnly]
AbsoluteRotation: float [ReadOnly]
AbsoluteSize: Vector2 [ReadOnly]
ActiveQueryNames: string
AutoLocalize: bool
ClippedRect: Rect [ReadOnly]
IsNotOccluded: bool [ReadOnly]
Localize: bool [Deprecated]
RawRect2D: Rect [ReadOnly]
ReplicatedInsertionOrder: int
RootLocalizationTable: LocalizationTable
SelectionBehaviorDown: SelectionBehavior
SelectionBehaviorLeft: SelectionBehavior
SelectionBehaviorRight: SelectionBehavior
SelectionBehaviorUp: SelectionBehavior
SelectionGroup: bool
TotalGroupScale: float [ReadOnly]
```

## Events
```
SelectionChanged(amISelected: bool, previousSelection: GuiObject, newSelection: GuiObject)
```

---

# GuiObject
**Extends:** GuiBase2d

## Properties
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
SelectionRect2D: Rect [ReadOnly]
Size: UDim2
SizeConstraint: SizeConstraint
Transparency: float
Visible: bool
ZIndex: int
```

## Functions
```
TweenPosition(endPosition: UDim2, easingDirection: EasingDirection, easingStyle: EasingStyle, time: float, override: bool, callback: Function) → bool
TweenSize(endSize: UDim2, easingDirection: EasingDirection, easingStyle: EasingStyle, time: float, override: bool, callback: Function) → bool
TweenSizeAndPosition(endSize: UDim2, endPosition: UDim2, easingDirection: EasingDirection, easingStyle: EasingStyle, time: float, override: bool, callback: Function) → bool
```

## Events
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

# CanvasGroup
**Extends:** GuiObject

## Properties
```
GroupColor3: Color3
GroupTransparency: float
ResolutionScale: float
```

---

# Frame
**Extends:** GuiObject

## Properties
```
Style: FrameStyle
```

---

# GuiButton
**Extends:** GuiObject

## Properties
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

## Events
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

# ImageButton
**Extends:** GuiButton

## Properties
```
ContentImageSize: Vector2 [ReadOnly]
HoverImage: ContentId
HoverImageContent: Content
Image: ContentId
ImageColor3: Color3
ImageContent: Content
ImageRectOffset: Vector2
ImageRectSize: Vector2
ImageTransparency: float
IsLoaded: bool [ReadOnly]
PressedImage: ContentId
PressedImageContent: Content
ResampleMode: ResamplerMode
ScaleType: ScaleType
SliceCenter: Rect
SliceScale: float
TileSize: UDim2
```

## Functions
```
SetEnableContentImageSizeChangedEvents(enabled: bool) → null
```

---

# TextButton
**Extends:** GuiButton

## Properties
```
Confidential: bool
ContentText: string [ReadOnly]
Font: Font
FontFace: Font
FontSize: FontSize [Deprecated]
LineHeight: float
LocalizationMatchIdentifier: string
LocalizationMatchedSourceText: string
LocalizedText: string [ReadOnly]
MaxVisibleGraphemes: int
OpenTypeFeatures: string
OpenTypeFeaturesError: string [ReadOnly]
RichText: bool
Text: string
TextBounds: Vector2 [ReadOnly]
TextColor: BrickColor [Deprecated]
TextColor3: Color3
TextDirection: TextDirection
TextFits: bool [ReadOnly]
TextScaled: bool
TextSize: float
TextStrokeColor3: Color3
TextStrokeTransparency: float
TextTransparency: float
TextTruncate: TextTruncate
TextWrap: bool [Deprecated]
TextWrapped: bool
TextXAlignment: TextXAlignment
TextYAlignment: TextYAlignment
```

## Functions
```
SetTextFromInput(text: string) → null
```

---

# GuiLabel
**Extends:** GuiObject

---

# ImageLabel
**Extends:** GuiLabel

## Properties
```
ContentImageSize: Vector2 [ReadOnly]
Image: ContentId
ImageColor3: Color3
ImageContent: Content
ImageRectOffset: Vector2
ImageRectSize: Vector2
ImageTransparency: float
IsLoaded: bool [ReadOnly]
ResampleMode: ResamplerMode
ScaleType: ScaleType
SliceCenter: Rect
SliceScale: float
TileSize: UDim2
```

## Functions
```
SetEnableContentImageSizeChangedEvents(enabled: bool) → null
```

---

# TextLabel
**Extends:** GuiLabel

## Properties
```
Confidential: bool
ContentText: string [ReadOnly]
Font: Font
FontFace: Font
FontSize: FontSize [Deprecated]
LineHeight: float
LocalizationMatchIdentifier: string
LocalizationMatchedSourceText: string
LocalizedText: string [ReadOnly]
MaxVisibleGraphemes: int
OpenTypeFeatures: string
OpenTypeFeaturesError: string [ReadOnly]
RichText: bool
Text: string
TextBounds: Vector2 [ReadOnly]
TextColor: BrickColor [Deprecated]
TextColor3: Color3
TextDirection: TextDirection
TextFits: bool [ReadOnly]
TextScaled: bool
TextSize: float
TextStrokeColor3: Color3
TextStrokeTransparency: float
TextTransparency: float
TextTruncate: TextTruncate
TextWrap: bool [Deprecated]
TextWrapped: bool
TextXAlignment: TextXAlignment
TextYAlignment: TextYAlignment
```

## Functions
```
SetTextFromInput(text: string) → null
```

---

# RelativeGui
**Extends:** GuiObject

---

# ScrollingFrame
**Extends:** GuiObject

## Properties
```
AbsoluteCanvasSize: Vector2 [ReadOnly]
AbsoluteWindowSize: Vector2 [ReadOnly]
AutomaticCanvasSize: AutomaticSize
BottomImage: ContentId
BottomImageContent: Content
CanvasPosition: Vector2
CanvasSize: UDim2
DraggingScrollBar: DraggingScrollBar [ReadOnly]
ElasticBehavior: ElasticBehavior
HorizontalBarRect: Rect [ReadOnly]
HorizontalScrollBarInset: ScrollBarInset
MaxCanvasPosition: Vector2 [ReadOnly]
MidImage: ContentId
MidImageContent: Content
ScrollBarImageColor3: Color3
ScrollBarImageTransparency: float
ScrollBarThickness: int
ScrollRate: float
ScrollVelocity: Vector2
ScrollingDirection: ScrollingDirection
ScrollingEnabled: bool
SmoothScroll: bool
TopImage: ContentId
TopImageContent: Content
VerticalBarRect: Rect [ReadOnly]
VerticalScrollBarInset: ScrollBarInset
VerticalScrollBarPosition: VerticalScrollBarPosition
```

## Functions
```
ClearInertialScrolling() → null
GetSampledInertialVelocity() → Vector2
ScrollToTop() → null
```

---

# TextBox
**Extends:** GuiObject

## Properties
```
ClearTextOnFocus: bool
Confidential: bool
ContentText: string [ReadOnly]
CursorPosition: int
Font: Font
FontFace: Font
FontSize: FontSize [Deprecated]
LineHeight: float
LocalizationMatchIdentifier: string
LocalizationMatchedSourceText: string
LocalizedPlaceholderText: string [ReadOnly]
ManualFocusRelease: bool
MaxVisibleGraphemes: int
MultiLine: bool
OpenTypeFeatures: string
OpenTypeFeaturesError: string [ReadOnly]
OverlayNativeInput: bool
PlaceholderColor3: Color3
PlaceholderText: string
ReturnKeyType: ReturnKeyType
RichText: bool
SelectionStart: int
ShouldEmitReturnEvents: bool
ShouldEmitTabEvents: bool
ShouldEmitUpAndDownArrowEvents: bool
ShowNativeInput: bool
Text: string
TextBounds: Vector2 [ReadOnly]
TextColor: BrickColor [Deprecated]
TextColor3: Color3
TextDirection: TextDirection
TextEditable: bool
TextFits: bool [ReadOnly]
TextInputType: TextInputType
TextScaled: bool
TextSize: float
TextStrokeColor3: Color3
TextStrokeTransparency: float
TextTransparency: float
TextTruncate: TextTruncate
TextWrap: bool [Deprecated]
TextWrapped: bool
TextXAlignment: TextXAlignment
TextYAlignment: TextYAlignment
```

## Functions
```
CaptureFocus() → null
IsFocused() → bool
ReleaseFocus(submitted: bool) → null
ResetKeyboardMode() → null
SetTextFromInput(text: string) → null
```

## Events
```
FocusLost(enterPressed: bool, inputThatCausedFocusLoss: InputObject)
Focused()
ReturnPressedFromOnScreenKeyboard()
```

---

# VideoDisplay
**Extends:** GuiObject

## Properties
```
ResampleMode: ResamplerMode
ScaleType: ScaleType
TileSize: UDim2
VideoColor3: Color3
VideoRectOffset: Vector2
VideoRectSize: Vector2
VideoTransparency: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
```

## Events
```
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# VideoFrame
**Extends:** GuiObject

## Properties
```
IsLoaded: bool [ReadOnly]
Looped: bool
Playing: bool
PlayingReplicating: bool
Resolution: Vector2 [ReadOnly]
TimeLength: double [ReadOnly]
TimePosition: double
TimePositionReplicating: double
Video: ContentId
VideoContent: Content
Volume: float
```

## Functions
```
Pause() → null
Play() → null
SetStudioPreview(isPreview: bool) → null
```

## Events
```
DidLoop(video: string)
Ended(video: string)
Loaded(video: string)
Paused(video: string)
Played(video: string)
PlayingUpdatedFromServer(value: bool)
TimePositionUpdatedFromServer(value: double)
```

---

# ViewportFrame
**Extends:** GuiObject

## Properties
```
Ambient: Color3
CameraCFrame: CFrame
CameraFieldOfView: float
CurrentCamera: Camera
ImageColor3: Color3
ImageTransparency: float
IsMirrored: bool
LightColor: Color3
LightDirection: Vector3
```

## Functions
```
CaptureSnapshotAsync() → ContentId
```

---

# LayerCollector
**Extends:** GuiBase2d

## Properties
```
Enabled: bool
ResetOnSpawn: bool
ZIndexBehavior: ZIndexBehavior
```

## Functions
```
GetGuiObjectsAtPosition(x: int, y: int) → Instances
GetLayoutNodeTree() → Dictionary [Deprecated]
```

---

# BillboardGui
**Extends:** LayerCollector

## Properties
```
Active: bool
Adornee: Instance
AlwaysOnTop: bool
Brightness: float
ClipsDescendants: bool
CurrentDistance: float [ReadOnly]
DistanceLowerLimit: float
DistanceStep: float
DistanceUpperLimit: float
ExtentsOffset: Vector3
ExtentsOffsetWorldSpace: Vector3
LightInfluence: float
MaxDistance: float
PlayerToHideFrom: Instance
Size: UDim2
SizeOffset: Vector2
StudsOffset: Vector3
StudsOffsetWorldSpace: Vector3
```

## Functions
```
GetScreenSpaceBounds() → Variant
```

---

# PluginGui
**Extends:** LayerCollector

## Properties
```
Title: string
```

## Functions
```
BindToClose(function: Function) → null
GetRelativeMousePosition() → Vector2
```

## Events
```
InputBegan(input: InputObject, gameProcessedEvent: bool)
InputChanged(input: InputObject, gameProcessedEvent: bool)
InputEnded(input: InputObject, gameProcessedEvent: bool)
MouseEnter()
MouseLeave()
PluginDragDropped(dragData: Dictionary)
PluginDragEntered(dragData: Dictionary)
PluginDragLeft(dragData: Dictionary)
PluginDragMoved(dragData: Dictionary)
WindowFocusReleased()
WindowFocused()
```

---

# DockWidgetPluginGui
**Extends:** PluginGui

## Properties
```
HostWidgetWasRestored: bool [ReadOnly]
```

## Functions
```
RequestRaise() → null
```

---

# QWidgetPluginGui
**Extends:** PluginGui

---

# ScreenGui
**Extends:** LayerCollector

## Properties
```
ClipToDeviceSafeArea: bool
DisplayOrder: int
IgnoreGuiInset: bool
OnTopOfCoreBlur: bool
SafeAreaCompatibility: SafeAreaCompatibility
ScreenInsets: ScreenInsets
```

---

# GuiMain
**Extends:** ScreenGui

---

# SurfaceGuiBase
**Extends:** LayerCollector

## Properties
```
Active: bool
Adornee: Instance
Face: NormalId
```

---

# AdGui
**Extends:** SurfaceGuiBase

## Properties
```
AdShape: AdShape
EnableVideoAds: bool
FallbackImage: ContentId
Status: AdUnitStatus [ReadOnly]
```

## Functions
```
GetSingleReportAdInfo() → Map
HandleLuaUIEvent(eventType: AdUIEventType) → null
forwardStateToLuaUI() → null
```

## Events
```
AdEvent(adEventType: AdEventType)
ReportIsSubscribedToVideoCompletion()
adGuiStateChanged(adUIState: Variant)
```

---

# SurfaceGui
**Extends:** SurfaceGuiBase

## Properties
```
AlwaysOnTop: bool
Brightness: float
CanvasSize: Vector2
ClipsDescendants: bool
HorizontalCurvature: float
LightInfluence: float
MaxDistance: float
PixelsPerStud: float
Shape: SurfaceGuiShape
SizingMode: SurfaceGuiSizingMode
ToolPunchThroughDistance: float
ZOffset: float
```

---

# GuiBase3d
**Extends:** GuiBase

## Properties
```
Color: BrickColor [Deprecated]
Color3: Color3
Transparency: float
Visible: bool
```

---

# FloorWire
**Extends:** GuiBase3d

## Properties
```
CycleOffset: float
From: BasePart
StudsBetweenTextures: float
Texture: ContentId
TextureSize: Vector2
To: BasePart
Velocity: float
WireRadius: float
```

---

# InstanceAdornment
**Extends:** GuiBase3d

## Properties
```
Adornee: Instance
```

---

# SelectionBox
**Extends:** InstanceAdornment

## Properties
```
LineThickness: float
StudioSelectionBox: bool
SurfaceColor: BrickColor [Deprecated]
SurfaceColor3: Color3
SurfaceTransparency: float
```

---

# PVAdornment
**Extends:** GuiBase3d

## Properties
```
Adornee: PVInstance
```

---

# HandleAdornment
**Extends:** PVAdornment

## Properties
```
AdornCullingMode: AdornCullingMode
AlwaysOnTop: bool
CFrame: CFrame
SizeRelativeOffset: Vector3
ZIndex: int
```

## Events
```
MouseButton1Down()
MouseButton1Up()
MouseEnter()
MouseLeave()
```

---

# BoxHandleAdornment
**Extends:** HandleAdornment

## Properties
```
Size: Vector3
```

---

# ConeHandleAdornment
**Extends:** HandleAdornment

## Properties
```
Height: float
Radius: float
```

---

# CylinderHandleAdornment
**Extends:** HandleAdornment

## Properties
```
Angle: float
Height: float
InnerRadius: float
Radius: float
```

---

# ImageHandleAdornment
**Extends:** HandleAdornment

## Properties
```
Image: ContentId
Size: Vector2
```

---

# LineHandleAdornment
**Extends:** HandleAdornment

## Properties
```
Length: float
Thickness: float
```

---

# SphereHandleAdornment
**Extends:** HandleAdornment

## Properties
```
Radius: float
```

---

# WireframeHandleAdornment
**Extends:** HandleAdornment

## Properties
```
Scale: Vector3
Thickness: float
```

## Functions
```
AddLine(from: Vector3, to: Vector3) → null
AddLines(points: Array) → null
AddPath(points: Array, loop: bool) → null
AddText(point: Vector3, text: string, size: int) → null
Clear() → null
```

---

# ParabolaAdornment
**Extends:** PVAdornment

## Properties
```
A: float
B: float
C: float
Range: float
Thickness: float
```

## Functions
```
FindPartOnParabola(ignoreDescendentsTable: Instances) → Tuple
```

---

# SelectionSphere
**Extends:** PVAdornment

## Properties
```
SurfaceColor: BrickColor [Deprecated]
SurfaceColor3: Color3
SurfaceTransparency: float
```

---

# PartAdornment
**Extends:** GuiBase3d

## Properties
```
Adornee: BasePart
```

---

# HandlesBase
**Extends:** PartAdornment

---

# ArcHandles
**Extends:** HandlesBase

## Properties
```
Axes: Axes
MouseButton1DownConnectionCount: int
MouseButton1UpConnectionCount: int
MouseDragConnectionCount: int
MouseEnterConnectionCount: int
MouseLeaveConnectionCount: int
```

## Events
```
MouseButton1Down(axis: Axis)
MouseButton1Up(axis: Axis)
MouseDrag(axis: Axis, relativeAngle: float, deltaRadius: float)
MouseEnter(axis: Axis)
MouseLeave(axis: Axis)
```

---

# Handles
**Extends:** HandlesBase

## Properties
```
Faces: Faces
MouseButton1DownConnectionCount: int
MouseButton1UpConnectionCount: int
MouseDragConnectionCount: int
MouseEnterConnectionCount: int
MouseLeaveConnectionCount: int
Style: HandlesStyle
```

## Events
```
MouseButton1Down(face: NormalId)
MouseButton1Up(face: NormalId)
MouseDrag(face: NormalId, distance: float)
MouseEnter(face: NormalId)
MouseLeave(face: NormalId)
```

---

# SurfaceSelection
**Extends:** PartAdornment

## Properties
```
TargetSurface: NormalId
```

---

# SelectionLasso
**Extends:** GuiBase3d

## Properties
```
Humanoid: Humanoid
```

---

# SelectionPartLasso
**Extends:** SelectionLasso

## Properties
```
Part: BasePart
```

---

# SelectionPointLasso
**Extends:** SelectionLasso

## Properties
```
Point: Vector3
```

---

# Path2D
**Extends:** GuiBase

## Properties
```
Closed: bool
Color3: Color3
PropertiesSerialize: BinaryString
SelectedControlPoint: int
SelectedControlPointData: Path2DControlPoint
Thickness: float
Transparency: float
Visible: bool
ZIndex: int
```

## Functions
```
GetBoundingRect() → Rect
GetControlPoint(index: int) → Path2DControlPoint
GetControlPoints() → Array
GetLength() → float
GetMaxControlPoints() → int
GetPositionOnCurve(t: float) → UDim2
GetPositionOnCurveArcLength(t: float) → UDim2
GetSegmentCount() → int
GetTangentOnCurve(t: float) → Vector2
GetTangentOnCurveArcLength(t: float) → Vector2
InsertControlPoint(index: int, point: Path2DControlPoint) → null
RemoveControlPoint(index: int) → null
SetControlPoints(controlPoints: Array) → null
UpdateControlPoint(index: int, point: Path2DControlPoint) → null
```

## Events
```
ControlPointChanged()
```

---

# GuiService
**Extends:** Instance

## Properties
```
AutoSelectGuiEnabled: bool
CoreEffectFolder: Folder
CoreGuiFolder: Folder
CoreGuiNavigationEnabled: bool
GuiNavigationEnabled: bool
IsModalDialog: bool [ReadOnly] [Deprecated]
IsWindows: bool [ReadOnly] [Deprecated]
MenuIsOpen: bool [ReadOnly]
PreferredTextSize: PreferredTextSize [ReadOnly]
PreferredTransparency: float [ReadOnly]
ReducedMotionEnabled: bool [ReadOnly]
SelectedCoreObject: GuiObject
SelectedObject: GuiObject
TopbarInset: Rect [ReadOnly]
TouchControlsEnabled: bool
ViewportDisplaySize: DisplaySize [ReadOnly]
ViewportSizeInMM: Vector2 [ReadOnly]
```

## Functions
```
AddCenterDialog(dialog: Instance, centerDialogType: CenterDialogType, showFunction: Function, hideFunction: Function) → null
AddKey(key: string) → null
AddSelectionParent(selectionName: string, selectionParent: Instance) → null [Deprecated]
AddSelectionTuple(selectionName: string, selections: Tuple) → null [Deprecated]
AddSpecialKey(key: SpecialKey) → null
BroadcastNotification(data: string, notificationType: int) → null
ClearError() → null
CloseInspectMenu() → null
CloseStatsBasedOnInputString(input: string) → bool
DismissNotification(notificationId: string) → bool
ForceTenFootInterface(isForced: bool) → null
GetBrickCount() → int
GetClosestDialogToPosition(position: Vector3) → Instance
GetClosestVisibleDialogToPosition(position: Vector3) → Dialog
GetEmotesMenuOpen() → bool
GetErrorCode() → ConnectionError
GetErrorDetails() → Dictionary
GetErrorMessage() → string [Deprecated]
GetErrorType() → ConnectionError
GetGameplayPausedNotificationEnabled() → bool
GetGuiInset() → Tuple
GetGuiIsVisible(guiType: GuiType) → bool
GetHardwareSafeViewport() → Vector2
GetInspectMenuEnabled() → bool
GetNotificationTypeList() → Dictionary
GetRawScreenScale() → float
GetResolutionScale() → int
GetSafeZoneOffsets() → Dictionary
GetUiMessage() → string
InspectPlayerFromHumanoidDescription(humanoidDescription: Instance, name: string) → null
InspectPlayerFromUserId(userId: int64) → null
InspectPlayerFromUserIdWithCtx(userId: int64, ctx: string) → null
IsMemoryTrackerEnabled() → bool
IsTenFootInterface() → bool
OnNotificationDisplayed(notificationId: string) → null
OnNotificationInteraction(notificationId: string, buttonIndex: int) → null
OpenBrowserWindow(url: string) → null [Deprecated]
OpenNativeOverlay(title: string, url: string) → null [Deprecated]
RemoveCenterDialog(dialog: Instance) → null
RemoveKey(key: string) → null
RemoveSelectionGroup(selectionName: string) → null [Deprecated]
RemoveSpecialKey(key: SpecialKey) → null
Select(selectionParent: Instance) → null
SendNotification(notificationInfo: Dictionary) → string
SendUIOcclusionMetricsForQueryRegion(position: UDim2, size: UDim2, regionName: string) → null
SetEmotesMenuOpen(isOpen: bool) → null
SetGameplayPausedNotificationEnabled(enabled: bool) → null
SetGlobalGuiInset(x1: int, y1: int, x2: int, y2: int) → null
SetHardwareSafeAreaInsets(left: float, top: float, right: float, bottom: float) → null
SetInspectMenuEnabled(enabled: bool) → null
SetMenuIsOpen(open: bool, menuName: string) → null
SetPurchasePromptIsShown(isShown: bool) → null
SetSafeZoneOffsets(top: float, bottom: float, left: float, right: float) → null
SetTopbarInset(topbarInset: Rect) → null
SetUiMessage(msgType: UiMessageType, uiMessage: string) → null
ShowStatsBasedOnInputString(input: string) → bool
ToggleFullscreen() → null
ToggleGuiIsVisibleForCaptures(guiType: GuiType) → null
ToggleGuiIsVisibleIfAllowed(guiType: GuiType) → null
GetScreenResolution() → Vector2
```

## Events
```
BrowserWindowClosed()
CloseInspectMenuRequest()
CoreGuiRenderOverflowed()
EmotesMenuOpenChanged(isOpen: bool)
ErrorMessageChanged(newErrorMessage: string)
GuiVisibilityChangedSignal(guiType: GuiType, visible: bool)
InspectMenuEnabledChangedSignal(enabled: bool)
InspectPlayerFromHumanoidDescriptionRequest(humanoidDescription: Instance, name: string)
InspectPlayerFromUserIdWithCtxRequest(userId: int64, ctx: string)
KeyPressed(key: string, modifiers: string)
MenuClosed()
MenuOpened()
NativeClose()
NetworkPausedEnabledChanged(enabled: bool)
Open9SliceEditor(selectedImageObject: Instance)
OpenStyleEditor(styleBase: Instance)
PurchasePromptShown()
SafeZoneOffsetsChanged()
ShowLeaveConfirmation()
SpecialKeyPressed(key: SpecialKey, modifiers: string)
UiMessageChanged(msgType: UiMessageType, newUiMessage: string)
```

---

# GuidRegistryService
**Extends:** Instance

---

# HandRigDescription
**Extends:** Instance

## Properties
```
Index1: Instance
Index1TposeAdjustment: CFrame
Index2: Instance
Index2TposeAdjustment: CFrame
Index3: Instance
Index3TposeAdjustment: CFrame
IndexRange: Vector3
IndexSize: float
Middle1: Instance
Middle1TposeAdjustment: CFrame
Middle2: Instance
Middle2TposeAdjustment: CFrame
Middle3: Instance
Middle3TposeAdjustment: CFrame
MiddleRange: Vector3
MiddleSize: float
Pinky1: Instance
Pinky1TposeAdjustment: CFrame
Pinky2: Instance
Pinky2TposeAdjustment: CFrame
Pinky3: Instance
Pinky3TposeAdjustment: CFrame
PinkyRange: Vector3
PinkySize: float
Ring1: Instance
Ring1TposeAdjustment: CFrame
Ring2: Instance
Ring2TposeAdjustment: CFrame
Ring3: Instance
Ring3TposeAdjustment: CFrame
RingRange: Vector3
RingSize: float
Side: HandRigDescriptionSide
Thumb1: Instance
Thumb1TposeAdjustment: CFrame
Thumb2: Instance
Thumb2TposeAdjustment: CFrame
Thumb3: Instance
Thumb3TposeAdjustment: CFrame
ThumbRange: Vector3
ThumbSize: float
```

## Functions
```
GetFingerControl(fingerIndex: int) → Vector3
GetFingerTip(fingerIndex: int) → Vector3
SetFingerControl(fingerIndex: int, control: Vector3) → null
SetFingerTip(fingerIndex: int, point: Vector3) → null
```

---

# HapticEffect
**Extends:** Instance

## Properties
```
Looped: bool
Position: Vector3
Radius: float
Type: HapticEffectType
Waveform: FloatCurve
```

## Functions
```
Play() → null
SetWaveformKeys(keys: Array) → null
Stop() → null
```

---

# HapticService
**Extends:** Instance

## Functions
```
GetMotor(inputType: UserInputType, vibrationMotor: VibrationMotor) → Tuple
IsMotorSupported(inputType: UserInputType, vibrationMotor: VibrationMotor) → bool
IsVibrationSupported(inputType: UserInputType) → bool
SetMotor(inputType: UserInputType, vibrationMotor: VibrationMotor, vibrationValues: Tuple) → null
```

---

# HarmonyService
**Extends:** Instance

---

# HeapProfilerService
**Extends:** Instance

## Functions
```
ClientRequestDataAsync(player: Player) → string
ServerRequestDataAsync() → string
```

## Events
```
OnNewData(player: Player, jsonString: buffer, id: int, compressedLength: int, uncompressedLength: int)
RequestData(id: int)
```

---

# HeatmapService
**Extends:** Instance

---

# HeightmapImporterService
**Extends:** Instance

## Functions
```
CancelImportHeightmap() → null
IsValidColormap(colormapAssetId: ContentId) → Tuple
IsValidHeightmap(heightmapAssetId: ContentId) → Tuple
SetImportHeightmapPaused(paused: bool) → null
GetHeightmapPreviewAsync(heightmapAssetId: ContentId) → Tuple
ImportHeightmap(region: Region3, heightmapAssetId: ContentId, colormapAssetId: ContentId, defaultMaterial: Material) → null
```

## Events
```
ColormapHasUnknownPixels()
ProgressUpdate(progressRatio: float, operation: string)
```

---

# HiddenSurfaceRemovalAsset
**Extends:** Instance

## Properties
```
HSRData: BinaryString
HSRMeshIdData: BinaryString
```

---

# Highlight
**Extends:** Instance

## Properties
```
Adornee: Instance
DepthMode: HighlightDepthMode
Enabled: bool
FillColor: Color3
FillTransparency: float
LineThickness: int
OutlineColor: Color3
OutlineTransparency: float
ReservedId: ReservedHighlightId
```

---

# Hopper
**Extends:** Instance

---

# HttpRbxApiService
**Extends:** Instance

## Functions
```
GetDocumentationUrl(partialUrl: string) → string
GetAsync(apiUrlPath: string, priority: ThrottlingPriority, httpRequestType: HttpRequestType) → string
GetAsyncFullUrl(apiUrl: string, priority: ThrottlingPriority, httpRequestType: HttpRequestType) → string
PostAsync(apiUrlPath: string, data: string, priority: ThrottlingPriority, content_type: HttpContentType, httpRequestType: HttpRequestType) → string
PostAsyncFullUrl(apiUrl: string, data: string, priority: ThrottlingPriority, content_type: HttpContentType, httpRequestType: HttpRequestType) → string
RequestAsync(requestOptions: Dictionary, priority: ThrottlingPriority, content_type: HttpContentType, httpRequestType: HttpRequestType) → string
RequestLimitedAsync(requestOptions: Dictionary, priority: ThrottlingPriority, content_type: HttpContentType, httpRequestType: HttpRequestType) → string
```

---

# HttpRequest
**Extends:** Instance

## Functions
```
Cancel() → null
Start(callback: Function) → null
```

---

# HttpService
**Extends:** Instance

## Properties
```
HttpEnabled: bool
```

## Functions
```
GenerateGUID(wrapInCurlyBraces: bool) → string
GetHttpEnabled() → bool
GetSecret(key: string) → Secret
GetUserAgent() → string
JSONDecode(input: string) → Variant
JSONEncode(input: Variant) → string
RequestInternal(options: Dictionary) → Instance
SetHttpEnabled(enabled: bool) → null
UrlEncode(input: string) → string
GetAsync(url: Variant, nocache: bool, headers: Variant) → string
PostAsync(url: Variant, data: string, content_type: HttpContentType, compress: bool, headers: Variant) → string
RequestAsync(requestOptions: Dictionary) → Dictionary
```

---

# Humanoid
**Extends:** Instance

## Properties
```
AutoJumpEnabled: bool
AutoRotate: bool
AutomaticScalingEnabled: bool
BreakJointsOnDeath: bool
CameraMaxDistance: float
CameraMinDistance: float
CameraMode: CameraMode
CameraOffset: Vector3
CollisionType: HumanoidCollisionType [Deprecated]
DisplayDistanceType: HumanoidDisplayDistanceType
DisplayName: string
EvaluateStateMachine: bool
FloorMaterial: Material [ReadOnly]
Health: float
HealthDisplayDistance: float
HealthDisplayType: HumanoidHealthDisplayType
Health_XML: float
HipHeight: float
InternalBodyScale: Vector3
InternalDisplayName: string
InternalHeadScale: float
InternalOriginalHipHeight: float
Jump: bool
JumpHeight: float
JumpPower: float
JumpReplicate: bool
LeftLeg: BasePart [Deprecated]
MaxHealth: float
MaxSlopeAngle: float
MoveDirection: Vector3 [ReadOnly]
MoveDirectionInternal: Vector3
NameDisplayDistance: float
NameOcclusion: NameOcclusion
NetworkHumanoidState: HumanoidStateType
OverrideDefaultCollisions: bool
PlatformStand: bool
RequiresNeck: bool
RigType: HumanoidRigType
RightLeg: BasePart [Deprecated]
RootPart: BasePart [ReadOnly]
RotationType: RotationType
SeatPart: BasePart [ReadOnly]
Sit: bool
Strafe: bool
TargetPoint: Vector3
Torso: BasePart [Deprecated]
UseJumpPower: bool
WalkAngleError: float
WalkDirection: Vector3
WalkSpeed: float
WalkToPart: BasePart
WalkToPoint: Vector3
maxHealth: float [Deprecated]
```

## Functions
```
AddAccessory(accessory: Instance) → null
AddCustomStatus(status: string) → bool [Deprecated]
AddStatus(status: Status) → bool [Deprecated]
BuildRigFromAttachments() → null
CacheDefaults() → null
ChangeState(state: HumanoidStateType) → null
ComputeOriginalSizeForPart(part: Instance) → Vector3?
ComputeR15BodyBoundingBox() → void
EquipTool(tool: Instance) → null
GetAccessories() → Array
GetAccessoryHandleScale(instance: Instance, partType: BodyPartR15) → Vector3
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
SetClickToWalkEnabled(enabled: bool) → null
SetStateEnabled(state: HumanoidStateType, enabled: bool) → null
TakeDamage(amount: float) → null
UnequipTools() → null
loadAnimation(animation: Animation) → AnimationTrack [Deprecated]
takeDamage(amount: float) → null [Deprecated]
ApplyAvatarRules(avatarRules: AvatarRules) → null
ApplyDescription(humanoidDescription: HumanoidDescription, assetTypeVerification: AssetTypeVerification) → null
ApplyDescriptionClientServer(humanoidDescription: HumanoidDescription) → null
ApplyDescriptionReset(humanoidDescription: HumanoidDescription, assetTypeVerification: AssetTypeVerification) → null
PlayEmote(emoteName: string) → bool
PlayEmoteAndGetAnimTrackById(emoteId: int64) → Tuple
```

## Events
```
AnimationPlayed(animationTrack: AnimationTrack)
ApplyDescriptionFinished(description: HumanoidDescription)
Climbing(speed: float)
ClusterCompositionFinished()
CustomStatusAdded(status: string)
CustomStatusRemoved(status: string)
Died()
EmoteTriggered(success: bool, animationTrack: AnimationTrack)
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
ServerApplyDescription(status: bool)
ServerBreakJoints()
ServerEquipTool(tool: Tool)
StateChanged(old: HumanoidStateType, new: HumanoidStateType)
StateEnabledChanged(state: HumanoidStateType, isEnabled: bool)
StatusAdded(status: Status)
StatusRemoved(status: Status)
Strafing(active: bool)
Swimming(speed: float)
Touched(touchingPart: BasePart, humanoidPart: BasePart)
```

---

# HumanoidDescription
**Extends:** Instance

## Properties
```
AccessoryBlob: string
BackAccessory: string
BodyTypeScale: float
ClimbAnimation: int64
DepthScale: float
EmotesDataInternal: string
EquippedEmotesDataInternal: string
Face: int64
FaceAccessory: string
FallAnimation: int64
FrontAccessory: string
GraphicTShirt: int64
HairAccessory: string
HatAccessory: string
Head: int64
HeadColor: Color3
HeadScale: float
HeightScale: float
IdleAnimation: int64
JumpAnimation: int64
LeftArm: int64
LeftArmColor: Color3
LeftLeg: int64
LeftLegColor: Color3
MoodAnimation: int64
NeckAccessory: string
NumberEmotesLoaded: int
Pants: int64
ProportionScale: float
ResetIncludesBodyParts: bool
RightArm: int64
RightArmColor: Color3
RightLeg: int64
RightLegColor: Color3
RunAnimation: int64
Shirt: int64
ShouldersAccessory: string
SwimAnimation: int64
Torso: int64
TorsoColor: Color3
WaistAccessory: string
WalkAnimation: int64
WidthScale: float
```

## Functions
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

## Events
```
EmotesChanged(newEmotes: Dictionary)
EquippedEmotesChanged(newEquippedEmotes: Array)
```

---

# HumanoidRigDescription
**Extends:** Instance

## Properties
```
Chest: Instance
ChestRangeMax: Vector3
ChestRangeMin: Vector3
ChestSize: float
ChestTposeAdjustment: CFrame
HeadBase: Instance
HeadBaseRangeMax: Vector3
HeadBaseRangeMin: Vector3
HeadBaseSize: float
HeadBaseTposeAdjustment: CFrame
LeftAnkle: Instance
LeftAnkleRangeMax: Vector3
LeftAnkleRangeMin: Vector3
LeftAnkleSize: float
LeftAnkleTposeAdjustment: CFrame
LeftClavicle: Instance
LeftClavicleRangeMax: Vector3
LeftClavicleRangeMin: Vector3
LeftClavicleSize: float
LeftClavicleTposeAdjustment: CFrame
LeftElbow: Instance
LeftElbowRangeMax: Vector3
LeftElbowRangeMin: Vector3
LeftElbowSize: float
LeftElbowTposeAdjustment: CFrame
LeftHip: Instance
LeftHipRangeMax: Vector3
LeftHipRangeMin: Vector3
LeftHipSize: float
LeftHipTposeAdjustment: CFrame
LeftKnee: Instance
LeftKneeRangeMax: Vector3
LeftKneeRangeMin: Vector3
LeftKneeSize: float
LeftKneeTposeAdjustment: CFrame
LeftShoulder: Instance
LeftShoulderRangeMax: Vector3
LeftShoulderRangeMin: Vector3
LeftShoulderSize: float
LeftShoulderTposeAdjustment: CFrame
LeftToes: Instance
LeftToesRangeMax: Vector3
LeftToesRangeMin: Vector3
LeftToesSize: float
LeftToesTposeAdjustment: CFrame
LeftWrist: Instance
LeftWristRangeMax: Vector3
LeftWristRangeMin: Vector3
LeftWristSize: float
LeftWristTposeAdjustment: CFrame
Neck: Instance
NeckRangeMax: Vector3
NeckRangeMin: Vector3
NeckSize: float
NeckTposeAdjustment: CFrame
Pelvis: Instance
PelvisRangeMax: Vector3
PelvisRangeMin: Vector3
PelvisSize: float
PelvisTposeAdjustment: CFrame
RightAnkle: Instance
RightAnkleRangeMax: Vector3
RightAnkleRangeMin: Vector3
RightAnkleSize: float
RightAnkleTposeAdjustment: CFrame
RightClavicle: Instance
RightClavicleRangeMax: Vector3
RightClavicleRangeMin: Vector3
RightClavicleSize: float
RightClavicleTposeAdjustment: CFrame
RightElbow: Instance
RightElbowRangeMax: Vector3
RightElbowRangeMin: Vector3
RightElbowSize: float
RightElbowTposeAdjustment: CFrame
RightHip: Instance
RightHipRangeMax: Vector3
RightHipRangeMin: Vector3
RightHipSize: float
RightHipTposeAdjustment: CFrame
RightKnee: Instance
RightKneeRangeMax: Vector3
RightKneeRangeMin: Vector3
RightKneeSize: float
RightKneeTposeAdjustment: CFrame
RightShoulder: Instance
RightShoulderRangeMax: Vector3
RightShoulderRangeMin: Vector3
RightShoulderSize: float
RightShoulderTposeAdjustment: CFrame
RightToes: Instance
RightToesRangeMax: Vector3
RightToesRangeMin: Vector3
RightToesSize: float
RightToesTposeAdjustment: CFrame
RightWrist: Instance
RightWristRangeMax: Vector3
RightWristRangeMin: Vector3
RightWristSize: float
RightWristTposeAdjustment: CFrame
Root: Instance
RootRangeMax: Vector3
RootRangeMin: Vector3
RootSize: float
RootTposeAdjustment: CFrame
Waist: Instance
WaistRangeMax: Vector3
WaistRangeMin: Vector3
WaistSize: float
WaistTposeAdjustment: CFrame
```

## Functions
```
Automap(character: Instance) → null
GetJointFromName(name: string) → Instance
GetJointNames() → Array
GetR15JointNames() → Array
GetR6JointNames() → Array
```

---

# IKControl
**Extends:** Instance

## Properties
```
ChainRoot: Instance
Enabled: bool
EndEffector: Instance
EndEffectorOffset: CFrame
Offset: CFrame
Pole: Instance
Priority: int
SmoothTime: float
Target: Instance
Type: IKControlType
Weight: float
```

## Functions
```
GetChainCount() → int
GetChainLength() → float
GetNodeLocalCFrame(index: int) → CFrame
GetNodeWorldCFrame(index: int) → CFrame
GetRawFinalTarget() → CFrame
GetSmoothedFinalTarget() → CFrame
Solve() → null
```

---

# ILegacyStudioBridge
**Extends:** Instance

---

# LegacyStudioBridge
**Extends:** ILegacyStudioBridge

---

# IXPService
**Extends:** Instance

## Functions
```
ClearUserLayers() → null
GetBrowserTrackerLayerLoadingStatus() → IXPLoadingStatus
GetBrowserTrackerLayerVariables(layerName: string) → Dictionary
GetBrowserTrackerStatusForLayer(layerName: string) → IXPLoadingStatus?
GetRegisteredUserLayersToStatus() → Dictionary
GetUserLayerLoadingStatus() → IXPLoadingStatus
GetUserLayerVariables(layerName: string) → Dictionary
GetUserStatusForLayer(layerName: string) → IXPLoadingStatus?
InitializeUserLayers(userId: int64) → null
LogBrowserTrackerLayerExposure(layerName: string) → null
LogFlagLinkedUserLayerExposure(layerName: string) → null
LogUserLayerExposure(layerName: string) → null
RegisterUserLayers(userLayers: Variant) → null
```

## Events
```
OnBrowserTrackerLayerLoadingStatusChanged(status: IXPLoadingStatus)
OnUserLayerLoadingStatusChanged(status: IXPLoadingStatus)
```

---

# ImportSession
**Extends:** Instance

## Functions
```
Cancel() → null
GetFilename() → string
GetStatuses() → Dictionary
Upload() → null
```

## Events
```
UploadComplete(results: Dictionary)
UploadProgress(progressRatio: float)
```

---

# AssetImportSession
**Extends:** ImportSession

## Functions
```
ApplyPreset(preset: Dictionary) → null
CreatePresetFromData(importData: Instance) → Dictionary
GetImportTree() → Instance
GetRigVisualization(importDataInstance: Instance) → Instance
GetUploadStatus() → Dictionary
HasAnimation() → bool
IsAvatar() → bool
IsGltf() → bool
IsR15() → bool
Reset() → null
usesCustomRestPoseLua() → bool
```

---

# IncrementalPatchBuilder
**Extends:** Instance

## Properties
```
AddPathsToBundle: bool
BuildDebouncePeriod: double
HighCompression: bool
SerializePatch: bool
ZstdCompression: bool
```

---

# InputAction
**Extends:** Instance

## Properties
```
BoolState: bool [ReadOnly]
Direction1DState: float [ReadOnly]
Direction2DState: Vector2 [ReadOnly]
Direction3DState: Vector3 [ReadOnly]
Enabled: bool
Type: InputActionType
```

## Functions
```
Fire(state: Variant) → null
GetState() → Variant
```

## Events
```
Pressed()
Released()
StateChanged(value: Variant)
```

---

# InputBinding
**Extends:** Instance

## Properties
```
Backward: KeyCode
Down: KeyCode
Forward: KeyCode
KeyCode: KeyCode
Left: KeyCode
PressedThreshold: float
ReleasedThreshold: float
Right: KeyCode
Scale: float
UIButton: GuiButton
Up: KeyCode
Vector2Scale: Vector2
```

---

# InputContext
**Extends:** Instance

## Properties
```
Enabled: bool
Priority: int
Sink: bool
```

---

# InputObject
**Extends:** Instance

## Properties
```
Delta: Vector3
KeyCode: KeyCode
Position: Vector3
UserInputState: UserInputState
UserInputType: UserInputType
```

## Functions
```
IsModifierKeyDown(modifierKey: ModifierKey) → bool
```

---

# InsertService
**Extends:** Instance

## Properties
```
AllowClientInsertModels: bool
AllowInsertFreeModels: bool [Deprecated]
```

## Functions
```
ApproveAssetId(assetId: int64) → null [Deprecated]
ApproveAssetVersionId(assetVersionId: int64) → null [Deprecated]
GetLocalFileContents(contentId: string) → string
Insert(instance: Instance) → null [Deprecated]
LoadLocalAsset(assetPath: string) → Instance
LoadPackageAsset(url: ContentId) → Instances
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
LoadAssetWithFormat(assetId: int64, format: string) → Instances
LoadPackageAssetAsync(url: ContentId) → Instances
loadAsset(assetId: int64) → Instance [Deprecated]
```

## Events
```
InternalDelete(instance: Instance)
```

---

# InternalSyncItem
**Extends:** Instance

## Properties
```
AutoSync: bool
Enabled: bool
Path: string
Target: Instance
```

---

# InternalSyncService
**Extends:** Instance

---

# JointInstance
**Extends:** Instance

## Properties
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

# DynamicRotate
**Extends:** JointInstance

## Properties
```
BaseAngle: float
```

---

# RotateP
**Extends:** DynamicRotate

---

# RotateV
**Extends:** DynamicRotate

---

# Glue
**Extends:** JointInstance

## Properties
```
F0: Vector3
F1: Vector3
F2: Vector3
F3: Vector3
```

---

# ManualSurfaceJointInstance
**Extends:** JointInstance

---

# ManualGlue
**Extends:** ManualSurfaceJointInstance

---

# ManualWeld
**Extends:** ManualSurfaceJointInstance

---

# Motor
**Extends:** JointInstance

## Properties
```
CurrentAngle: float
DesiredAngle: float
MaxVelocity: float
ReplicateCurrentAngle: float
```

## Functions
```
SetDesiredAngle(value: float) → null
```

---

# Motor6D
**Extends:** Motor

## Properties
```
ChildName: string [ReadOnly]
ParentName: string [ReadOnly]
ReplicateCurrentAngle6D: Vector3
ReplicateCurrentOffset6D: Vector3
Transform: CFrame
```

---

# Rotate
**Extends:** JointInstance

---

# Snap
**Extends:** JointInstance

---

# VelocityMotor
**Extends:** JointInstance

## Properties
```
CurrentAngle: float
DesiredAngle: float
Hole: Hole
MaxVelocity: float
```

---

# Weld
**Extends:** JointInstance

---

# JointsService
**Extends:** Instance

## Functions
```
ClearJoinAfterMoveJoints() → null
CreateJoinAfterMoveJoints() → null
SetJoinAfterMoveInstance(joinInstance: Instance) → null
SetJoinAfterMoveTarget(joinTarget: Instance) → null
ShowPermissibleJoints() → null
```

---

# KeyboardService
**Extends:** Instance

---

# Keyframe
**Extends:** Instance

## Properties
```
Time: float
```

## Functions
```
AddMarker(marker: Instance) → null
AddPose(pose: Instance) → null
GetMarkers() → Instances
GetPoses() → Instances
RemoveMarker(marker: Instance) → null
RemovePose(pose: Instance) → null
```

---

# KeyframeMarker
**Extends:** Instance

## Properties
```
Value: string
```

---

# KeyframeSequenceProvider
**Extends:** Instance

## Functions
```
GetKeyframeSequence(assetId: ContentId) → Instance [Deprecated]
GetKeyframeSequenceById(assetId: int64, useCache: bool) → Instance [Deprecated]
GetMemStats() → Dictionary
RegisterActiveKeyframeSequence(keyframeSequence: Instance) → ContentId
RegisterKeyframeSequence(keyframeSequence: Instance) → ContentId
GetAnimations(userId: int64) → Instance
GetKeyframeSequenceAsync(assetId: ContentId) → Instance
```

---

# LSPFileSyncService
**Extends:** Instance

---

# LanguageService
**Extends:** Instance

## Functions
```
GetCapabilitiesUsedInPackageAsync(instances: Instances) → Dictionary
```

---

# Light
**Extends:** Instance

## Properties
```
Brightness: float
Color: Color3
Enabled: bool
Shadows: bool
```

---

# PointLight
**Extends:** Light

## Properties
```
Range: float
```

---

# SpotLight
**Extends:** Light

## Properties
```
Angle: float
Face: NormalId
Range: float
```

---

# SurfaceLight
**Extends:** Light

## Properties
```
Angle: float
Face: NormalId
Range: float
```

---

# Lighting
**Extends:** Instance

## Properties
```
Ambient: Color3
Brightness: float
ClockTime: float
ColorShift_Bottom: Color3
ColorShift_Top: Color3
EnvironmentDiffuseScale: float
EnvironmentSpecularScale: float
ExposureCompensation: float
ExtendLightRangeTo120: RolloutState
FogColor: Color3
FogEnd: float
FogStart: float
GeographicLatitude: float
GlobalShadows: bool
LightingStyle: LightingStyle
OutdoorAmbient: Color3
Outlines: bool [Deprecated]
PrioritizeLightingQuality: bool
ShadowColor: Color3 [Deprecated]
ShadowSoftness: float
Technology: Technology
TimeOfDay: string
```

## Functions
```
GetMinutesAfterMidnight() → double
GetMoonDirection() → Vector3
GetMoonPhase() → float
GetSunDirection() → Vector3
SetMinutesAfterMidnight(minutes: double) → null
getMinutesAfterMidnight() → double [Deprecated]
setMinutesAfterMidnight(minutes: double) → null [Deprecated]
```

## Events
```
LightingChanged(skyChanged: bool)
```

---

# LinkingService
**Extends:** Instance

## Functions
```
DetectUrl(url: string) → null
GetAndClearLastPendingUrl() → Dictionary
GetLastLuaUrl() → string?
IsUrlRegistered(url: string) → bool
RegisterLuaUrl(url: string) → null
StartLuaUrlDelivery() → Dictionary?
StopLuaUrlDelivery() → null
OpenUrl(url: string) → bool
SupportsSwitchToSettingsApp() → bool
SwitchToSettingsApp(route: string?) → null
```

## Events
```
OnLuaUrl(url: string, matchedUrl: string, attributionUrl: string?)
```

---

# LiveScriptingService
**Extends:** Instance

## Properties
```
ServerLiveEditingMode: ServerLiveEditingMode
```

## Events
```
BeginEdit(id: int64, guid: string)
BroadcastMessage(message: string, type: LiveEditingBroadcastMessageType)
EndEdit(id: int64)
FailedToOpen(id: int64, legalToOpenLocal: bool)
KickFromEdit(id: int64, msg: string)
LiveEditingClientConfiguration(serializedConfig: string)
OpenedWithSource(id: int64, source: string)
SendAtomicOperation(requestId: int, guid: string, op: string, hash: string)
SendAtomicUpdateResponse(guid: int, response: LiveEditingAtomicUpdateResponse)
SendOperation(id: int64, op: string)
```

---

# LiveSyncService
**Extends:** Instance

## Properties
```
HasSyncedInstances: bool [ReadOnly]
```

## Functions
```
GetSyncState(instance: Instance) → Tuple
```

## Events
```
SyncStatusChanged(instance: Instance)
```

---

# LocalStorageService
**Extends:** Instance

## Functions
```
Flush() → null
GetItem(key: string) → string
SetItem(key: string, value: string) → null
WhenLoaded(callback: Function) → null
```

## Events
```
ItemWasSet(key: string, value: string)
StoreWasCleared()
```

---

# AppStorageService
**Extends:** LocalStorageService

---

# UserStorageService
**Extends:** LocalStorageService

---

# LocalizationService
**Extends:** Instance

## Properties
```
ForcePlayModeGameLocaleId: string
ForcePlayModeRobloxLocaleId: string
GameSourceLanguageId: string
IsTextScraperRunning: bool
LocaleManifest: string
RobloxForcePlayModeGameLocaleId: string
RobloxForcePlayModeRobloxLocaleId: string
RobloxLocaleId: string [ReadOnly]
ShouldUseCloudTable: bool
SystemLocaleId: string [ReadOnly]
```

## Functions
```
GetCorescriptLocalizations() → Instances
GetTableEntries(instance: Instance) → Array
GetTranslatorForPlayer(player: Instance) → Instance
SetRobloxLocaleId(locale: string) → null
StartTextScraper() → null
StopTextScraper() → null
GetCountryRegionForPlayerAsync(player: Instance) → string
GetTranslatorForLocaleAsync(locale: string) → Instance
GetTranslatorForPlayerAsync(player: Instance) → Instance
PromptDownloadGameTableToCSV(table: Instance) → null
PromptExportToCSVs() → null
PromptImportFromCSVs() → null
PromptUploadCSVToGameTable() → Instance
```

## Events
```
AutoTranslateWillRun()
DynamicTranslationServerToClientResponse(entries: Tuple)
TextScraperClientMessageWithPlayerSignal(version: int, player: Instance, message: Tuple)
```

---

# LocalizationTable
**Extends:** Instance

## Properties
```
Contents: string
DevelopmentLanguage: string [Deprecated]
IsExemptFromUGCAnalytics: bool
Root: Instance [Deprecated]
SourceLocaleId: string
```

## Functions
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
SetIsExemptFromUGCAnalytics(value: bool) → null
```

---

# CloudLocalizationTable
**Extends:** LocalizationTable

---

# LodDataEntity
**Extends:** Instance

## Properties
```
EntityData: SharedString
EntityLodEnabled: bool
EntityPosition: CFrame
EntityScale: Vector3
EntitySource: Instance
```

---

# LodDataService
**Extends:** Instance

---

# LogReporterService
**Extends:** Instance

## Functions
```
ReportLog(fingerprint: string, uuid: string, desc: string, attributes: Dictionary, annotations: Dictionary) → bool
ReportMultipleLogs(fingerprint: string, uuid: string, desc: string, attributes: Dictionary, annotations: Dictionary, numLogs: int) → bool
```

---

# LogService
**Extends:** Instance

## Functions
```
ClearOutput() → null
ExecuteScript(source: string) → null
GetHttpResultHistory() → Array
GetLogHistory() → Array
RequestHttpResultApproved() → null
RequestServerHttpResult() → null
RequestServerOutput() → null
```

## Events
```
HttpResultOut(httpResult: Dictionary)
MessageOut(message: string, messageType: MessageType)
OnHttpResultApproved(isApproved: bool)
RequestHttpResultApprovedSignal(requestingPlayer: Instance)
RequestScriptExecutionSignal(requestingPlayer: Instance, source: string)
RequestServerHttpResultSignal(requestingPlayer: Instance)
RequestServerOutputSignal(requestingPlayer: Instance)
RequestSettingsChange(requestingPlayer: Instance, expressivePrinting: bool)
ServerHttpResultOut(httpResult: Dictionary)
ServerMessageOut(message: string, messageType: MessageType, timestamp: double)
ServerVariantMessageOut(data: Dictionary)
```

---

# LoginService
**Extends:** Instance

## Functions
```
Logout() → null
PromptLogin() → null
```

## Events
```
LoginFailed(loginError: string)
LoginSucceeded(username: string)
```

---

# LuaSettings
**Extends:** Instance

---

# LuaSourceContainer
**Extends:** Instance

## Properties
```
CachedRemoteSource: ProtectedString
CachedRemoteSourceLoadState: int
HasAssociatedDrafts: bool
IsDifferentFromFileSystem: bool
SandboxedSource: ProtectedString
ScriptGuid: string
isPlayerScript: bool
```

---

# AuroraScript
**Extends:** LuaSourceContainer

## Properties
```
AuroraScriptBindingsSerialize: BinaryString
EnableCulling: bool
EnableLOD: bool
LODCriticality: int
Priority: int
Source: ProtectedString
```

## Functions
```
AddTo(instance: Instance) → null
IsOnInstance(instance: Instance) → bool
RemoveFrom(instance: Instance) → null
SignalFired(instance: Instance, topic: string) → RBXScriptSignal
```

## Events
```
SynchronizeState(frameId: int, instance: Instance, state: Dictionary, ingressHeaders: string, ingressArgs: Array, egressHeaders: string, egressArgs: Array, lodLevel: int, priorInvocationFrame: int)
```

---

# BaseScript
**Extends:** LuaSourceContainer

## Properties
```
Disabled: bool
Enabled: bool
LinkedSource: ContentId [Deprecated]
RunContext: RunContext
```

---

# CoreScript
**Extends:** BaseScript

---

# Script
**Extends:** BaseScript

## Properties
```
Source: ProtectedString
```

## Functions
```
GetHash() → string
```

---

# LocalScript
**Extends:** Script

---

# ModuleScript
**Extends:** LuaSourceContainer

## Properties
```
Confidential: bool
LinkedSource: ContentId [Deprecated]
Source: ProtectedString
```

---

# LuaWebService
**Extends:** Instance

---

# LuauScriptAnalyzerService
**Extends:** Instance

---

# MLModelDeliveryService
**Extends:** Instance

---

# MLService
**Extends:** Instance

## Functions
```
CreateSessionAsync(assetId: string) → MLSession
```

---

# MarkerCurve
**Extends:** Instance

## Properties
```
Length: int [ReadOnly]
ValuesAndTimes: BinaryString
```

## Functions
```
GetMarkerAtIndex(index: int) → Dictionary
GetMarkers() → Array
InsertMarkerAtTime(time: float, marker: string) → Array
RemoveMarkerAtIndex(startingIndex: int, count: int) → int
```

---

# MarketplaceService
**Extends:** Instance

## Functions
```
PlayerCanMakePurchases(player: Instance) → bool
PrepareCollectiblesPurchase(player: Instance, assetId: int64, collectibleItemId: string, collectibleItemInstanceId: string, collectibleProductId: string, expectedPrice: int) → null
PromptBulkPurchase(player: Player, lineItems: Array, options: Dictionary) → null
PromptBundlePurchase(player: Instance, bundleId: int64) → null
PromptCancelSubscription(user: Player, subscriptionId: string) → null
PromptCollectiblesPurchase(player: Instance, assetId: int64, collectibleItemId: string, collectibleItemInstanceId: string, collectibleProductId: string, expectedPrice: int) → null
PromptGamePassPurchase(player: Instance, gamePassId: int64) → null
PromptNativePurchase(player: Instance, productId: string) → null
PromptNativePurchaseWithLocalPlayer(productId: string) → null
PromptPremiumPurchase(player: Instance) → null
PromptProductPurchase(player: Instance, productId: int64, equipIfPurchased: bool, currencyType: CurrencyType) → null
PromptPurchase(player: Instance, assetId: int64, equipIfPurchased: bool, currencyType: CurrencyType) → null
PromptRobloxPurchase(assetId: int64, equipIfPurchased: bool) → null
PromptSubscriptionPurchase(user: Player, subscriptionId: string) → null
PromptThirdPartyPurchase(player: Instance, productId: string) → null
ReportAssetSale(assetId: string, robuxAmount: int) → null
ReportRobuxUpsellStarted() → null
SignalAssetTypePurchased(player: Instance, assetType: AssetType) → null
SignalClientPurchaseSuccess(ticket: string, playerId: int64, productId: int64) → null
SignalMockPurchasePremium() → null
SignalPromptBulkPurchaseFinished(status: MarketplaceBulkPurchasePromptStatus, results: Dictionary) → null
SignalPromptBundlePurchaseFinished(player: Instance, bundleId: int64, success: bool) → null
SignalPromptGamePassPurchaseFinished(player: Instance, gamePassId: int64, success: bool) → null
SignalPromptPremiumPurchaseFinished(didTryPurchasing: bool) → null
SignalPromptProductPurchaseFinished(userId: int64, productId: int64, success: bool) → null
SignalPromptPurchaseFinished(player: Instance, assetId: int64, success: bool) → null
SignalPromptSubscriptionPurchaseFinished(subscriptionId: string, didTryPurchasing: bool) → null
SignalServerLuaDialogClosed(value: bool) → null
SignalUserSubscriptionStatusChanged(subscriptionId: string) → null
GetDeveloperProductsAsync() → Instance
GetDeveloperProductsForExperienceDetailsPageAsync() → Instance
GetProductInfo(assetId: int64, infoType: InfoType) → Dictionary
GetRobuxBalance() → int
GetSubscriptionProductInfoAsync(subscriptionId: string) → Dictionary
GetSubscriptionPurchaseInfoAsync(subscriptionId: string) → Dictionary
GetUserSubscriptionDetailsAsync(user: Player, subscriptionId: string) → Dictionary
GetUserSubscriptionDetailsInternalAsync(subscriptionId: string) → Dictionary
GetUserSubscriptionPaymentHistoryAsync(user: Player, subscriptionId: string) → Array
GetUserSubscriptionStatusAsync(user: Player, subscriptionId: string) → Dictionary
GetUsersPriceLevelsAsync(userIds: Array) → Array
PerformBulkPurchase(orderRequest: Dictionary, options: Dictionary) → Dictionary
PerformCancelSubscription(subscriptionId: string) → null
PerformPurchase(infoType: InfoType, productId: int64, expectedPrice: int, requestId: string, isRobloxPurchase: bool, collectibleItemId: string, collectibleProductId: string, idempotencyKey: string, purchaseAuthToken: string) → Dictionary
PerformPurchaseV2(infoType: InfoType, productId: int64, expectedPrice: int, requestId: string, isRobloxPurchase: bool, collectiblesProductDetails: Dictionary) → Dictionary
PerformSubscriptionPurchase(subscriptionId: string) → string
PerformSubscriptionPurchaseV2(subscriptionId: string, paymentProvider: string) → null
PlayerOwnsAsset(player: Instance, assetId: int64) → bool
PlayerOwnsBundle(player: Player, bundleId: int64) → bool
UserOwnsGamePassAsync(userId: int64, gamePassId: int64) → bool
```

## Events
```
AssetTypePurchased(player: Instance, assetType: AssetType)
ClientLuaDialogRequested(arguments: Tuple)
ClientPurchaseSuccess(ticket: string, playerId: int64, productId: int64)
ConfirmPlayerMembership()
ConfirmUserSubscriptionPurchase(subscriptionId: string)
LuaDialogCallbackSignal(value: bool, player: Instance)
MockConfirmUserSubscriptionPurchase(userId: int64, subscriptionId: string)
MockPurchasePremium()
NativePurchaseFinished(player: Instance, productId: string, wasPurchased: bool)
NativePurchaseFinishedWithLocalPlayer(productId: string, wasPurchased: bool)
PrepareCollectiblesPurchaseRequested(player: Instance, assetId: int64, collectibleItemId: string, collectibleItemInstanceId: string, collectibleProductId: string, expectedPrice: int)
PromptBulkPurchaseFinished(player: Instance, status: MarketplaceBulkPurchasePromptStatus, results: Dictionary)
PromptBulkPurchaseRequested(player: Instance, displayData: Array, orderRequest: Dictionary, purchaserRobuxBalance: int64, orderTotalRobux: int64, options: Dictionary)
PromptBundlePurchaseFinished(player: Instance, bundleId: int64, wasPurchased: bool)
PromptBundlePurchaseRequested(player: Instance, bundleId: int64)
PromptCancelSubscriptionRequested(subscriptionId: string)
PromptCollectibleBundlePurchaseRequested(player: Instance, bundleId: int64, collectibleItemId: string, collectibleItemInstanceId: string, collectibleProductId: string, expectedPrice: int, idempotencyKey: string, purchaseAuthToken: string)
PromptCollectiblesPurchaseRequested(player: Instance, assetId: int64, collectibleItemId: string, collectibleItemInstanceId: string, collectibleProductId: string, expectedPrice: int, idempotencyKey: string, purchaseAuthToken: string)
PromptGamePassPurchaseFinished(player: Instance, gamePassId: int64, wasPurchased: bool)
PromptGamePassPurchaseRequested(player: Instance, gamePassId: int64)
PromptNativePurchaseRequested(player: Instance, productId: string)
PromptNativePurchaseRequestedWithLocalPlayer(userId: int64, productId: string)
PromptPremiumPurchaseFinished()
PromptPremiumPurchaseRequested(player: Instance)
PromptProductPurchaseFinished(userId: int64, productId: int64, isPurchased: bool)
PromptProductPurchaseRequested(player: Instance, productId: int64, equipIfPurchased: bool, currencyType: CurrencyType)
PromptPurchaseFinished(player: Instance, assetId: int64, isPurchased: bool)
PromptPurchaseRequested(player: Instance, assetId: int64, equipIfPurchased: bool, currencyType: CurrencyType)
PromptPurchaseRequestedV2(player: Instance, assetId: int64, equipIfPurchased: bool, currencyType: CurrencyType, idempotencyKey: string, purchaseAuthToken: string)
PromptRobloxPurchaseRequested(assetId: int64, equipIfPurchased: bool)
PromptSubscriptionPurchaseFinished(user: Player, subscriptionId: string, didTryPurchasing: bool)
PromptSubscriptionPurchaseRequested(subscriptionId: string)
PromptThirdPartyPurchaseRequested(player: Instance, productId: string)
ServerPurchaseVerification(serverResponseTable: Dictionary)
ThirdPartyPurchaseFinished(player: Instance, productId: string, receipt: string, wasPurchased: bool)
UserSubscriptionStatusChanged(subscriptionId: string)
```

---

# MatchmakingService
**Extends:** Instance

## Functions
```
GetServerAttribute(name: string) → Tuple
InitializeServerAttributesForStudio(serverAttributes: Dictionary) → Tuple
SetServerAttribute(name: string, value: Variant) → Tuple
```

---

# MaterialGenerationService
**Extends:** Instance

## Functions
```
GenerateMaterialVariantsAsync(prompt: string, samples: int64) → Dictionary
```

---

# MaterialService
**Extends:** Instance

## Properties
```
AsphaltName: string
BasaltName: string
BrickName: string
CardboardName: string
CarpetName: string
CeramicTilesName: string
ClayRoofTilesName: string
CobblestoneName: string
ConcreteName: string
CorrodedMetalName: string
CrackedLavaName: string
DiamondPlateName: string
FabricName: string
FoilName: string
GlacierName: string
GraniteName: string
GrassName: string
GroundName: string
IceName: string
LeafyGrassName: string
LeatherName: string
LimestoneName: string
MarbleName: string
MetalName: string
MudName: string
PavementName: string
PebbleName: string
PlasterName: string
PlasticName: string
RockName: string
RoofShinglesName: string
RubberName: string
SaltName: string
SandName: string
SandstoneName: string
SlateName: string
SmoothPlasticName: string
SnowName: string
Use2022Materials: bool
Use2022MaterialsXml: bool
WoodName: string
WoodPlanksName: string
```

## Functions
```
GetBaseMaterialOverride(material: Material) → string
GetIsMaterialActionAsToolEnabled() → bool
GetMaterialOverrideChanged(material: Material) → RBXScriptSignal
GetMaterialVariant(material: Material, name: string) → MaterialVariant
GetOverrideStatus(material: Material) → PropertyStatus
SetBaseMaterialOverride(material: Material, name: string) → null
SetCurrentMaterial(baseMaterial: Material, materialVariant: string) → null
ToggleMaterialFillToolEnabled() → null
```

## Events
```
MaterialFillToolEnabledChanged(shouldEnable: bool)
OverrideStatusChanged(material: Material)
```

---

# MaterialVariant
**Extends:** Instance

## Properties
```
AvgMetalness: int
AvgRoughness: int
BaseMaterial: Material
ColorMap: ContentId
ColorMapContent: Content
CustomPhysicalProperties: PhysicalProperties
MaterialPattern: MaterialPattern
MetalnessMap: ContentId
MetalnessMapContent: Content
NormalMap: ContentId
NormalMapContent: Content
RoughnessMap: ContentId
RoughnessMapContent: Content
StudsPerTile: float
TexturePack: ContentId
```

---

# MemStorageConnection
**Extends:** Instance

## Functions
```
Disconnect() → null
```

---

# MemStorageService
**Extends:** Instance

## Functions
```
Bind(key: string, callback: Function) → MemStorageConnection
BindAndFire(key: string, callback: Function) → MemStorageConnection
Call(key: string, input: Variant) → Variant
Fire(key: string, value: string) → null
GetItem(key: string, defaultValue: string) → string
HasItem(key: string) → bool
RemoveItem(key: string) → bool
SetItem(key: string, value: string) → null
```

---

# MemoryStoreHashMap
**Extends:** Instance

## Functions
```
GetAsync(key: string) → Variant
ListItemsAsync(count: int) → MemoryStoreHashMapPages
RemoveAsync(key: string) → null
SetAsync(key: string, value: Variant, expiration: int64) → bool
UpdateAsync(key: string, transformFunction: Function, expiration: int64) → Variant
```

---

# MemoryStoreQueue
**Extends:** Instance

## Functions
```
AddAsync(value: Variant, expiration: int64, priority: double) → null
GetSizeAsync(excludeInvisible: bool) → int
ReadAsync(count: int, allOrNothing: bool, waitTimeout: double) → Tuple
RemoveAsync(id: string) → null
```

---

# MemoryStoreService
**Extends:** Instance

## Functions
```
GetHashMap(name: string) → MemoryStoreHashMap
GetQueue(name: string, invisibilityTimeout: int) → MemoryStoreQueue
GetSortedMap(name: string) → MemoryStoreSortedMap
```

---

# MemoryStoreSortedMap
**Extends:** Instance

## Functions
```
GetAsync(key: string) → Tuple
GetRangeAsync(direction: SortDirection, count: int, exclusiveLowerBound: Variant, exclusiveUpperBound: Variant) → Array
GetSizeAsync() → int
RemoveAsync(key: string) → null
SetAsync(key: string, value: Variant, expiration: int64, sortKey: Variant) → bool
UpdateAsync(key: string, transformFunction: Function, expiration: int64) → Tuple
```

---

# Message
**Extends:** Instance

## Properties
```
Text: string
```

---

# Hint
**Extends:** Message

---

# MessageBusConnection
**Extends:** Instance

## Functions
```
Disconnect() → null
```

---

# MessageBusService
**Extends:** Instance

## Functions
```
Call(key: string, input: Variant) → Variant
GetLast(mid: string) → Variant
GetMessageId(domainName: string, messageName: string) → string
GetProtocolMethodRequestMessageId(protocolName: string, methodName: string) → string
GetProtocolMethodResponseMessageId(protocolName: string, methodName: string) → string
MakeRequest(protocolName: string, methodName: string, message: Variant, callback: Function, customTelemetryData: Variant) → null
Publish(mid: string, params: Variant) → null
PublishProtocolMethodRequest(protocolName: string, methodName: string, message: Variant, customTelemetryData: Variant) → null
PublishProtocolMethodResponse(protocolName: string, methodName: string, message: Variant, responseCode: int, customTelemetryData: Variant) → null
SetRequestHandler(protocolName: string, methodName: string, callback: Function) → null
Subscribe(mid: string, callback: Function, once: bool, sticky: bool) → Instance
SubscribeToProtocolMethodRequest(protocolName: string, methodName: string, callback: Function, once: bool, sticky: bool) → Instance
SubscribeToProtocolMethodResponse(protocolName: string, methodName: string, callback: Function, once: bool, sticky: bool) → Instance
```

---

# MessagingService
**Extends:** Instance

## Functions
```
PublishAsync(topic: string, message: Variant) → null
SubscribeAsync(topic: string, callback: Function) → RBXScriptConnection
```

---

# MetaBreakpoint
**Extends:** Instance

## Properties
```
Condition: string
ContinueExecution: bool
Enabled: bool
Id: int [ReadOnly]
IsLogpoint: bool [ReadOnly]
Line: int
LogMessage: string
RemoveOnHit: bool
Script: string
Valid: bool [ReadOnly]
```

## Functions
```
GetContextBreakpoints() → Dictionary
Remove(status: Function) → int
SetChildBreakpointEnabledByScriptAndContext(script: string, contextGST: int, enabled: bool) → null
SetContextEnabled(context: int, enabled: bool) → null
SetContinueExecution(enabled: bool) → null
SetEnabled(enabled: bool) → null
SetLine(line: int, status: Function) → int
SetRemoveOnHit(enabled: bool) → null
```

---

# MetaBreakpointContext
**Extends:** Instance

## Properties
```
ContextDataInternal: string
```

---

# MetaBreakpointManager
**Extends:** Instance

## Functions
```
AddBreakpoint(script: Instance, line: int, condition: Instance) → Instance
GetBreakpointById(metaBreakpointId: int) → MetaBreakpoint
RemoveBreakpointById(metaBreakpointId: int) → null
```

## Events
```
MetaBreakpointAdded(breakpoint: MetaBreakpoint)
MetaBreakpointChanged(breakpoint: MetaBreakpoint)
MetaBreakpointRemoved(breakpoint: MetaBreakpoint)
MetaBreakpointSetChanged(breakpoint: MetaBreakpoint, detail: Dictionary)
```

---

# MicroProfilerService
**Extends:** Instance

---

# ModerationService
**Extends:** Instance

## Functions
```
InternalCreateReviewableContentAsync(config: Dictionary) → string
InternalRequestReviewableContentReviewAsync(config: Dictionary) → null
```

---

# Mouse
**Extends:** Instance

## Properties
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

## Events
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

# PlayerMouse
**Extends:** Mouse

---

# PluginMouse
**Extends:** Mouse

## Events
```
DragEnter(instances: Instances)
```

---

# MouseService
**Extends:** Instance

## Events
```
MouseEnterStudioViewport()
MouseLeaveStudioViewport()
```

---

# MultipleDocumentInterfaceInstance
**Extends:** Instance

## Properties
```
FocusedDataModelSession: DataModelSession [ReadOnly]
```

## Events
```
DataModelSessionEnded(dataModelSession: Instance)
DataModelSessionStarted(dataModelSession: Instance)
```

---

# NetworkMarker
**Extends:** Instance

## Events
```
Received()
```

---

# NetworkPeer
**Extends:** Instance

## Functions
```
SetOutgoingKBPSLimit(limit: int) → null
```

---

# NetworkClient
**Extends:** NetworkPeer

## Events
```
ConnectionAccepted(peer: string, replicator: Instance)
ConnectionFailed(peer: string, code: int, reason: string)
```

---

# NetworkServer
**Extends:** NetworkPeer

## Functions
```
EncryptStringForPlayerId(toEncrypt: string, playerId: int64) → string
```

---

# NetworkReplicator
**Extends:** Instance

## Functions
```
GetPlayer() → Instance
```

---

# ClientReplicator
**Extends:** NetworkReplicator

## Functions
```
RequestRCCProfilerData(frameRate: int, timeFrame: int) → null
RequestServerLuauHeapData() → null
RequestServerScriptProfiling(start: bool, frequency: int?) → null
RequestServerScriptProfilingData() → null
RequestServerStats(request: bool) → null
```

## Events
```
RCCProfilerDataComplete(success: bool, message: string)
StatsReceived(stats: Dictionary)
```

---

# ServerReplicator
**Extends:** NetworkReplicator

---

# NetworkSettings
**Extends:** Instance

## Properties
```
EmulatedTotalMemoryInMB: int
FreeMemoryMBytes: float [ReadOnly]
HttpProxyEnabled: bool
HttpProxyURL: string
IncomingReplicationLag: double
OpenCertManagerDialog: int
PrintJoinSizeBreakdown: bool
PrintPhysicsErrors: bool
PrintStreamInstanceQuota: bool
RandomizeJoinInstanceOrder: bool
RenderStreamedRegions: bool
ShowActiveAnimationAsset: bool
```

---

# NoCollisionConstraint
**Extends:** Instance

## Properties
```
Enabled: bool
Part0: BasePart
Part1: BasePart
```

---

# Noise
**Extends:** Instance

## Properties
```
NoiseType: NoiseType
Seed: int
```

## Functions
```
SampleDirectional(position: Vector3, direction: Vector3) → float
SampleUniform(position: Vector3) → float
```

---

# NotificationService
**Extends:** Instance

## Properties
```
IsConnected: bool [ReadOnly]
IsLuaChatEnabled: bool [ReadOnly]
IsLuaGameDetailsEnabled: bool [ReadOnly]
SelectedTheme: string
```

## Functions
```
ActionEnabled(actionType: AppShellActionType) → null
ActionTaken(actionType: AppShellActionType) → null
CancelAllNotification(userId: int64) → null
CancelNotification(userId: int64, alertId: int) → null
ScheduleNotification(userId: int64, alertId: int, alertMsg: string, minutesToFire: int) → null
SwitchedToAppShellFeature(appShellFeature: AppShellFeature) → null
GetScheduledNotifications(userId: int64) → Array
```

## Events
```
Roblox17sConnectionChanged(connectionName: string, connectionState: ConnectionState, namespaceSequenceNumbers: string)
Roblox17sEventReceived(eventData: Map)
RobloxConnectionChanged(connectionName: string, connectionState: ConnectionState, sequenceNumber: string, namespaceSequenceNumbers: string)
RobloxEventReceived(eventData: Map)
```

---

# OmniRecommendationsService
**Extends:** Instance

## Functions
```
ClearSessionId() → null
GetSessionId() → string
MakeRequest(nextPageToken: string) → HttpRequest
```

---

# OpenCloudApiV1
**Extends:** Instance

## Functions
```
CreateModel(name: string) → OpenCloudModel
CreateUserNotificationAsync(user: string, userNotification: OpenCloudModel) → OpenCloudModel
```

---

# OpenCloudService
**Extends:** Instance

## Functions
```
GetApiV1() → OpenCloudApiV1
RegisterOpenCloud(version: string, methodName: string, method: Function) → null
RegistrationComplete() → null
HttpRequestAsync(options: Dictionary) → Dictionary
InvokeAsync(version: string, methodName: string, arguments: Dictionary, headers: Dictionary) → Dictionary
```

---

# OperationGraph
**Extends:** Instance

---

# PVInstance
**Extends:** Instance

## Properties
```
Origin: CFrame
Pivot Offset: CFrame
```

## Functions
```
GetPivot() → CFrame
PivotTo(targetCFrame: CFrame) → null
```

---

# BasePart
**Extends:** PVInstance

## Properties
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
CollisionGroupReplicate: string
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
PhysicsRepRootPart: BasePart
PivotOffset: CFrame
Position: Vector3
ReceiveAge: float [ReadOnly]
Reflectance: float
ReplicationPV: ReplicationPV
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

## Functions
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
GetPhysicsCost() → float
GetRenderCFrame() → CFrame [Deprecated]
GetRootPart() → Instance [Deprecated]
GetTouchingParts() → Instances
GetVelocityAtPosition(position: Vector3) → Vector3
IsGrounded() → bool
MakeJoints() → null [Deprecated]
Resize(normalId: NormalId, deltaAmount: int) → bool
SetNetworkOwner(playerInstance: Player) → null
SetNetworkOwnershipAuto() → null
SetPredictionMode(mode: PredictionMode) → null [Deprecated]
TorqueToAngularAcceleration(torque: Vector3, angVelocity: Vector3) → Vector3
breakJoints() → null [Deprecated]
getMass() → float [Deprecated]
makeJoints() → null [Deprecated]
resize(normalId: NormalId, deltaAmount: int) → bool [Deprecated]
IntersectAsync(parts: Instances, collisionfidelity: CollisionFidelity, renderFidelity: RenderFidelity) → Instance
SubtractAsync(parts: Instances, collisionfidelity: CollisionFidelity, renderFidelity: RenderFidelity) → Instance
UnionAsync(parts: Instances, collisionfidelity: CollisionFidelity, renderFidelity: RenderFidelity) → Instance
```

## Events
```
LocalSimulationTouched(part: BasePart)
NetworkOwnerChanged(systemAddress: SystemAddress)
OutfitChanged()
StoppedTouching(otherPart: BasePart)
TouchEnded(otherPart: BasePart)
Touched(otherPart: BasePart)
```

---

# CornerWedgePart
**Extends:** BasePart

---

# FormFactorPart
**Extends:** BasePart

## Properties
```
FormFactor: FormFactor [Deprecated]
formFactor: FormFactor [Deprecated]
formFactorRaw: FormFactor
```

---

# Part
**Extends:** FormFactorPart

## Properties
```
Shape: PartType
shap: PartType
shape: PartType
```

---

# FlagStand
**Extends:** Part

## Properties
```
TeamColor: BrickColor
```

## Events
```
FlagCaptured(player: Instance)
```

---

# Platform
**Extends:** Part

## Events
```
RemoteCreateMotor6D(humanoid: Instance)
RemoteDestroyMotor6D()
```

---

# Seat
**Extends:** Part

## Properties
```
Disabled: bool
Occupant: Humanoid [ReadOnly]
```

## Functions
```
Sit(humanoid: Instance) → null
```

## Events
```
RemoteCreateSeatWeld(humanoid: Instance)
RemoteDestroySeatWeld()
```

---

# SkateboardPlatform
**Extends:** Part

## Properties
```
Controller: SkateboardController [ReadOnly]
ControllingHumanoid: Humanoid [ReadOnly]
MoveState: MoveState
Steer: int
StickyWheels: bool
Throttle: int
```

## Functions
```
ApplySpecificImpulse(impulseWorld: Vector3) → null
```

## Events
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

# SpawnLocation
**Extends:** Part

## Properties
```
AllowTeamChangeOnTouch: bool
Duration: int
Enabled: bool
Neutral: bool
TeamColor: BrickColor
```

---

# WedgePart
**Extends:** FormFactorPart

---

# Terrain
**Extends:** BasePart

## Properties
```
AcquisitionMethod: TerrainAcquisitionMethod
ClusterGrid: string
ClusterGridV2: string
ClusterGridV3: BinaryString
Decoration: bool
GrassLength: float
IsSmooth: bool [ReadOnly] [Deprecated]
LastUsedModificationMethod: TerrainAcquisitionMethod
MaterialColors: BinaryString
MaxExtents: Region3int16 [ReadOnly]
PhysicsGrid: BinaryString
SmoothGrid: BinaryString
SmoothVoxelsUpgraded: bool
WaterColor: Color3
WaterReflectance: float
WaterTransparency: float
WaterWaveSize: float
WaterWaveSpeed: float
```

## Functions
```
AutowedgeCell(x: int, y: int, z: int) → bool [Deprecated]
AutowedgeCells(region: Region3int16) → null [Deprecated]
CanSmoothVoxelsBeUpgraded() → bool
CellCenterToWorld(x: int, y: int, z: int) → Vector3
CellCornerToWorld(x: int, y: int, z: int) → Vector3
Clear() → null
ClearVoxelsAsync_beta(region: Region3, channelIds: Array) → null
ConvertToSmooth() → null [Deprecated]
CopyRegion(region: Region3int16) → TerrainRegion
CountCells() → int
FillBall(center: Vector3, radius: float, material: Material) → null
FillBlock(cframe: CFrame, size: Vector3, material: Material) → null
FillCylinder(cframe: CFrame, height: float, radius: float, material: Material) → null
FillRegion(region: Region3, resolution: float, material: Material) → null
FillWedge(cframe: CFrame, size: Vector3, material: Material) → null
GetCell(x: int, y: int, z: int) → Tuple [Deprecated]
GetMaterialColor(material: Material) → Color3
GetTerrainWireframe(cframe: CFrame, size: Vector3) → Array
GetWaterCell(x: int, y: int, z: int) → Tuple [Deprecated]
IterateVoxelsAsync_beta(region: Region3, resolution: int, channelIds: Array) → TerrainIterateOperation
ModifyVoxelsAsync_beta(region: Region3, resolution: int, channelIds: Array) → TerrainModifyOperation
PasteRegion(region: TerrainRegion, corner: Vector3int16, pasteEmptyCells: bool) → null
ReadVoxelChannels(region: Region3, resolution: float, channelIds: Array) → Dictionary
ReadVoxels(region: Region3, resolution: float) → Tuple
ReadVoxelsAsync_beta(region: Region3, resolution: int, channelIds: Array) → TerrainReadOperation
ReplaceMaterial(region: Region3, resolution: float, sourceMaterial: Material, targetMaterial: Material) → null
ReplaceMaterialInTransform(cframe: CFrame, size: Vector3, sourceMaterial: Material, targetMaterial: Material) → null
ReplaceMaterialInTransformSubregion(cframe: CFrame, size: Vector3, sourceMaterial: Material, targetMaterial: Material, targetRegion: Region3int16) → null
SetCell(x: int, y: int, z: int, material: CellMaterial, block: CellBlock, orientation: CellOrientation) → null [Deprecated]
SetCells(region: Region3int16, material: CellMaterial, block: CellBlock, orientation: CellOrientation) → null [Deprecated]
SetMaterialColor(material: Material, value: Color3) → null
SetMaterialInTransform(cframe: CFrame, size: Vector3, targetMaterial: Material) → null
SetMaterialInTransformSubregion(cframe: CFrame, size: Vector3, targetMaterial: Material, targetRegion: Region3int16) → null
SetWaterCell(x: int, y: int, z: int, force: WaterForce, direction: WaterDirection) → null [Deprecated]
SmoothRegion(region: Region3, resolution: float, strength: float) → Tuple
WorldToCell(position: Vector3) → Vector3
WorldToCellPreferEmpty(position: Vector3) → Vector3
WorldToCellPreferSolid(position: Vector3) → Vector3
WriteVoxelChannels(region: Region3, resolution: float, channels: Dictionary) → null
WriteVoxels(region: Region3, resolution: float, materials: Array, occupancy: Array) → null
WriteVoxelsAsync_beta(region: Region3, resolution: int, channelIds: Array) → TerrainWriteOperation
```

---

# TriangleMeshPart
**Extends:** BasePart

## Properties
```
AeroMeshData: SharedString
CollisionFidelity: CollisionFidelity
ConvexDecompHolder: NetAssetRef
FluidFidelity: FluidFidelity
FluidFidelityInternal: FluidFidelity
InertiaMigrated: bool
MeshSize: Vector3 [ReadOnly]
PhysicalConfigData: SharedString
UnscaledCofm: Vector3
UnscaledVolInertiaDiags: Vector3
UnscaledVolInertiaOffDiags: Vector3
UnscaledVolume: float
```

---

# MeshPart
**Extends:** TriangleMeshPart

## Properties
```
AlternateMeshHash: int64 [ReadOnly]
DoubleSided: bool
EditableMeshString: SharedString
HasJointOffset: bool
HasSkinnedMesh: bool
InitialSize: Vector3
JointOffset: Vector3
MeshContent: Content
MeshID: ContentId [Deprecated]
MeshId: ContentId
PhysicsData: BinaryString
RenderFidelity: RenderFidelity
RenderFidelityReplicate: RenderFidelity
TextureContent: Content
TextureID: ContentId
VertexCount: int
```

## Functions
```
ApplyMesh(meshPart: Instance) → null
```

---

# PartOperation
**Extends:** TriangleMeshPart

## Properties
```
AssetId: ContentId
ChildData: BinaryString
ChildData2: SharedString
ComponentIndex: int
DCDPropertyData: CSGPropertyData
FormFactor: FormFactor
InitialSize: Vector3
ManifoldMesh_DEPRECATED: SharedString [Deprecated]
MeshData: BinaryString
MeshData2: SharedString
OffCentered: bool
PhysicsData: BinaryString
RenderFidelity: RenderFidelity
SerializedCSGTree: SharedString
SerializedOperationGraph: SharedString
SmoothingAngle: float
SolidMeshHolder: NetAssetRef
TriangleCount: int [ReadOnly]
UsePartColor: bool
```

## Functions
```
SubstituteGeometry(source: Instance) → null
```

---

# IntersectOperation
**Extends:** PartOperation

---

# NegateOperation
**Extends:** PartOperation

## Properties
```
PreviousOperation: NegateOperationHiddenHistory
```

---

# UnionOperation
**Extends:** PartOperation

---

# TrussPart
**Extends:** BasePart

## Properties
```
Style: Style
style: Style
```

---

# VehicleSeat
**Extends:** BasePart

## Properties
```
AreHingesDetected: int [ReadOnly]
Disabled: bool
HeadsUpDisplay: bool
MaxSpeed: float
Occupant: Humanoid [ReadOnly]
Steer: int
SteerFloat: float
Throttle: int
ThrottleFloat: float
Torque: float
TurnSpeed: float
```

## Functions
```
Sit(humanoid: Instance) → null
```

## Events
```
RemoteCreateSeatWeld(humanoid: Instance)
RemoteDestroySeatWeld()
```

---

# Camera
**Extends:** PVInstance

## Properties
```
CFrame: CFrame
CameraSubject: Instance
CameraType: CameraType
CoordinateFrame: CFrame [Deprecated]
DiagonalFieldOfView: float
FieldOfView: float
FieldOfViewMode: FieldOfViewMode
Focus: CFrame
HeadLocked: bool
HeadScale: float
MaxAxisFieldOfView: float
NearPlaneZ: float [ReadOnly]
VRTiltAndRollEnabled: bool
ViewportSize: Vector2 [ReadOnly]
focus: CFrame [Deprecated]
```

## Functions
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
SetImageServerView(modelCoord: CFrame) → null
SetRoll(rollAngle: float) → null
TiltUnits(units: int) → bool [Deprecated]
ViewportPointToRay(x: float, y: float, depth: float) → Ray
WorldToScreenPoint(worldPoint: Vector3) → Tuple
WorldToViewportPoint(worldPoint: Vector3) → Tuple
Zoom(distance: float) → bool
ZoomToExtents(boundingBoxCFrame: CFrame, boundingBoxSize: Vector3) → null
```

## Events
```
FirstPersonTransition(entering: bool)
InterpolationFinished()
```

---

# Model
**Extends:** PVInstance

## Properties
```
LevelOfDetail: ModelLevelOfDetail
LodEntity: LodDataEntity
ModelMeshCFrame: CFrame
ModelMeshData: SharedString
ModelMeshSize: Vector3
ModelStreamingMode: ModelStreamingMode
NeedsPivotMigration: bool
PrimaryPart: BasePart
Scale: float
ScaleFactor: float
SlimHash: BinaryString
WorldPivot: CFrame
WorldPivotData: OptionalCoordinateFrame
```

## Functions
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

# Actor
**Extends:** Model

## Functions
```
BindToMessage(topic: string, function: Function) → RBXScriptConnection
BindToMessageParallel(topic: string, function: Function) → RBXScriptConnection
SendMessage(topic: string, message: Tuple) → null
```

---

# BackpackItem
**Extends:** Model

## Properties
```
TextureId: ContentId
```

---

# HopperBin
**Extends:** BackpackItem

## Properties
```
Active: bool
BinType: BinType
Command: string
TextureName: string
```

## Functions
```
Disable() → null
ToggleSelect() → null
```

## Events
```
Deselected()
ReplicatedSelected()
Selected(mouse: Instance)
```

---

# Tool
**Extends:** BackpackItem

## Properties
```
CanBeDropped: bool
Enabled: bool
Grip: CFrame
GripForward: Vector3
GripPos: Vector3
GripRight: Vector3
GripUp: Vector3
ManualActivationOnly: bool
RequiresHandle: bool
ToolTip: string
```

## Functions
```
Activate() → null
Deactivate() → null
```

## Events
```
Activated()
Deactivated()
Equipped(mouse: Mouse)
Unequipped()
VRLaserPointerClicked(player: Player)
```

---

# Flag
**Extends:** Tool

## Properties
```
TeamColor: BrickColor
```

---

# Status
**Extends:** Model

---

# WorldRoot
**Extends:** Model

## Properties
```
PhysicsStepTime: float
```

## Functions
```
ArePartsTouchingOthers(partList: Instances, overlapIgnored: float) → bool
Blockcast(cframe: CFrame, size: Vector3, direction: Vector3, params: RaycastParams) → RaycastResult?
BulkMoveTo(partList: Instances, cframeList: Array, eventMode: BulkMoveMode) → null
CacheCurrentTerrain(id: string, center: Vector3, radius: float) → string
ClearCachedTerrain(id: string) → bool
FindPartOnRay(ray: Ray, ignoreDescendantsInstance: Instance, terrainCellsAreCubes: bool, ignoreWater: bool) → Tuple [Deprecated]
FindPartOnRayWithIgnoreList(ray: Ray, ignoreDescendantsTable: Instances, terrainCellsAreCubes: bool, ignoreWater: bool) → Tuple [Deprecated]
FindPartOnRayWithWhitelist(ray: Ray, whitelistDescendantsTable: Instances, ignoreWater: bool) → Tuple [Deprecated]
FindPartsInRegion3(region: Region3, ignoreDescendantsInstance: Instance, maxParts: int) → Instances [Deprecated]
FindPartsInRegion3WithIgnoreList(region: Region3, ignoreDescendantsTable: Instances, maxParts: int) → Instances [Deprecated]
FindPartsInRegion3WithWhiteList(region: Region3, whitelistDescendantsTable: Instances, maxParts: int) → Instances [Deprecated]
GetAwakeContactNormals() → Array
GetAwakeContactParts() → Array
GetAwakeContactPositions() → Array
GetAwakeRootParts() → Instances
GetPartBoundsInBox(cframe: CFrame, size: Vector3, overlapParams: OverlapParams) → Instances
GetPartBoundsInRadius(position: Vector3, radius: float, overlapParams: OverlapParams) → Instances
GetPartsInPart(part: BasePart, overlapParams: OverlapParams) → Instances
IKMoveTo(part: BasePart, target: CFrame, translateStiffness: float, rotateStiffness: float, collisionsMode: IKCollisionsMode) → null
IsRegion3Empty(region: Region3, ignoreDescendentsInstance: Instance) → bool [Deprecated]
IsRegion3EmptyWithIgnoreList(region: Region3, ignoreDescendentsTable: Instances) → bool [Deprecated]
Raycast(origin: Vector3, direction: Vector3, raycastParams: RaycastParams) → RaycastResult?
RaycastCachedTerrain(id: string, origin: Vector3, direction: Vector3, ignoreWater: bool) → RaycastResult?
SetInsertPoint(point: Vector3) → null
Shapecast(part: BasePart, direction: Vector3, params: RaycastParams) → RaycastResult?
Spherecast(position: Vector3, radius: float, direction: Vector3, params: RaycastParams) → RaycastResult?
StepPhysics(dt: float, parts: Instances) → null
findPartOnRay(ray: Ray, ignoreDescendantsInstance: Instance, terrainCellsAreCubes: bool, ignoreWater: bool) → Tuple [Deprecated]
findPartsInRegion3(region: Region3, ignoreDescendantsInstance: Instance, maxParts: int) → Instances [Deprecated]
```

---

# Workspace
**Extends:** WorldRoot

## Properties
```
AirDensity: float
AllowThirdPartySales: bool
AuthorityMode: AuthorityMode
AvatarUnificationMode: AvatarUnificationMode
ClientAnimatorThrottling: ClientAnimatorThrottlingMode
CollisionGroupData: BinaryString
CollisionGroups: string
ConvexDecompCompressed: bool
CurrentCamera: Camera
DataModelPlaceVersion: int
DistributedGameTime: double
ExplicitAutoJoints: bool
FallHeightEnabled: bool
FallenPartsDestroyHeight: float
FilteringEnabled: bool [Deprecated]
FluidForces: FluidForces
GlobalWind: Vector3
Gravity: float
IKControlConstraintSupport: IKControlConstraintSupport
InsertPoint: Vector3
InterpolationThrottling: InterpolationThrottlingMode [Deprecated]
LuauTypeCheckMode: LuauTypeCheckMode
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
StreamingEnabled: bool
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

## Functions
```
BreakJoints(objects: Instances) → null [Deprecated]
CalculateJumpDistance(gravity: float, jumpPower: float, walkSpeed: float) → float
CalculateJumpHeight(gravity: float, jumpPower: float) → float
CalculateJumpPower(gravity: float, jumpHeight: float) → float
ExperimentalSolverIsEnabled() → bool
GetNumAwakeParts() → int
GetPhysicsThrottling() → int
GetRealPhysicsFPS() → double
GetServerTimeNow() → double
JoinToOutsiders(objects: Instances, jointType: JointCreationMode) → null
MakeJoints(objects: Instances) → null [Deprecated]
PGSIsEnabled() → bool
SetAvatarUnificationMode(value: AvatarUnificationMode) → null
SetMeshPartHeadsAndAccessories(value: MeshPartHeadsAndAccessories) → null
SetPhysicsThrottleEnabled(value: bool) → null
UnjoinFromOutsiders(objects: Instances) → null
ZoomToExtents() → null
```

## Events
```
PersistentLoaded(player: Player)
```

---

# WorldModel
**Extends:** WorldRoot

---

# PackageLink
**Extends:** Instance

## Properties
```
AutoUpdate: bool
CanAutoUpdate: bool
Creator: string [ReadOnly]
DefaultName: string
HasNewVersion: bool
ModifiedState: int
PackageAssetName: string [ReadOnly]
PackageGuid: int64
PackageId: ContentId [ReadOnly]
PackageIdSerialize: ContentId
PermissionLevel: PackagePermission [ReadOnly]
SerializedDefaultAttributes: BinaryString
Status: string [ReadOnly]
VersionIdSerialize: int64
VersionNumber: int64
```

---

# PackageService
**Extends:** Instance

---

# PackageUIService
**Extends:** Instance

## Functions
```
ConvertToMockPackage(instance: Instance) → null
ConvertToPackageUpload(uploadUrl: string, cloneInstances: Instances, originalInstances: Instances) → null
GetPackageInfo(packageAssetId: int64) → Dictionary
PublishPackage(packageInstance: Instance, addUndoWayPoint: bool) → null
SetPackageVersion(packageInstance: Instance, versionNumber: int64) → Instance
```

## Events
```
OnConvertToPackageResult(isSuccessful: bool, errorMessage: string)
OnOpenConvertToPackagePlugin(instances: Instances, name: string, cloneInstances: Instances)
```

---

# Pages
**Extends:** Instance

## Properties
```
IsFinished: bool [ReadOnly]
```

## Functions
```
GetCurrentPage() → Array
AdvanceToNextPageAsync() → null
```

---

# AudioPages
**Extends:** Pages

---

# BanHistoryPages
**Extends:** Pages

---

# CapturesPages
**Extends:** Pages

---

# CatalogPages
**Extends:** Pages

---

# DataStoreKeyPages
**Extends:** Pages

## Properties
```
Cursor: string [ReadOnly]
```

---

# DataStoreListingPages
**Extends:** Pages

## Properties
```
Cursor: string [ReadOnly]
```

---

# DataStorePages
**Extends:** Pages

---

# DataStoreVersionPages
**Extends:** Pages

---

# FriendPages
**Extends:** Pages

---

# InventoryPages
**Extends:** Pages

---

# EmotesPages
**Extends:** InventoryPages

---

# MemoryStoreHashMapPages
**Extends:** Pages

---

# OutfitPages
**Extends:** Pages

---

# RecommendationPages
**Extends:** Pages

---

# StandardPages
**Extends:** Pages

---

# PartOperationAsset
**Extends:** Instance

## Properties
```
ChildData: BinaryString
MeshData: BinaryString
```

---

# ParticleEmitter
**Extends:** Instance

## Properties
```
Acceleration: Vector3
Brightness: float
Color: ColorSequence
Drag: float
EmissionDirection: NormalId
Enabled: bool
FlipbookFramerate: NumberRange
FlipbookIncompatible: string
FlipbookLayout: ParticleFlipbookLayout
FlipbookMode: ParticleFlipbookMode
FlipbookStartRandom: bool
Lifetime: NumberRange
LightEmission: float
LightInfluence: float
LocalTransparencyModifier: float
LockedToPart: bool
Orientation: ParticleOrientation
Rate: float
RotSpeed: NumberRange
Rotation: NumberRange
Shape: ParticleEmitterShape
ShapeInOut: ParticleEmitterShapeInOut
ShapePartial: float
ShapeStyle: ParticleEmitterShapeStyle
Size: NumberSequence
Speed: NumberRange
SpreadAngle: Vector2
Squash: NumberSequence
Texture: ContentId
TimeScale: float
Transparency: NumberSequence
VelocityInheritance: float
VelocitySpread: float [Deprecated]
WindAffectsDrag: bool
ZOffset: float
```

## Functions
```
Clear() → null
Emit(particleCount: int) → null
FastForward(numFrames: int) → null
```

## Events
```
OnClearRequested()
OnEmitRequested(particleCount: int)
```

---

# PartyEmulatorService
**Extends:** Instance

## Functions
```
CreateNewParty() → string
DeleteParty(partyId: string) → null
GetEmulatedPartyConfiguration() → Dictionary
GetIsEmulationEnabled() → bool
OnTestPlayerCountChanged(newPlayerCount: int) → null
SetIsEmulationEnabled(isEnabled: bool) → null
SetPlayerPartyId(userId: int64, partyId: string) → null
applyPartyIdToPlayer(player: Player) → null
GetEmulatedPartyAsync(partyId: string) → Array
```

## Events
```
ConfigurationChanged(configuration: Dictionary)
```

---

# PatchBundlerFileWatch
**Extends:** Instance

---

# PatchMapping
**Extends:** Instance

## Properties
```
FlattenTree: bool
PatchId: string
TargetPath: string
```

---

# Path
**Extends:** Instance

## Properties
```
Status: PathStatus [ReadOnly]
```

## Functions
```
GetPointCoordinates() → Array [Deprecated]
GetWaypoints() → Array
CheckOcclusionAsync(start: int) → int
ComputeAsync(start: Vector3, finish: Vector3) → null
```

## Events
```
Blocked(blockedWaypointIdx: int)
Unblocked(unblockedWaypointIdx: int)
```

---

# PathfindingLink
**Extends:** Instance

## Properties
```
Attachment0: Attachment
Attachment1: Attachment
IsBidirectional: bool
Label: string
```

---

# PathfindingModifier
**Extends:** Instance

## Properties
```
Label: string
PassThrough: bool
```

---

# PathfindingService
**Extends:** Instance

## Properties
```
EmptyCutoff: float [Deprecated]
```

## Functions
```
CreatePath(agentParameters: Dictionary) → Path
ComputeRawPathAsync(start: Vector3, finish: Vector3, maxDistance: float) → Path [Deprecated]
ComputeSmoothPathAsync(start: Vector3, finish: Vector3, maxDistance: float) → Path [Deprecated]
FindPathAsync(start: Vector3, finish: Vector3) → Path
```

---

# PausedState
**Extends:** Instance

## Properties
```
AllThreadsPaused: bool [ReadOnly]
Reason: DebuggerPauseReason [ReadOnly]
ThreadId: int [ReadOnly]
```

---

# PausedStateBreakpoint
**Extends:** PausedState

## Properties
```
Breakpoint: Breakpoint [ReadOnly]
```

---

# PausedStateException
**Extends:** PausedState

## Properties
```
ExceptionText: string [ReadOnly]
```

---

# PerformanceControlService
**Extends:** Instance

## Functions
```
IsCrossExperienceLaunchFeasible(type: string) → bool
```

---

# PermissionsService
**Extends:** Instance

## Functions
```
GetIsThirdPartyAssetAllowed() → bool
GetIsThirdPartyPurchaseAllowed() → bool
GetIsThirdPartyTeleportAllowed() → bool
GetPermissions(assetId: string) → Array
SetPermissions(assetId: string, permissions: Array) → null
```

---

# PhysicsService
**Extends:** Instance

## Functions
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
IkSolve(part: BasePart, target: CFrame, translateStiffness: float, rotateStiffness: float) → null
IsCollisionGroupRegistered(name: string) → bool
LocalIkSolve(part: BasePart, target: CFrame, translateStiffness: float, rotateStiffness: float) → null
RegisterCollisionGroup(name: string) → null
RemoveCollisionGroup(name: string) → null [Deprecated]
RenameCollisionGroup(from: string, to: string) → null
SetPartCollisionGroup(part: BasePart, name: string) → null [Deprecated]
UnregisterCollisionGroup(name: string) → null
```

---

# PhysicsSettings
**Extends:** Instance

## Properties
```
AllowSleep: bool
AreAnchorsShown: bool
AreAssembliesShown: bool
AreAssemblyCentersOfMassShown: bool
AreAwakePartsHighlighted: bool
AreBodyTypesShown: bool
AreCollisionCostsShown: bool
AreConstraintForcesShownForSelectedOrHoveredInstances: bool
AreConstraintTorquesShownForSelectedOrHoveredInstances: bool
AreContactForcesShownForSelectedOrHoveredAssemblies: bool
AreContactIslandsShown: bool
AreContactPointsShown: bool
AreGravityForcesShownForSelectedOrHoveredAssemblies: bool
AreJointCoordinatesShown: bool
AreMagnitudesShownForDrawnForcesAndTorques: bool
AreMechanismsShown: bool
AreModelCoordsShown: bool
AreNonAnchorsShown: bool
AreOwnersShown: bool
ArePartCoordsShown: bool
AreRegionsShown: bool
AreSolverIslandsShown: bool
AreTerrainReplicationRegionsShown: bool
AreTimestepsShown: bool
AreUnalignedPartsShown: bool
AreWorldCoordsShown: bool
DisableCSGv2: bool
DisableCSGv3ForPlugins: bool
DrawConstraintsNetForce: bool
DrawContactsNetForce: bool
DrawTotalNetForce: bool
EnableForceVisualizationSmoothing: bool
FluidForceDrawScale: float
ForceCSGv2: bool
ForceDrawScale: float
ForceVisualizationSmoothingSteps: int
IsInterpolationThrottleShown: bool
IsReceiveAgeShown: bool
IsTreeShown: bool
PhysicsEnvironmentalThrottle: EnviromentalPhysicsThrottle
ShowDecompositionGeometry: bool
ShowFluidForcesForSelectedOrHoveredMechanisms: bool
ShowInstanceNamesForDrawnForcesAndTorques: bool
SolverConvergenceMetricType: SolverConvergenceMetricType
SolverConvergenceVisualizationMode: SolverConvergenceVisualizationMode
ThrottleAdjustTime: double
TorqueDrawScale: float
UseCSGv2: bool
```

---

# PlaceAssetIdsService
**Extends:** Instance

---

# PlaceStatsService
**Extends:** Instance

---

# PlacesService
**Extends:** Instance

## Functions
```
StartPlaySolo() → null
StopPlaySolo() → null
```

---

# PlatformCloudStorageService
**Extends:** Instance

## Functions
```
IsUserDataAvailable() → bool
GetUserDataAsync(key: string) → Dictionary
SetUserDataAsync(key: string, data: Dictionary) → null
```

---

# PlatformFriendsService
**Extends:** Instance

## Functions
```
IsInviteFriendsEnabled() → bool
IsProfileEnabled() → bool
ShowInviteFriendsUI() → null
ShowProfile(platformUserId: string) → null
GetPartyMembers() → Array
```

---

# Player
**Extends:** Instance

## Properties
```
AccountAge: int [ReadOnly]
AccountAgeReplicate: int
AppearanceDidLoad: bool [ReadOnly] [Deprecated]
AutoJumpEnabled: bool
CameraMaxZoomDistance: float
CameraMinZoomDistance: float
CameraMode: CameraMode
CanLoadCharacterAppearance: bool
Character: Model
CharacterAppearance: string [Deprecated]
CharacterAppearanceId: int64
ChararacterRegionId: Vector3
ChatMode: ChatMode [ReadOnly]
ChatPrivacyMode: ChatPrivacyMode
CloudEditCameraCoordinateFrame: CFrame
CloudEditPlayerActive: bool
CountryRegionCodeReplicate: string
DataComplexity: int [ReadOnly] [Deprecated]
DataComplexityLimit: int [Deprecated]
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
GameplayPaused: bool
Guest: bool [ReadOnly]
HasVerifiedBadge: bool
HealthDisplayDistance: float
InternalCharacterAppearanceLoaded: bool
LocaleId: string [ReadOnly]
MaxSimulationRadius: float
MaximumSimulationRadius: float
MembershipType: MembershipType [ReadOnly]
MembershipTypeReplicate: MembershipType
NameDisplayDistance: float
Neutral: bool
OsPlatform: string
PartyId: string
PlatformName: string
RawJoinData: BinaryString
ReplicationFocus: Instance
RespawnLocation: SpawnLocation
SimulationRadius: float
StepIdOffset: int
SuperSafeChatReplicate: bool
Team: Team
TeamColor: BrickColor
Teleported: bool [ReadOnly]
TeleportedIn: bool
ThirdPartyTextChatRestrictionStatus: ChatRestrictionStatus [ReadOnly]
UnfilteredChat: bool [ReadOnly]
UserId: int64
VRDevice: string
VREnabled: bool
userId: int64 [Deprecated]
```

## Functions
```
AddReplicationFocus(part: BasePart) → null
AddReplicationFocusPosition(center: Vector3, radius: int) → null
AddToBlockList(userIds: Array) → null
ClearCharacterAppearance() → null
DistanceFromCharacter(point: Vector3) → float
GetData() → PlayerData
GetFriendStatus(player: Player) → FriendStatus
GetGameSessionID() → string
GetJoinData() → Dictionary
GetMouse() → Mouse
GetNetworkPing() → float
GetUnder13() → bool
HasAppearanceLoaded() → bool
IsVerified() → bool
Kick(message: string) → null
LoadBoolean(key: string) → bool [Deprecated]
LoadCharacterAppearance(assetInstance: Instance) → null [Deprecated]
LoadData() → null [Deprecated]
LoadInstance(key: string) → Instance [Deprecated]
LoadNumber(key: string) → double [Deprecated]
LoadString(key: string) → string [Deprecated]
Move(walkDirection: Vector3, relativeToCamera: bool) → null
OverrideStreamingRadii(minRadius: int, targetRadius: int) → null
PinStreamingForInstance(instance: Instance, depth: int) → null
RemoveCharacter() → null
RemoveReplicationFocus(part: BasePart) → null
RemoveReplicationFocusPosition(center: Vector3, radius: int) → null
RequestFriendship(player: Player) → null
RevokeFriendship(player: Player) → null
SaveBoolean(key: string, value: bool) → null [Deprecated]
SaveData() → null [Deprecated]
SaveInstance(key: string, value: Instance) → null [Deprecated]
SaveNumber(key: string, value: double) → null [Deprecated]
SaveString(key: string, value: string) → null [Deprecated]
SetAccountAge(accountAge: int) → null
SetBlockListInitialized() → null
SetCharacterAppearanceJson(jsonBlob: string) → null
SetChatTranslationSettingsLocaleId(locale: string) → null
SetExperienceSettingsLocaleId(locale: string) → null
SetMembershipType(membershipType: MembershipType) → null
SetModerationAccessKey(moderationAccessKey: string) → null
SetSuperSafeChat(value: bool) → null
SetUnder13(value: bool) → null [Deprecated]
UnpinStreamingForInstance(instance: Instance, depth: int) → null
UpdatePlayerBlocked(userId: int64, blocked: bool) → null
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
LoadCharacterBlocking() → null
LoadCharacterWithAvatarRules(avatarRules: AvatarRules) → null
LoadCharacterWithHumanoidDescription(humanoidDescription: HumanoidDescription) → null
RequestStreamAroundAsync(position: Vector3, timeOut: double) → null
WaitForDataReady() → bool [Deprecated]
isFriendsWith(userId: int64) → bool [Deprecated]
waitForDataReady() → bool [Deprecated]
```

## Events
```
CharacterAdded(character: Model)
CharacterAppearanceLoaded(character: Model)
CharacterRemoving(character: Model)
Chatted(message: string, recipient: Player)
CloudEditSelectionChanged(newSelection: Array)
ConnectDiedSignalBackend()
FriendStatusChanged(player: Player, friendStatus: FriendStatus)
Idled(time: double)
Kill()
NotifyStreamingUnpinned(instance: Instance, depth: int)
OnTeleport(teleportState: TeleportState, placeId: int64, spawnName: string)
OnTeleportInternal(teleportState: TeleportState, teleportInfo: Dictionary, customLoadingScreen: Instance)
OverrideStreamRadii(minRadius: int, targetRadius: int)
PlayerCharacterLoaded(metrics: Dictionary)
PlayerChatTranslationSettingsLocaleSetFromLua(newLocaleId: string)
PlayerExperienceSettingsLocaleSetFromLua(newLocaleId: string)
RemoteFriendRequestSignal(otherUserId: int64, eventType: FriendRequestEvent)
RemoteInsert(url: string, position: Vector3)
RequestStreamingPin(instance: Instance, depth: int)
ScopeCheckInitiated(guid: string, serializedScopes: Array, metadata: Dictionary)
ScriptSecurityError(hash: string, error: string, stack: string)
ServerToClientUnfilteredChatReplicate(value: bool)
ServerUpdatedHead(assetType: AssetType, assetId: int64)
SetShutdownMessage(message: string)
SimulationRadiusChanged(radius: float)
StatsAvailable(info: string)
StreamingPinComplete(instance: Instance)
UnpinStreaming(instance: Instance, depth: int)
```

---

# PlayerData
**Extends:** Instance

## Functions
```
GetPlayer() → Player
GetRecordAsync(recordName: string) → PlayerDataRecord
```

---

# PlayerDataRecord
**Extends:** Instance

## Properties
```
CreatedTime: int64 [ReadOnly]
DefaultRecordName: bool [ReadOnly]
Dirty: bool [ReadOnly]
Error: PlayerDataErrorState [ReadOnly]
FlushedTime: int64 [ReadOnly]
LoadedTime: int64 [ReadOnly]
ModifiedTime: int64 [ReadOnly]
NewRecord: bool [ReadOnly]
Readable: bool [ReadOnly]
RecordName: string [ReadOnly]
Writable: bool [ReadOnly]
```

## Functions
```
GetPlayer() → Player
GetValue(key: string) → Variant
GetValueChangedSignal(key: string) → RBXScriptSignal
RemoveValue(key: string) → null
SetValue(key: string, value: Variant) → null
ReleaseAsync() → null
RequestFlushAsync() → null
```

## Events
```
Changed(key: string, value: Variant)
Flushed(flushState: bool, error: string?)
Loaded(success: bool, error: string?)
```

---

# PlayerDataRecordConfig
**Extends:** Instance

## Properties
```
RecordName: string [ReadOnly]
```

## Functions
```
GetDefaultValue(key: string) → Variant
SetDefaultValue(key: string, value: Variant) → null
```

---

# PlayerDataService
**Extends:** Instance

## Properties
```
LoadFailureBehavior: PlayerDataLoadFailureBehavior
```

## Functions
```
GetRecordConfig(recordName: string) → PlayerDataRecordConfig
```

---

# PlayerEmulatorService
**Extends:** Instance

## Properties
```
CustomPoliciesEnabled: bool
EmulatedCountryCode: string
EmulatedGameLocale: string
PlayerEmulationEnabled: bool
PseudolocalizationEnabled: bool
SerializedEmulatedPolicyInfo: BinaryString
TextElongationFactor: int
```

## Functions
```
GetEmulatedPolicyInfo() → Dictionary
RegionCodeWillHaveAutomaticNonCustomPolicies(regionCode: string) → bool
SetEmulatedPolicyInfo(emulatedPolicyInfo: Dictionary) → null
```

---

# PlayerHydrationService
**Extends:** Instance

## Events
```
PlayerHydration(userId: int64, playerHydrationBlob: string, playerHydrationSignature: string)
```

---

# PlayerScripts
**Extends:** Instance

## Functions
```
ClearComputerCameraMovementModes() → null
ClearComputerMovementModes() → null
ClearTouchCameraMovementModes() → null
ClearTouchMovementModes() → null
GetRegisteredComputerCameraMovementModes() → Array
GetRegisteredComputerMovementModes() → Array
GetRegisteredTouchCameraMovementModes() → Array
GetRegisteredTouchMovementModes() → Array
RegisterComputerCameraMovementMode(cameraMovementMode: ComputerCameraMovementMode) → null
RegisterComputerMovementMode(movementMode: ComputerMovementMode) → null
RegisterTouchCameraMovementMode(cameraMovementMode: TouchCameraMovementMode) → null
RegisterTouchMovementMode(movementMode: TouchMovementMode) → null
```

## Events
```
ComputerCameraMovementModeRegistered()
ComputerMovementModeRegistered()
TouchCameraMovementModeRegistered()
TouchMovementModeRegistered()
```

---

# PlayerViewService
**Extends:** Instance

## Functions
```
GetDeviceCameraCFrame(player: Player) → CFrame
GetDeviceCameraCFrameForSelfView() → CFrame
OnCameraCFrameReplicationRequest() → null
UpdateDeviceCFrame(player: Player, cframe: CFrame, timestamp: int64) → null
```

---

# Players
**Extends:** Instance

## Properties
```
BanningEnabled: bool
BubbleChat: bool [ReadOnly]
CharacterAutoLoads: bool
ClassicChat: bool [ReadOnly]
LocalPlayer: Player [ReadOnly]
MaxPlayers: int [ReadOnly]
MaxPlayersInternal: int
NumPlayers: int [ReadOnly] [Deprecated]
PreferredPlayers: int [ReadOnly]
PreferredPlayersInternal: int
RespawnTime: float
ServerGitHash: string
ServerLogPrefix: string
UseStrafingAnimations: bool
localPlayer: Player [ReadOnly] [Deprecated]
numPlayers: int [ReadOnly] [Deprecated]
```

## Functions
```
Chat(message: string) → null
CreateLocalPlayer() → Player
GetPlayerByUserId(userId: int64) → Player
GetPlayerFromCharacter(character: Model) → Player
GetPlayers() → Instances
ReportAbuse(player: Player, reason: string, optionalMessage: string) → null
ReportAbuseV3(player: Player, jsonTags: string) → null
ReportChatAbuse(eligibleChatLines: Array, targetChatLines: Array, tags: Dictionary) → null
ResetLocalPlayer() → null
SetChatStyle(style: ChatStyle) → null
SetLocalPlayerInfo(userId: int64, userName: string, displayName: string, membershipType: MembershipType, isUnder13: bool) → null
TeamChat(message: string) → null
WhisperChat(message: string, player: Instance) → null
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

## Events
```
CloudEditApplyEditsMessage(playerName: string, scriptName: string)
FriendRequestEvent(player: Player, player: Player, friendRequestEvent: FriendRequestEvent)
GameAnnounce(message: string)
PlayerAdded(player: Player)
PlayerChatted(chatType: PlayerChatType, player: Player, message: string, targetPlayer: Player)
PlayerConnecting(player: Player)
PlayerDisconnecting(player: Player)
PlayerMembershipChanged(player: Player)
PlayerRejoining(player: Player)
PlayerRemoving(player: Player)
PromptGameServerReportEnrichment(reportId: string)
PromptGameServerTargetedChatReportEnrichment(reportId: string, eligibleChatLines: Array, targetChatLines: Array)
PromptReportServerEnrichmentAndScan(v1comment: string, submitterId: int64, abuserId: int64, reportId: string)
RequestCloudEditImmediatePublishWithContext(spanContext: string)
RequestCloudEditKick(playerId: int64)
RequestCloudEditShutdown()
RequestTeamCreateImmediateSaveWithContext(spanContext: string)
TeamCreatePublishFinished(publishSuccessful: bool)
TeamCreateSaveFinished(saveSuccessful: bool)
TeamCreateServerMessage(messageType: MessageType, message: string, printToStatusBar: bool)
UserSubscriptionStatusChanged(user: Player, subscriptionId: string)
```

---

# Plugin
**Extends:** Instance

## Properties
```
CollisionEnabled: bool [ReadOnly]
DisableUIDragDetectorDrags: bool
GridSize: float [ReadOnly]
HostDataModelType: StudioDataModelType [ReadOnly]
HostDataModelTypeIsCurrent: bool [ReadOnly]
IsDebuggable: bool
MultipleDocumentInterfaceInstance: MultipleDocumentInterfaceInstance [ReadOnly]
UsesAssetInsertionDrag: bool
```

## Functions
```
Activate(exclusiveMouse: bool) → null
CreatePluginAction(actionId: string, text: string, statusTip: string, iconName: string, allowBinding: bool) → PluginAction
CreatePluginMenu(id: string, title: string, icon: string) → PluginMenu
CreateToolbar(name: string) → PluginToolbar
Deactivate() → null
GetItem(key: string, defaultValue: Variant) → Variant
GetJoinMode() → JointCreationMode
GetMouse() → PluginMouse
GetPluginComponent(name: string) → Variant
GetSelectedRibbonTool() → RibbonTool
GetSetting(key: string) → Variant
GetStudioUserId() → int64 [Deprecated]
GetUri() → Dictionary
Intersect(objects: Instances) → Instance
Invoke(key: string, arguments: Tuple) → null
IsActivated() → bool
IsActivatedWithExclusiveMouse() → bool
IsLoadedFromProject() → bool
Negate(objects: Instances) → Instances
OnInvoke(key: string, callback: Function) → Instance
OnInvokeSuspendOverride(key: string, callback: Function) → Instance
OnSetItem(key: string, callback: Function) → Instance
OpenScript(script: LuaSourceContainer, lineNumber: int) → null
OpenWikiPage(url: string) → null
PauseSound(sound: Instance) → null
PlaySound(sound: Instance, normalizedTimePosition: double) → null
ResumeSound(sound: Instance) → null
SaveSelectedToRoblox() → null
SelectRibbonTool(tool: RibbonTool, position: UDim2) → null
Separate(objects: Instances) → Instances
SetItem(key: string, value: Variant) → null
SetReady() → null
SetSetting(key: string, value: Variant) → null
StartDecalDrag(decal: Instance) → null
StartDrag(dragData: Dictionary) → null
StopAllSounds() → null
Union(objects: Instances) → Instance
CreateDockWidgetPluginGui(pluginGuiId: string, dockWidgetPluginGuiInfo: DockWidgetPluginGuiInfo) → DockWidgetPluginGui
CreateQWidgetPluginGui(pluginGuiId: string, pluginGuiOptions: Dictionary) → QWidgetPluginGui
ImportFbxAnimation(rigModel: Instance, isR15: bool) → Instance
ImportFbxRig(isR15: bool) → Instance
PromptForExistingAssetId(assetType: string) → int64
PromptSaveSelection(suggestedFileName: string) → bool
```

## Events
```
Deactivation()
Ready()
Unloading()
```

---

# PluginAction
**Extends:** Instance

## Properties
```
ActionId: string [ReadOnly]
AllowBinding: bool [ReadOnly]
Checked: bool
DefaultShortcut: string
Enabled: bool
StatusTip: string [ReadOnly]
Text: string
```

## Events
```
Triggered()
```

---

# PluginCapabilities
**Extends:** Instance

## Properties
```
Manifest: string
```

---

# PluginDebugService
**Extends:** Instance

---

# PluginDragEvent
**Extends:** Instance

## Properties
```
Data: string [ReadOnly]
MimeType: string [ReadOnly]
Position: Vector2 [ReadOnly]
Sender: string [ReadOnly]
```

---

# PluginGuiService
**Extends:** Instance

---

# PluginManagementService
**Extends:** Instance

## Functions
```
SetAutoUpdate(pluginId: int64, state: bool) → null
GetOTAPluginVersion(pluginName: string) → int64
```

---

# PluginManager
**Extends:** Instance

## Functions
```
CreatePlugin() → Instance [Deprecated]
ExportPlace(filePath: string) → null
ExportSelection(filePath: string) → null
```

---

# PluginManagerInterface
**Extends:** Instance

## Functions
```
CreatePlugin() → Instance [Deprecated]
ExportPlace(filePath: string) → null
ExportSelection(filePath: string) → null
```

---

# PluginMenu
**Extends:** Instance

## Properties
```
Icon: string
Title: string
```

## Functions
```
AddAction(action: Instance) → null
AddMenu(menu: Instance) → null
AddNewAction(actionId: string, text: string, icon: string) → Instance
AddSeparator() → null
Clear() → null
ShowAsync() → Instance
```

---

# PluginPolicyService
**Extends:** Instance

## Functions
```
GetPluginPolicy(pluginName: string) → Dictionary
```

---

# PluginToolbar
**Extends:** Instance

## Functions
```
CreateButton(buttonId: string, tooltip: string, iconname: string, text: string) → PluginToolbarButton
CreatePopupButton(buttonId: string, tooltip: string, iconname: string, text: string) → PluginToolbarButton
```

---

# PluginToolbarButton
**Extends:** Instance

## Properties
```
ClickableWhenViewportHidden: bool
Enabled: bool
Icon: ContentId
```

## Functions
```
SetActive(active: bool) → null
SetDropdownActive(active: bool) → null
```

## Events
```
Click()
DropdownClick()
```

---

# PointsService
**Extends:** Instance

## Functions
```
GetAwardablePoints() → int [Deprecated]
AwardPoints(userId: int64, amount: int) → Tuple [Deprecated]
GetGamePointBalance(userId: int64) → int [Deprecated]
GetPointBalance(userId: int64) → int [Deprecated]
```

## Events
```
PointsAwarded(userId: int64, pointsAwarded: int, userBalanceInGame: int, userTotalBalance: int)
```

---

# PolicyService
**Extends:** Instance

## Properties
```
IsLuobuServer: TriStateBoolean
LuobuWhitelisted: TriStateBoolean
```

## Functions
```
CanViewBrandProjectAsync(player: Player, brandProjectId: string) → bool
GetPolicyInfoForPlayerAsync(player: Instance) → Dictionary
GetPolicyInfoForServerRobloxOnlyAsync() → Dictionary
```

---

# PoseBase
**Extends:** Instance

## Properties
```
EasingDirection: PoseEasingDirection
EasingStyle: PoseEasingStyle
Weight: float
```

---

# NumberPose
**Extends:** PoseBase

## Properties
```
Value: double
```

---

# Pose
**Extends:** PoseBase

## Properties
```
CFrame: CFrame
MaskWeight: float [Deprecated]
```

## Functions
```
AddSubPose(pose: Instance) → null
GetSubPoses() → Instances
RemoveSubPose(pose: Instance) → null
```

---

# PostEffect
**Extends:** Instance

## Properties
```
Enabled: bool
```

---

# BloomEffect
**Extends:** PostEffect

## Properties
```
Intensity: float
Size: float
Threshold: float
```

---

# BlurEffect
**Extends:** PostEffect

## Properties
```
Size: float
```

---

# ColorCorrectionEffect
**Extends:** PostEffect

## Properties
```
Brightness: float
Contrast: float
Saturation: float
TintColor: Color3
```

---

# ColorGradingEffect
**Extends:** PostEffect

## Properties
```
TonemapperPreset: TonemapperPreset
```

---

# DepthOfFieldEffect
**Extends:** PostEffect

## Properties
```
FarIntensity: float
FocusDistance: float
InFocusRadius: float
NearIntensity: float
```

---

# SunRaysEffect
**Extends:** PostEffect

## Properties
```
Intensity: float
Spread: float
```

---

# ProcessInstancePhysicsService
**Extends:** Instance

---

# ProximityPrompt
**Extends:** Instance

## Properties
```
ActionText: string
AutoLocalize: bool
ClickablePrompt: bool
Enabled: bool
Exclusivity: ProximityPromptExclusivity
GamepadKeyCode: KeyCode
HoldDuration: float
KeyboardKeyCode: KeyCode
MaxActivationDistance: float
MaxIndicatorDistance: float
ObjectText: string
RequiresLineOfSight: bool
RootLocalizationTable: LocalizationTable
Style: ProximityPromptStyle
UIOffset: Vector2
```

## Functions
```
InputHoldBegin() → null
InputHoldEnd() → null
```

## Events
```
ButtonHoldBeganActionReplicated(player: Player)
ButtonHoldEndedActionReplicated(player: Player)
IndicatorHidden()
IndicatorShown()
PromptButtonHoldBegan(playerWhoTriggered: Player)
PromptButtonHoldEnded(playerWhoTriggered: Player)
PromptHidden()
PromptShown(inputType: ProximityPromptInputType)
TriggerEnded(playerWhoTriggered: Player)
TriggerEndedActionReplicated(player: Player)
Triggered(playerWhoTriggered: Player)
TriggeredActionReplicated(player: Instance)
```

---

# ProximityPromptService
**Extends:** Instance

## Properties
```
Enabled: bool
MaxIndicatorsVisible: int
MaxPromptsVisible: int
```

## Events
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

# PublishService
**Extends:** Instance

## Functions
```
PublishDescendantAssets(instance: Instance) → bool
CreateAssetAndWaitForAssetId(instances: Instances, operationId: string, creatorType: AssetCreatorType, creatorId: int64, assetType: string, name: string, description: string, expectedPrice: int) → int64
CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsync(serializedInstance: string, creatorType: AssetCreatorType, creatorId: int64, assetType: string, assetId: int64, name: string, description: string, token: string, contentType: string, expectedPrice: int) → Dictionary
CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsyncWithAddParam(serializedInstance: string, publishInfo: Dictionary) → Dictionary
CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsyncWithAddParamErrorJson(serializedInstance: string, publishInfo: Dictionary) → Dictionary
PublishCageMeshAsync(wrap: Instance, cageType: CageType) → ContentId
PublishDescendantAssetsAsync(instance: Instance) → bool
```

---

# RTAnimationTracker
**Extends:** Instance

## Properties
```
Active: bool
EnableFallbackAudioInput: bool
SessionName: string
TrackerMode: TrackerMode [ReadOnly]
TrackerType: TrackerType
```

## Functions
```
Step() → null
```

## Events
```
TrackerError(errorCode: TrackerError, msg: string)
TrackerPrompt(prompt: TrackerPromptEvent)
```

---

# RbxAnalyticsService
**Extends:** Instance

## Functions
```
AddGlobalPointsField(key: string, value: int) → null
AddGlobalPointsTag(key: string, value: string) → null
DEPRECATED_TrackEvent(category: string, action: string, label: string, value: int64) → null
DEPRECATED_TrackEventWithArgs(category: string, action: string, label: string, args: Dictionary, value: int64) → null
GetClientId() → string
GetPlaySessionId() → string
GetSessionId() → string
ReleaseRBXEventStream(target: string) → null
RemoveGlobalPointsField(key: string) → null
RemoveGlobalPointsTag(key: string) → null
ReportCounter(counterName: string, amount: int) → null
ReportInfluxSeries(seriesName: string, points: Dictionary, throttlingPercentage: int) → null
ReportStats(category: string, value: float) → null
ReportToDiagByCountryCode(featureName: string, measureName: string, seconds: double) → null
SendEventDeferred(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null
SendEventImmediately(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null
SetRBXEvent(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null
SetRBXEventStream(target: string, eventContext: string, eventName: string, additionalArgs: Dictionary) → null
TrackEvent(category: string, action: string, label: string, value: int64) → null
TrackEventWithArgs(category: string, action: string, label: string, args: Dictionary, value: int64) → null
UpdateHeartbeatObject(args: Dictionary) → null
```

---

# RecommendationService
**Extends:** Instance

## Functions
```
LogActionEvent(actionType: RecommendationActionType, itemId: string, tracingId: string, actionEventDetails: Dictionary) → null
LogImpressionEvent(impressionType: RecommendationImpressionType, itemId: string, tracingId: string, impressionEventDetails: Dictionary) → null
GenerateItemListAsync(generateRecommendationItemListRequest: Dictionary) → RecommendationPages
RegisterItemAsync(player: Player, registerRecommendationItemsRequest: Dictionary) → Dictionary
RemoveItemAsync(itemId: string) → null
UpdateItemAsync(updateRecommendationItemRequest: Dictionary) → null
```

---

# ReflectionMetadata
**Extends:** Instance

---

# ReflectionMetadataCallbacks
**Extends:** Instance

---

# ReflectionMetadataClasses
**Extends:** Instance

---

# ReflectionMetadataEnums
**Extends:** Instance

---

# ReflectionMetadataEvents
**Extends:** Instance

---

# ReflectionMetadataFunctions
**Extends:** Instance

---

# ReflectionMetadataItem
**Extends:** Instance

## Properties
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

# ReflectionMetadataClass
**Extends:** ReflectionMetadataItem

## Properties
```
ExplorerImageIndex: int
ExplorerOrder: int
Insertable: bool
PreferredParent: string
ServiceVisibility: ServiceVisibility
```

---

# ReflectionMetadataEnum
**Extends:** ReflectionMetadataItem

---

# ReflectionMetadataEnumItem
**Extends:** ReflectionMetadataItem

---

# ReflectionMetadataMember
**Extends:** ReflectionMetadataItem

---

# ReflectionMetadataProperties
**Extends:** Instance

---

# ReflectionMetadataYieldFunctions
**Extends:** Instance

---

# ReflectionService
**Extends:** Instance

## Functions
```
GetClass(className: string, filter: Dictionary) → Dictionary?
GetClasses(filter: Dictionary) → Array
GetPropertiesOfClass(className: string, filter: Dictionary) → Array
GetPropertyNames(name: string) → Array
GetStyledPropertyNames(name: string) → Array
```

---

# RemoteCursorService
**Extends:** Instance

## Events
```
BroadcastRemoteCursorPositions(script: string, remoteCursorPosition: string)
RequestAllRemoteCursorPositionForScript(script: string)
UpdateClientRemoteCursorPosition(script: string, remoteCursorPosition: string)
```

---

# RemoteDebuggerServer
**Extends:** Instance

---

# RemoteFunction
**Extends:** Instance

## Functions
```
InvokeClient(player: Player, arguments: Tuple) → Tuple
InvokeServer(arguments: Tuple) → Tuple
```

## Events
```
RemoteOnInvokeClient(id: int, arguments: Tuple)
RemoteOnInvokeError(id: int, arguments: string)
RemoteOnInvokeServer(id: int, player: Player, arguments: Tuple)
RemoteOnInvokeSuccess(id: int, arguments: Tuple)
```

---

# RenderSettings
**Extends:** Instance

## Properties
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

## Functions
```
GetMaxQualityLevel() → int
```

---

# RenderingTest
**Extends:** Instance

## Properties
```
CFrame: CFrame
ComparisonDiffThreshold: int
ComparisonMethod: RenderingTestComparisonMethod
ComparisonPsnrThreshold: float
Description: string
FieldOfView: float
Orientation: Vector3
PerfTest: bool
Position: Vector3
QualityAuto: bool
QualityLevel: int
RenderingTestFrameCount: int
ShouldSkip: bool
Ticket: string
Timeout: int
```

## Functions
```
RenderdocTriggerCapture() → null
```

---

# ReplicatedFirst
**Extends:** Instance

## Functions
```
IsDefaultLoadingGuiRemoved() → bool
IsFinishedReplicating() → bool
RemoveDefaultLoadingScreen() → null
SetDefaultLoadingGuiRemoved() → null
```

## Events
```
DefaultLoadingGuiRemoved()
FinishedReplicating()
RemoveDefaultLoadingGuiSignal()
```

---

# ReplicatedStorage
**Extends:** Instance

---

# RibbonNotificationService
**Extends:** Instance

## Functions
```
OnNotificationUpdateFromPlugin(newNotificationId: string, seenNotificationId: string) → null
```

## Events
```
AllNotificationsReadFromRibbon()
NewNotificationFromRibbon(newNotificationId: string)
NotificationReadFromRibbon(newNotificationId: string)
ToggleNotificationTray(checked: bool, newNotificationAvailable: bool)
```

---

# RobloxPluginGuiService
**Extends:** Instance

---

# RobloxReplicatedStorage
**Extends:** Instance

---

# RobloxSerializableInstance
**Extends:** Instance

## Properties
```
Data: BinaryString
```

---

# RobloxServerStorage
**Extends:** Instance

---

# RomarkRbxAnalyticsService
**Extends:** Instance

---

# RomarkService
**Extends:** Instance

## Functions
```
EndRemoteRomarkTest() → null
```

## Events
```
RomarkEndOfTest()
```

---

# RotationCurve
**Extends:** Instance

## Properties
```
Length: int [ReadOnly]
ValuesAndTimes: BinaryString
```

## Functions
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

# RtMessagingService
**Extends:** Instance

---

# RunService
**Extends:** Instance

## Properties
```
ClientGitHash: string [ReadOnly]
RunState: RunState
```

## Functions
```
BindToRenderStep(name: string, priority: int, function: Function) → null
GetCoreScriptVersion() → string
GetRobloxClientChannel() → string
GetRobloxGuiFocused() → bool
GetRobloxVersion() → string
IsClient() → bool
IsEdit() → bool
IsRunMode() → bool
IsRunning() → bool
IsServer() → bool
IsStudio() → bool
Pause() → null
Reset() → null [Deprecated]
Run() → null
Set3dRenderingEnabled(enable: bool) → null
SetRobloxGuiFocused(focus: bool) → null
Stop() → null
UnbindFromRenderStep(name: string) → null
setThrottleFramerateEnabled(enable: bool) → null
```

## Events
```
Heartbeat(deltaTime: double)
PostSimulation(deltaTimeSim: double)
PreAnimation(deltaTimeSim: double)
PreRender(deltaTimeRender: double)
PreSimulation(deltaTimeSim: double)
RenderStepped(deltaTime: double)
RobloxGuiFocusedChanged(isRobloxGuiFocused: bool)
Stepped(time: double, deltaTime: double)
```

---

# RuntimeScriptService
**Extends:** Instance

---

# SafetyService
**Extends:** Instance

## Properties
```
IsCaptureModeForReport: bool
```

## Functions
```
DecodeAvatarMovementProto(avatarMovementProtoString: string) → Dictionary
ReportMenuTabClose() → null
ReportMenuTabOpen() → null
TakeScreenshot(screenshotOptions: Dictionary) → int64
```

## Events
```
FSTriggeredSignal(requestId: string, playerId: int64, mac: string, args: Tuple)
ScreenshotContentReady(screenshotJobId: int64, contentId: ContentId)
ScreenshotUploaded(screenshotJobId: int64, screenshotId: string)
```

---

# ScreenshotHud
**Extends:** Instance

## Properties
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

# ScriptBuilder
**Extends:** Instance

---

# SyncScriptBuilder
**Extends:** ScriptBuilder

## Properties
```
CompileTarget: CompileTarget
CoverageInfo: bool
DebugInfo: bool
PackAsSource: bool
RawBytecode: bool [Deprecated]
```

---

# ScriptChangeService
**Extends:** Instance

## Events
```
ScriptAdded(script: LuaSourceContainer)
ScriptBeingRemoved(script: LuaSourceContainer)
ScriptChanged(script: LuaSourceContainer, property: string)
ScriptFullNameChanged(script: LuaSourceContainer)
ScriptSourceChanged(script: LuaSourceContainer)
```

---

# ScriptCloneWatcher
**Extends:** Instance

---

# ScriptCloneWatcherHelper
**Extends:** Instance

---

# ScriptCommitService
**Extends:** Instance

---

# ScriptContext
**Extends:** Instance

## Properties
```
ScriptsDisabled: bool
```

## Functions
```
AddCoreScriptLocal(name: string, parent: Instance) → null
CompressLuaApp() → null
GetCoverageStats() → Array
GetLuauHeapInstanceReferenceReport(target: string) → Dictionary
GetLuauHeapMemoryReport(target: string) → Dictionary
ReportLuaRequireCount() → null
SetTimeout(seconds: double) → null
```

## Events
```
Error(message: string, stackTrace: string, script: Instance)
ErrorDetailed(message: string, stackTrace: string, script: Instance, details: string, securityLevel: int, messageId: string)
```

---

# ScriptDebugger
**Extends:** Instance

## Properties
```
CoreScriptIdentifier: string
CurrentLine: int [ReadOnly]
IsDebugging: bool [ReadOnly]
IsPaused: bool [ReadOnly]
Script: Instance [ReadOnly]
ScriptGuid: string
```

## Functions
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

## Events
```
BreakpointAdded(breakpoint: Instance)
BreakpointRemoved(breakpoint: Instance)
EncounteredBreak(line: int, breakReason: BreakReason)
Resuming()
WatchAdded(watch: Instance)
WatchRemoved(watch: Instance)
```

---

# ScriptDocument
**Extends:** Instance

## Functions
```
GetInternalUri() → string
GetLine(lineIndex: int?) → string
GetLineCount() → int
GetScript() → LuaSourceContainer
GetSelectedText() → string
GetSelection() → Tuple
GetSelectionEnd() → Tuple
GetSelectionStart() → Tuple
GetText(startLine: int?, startCharacter: int?, endLine: int?, endCharacter: int?) → string
GetViewport() → Tuple
HasSelectedText() → bool
IsCommandBar() → bool
CloseAsync() → Tuple
EditTextAsync(newText: string, startLine: int, startCharacter: int, endLine: int, endCharacter: int) → Tuple
ForceSetSelectionAsync(cursorLine: int, cursorCharacter: int, anchorLine: int?, anchorCharacter: int?) → Tuple
MultiEditTextAsync(edits: Array) → Tuple
RequestSetSelectionAsync(cursorLine: int, cursorCharacter: int, anchorLine: int?, anchorCharacter: int?) → Tuple
```

## Events
```
SelectionChanged(positionLine: int64, positionCharacter: int64, anchorLine: int64, anchorCharacter: int64)
ViewportChanged(startLine: int64, endLine: int64)
```

---

# ScriptEditorService
**Extends:** Instance

## Functions
```
DeregisterAutocompleteCallback(name: string) → null
DeregisterScriptAnalysisCallback(name: string) → null
FindScriptDocument(script: LuaSourceContainer) → ScriptDocument
ForceReloadSource(uri: string, newsrc: string) → null
GetEditorSource(script: LuaSourceContainer) → string
GetScriptDocuments() → Instances
IsAutocompleteCallbackRegistered(name: string) → bool
IsScriptAnalysisCallbackRegistered(name: string) → bool
RegisterAutocompleteCallback(name: string, priority: int, callbackFunction: Function) → null
RegisterScriptAnalysisCallback(name: string, priority: int, callbackFunction: Function) → null
StripComments(code: string) → string
EditSourceAsyncWithRanges(script: LuaSourceContainer, newText: string, startLine: int, startCharacter: int, endLine: int, endCharacter: int) → Tuple
OpenScriptDocumentAsync(script: LuaSourceContainer, options: Dictionary) → Tuple
UpdateSourceAsync(script: LuaSourceContainer, callback: Function) → null
```

## Events
```
TextDocumentDidChange(document: ScriptDocument, changesArray: Variant)
TextDocumentDidClose(oldDocument: ScriptDocument)
TextDocumentDidOpen(newDocument: ScriptDocument)
```

---

# ScriptProfilerService
**Extends:** Instance

## Functions
```
ClientRequestData(player: Player) → null
ClientStart(player: Player, frequency: int?) → null
ClientStop(player: Player) → null
DeserializeJSON(jsonString: string?) → Dictionary
SaveScriptProfilingData(jsonString: string, filename: string) → string
ServerRequestData() → null
ServerStart(frequency: int?) → null
ServerStop() → null
```

## Events
```
OnNewData(player: Player, jsonString: string)
RequestData()
SetProfilingState(start: bool, frequency: int)
```

---

# ScriptRegistrationService
**Extends:** Instance

## Functions
```
GetSourceContainerByScriptGuid(guid: string) → LuaSourceContainer
```

---

# ScriptRuntime
**Extends:** Instance

---

# ScriptService
**Extends:** Instance

---

# Selection
**Extends:** Instance

## Properties
```
ActiveInstance: Instance [ReadOnly]
RenderMode: SelectionRenderMode [ReadOnly]
SelectionBoxThickness: float [ReadOnly]
SelectionLineThickness: int [ReadOnly]
SelectionThickness: float [ReadOnly]
ShowActiveInstanceHighlight: bool
```

## Functions
```
Add(instancesToAdd: Instances) → null
AddFocusCallback(priority: int, function: Function) → RBXScriptConnection
ClearTerrainSelectionHack() → null
Get() → Instances
Remove(instancesToRemove: Instances) → null
Set(selection: Instances) → null
SetTerrainSelectionHack(center: Vector3, size: Vector3) → null
```

## Events
```
SelectionChanged()
SelectionChangedThisFrame()
```

---

# SelectionHighlightManager
**Extends:** Instance

---

# SensorBase
**Extends:** Instance

## Properties
```
UpdateType: SensorUpdateType
```

## Functions
```
Sense() → null [Deprecated]
```

## Events
```
OnSensorOutputChanged()
```

---

# AtmosphereSensor
**Extends:** SensorBase

## Properties
```
AirDensity: float [ReadOnly]
RelativeWindVelocity: Vector3 [ReadOnly]
```

---

# BuoyancySensor
**Extends:** SensorBase

## Properties
```
FullySubmerged: bool
TouchingSurface: bool
```

---

# ControllerSensor
**Extends:** SensorBase

---

# ControllerPartSensor
**Extends:** ControllerSensor

## Properties
```
HitFrame: CFrame
HitNormal: Vector3
SearchDistance: float
SensedPart: BasePart
SensorMode: SensorMode
```

---

# FluidForceSensor
**Extends:** SensorBase

## Properties
```
CenterOfPressure: Vector3 [ReadOnly]
Force: Vector3 [ReadOnly]
Torque: Vector3 [ReadOnly]
```

## Functions
```
EvaluateAsync(linearVelocity: Vector3, angularVelocity: Vector3, cframe: CFrame) → Tuple
```

---

# SerializationService
**Extends:** Instance

## Functions
```
DeserializeInstancesAsync(buffer: buffer) → Instances
SerializeInstancesAsync(inputInstances: Instances) → buffer
```

---

# ServerScriptService
**Extends:** Instance

## Properties
```
LoadStringEnabled: bool
```

---

# ServerStorage
**Extends:** Instance

---

# ServiceProvider
**Extends:** Instance

## Functions
```
FindService(className: string) → Instance
GetService(className: string) → Instance
getService(className: string) → Instance [Deprecated]
service(className: string) → Instance [Deprecated]
```

## Events
```
Close()
CloseLate()
ServiceAdded(service: Instance)
ServiceRemoving(service: Instance)
```

---

# DataModel
**Extends:** ServiceProvider

## Properties
```
CreatorId: int64 [ReadOnly]
CreatorType: CreatorType [ReadOnly]
Environment: string [ReadOnly]
ForceR15: bool
GameAvatarType: GameAvatarType [Deprecated]
GameId: int64 [ReadOnly]
GearGenreSetting: GearGenreSetting [ReadOnly] [Deprecated]
Genre: Genre [ReadOnly]
IsSFFlagsLoaded: bool [ReadOnly]
JobId: string [ReadOnly]
MatchmakingType: MatchmakingType [ReadOnly]
PlaceId: int64 [ReadOnly]
PlaceVersion: int [ReadOnly]
PrivateServerId: string [ReadOnly]
PrivateServerOwnerId: int64 [ReadOnly]
R15CollisionType: R15CollisionType [Deprecated]
VIPServerId: string [ReadOnly] [Deprecated]
VIPServerOwnerId: int64 [ReadOnly] [Deprecated]
Workspace: Workspace [ReadOnly]
lighting: Instance [ReadOnly] [Deprecated]
workspace: Workspace [ReadOnly] [Deprecated]
```

## Functions
```
BindToClose(function: Function) → null
DefineFastFlag(name: string, defaultValue: bool) → bool
DefineFastInt(name: string, defaultValue: int) → int
DefineFastString(name: string, defaultValue: string) → string
GetEngineFeature(name: string) → bool
GetFastFlag(name: string) → bool
GetFastInt(name: string) → int
GetFastString(name: string) → string
GetJobsInfo() → Array
GetMessage() → string [Deprecated]
GetObjects(url: ContentId) → Instances
GetObjectsAllOrNone(url: ContentId, binaryFormatOnly: bool) → Instances
GetObjectsList(urls: Array) → Array
GetPlaySessionId() → string
GetRemoteBuildMode() → bool [Deprecated]
IsContentLoaded() → bool
IsGearTypeAllowed(gearType: GearType) → bool [Deprecated]
IsLoaded() → bool
IsUniverseMetadataLoaded() → bool
Load(url: ContentId) → null
OpenScreenshotsFolder() → null
OpenVideosFolder() → null
ReportInGoogleAnalytics(category: string, action: string, label: string, value: int) → null
SetFastFlagForTesting(name: string, newValue: bool) → bool
SetFastIntForTesting(name: string, newValue: int) → int
SetFastStringForTesting(name: string, newValue: string) → string
SetFlagVersion(name: string, version: int) → null
SetIsLoaded(value: bool, placeSizeInBytes: int?) → null
SetPlaceId(placeId: int64) → null
SetUniverseId(universeId: int64) → null
Shutdown() → null
GetObjectsAsync(url: ContentId) → Instances
HttpGetAsync(url: string, httpRequestType: HttpRequestType) → string
HttpPostAsync(url: string, data: string, contentType: string, httpRequestType: HttpRequestType) → string
InsertObjectsAndJoinIfLegacyAsync(url: ContentId) → Instances
SavePlace(saveFilter: SaveFilter) → bool [Deprecated]
```

## Events
```
AllowedGearTypeChanged()
GraphicsQualityChangeRequest(betterQuality: bool)
ItemChanged(object: Instance, descriptor: string)
Loaded()
ScreenshotReady(path: string)
ScreenshotSavedToAlbum(filename: string, success: bool, message: string)
UniverseMetadataLoaded()
```

---

# GenericSettings
**Extends:** ServiceProvider

---

# GlobalSettings
**Extends:** GenericSettings

## Functions
```
GetFFlag(name: string) → bool
GetFFlagOverrides() → string
GetFFlags() → string
GetFVariable(name: string) → string
SetFFlagOverrides(overrides: string) → bool
```

---

# UserSettings
**Extends:** GenericSettings

## Functions
```
IsUserFeatureEnabled(name: string) → bool
Reset() → null
SaveState() → null
```

---

# ServiceVisibilityService
**Extends:** Instance

## Properties
```
HiddenServices: BinaryString
VisibleServices: BinaryString
```

## Functions
```
SetServiceVisibilityPreference(service: Instance, visible: bool) → null
```

## Events
```
ServiceVisibilityChanged(serviceName: string)
```

---

# SessionCheckService
**Extends:** Instance

---

# SessionService
**Extends:** Instance

## Functions
```
AcquireContextFocus(context: string) → null
GenerateSessionInfoString(includeArbitrarySessions: bool, includeTag: bool, includeTimestamps: bool, includeMetadata: bool) → string
GetCreatedTimestampUtcMs(sid: string) → int64
GetMetadata(sid: string, key: string) → Variant
GetRootSID() → string
GetSessionID(structuralId: string) → string
GetSessionTag(sid: string) → string
IsContextFocused(context: string) → bool
ReleaseContextFocus(context: string) → null
RemoveMetadata(sid: string, key: string, context: string) → null
RemoveSession(sid: string, context: string) → null
RemoveSessionsWithMetadataKey(key: string) → null
ReplaceSession(sid: string, tag: string) → null
SessionExists(sid: string) → bool
SetMetadata(sid: string, key: string, value: Variant, context: string) → null
SetSession(parentSid: string, childSid: string, tag: string, context: string) → null
```

---

# SharedTableRegistry
**Extends:** Instance

## Functions
```
GetSharedTable(name: string) → SharedTable
SetSharedTable(name: string, st: SharedTable?) → null
```

---

# Sky
**Extends:** Instance

## Properties
```
CelestialBodiesShown: bool
MoonAngularSize: float
MoonTextureId: ContentId
SkyboxBk: ContentId
SkyboxDn: ContentId
SkyboxFt: ContentId
SkyboxLf: ContentId
SkyboxOrientation: Vector3
SkyboxRt: ContentId
SkyboxUp: ContentId
StarCount: int
SunAngularSize: float
SunTextureId: ContentId
```

---

# SlimService
**Extends:** Instance

---

# Smoke
**Extends:** Instance

## Properties
```
Color: Color3
Enabled: bool
LocalTransparencyModifier: float
Opacity: float
RiseVelocity: float
Size: float
TimeScale: float
opacity_xml: float
riseVelocity_xml: float
size_xml: float
```

## Functions
```
FastForward(numFrames: int) → null
```

---

# SmoothVoxelsUpgraderService
**Extends:** Instance

## Functions
```
Cancel() → null
Start() → null
```

## Events
```
Status(progressRatio: float)
```

---

# SnippetService
**Extends:** Instance

---

# SocialService
**Extends:** Instance

## Functions
```
GetPlayersByPartyId(partyId: string) → Instances
HideSelfView() → null
InvokeGameInvitePromptClosed(player: Instance, recipientIds: Array) → null
InvokeIrisInvite(player: Instance, tag: string, irisParticipants: Array) → null
InvokeIrisInvitePromptClosed(player: Instance) → null
InvokeShareSheetClosed() → null
PromptGameInvite(player: Instance, experienceInviteOptions: Instance) → null
PromptPhoneBook(player: Instance, tag: string) → null
PromptRsvpToEventCompleted(eventId: string, success: bool, rsvpStatus: RsvpStatus) → null
ShowSelfView(selfViewPosition: SelfViewPosition) → null
UpdatePlayerPartyData(partyId: string) → null
CanSendCallInviteAsync(player: Instance) → bool
CanSendGameInviteAsync(player: Instance, recipientId: int64) → bool
GetEventRsvpStatusAsync(eventId: string) → RsvpStatus
GetPartyAsync(partyId: string) → Array
PromptLinkSharing(player: Player, options: Dictionary) → Tuple
PromptRsvpToEventAsync(eventId: string) → RsvpStatus
```

## Events
```
CallInviteStateChanged(player: Instance, inviteState: InviteState)
GameInvitePromptClosed(player: Instance, recipientIds: Array)
IrisInviteInitiated(message: string)
OpenShareSheetWithLink(link: string)
PhoneBookPromptClosed(player: Instance)
PlayerPartyDataChanged(partyId: string)
PromptInviteRequested(player: Instance, experienceInviteOptions: Instance)
PromptIrisInviteRequested(player: Instance, tag: string)
SelfViewHidden()
SelfViewVisible(selfViewPosition: SelfViewPosition)
ShareSheetClosed(player: Player)
ShowPromptRsvpToEvent(eventId: string)
```

---

# Sound
**Extends:** Instance

## Properties
```
ChannelCount: int [ReadOnly]
EmitterSize: float [Deprecated]
IsLoaded: bool [ReadOnly]
IsMutedForCapture: bool
IsPaused: bool [ReadOnly]
IsPlaying: bool [ReadOnly]
IsSpatial: bool [ReadOnly]
LoopRegion: NumberRange
Looped: bool
MaxDistance: float [Deprecated]
MinDistance: float [Deprecated]
Pitch: float [Deprecated]
PlayOnRemove: bool
PlaybackLoudness: double [ReadOnly]
PlaybackRegion: NumberRange
PlaybackRegionsEnabled: bool
PlaybackSpeed: float
Playing: bool
PlayingReplicator: bool
RollOffGain: float [ReadOnly]
RollOffMaxDistance: float
RollOffMinDistance: float
RollOffMode: RollOffMode
SoundGroup: SoundGroup
SoundId: ContentId
TimeLength: double [ReadOnly]
TimePosition: double
TimePositionReplicator: double
UsageContextPermission: UsageContext
Volume: float
isPlaying: bool [ReadOnly] [Deprecated]
xmlRead_MaxDistance_3: float [Deprecated]
xmlRead_MinDistance_3: float [Deprecated]
```

## Functions
```
Pause() → null
Play() → null
Resume() → null
Stop() → null
pause() → null [Deprecated]
play() → null [Deprecated]
stop() → null [Deprecated]
```

## Events
```
DidLoop(soundId: string, numOfTimesLooped: int)
Ended(soundId: string)
Loaded(soundId: string)
Paused(soundId: string)
Played(soundId: string)
PlayingUpdatedFromClient(value: bool)
PlayingUpdatedFromServer(value: bool)
Resumed(soundId: string)
Stopped(soundId: string)
TimePositionUpdatedFromClient(newPositionSeconds: double, lastLuaSetTimePosition: double)
TimePositionUpdatedFromServer(newPositionSeconds: double, lastLuaSetTimePosition: double)
playbackActionSync(action: int)
```

---

# SoundEffect
**Extends:** Instance

## Properties
```
Enabled: bool
Priority: int
```

---

# ChorusSoundEffect
**Extends:** SoundEffect

## Properties
```
Depth: float
Mix: float
Rate: float
```

---

# CompressorSoundEffect
**Extends:** SoundEffect

## Properties
```
Attack: float
GainMakeup: float
Ratio: float
Release: float
SideChain: Instance
Threshold: float
```

---

# CustomSoundEffect
**Extends:** SoundEffect

---

# AssetSoundEffect
**Extends:** CustomSoundEffect

---

# ChannelSelectorSoundEffect
**Extends:** CustomSoundEffect

## Properties
```
Channel: int
```

---

# DistortionSoundEffect
**Extends:** SoundEffect

## Properties
```
Level: float
```

---

# EchoSoundEffect
**Extends:** SoundEffect

## Properties
```
Delay: float
DryLevel: float
Feedback: float
WetLevel: float
```

---

# EqualizerSoundEffect
**Extends:** SoundEffect

## Properties
```
HighGain: float
LowGain: float
MidGain: float
```

---

# FlangeSoundEffect
**Extends:** SoundEffect

## Properties
```
Depth: float
Mix: float
Rate: float
```

---

# PitchShiftSoundEffect
**Extends:** SoundEffect

## Properties
```
Octave: float
```

---

# ReverbSoundEffect
**Extends:** SoundEffect

## Properties
```
DecayTime: float
Density: float
Diffusion: float
DryLevel: float
WetLevel: float
```

---

# TremoloSoundEffect
**Extends:** SoundEffect

## Properties
```
Depth: float
Duty: float
Frequency: float
```

---

# SoundGroup
**Extends:** Instance

## Properties
```
Volume: float
```

---

# SoundService
**Extends:** Instance

## Properties
```
AmbientReverb: ReverbType
AudioApiByDefault: RolloutState
CharacterSoundsUseNewApi: RolloutState
DefaultListenerLocation: ListenerLocation
DistanceFactor: float
DopplerScale: float
IsNewExpForAudioApiByDefault: bool
RespectFilteringEnabled: bool
RolloffScale: float
VolumetricAudio: VolumetricAudio
```

## Functions
```
BeginRecording() → bool
GetAudioApiByDefault() → bool
GetAudioInstances() → Array
GetInputDevice() → Tuple
GetInputDevices() → Tuple
GetListener() → Tuple
GetOutputDevice() → Tuple
GetOutputDevices() → Tuple
GetSoundMemoryData() → Dictionary
InsertAsset(assetId: ContentId, assetName: string, useSelection: bool) → Instances
OpenAttenuationCurveEditor(selectedCurveObjects: Instances) → null
OpenDirectionalCurveEditor(selectedCurveObjects: Instances) → null
PlayLocalSound(sound: Instance) → null
SetAudioApiByDefault(enabled: bool) → null
SetInputDevice(name: string, guid: string) → null
SetListener(listenerType: ListenerType, listener: Tuple) → null
SetOutputDevice(name: string, guid: string) → null
SetRecordingDevice(deviceIndex: int) → bool
SetSoundEnabled(enabled: bool) → null
EndRecording() → Dictionary
GetRecordingDevices() → Dictionary
```

## Events
```
AudioInstanceAdded(instance: Instance)
ClientLoggedEvent(sessionIdRaw: string)
DeviceListChanged(newDevices: Tuple)
OpenAttenuationCurveEditorSignal(selectedCurveObjects: Instances)
OpenAudioCompressorEditorSignal(selectedCompressorObjects: Instances)
OpenAudioEqualizerEditorSignal(selectedEqualizerObjects: Instances)
OpenDirectionalCurveEditorSignal(selectedCurveObjects: Instances)
```

---

# Sparkles
**Extends:** Instance

## Properties
```
Color: Color3
Enabled: bool
LocalTransparencyModifier: float
SparkleColor: Color3
TimeScale: float
```

## Functions
```
FastForward(numFrames: int) → null
```

---

# SpawnerService
**Extends:** Instance

---

# StackFrame
**Extends:** Instance

## Properties
```
FrameId: int [ReadOnly]
FrameName: string [ReadOnly]
FrameType: DebuggerFrameType [ReadOnly]
Globals: DebuggerVariable [ReadOnly]
Line: int [ReadOnly]
Locals: DebuggerVariable [ReadOnly]
Populated: bool [ReadOnly]
Script: string [ReadOnly]
Upvalues: DebuggerVariable [ReadOnly]
```

---

# StandalonePluginScripts
**Extends:** Instance

---

# StartPageService
**Extends:** Instance

## Functions
```
generateTempUrlInContentProvider(url: string) → null
getDaysSinceFirstUserLogin() → int
getLocalGamesFromRegistry() → Array
getRecentAPIGamesFromRegistry() → Array
getTempUrlInContentProvider(url: string) → string
isTutorialBannerClosed() → bool
isTutorialPopupClosed() → bool
openLink(link: string) → null
openLocalFile(filePath: string) → null
openPlace(placeId: int64, universeId: int64, launchTutorial: bool) → null
removeAPIGameFromRegistry(gameId: int64) → null
removeLocalFileFromRegistry(fileName: string) → null
setTutorialBannerClosed(closed: bool) → null
setTutorialPopupClosed(closed: bool) → null
shouldShowMacOSDeprecationWarning() → bool
shouldShowWinOSDeprecationWarning() → bool
startTutorial() → null
```

## Events
```
ImageImportedSignal(urlImported: string, temporaryId: string)
LocalGamesFromRegistryUpdatedSignal(localGames: Array)
RecentApiGamesFromRegistryUpdatedSignal(recentGames: Array)
```

---

# StarterGear
**Extends:** Instance

---

# StarterPack
**Extends:** Instance

---

# StarterPlayer
**Extends:** Instance

## Properties
```
AllowCustomAnimations: bool
AutoJumpEnabled: bool
AvatarJointUpgrade: RolloutState
AvatarJointUpgrade_SerializedRollout: RolloutState
CameraMaxZoomDistance: float
CameraMinZoomDistance: float
CameraMode: CameraMode
CharacterJumpHeight: float
CharacterJumpPower: float
CharacterMaxSlopeAngle: float
CharacterUseJumpPower: bool
CharacterWalkSpeed: float
ClassicDeath: bool
DevCameraOcclusionMode: DevCameraOcclusionMode
DevComputerCameraMovementMode: DevComputerCameraMovementMode
DevComputerMovementMode: DevComputerMovementMode
DevTouchCameraMovementMode: DevTouchCameraMovementMode
DevTouchMovementMode: DevTouchMovementMode
EnableDynamicHeads: LoadDynamicHeads
EnableMouseLockOption: bool
GameSettingsAssetIDFace: int64
GameSettingsAssetIDHead: int64
GameSettingsAssetIDLeftArm: int64
GameSettingsAssetIDLeftLeg: int64
GameSettingsAssetIDPants: int64
GameSettingsAssetIDRightArm: int64
GameSettingsAssetIDRightLeg: int64
GameSettingsAssetIDShirt: int64
GameSettingsAssetIDTeeShirt: int64
GameSettingsAssetIDTorso: int64
GameSettingsAvatar: GameAvatarType
GameSettingsR15Collision: R15CollisionType
GameSettingsScaleRangeBodyType: NumberRange
GameSettingsScaleRangeHead: NumberRange
GameSettingsScaleRangeHeight: NumberRange
GameSettingsScaleRangeProportion: NumberRange
GameSettingsScaleRangeWidth: NumberRange
HealthDisplayDistance: float
LoadCharacterAppearance: bool
LoadCharacterLayeredClothing: LoadCharacterLayeredClothing
LoadCharacterLayeredClothing : LoadCharacterLayeredClothing
LuaCharacterController: CharacterControlMode
NameDisplayDistance: float
RagdollDeath: bool
UserEmotesEnabled: bool
```

## Functions
```
ClearDefaults() → null
```

---

# StarterPlayerScripts
**Extends:** Instance

---

# StarterCharacterScripts
**Extends:** StarterPlayerScripts

---

# StartupMessageService
**Extends:** Instance

## Functions
```
GetStartupMessage() → Variant
```

---

# Stats
**Extends:** Instance

## Properties
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

## Functions
```
GetBrowserTrackerId() → string
GetHarmonyQualityLevel() → int
GetMemoryCategoryNames() → Array
GetMemoryUsageMbAllCategories() → Array
GetMemoryUsageMbForTag(tag: DeveloperMemoryTag) → float
GetTotalMemoryUsageMb() → float
ResetHarmonyMemoryTarget() → null
SetHarmonyMemoryTarget(targetMB: int) → null
GetPaginatedMemoryByTexture(queryType: TextureQueryType, pageIndex: int, pageSize: int) → Dictionary
```

---

# StatsItem
**Extends:** Instance

## Properties
```
DisplayName: string [ReadOnly]
```

## Functions
```
GetValue() → double
GetValueString() → string
```

---

# RunningAverageItemDouble
**Extends:** StatsItem

---

# RunningAverageItemInt
**Extends:** StatsItem

---

# RunningAverageTimeIntervalItem
**Extends:** StatsItem

---

# TotalCountTimeIntervalItem
**Extends:** StatsItem

---

# StopWatchReporter
**Extends:** Instance

## Functions
```
FinishTask(taskId: int) → null
SendReport(reportName: string) → null
StartTask(reportName: string, taskName: string) → int
```

---

# StreamingService
**Extends:** Instance

## Functions
```
GetEphemeralVariable(key: string) → Variant
GetInstance(requestId: string, instanceId: string) → Instance
InvokeCommand(requestId: string, commandName: string, arg: Variant) → null
RegisterCommandInternal(commandName: string, function: Function, isSequential: bool, isPublic: bool) → null
RegisterContextCollector(collectorName: string, function: Function) → null
SetEphemeralVariable(key: string, value: Variant, timeToLive: int) → null
SetPluginInfoCallback(function: Function) → null
UnregisterCommand(commandName: string) → null
UnregisterContextCollector(collectorName: string) → null
AttemptSaveAndSendPlaceTelemetry(requestId: string, toolSource: string) → null
BindCodeToGuid(runCodeGuid: string, code: string) → Tuple
ExecuteCommandAsync(requestId: string, commandName: string, arg: Variant) → Variant
GetRequiredScripts(script: Instance) → Variant
RunSandboxedCode(runCodeGuid: string, requestId: string) → Tuple
SearchForAssets(body: Variant) → Variant
```

## Events
```
ConversationCleared()
RequestEnded(requestId: string)
RequestError(requestId: string, errorType: string, errorMessage: string)
RequestStarted(requestId: string, queryToProcess: string)
SequentialCommandsFinished(requestId: string, success: bool)
Stream(requestId: string, commandName: string, streamContent: string)
```

---

# Studio
**Extends:** Instance

## Properties
```
"TODO" Color: Color3
"function" Color: Color3
"local" Color: Color3
"nil" Color: Color3
"self" Color: Color3
ActionOnAutoResumeSync: ActionOnAutoResumeSync
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
AutoResumeSyncOnPlaceOpen: bool
AutocompleteAcceptanceBehavior: CompletionAcceptanceBehavior
Automatically trigger AI Code Completion: bool
Background Color: Color3
Basic Objects Display Mode: ListDisplayMode
Bool Color: Color3
Bracket Color: Color3
Built-in Function Color: Color3
Camera Mouse Wheel Speed: float
Camera Pan Speed: float
Camera Shift Speed: float
Camera Speed: float
Camera Speed Adjust Binding: CameraSpeedAdjustBinding
Camera Zoom to Mouse Position: bool
CameraAdaptiveSpeed: bool
CameraOrbitSensitivity: float
CameraPanSensitivity: float
CameraShiftFactor: float
CameraSpeedLockDefault: bool
CameraTweenFocus: bool
CameraZoomSpeed: float
Clear Output On Start: bool
CommandBarLocalState: bool
Comment Color: Color3
Current Line Highlight Color: Color3
Debugger Current Line Color: Color3
Debugger Error Line Color: Color3
DeprecatedObjectsShown: bool
DisplayLanguage: string
Doc View Code Background Color: Color3
DraggerActiveColor: Color3
DraggerMajorGridIncrement: int
DraggerMaxSoftSnaps: int
DraggerPassiveColor: Color3
DraggerShowHoverRuler: bool
DraggerShowMeasurement: bool
DraggerShowTargetSnap: bool
DraggerSoftSnapMarginFactor: float
DraggerSummonMarginFactor: float
DraggerTiltRotateDuration: float
Enable Autocomplete: bool
Enable Autocomplete Doc View: bool
Enable CoreScript Debugger: bool
Enable Http Sandboxing: bool
Enable Internal Beta Features: bool
Enable Internal Features: bool
Enable Script Analysis: bool
Enable Scrollbar Markers: bool
Enable Signature Help: bool
Enable Signature Help Doc View: bool
Enable Temporary Tabs: bool
Enable Temporary Tabs In Explorer: bool
Enable Type Hover: bool
EnableCodeAssist: bool
EnableIndentationRulers: bool
EnableOnTypeAutocomplete: bool
EnableSelectionTooltips: bool
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
Hover Box Thickness: float
Hover Line Thickness: int
Hover Over Color: Color3
IconOverrideDir: QDir
Indent Using Spaces: bool
IndentationRulerColor: Color3
InformationColor: Color3
Keyword Color: Color3
LargeFileLineCountThreshold: int
LargeFileThreshold: int
Line Thickness: float
LoadAllBuiltinPluginsInRunModes: bool
LoadInternalPlugins: bool
LoadUserPluginsInRunModes: bool
LocalAssetsFolder: QDir
LuaDebuggerEnabled: bool
LuaDebuggerEnabledAtStartup: bool [ReadOnly]
Luau Keyword Color: Color3
Main Volume: float
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
Physical Draggers Select Scope By Default: bool
Pivot Snap To Geometry Color: Color3
PluginDebuggingEnabled: bool
PluginsDir: QDir
Primary Text Color: Color3
Property Color: Color3
ReloadBuiltinPluginsOnChange: bool
ReloadLocalPluginsOnChange: bool
Respect Studio shortcuts when game has focus: bool
Ruler Color: Color3
Rulers: string
RuntimeUndoBehavior: RuntimeUndoBehavior
Script Editor Color Preset: StudioScriptEditorColorPresets
Script Editor Scrollbar Background Color: Color3
Script Editor Scrollbar Handle Color: Color3
ScriptEditorMenuBorderColor: Color3
ScriptEditorShouldShowPluginMethods: bool
ScriptTimeoutLength: int
Scroll Past Last Line: bool
Secondary Text Color: Color3
Select Color: Color3
Select/Hover Color: Color3
Selected Menu Item Background Color: Color3
Selected Text Color: Color3
Selection Background Color: Color3
Selection Box Thickness: float
Selection Color: Color3
Selection Line Thickness: int
Set Pivot of Imported Parts: bool
Show Core GUI in Explorer while Playing: bool
Show Diagnostics Bar: bool
Show FileSyncService: bool
Show Hidden Objects in Explorer: bool
Show Hover Over: bool
Show Light Guides: bool
Show Navigation Labels: bool
Show Navigation Mesh: bool
Show Pathfinding Links: bool
Show Plugin GUI Service in Explorer: bool
Show Singly Selected Attachment Parent Frame: bool
Show Whitespace: bool
Show plus button on hover in Explorer: bool
ShowCorePackagesInExplorer: bool
Skip Closing Brackets and Quotes: bool
String Color: Color3
Tab Width: int
Text Color: Color3
Text Wrapping: bool
Theme: Instance
TypeColor: Color3
UI Theme: UITheme [ReadOnly] [Deprecated]
Use Bounding Box Move Handles: bool
Warning Color: Color3
Whitespace Color: Color3
```

## Functions
```
GetAvailableThemes() → Array
```

## Events
```
ThemeChanged()
```

---

# StudioAssetService
**Extends:** Instance

## Functions
```
ConvertToPackageUpload(uploadUrl: string, cloneInstances: Instances, originalInstances: Instances) → null
FireOnUGCSubmitCompleted(cancelled: bool) → null
PublishPackage(instance: Instance, publishInfo: Dictionary) → null
ShowSaveToRoblox(instances: Instances, assetType: Variant, hasSubsequent: bool) → null
UpdatePublishedPackage(assetmetadata: Dictionary, rootInstance: Instance, isConvert: bool, addUndoWaypoint: bool) → null
AutoSetupAvatarAsync(modelId: ContentId, progressCallback: Function, notificationCallback: Function?) → Instance
AutoSetupSerializedAvatarAsync(serializedInstance: string, publishInfo: Dictionary, telemetryMetadata: Dictionary, progressCallback: Function, notificationCallback: Function?) → Instance
CancelAutoSetupAvatarAsync(jobId: string) → null
DEPRECATED_SerializeInstances(instances: Instances) → string
RequestAvatarAutosetupAsync(meshId: ContentId, textureId: ContentId, progressCallback: Function) → Instance
SerializeInstances(instances: Instances, groupId: int64, isPackage: bool) → string
```

## Events
```
OnConvertToPackageResult(isSuccessful: bool, errorMessage: string)
OnPublishPackageResult(result: Dictionary, errorMessage: string)
OnSaveToRoblox(instances: Instances, assetType: Variant, hasSubsequent: bool)
OnUGCSubmitCompleted(cancelled: bool)
```

---

# StudioAttachment
**Extends:** Instance

## Properties
```
AutoHideParent: bool
IsArrowVisible: bool
Offset: Vector2
SourceAnchorPoint: Vector2
TargetAnchorPoint: Vector2
```

---

# StudioCallout
**Extends:** Instance

## Properties
```
AnchorPoint: Vector2
IsArrowVisible: bool
IsNextVisible: bool
RowName: string
Text: string
Title: string
```

## Functions
```
SetOnNextClicked(onClick: Function) → null
```

---

# StudioCameraService
**Extends:** Instance

## Properties
```
LockCameraSpeed: bool
```

## Events
```
ShowCameraSpeed(speed: float)
```

---

# StudioData
**Extends:** Instance

## Properties
```
EnableScriptCollabByDefaultOnLoad: bool
```

---

# StudioDeviceEmulatorService
**Extends:** Instance

## Properties
```
HasMultiTouchStarted: bool [ReadOnly]
IsMultiTouchEmulationOn: bool
IsMultiTouchEnabled: bool [ReadOnly]
PivotPosition: Vector2 [ReadOnly]
```

## Functions
```
GetMaxNumTouches() → int
GetTouchInBounds(index: int) → bool
GetTouchPosition(index: int) → Vector2
EmulatePCDeviceWithResolution(deviceId: string, resolution: Vector2) → bool
GetCurrentDeviceId() → string
GetCurrentOrientation() → ScreenOrientation
HasDeviceWithId(deviceId: string) → bool
SetCurrentDeviceId(deviceId: string) → null
SetCurrentOrientation(orientation: ScreenOrientation) → null
```

## Events
```
CurrentDeviceIdChanged()
OrientationChanged()
TouchInBoundsChanged()
TouchPositionsChanged()
```

---

# StudioObjectBase
**Extends:** Instance

---

# StudioWidget
**Extends:** StudioObjectBase

## Functions
```
SetFixedSize(width: int, height: int) → null
```

---

# StudioPublishService
**Extends:** Instance

## Properties
```
PublishLocked: bool
```

## Functions
```
ClearUploadNames() → null
CloseAfterPublish(closeMode: StudioCloseMode) → null
PublishAs(universeId: int64, placeId: int64, groupId: int64, isPublish: bool, publishParameters: Variant, willRetryOnConflict: bool, allowOpeningNewPlace: bool) → null
PublishThenTurnOnTeamCreate() → null
RefreshDocumentDisplayName() → null
RegisterPublishHold(priority: int, callback: Function) → RBXScriptConnection
SetTeamCreateOnPublishInfo(shouldTurnOnTcOnPublish: bool, newPlaceName: string) → null
SetUniverseDisplayName(newName: string) → null
SetUploadNames(placeName: string, universeName: string) → null
ShowSaveOrPublishPlaceToRoblox(showGameSelect: bool, isPublish: bool, closeMode: StudioCloseMode) → null
```

## Events
```
GameNameUpdated(name: string)
GamePublishCancelled()
GamePublishFinished(success: bool, gameId: int64, message: string, reason: StudioPlaceUpdateFailureReason)
OnPublishAttempt(isPublishAs: bool)
OnSaveOrPublishPlaceToRoblox(showGameSelect: bool, isPublish: bool, closeMode: StudioCloseMode)
```

---

# StudioScriptDebugEventListener
**Extends:** Instance

---

# StudioSdkService
**Extends:** Instance

## Functions
```
GetSdk() → Instance
SetSdk(sdk: Instance) → null
```

---

# StudioService
**Extends:** Instance

## Properties
```
ActiveScript: Instance [ReadOnly]
AlignDraggedObjects: bool
DraggerSolveConstraints: bool [ReadOnly]
DrawConstraintsOnTop: bool [ReadOnly] [Deprecated]
GridSize: float [ReadOnly]
HoverInstance: Instance
InstalledPluginData: string [ReadOnly]
PivotSnapToGeometry: bool [ReadOnly]
RotateIncrement: float [ReadOnly]
Secrets: string
ShowConstraintDetails: bool [ReadOnly]
ShowWeldDetails: bool [ReadOnly]
StudioLocaleId: string [ReadOnly]
UseLocalSpace: bool
```

## Functions
```
AnimationIdSelected(id: int64) → null
CopyToClipboard(stringToCopy: string) → null
GetBadgeConfigureUrl(badgeId: int64) → string
GetBadgeUploadUrl() → string
GetClassIcon(className: string) → Dictionary
GetPlaceIsPersistedToCloud() → bool
GetResourceByCategory(category: string) → Dictionary
GetStartupAssetId() → string
GetStartupPluginId() → string
GetTermsOfUseUrl() → string
GetUserId() → int64
GizmoRaycast(origin: Vector3, direction: Vector3, raycastParams: RaycastParams) → RaycastResult?
HasInternalPermission() → bool
IsPluginInstalled(assetId: int64) → bool
IsPluginUpToDate(assetId: int64, currentAssetVersion: int64) → bool
OpenInBrowser_DONOTUSE(url: string) → null
SetPluginEnabled(assetId: int64, state: bool) → null
ShowPlaceVersionHistoryDialog(placeId: int64) → null [Deprecated]
ShowPublishToRoblox() → null
UninstallPlugin(assetId: int64) → null
UpdatePluginManagement() → null
PromptImportFile(fileTypeFilter: Array) → Instance
PromptImportFiles(fileTypeFilter: Array) → Instances
TryInstallPlugin(assetId: int64, assetVersionId: int64) → null
```

## Events
```
OnImportFromRoblox()
OnOpenGameSettings(pageIdentifier: string)
OnOpenManagePackagePlugin(userId: int64, assetId: int64)
OnPluginInstalledFromToolbox()
OnPluginInstalledFromWeb(pluginId: string)
OnPublishAsPlugin(instances: Instances)
OnSaveToRoblox(instances: Instances)
PromptTransformPluginCheckEnable()
SaveLocallyAsComplete(success: bool)
```

---

# StudioTheme
**Extends:** Instance

## Functions
```
GetColor(styleguideitem: StudioStyleGuideColor, modifier: StudioStyleGuideModifier) → Color3
```

---

# StudioUserService
**Extends:** Instance

## Properties
```
IsLoggedIn: bool [ReadOnly]
```

---

# StudioWidgetsService
**Extends:** Instance

## Functions
```
ApplyFillInBox(target: StudioWidget) → null
ApplyHighlight(target: StudioWidget, rowName: string?) → null
ApplyShadows() → null
ApplySpotlight(target: StudioWidget, rowName: string?) → null
GetWidgetFromLabel(label: string) → StudioWidget
GetWidgetFromPluginGui(gui: PluginGui) → StudioWidget
HideSpotlight() → null
```

---

# StyleBase
**Extends:** Instance

## Functions
```
GetStyleRules() → Instances
InsertStyleRule(rule: StyleRule, priority: int?) → null
SetStyleRules(rules: Instances) → null
```

## Events
```
StyleRulesChanged()
```

---

# StyleRule
**Extends:** StyleBase

## Properties
```
Index: int
Priority: int
PropertiesSerialize: BinaryString
Selector: string
SelectorError: string [ReadOnly]
```

## Functions
```
GetProperties() → Dictionary
GetPropertiesResolved() → Dictionary
GetProperty(name: string) → Variant
GetPropertyResolved(name: string) → Variant
SetProperties(styleProperties: Dictionary) → null
SetProperty(name: string, value: Variant) → null
```

## Events
```
StyleRulePropertyChanged(styleProperty: string)
```

---

# StyleSheet
**Extends:** StyleBase

## Functions
```
GetDerives() → Instances
SetDerives(derives: Instances) → null
```

---

# StyleDerive
**Extends:** Instance

## Properties
```
Index: int
Priority: int
StyleSheet: StyleSheet
```

---

# StyleLink
**Extends:** Instance

## Properties
```
StyleSheet: StyleSheet
```

---

# StylingService
**Extends:** Instance

## Functions
```
GetAppliedStyles(instance: Instance) → Array
GetStyleInfo(style: StyleRule) → Dictionary
GetStyleSheetDerivesChain(styleSheet: StyleSheet) → Instances
GetStyleSheetInfo(styleSheet: StyleSheet) → Dictionary
UpdateUnitTestOnly() → null
```

---

# SurfaceAppearance
**Extends:** Instance

## Properties
```
AlphaMode: AlphaMode
Color: Color3
ColorMap: ContentId
ColorMapContent: Content
MetalnessMap: ContentId
MetalnessMapContent: Content
NormalMap: ContentId
NormalMapContent: Content
RoughnessMap: ContentId
RoughnessMapContent: Content
TexturePack: ContentId
```

---

# SystemThemeService
**Extends:** Instance

## Functions
```
isSystemThemeAvailable() → bool
setTheme(theme: SystemThemeValue) → null
getSystemThemeAsync() → SystemThemeValue
```

## Events
```
OnLuaThemeUpdated(theme: SystemThemeValue)
```

---

# TaskScheduler
**Extends:** Instance

## Properties
```
SchedulerDutyCycle: double [ReadOnly]
SchedulerRate: double [ReadOnly]
ThreadPoolConfig: ThreadPoolConfig
ThreadPoolSize: int [ReadOnly]
```

---

# Team
**Extends:** Instance

## Properties
```
AutoAssignable: bool
AutoColorCharacters: bool [Deprecated]
ChildOrder: int
Score: int [Deprecated]
TeamColor: BrickColor
```

## Functions
```
GetPlayers() → Instances
```

## Events
```
PlayerAdded(player: Player)
PlayerRemoved(player: Player)
```

---

# TeamCreateData
**Extends:** Instance

## Properties
```
InitialCameraCFrame: CFrame
```

---

# TeamCreatePublishService
**Extends:** Instance

## Events
```
TeamCreateErrorStatus(result: TeamCreateErrorState, teamCreateSaveData: Dictionary)
TeamCreatePlaceUploadRequest(metadata: Dictionary)
TeamCreatePlaceUploadResponse(success: bool, metadata: Dictionary)
```

---

# TeamCreateService
**Extends:** Instance

## Functions
```
CloseGameIfUserDoesntHavePerms() → null
```

---

# Teams
**Extends:** Instance

## Functions
```
GetTeams() → Instances
RebalanceTeams() → null [Deprecated]
```

---

# TelemetryService
**Extends:** Instance

## Functions
```
LogCounter(config: Dictionary, data: Dictionary?, value: float) → Variant
LogDurationEvent(key: string) → Variant
LogDurationEventWithTimestamp(key: string, timestamp: int64) → Variant
LogEvent(config: Dictionary, data: Dictionary) → Variant
LogStat(config: Dictionary, data: Dictionary?, value: float) → Variant
```

---

# TeleportAsyncResult
**Extends:** Instance

## Properties
```
PrivateServerId: string [ReadOnly]
ReservedServerAccessCode: string [ReadOnly]
```

---

# TeleportOptions
**Extends:** Instance

## Properties
```
ReservedServerAccessCode: string
ServerInstanceId: string
ShouldReserveServer: bool
```

## Functions
```
GetTeleportData() → Variant
SetTeleportData(teleportData: Variant) → null
```

---

# TeleportService
**Extends:** Instance

## Properties
```
CustomizedTeleportUI: bool [Deprecated]
```

## Functions
```
Block() → null
GetArrivingTeleportGui() → Instance
GetLocalPlayerTeleportData() → Variant
GetTeleportSetting(setting: string) → Variant
GetThirdPartyTeleportInfo(goForth: bool) → Tuple
SetTeleportGui(gui: Instance) → null
SetTeleportSetting(setting: string, value: Variant) → null
Teleport(placeId: int64, player: Instance, teleportData: Variant, customLoadingScreen: Instance) → null
TeleportCancel() → null
TeleportToPlaceInstance(placeId: int64, instanceId: string, player: Instance, spawnName: string, teleportData: Variant, customLoadingScreen: Instance) → null
TeleportToPrivateServer(placeId: int64, reservedServerAccessCode: string, players: Instances, spawnName: string, teleportData: Variant, customLoadingScreen: Instance) → null
TeleportToSpawnByName(placeId: int64, spawnName: string, player: Instance, teleportData: Variant, customLoadingScreen: Instance) → null
TeleportTrustedBackForth(goForth: bool) → null
GetPlayerPlaceInstanceAsync(userId: int64) → Tuple
ReserveServer(placeId: int64) → Tuple
TeleportAsync(placeId: int64, players: Instances, teleportOptions: Instance) → Instance
TeleportPartyAsync(placeId: int64, players: Instances, teleportData: Variant, customLoadingScreen: Instance) → string
UnblockAsync() → Tuple
```

## Events
```
LocalPlayerArrivedFromTeleport(loadingGui: Instance, dataTable: Variant)
MenuTeleportAttempt()
SendVIPData(player: Instance, vipServerCode: string, dmPlaceID: int64)
TeleportInProgress(player: Instance, teleportInfo: Dictionary)
TeleportInitFailed(player: Instance, teleportResult: TeleportResult, errorMessage: string, placeId: int64, teleportOptions: Instance)
TeleportInitFailedInternal(player: Instance, teleportResult: TeleportResult, errorMessage: string, guid: string)
```

---

# TemporaryCageMeshProvider
**Extends:** Instance

---

# TemporaryScriptService
**Extends:** Instance

---

# TerrainDetail
**Extends:** Instance

## Properties
```
ColorMap: ContentId
ColorMapContent: Content
Face: TerrainFace
MaterialPattern: MaterialPattern
MetalnessMap: ContentId
MetalnessMapContent: Content
NormalMap: ContentId
NormalMapContent: Content
RoughnessMap: ContentId
RoughnessMapContent: Content
StudsPerTile: float
TexturePack: ContentId
```

---

# TerrainRegion
**Extends:** Instance

## Properties
```
ExtentsMax: Vector3int16
ExtentsMin: Vector3int16
GridV3: BinaryString
IsSmooth: bool [ReadOnly] [Deprecated]
SizeInCells: Vector3 [ReadOnly]
SmoothGrid: BinaryString
```

## Functions
```
ApplyTransform(rotation: CFrame, size: Vector3) → null
ApplyTransformSubregion(rotation: CFrame, size: Vector3, region: Region3int16) → TerrainRegion
ConvertToSmooth() → null [Deprecated]
GetRegionWireframe() → Array
```

---

# TestService
**Extends:** Instance

## Properties
```
AutoRuns: bool
Description: string
ErrorCount: int [ReadOnly]
ExecuteWithStudioRun: bool
Is30FpsThrottleEnabled: bool [Deprecated]
IsPhysicsEnvironmentalThrottled: bool
IsSleepAllowed: bool
NumberOfPlayers: int
SimulateSecondsLag: double
TestCount: int [ReadOnly]
ThrottlePhysicsToRealtime: bool
Timeout: double
WarnCount: int [ReadOnly]
```

## Functions
```
Check(condition: bool, description: string, source: Instance, line: int) → null
Checkpoint(text: string, source: Instance, line: int) → null
CreateAndSavePropertySet(source: Instance, fileName: string) → null
Done() → null
Error(description: string, source: Instance, line: int) → null
Fail(description: string, source: Instance, line: int) → null
Message(text: string, source: Instance, line: int) → null
Require(condition: bool, description: string, source: Instance, line: int) → null
ScopeTime() → Dictionary
TakeSnapshot(snapshotname: string) → null
Warn(condition: bool, description: string, source: Instance, line: int) → null
isFeatureEnabled(name: string) → bool
Run() → null
```

## Events
```
ServerCollectConditionalResult(condition: bool, text: string, script: Instance, line: int)
ServerCollectResult(text: string, script: Instance, line: int)
```

---

# TextBoxService
**Extends:** Instance

---

# TextChannel
**Extends:** Instance

## Properties
```
DirectChatRequester: Player [ReadOnly]
```

## Functions
```
DisplaySystemMessage(systemMessage: string, metadata: string) → TextChatMessage
SetDirectChatRequester(requester: Player) → null
AddUserAsync(userId: int64) → Tuple
SendAsync(message: string, metadata: string) → TextChatMessage
```

## Events
```
MessageReceived(incomingMessage: TextChatMessage)
```

---

# TextChatCommand
**Extends:** Instance

## Properties
```
AutocompleteVisible: bool
Enabled: bool
PrimaryAlias: string
SecondaryAlias: string
```

## Events
```
Triggered(originTextSource: TextSource, unfilteredText: string)
```

---

# TextChatConfigurations
**Extends:** Instance

---

# BubbleChatConfiguration
**Extends:** TextChatConfigurations

## Properties
```
AdorneeName: string
BackgroundColor3: Color3
BackgroundTransparency: double
BubbleDuration: float
BubblesSpacing: float
Enabled: bool
Font: Font
FontFace: Font
LocalPlayerStudsOffset: Vector3
MaxBubbles: float
MaxDistance: float
MinimizeDistance: float
TailVisible: bool
TextColor3: Color3
TextSize: int64
VerticalStudsOffset: float
```

---

# ChannelTabsConfiguration
**Extends:** TextChatConfigurations

## Properties
```
AbsolutePosition: Vector2 [ReadOnly]
AbsoluteSize: Vector2 [ReadOnly]
BackgroundColor3: Color3
BackgroundTransparency: double
Enabled: bool
FontFace: Font
HoverBackgroundColor3: Color3
SelectedTabTextColor3: Color3
TextColor3: Color3
TextSize: int64
TextStrokeColor3: Color3
TextStrokeTransparency: double
```

## Functions
```
SetAbsolutePosition(value: Vector2) → null
SetAbsoluteSize(value: Vector2) → null
```

---

# ChatInputBarConfiguration
**Extends:** TextChatConfigurations

## Properties
```
AbsolutePosition: Vector2 [ReadOnly]
AbsolutePositionWrite: Vector2
AbsoluteSize: Vector2 [ReadOnly]
AbsoluteSizeWrite: Vector2
AutocompleteEnabled: bool
BackgroundColor3: Color3
BackgroundTransparency: double
Enabled: bool
FontFace: Font
IsFocused: bool [ReadOnly]
IsFocusedWrite: bool
KeyboardKeyCode: KeyCode
PlaceholderColor3: Color3
TargetTextChannel: TextChannel
TextBox: TextBox
TextColor3: Color3
TextSize: int64
TextStrokeColor3: Color3
TextStrokeTransparency: double
```

---

# ChatWindowConfiguration
**Extends:** TextChatConfigurations

## Properties
```
AbsolutePosition: Vector2 [ReadOnly]
AbsolutePositionWrite: Vector2
AbsoluteSize: Vector2 [ReadOnly]
AbsoluteSizeWrite: Vector2
BackgroundColor3: Color3
BackgroundTransparency: double
Enabled: bool
FontFace: Font
HeightScale: float
HorizontalAlignment: HorizontalAlignment
TextColor3: Color3
TextSize: int64
TextStrokeColor3: Color3
TextStrokeTransparency: double
VerticalAlignment: VerticalAlignment
WidthScale: float
```

## Functions
```
DeriveNewMessageProperties() → ChatWindowMessageProperties
```

---

# TextChatMessage
**Extends:** Instance

## Properties
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
Verified: bool
```

---

# TextChatMessageProperties
**Extends:** Instance

## Properties
```
PrefixText: string
Text: string
Translation: string
```

---

# BubbleChatMessageProperties
**Extends:** TextChatMessageProperties

## Properties
```
BackgroundColor3: Color3
BackgroundTransparency: double
FontFace: Font
TailVisible: bool
TextColor3: Color3
TextSize: int64
```

---

# ChatWindowMessageProperties
**Extends:** TextChatMessageProperties

## Properties
```
FontFace: Font
PrefixTextProperties: ChatWindowMessageProperties
TextColor3: Color3
TextSize: int
TextStrokeColor3: Color3
TextStrokeTransparency: double
```

---

# TextChatService
**Extends:** Instance

## Properties
```
ChatTranslationEnabled: bool
ChatTranslationFTUXShown: bool
ChatTranslationToggleEnabled: bool
ChatVersion: ChatVersion
CreateDefaultCommands: bool
CreateDefaultTextChannels: bool
HasSeenDeprecationDialog: bool
IsLegacyChatDisabled: bool
```

## Functions
```
DisplayBubble(partOrCharacter: Instance, message: string) → null
CanUserChatAsync(userId: int64) → bool
CanUsersChatAsync(userIdFrom: int64, userIdTo: int64) → bool
CanUsersDirectChatAsync(requesterUserId: int64, userIds: Array) → Array
CanUsersWhisperAsync(fromUserId: int64, toUserId: int64) → bool
```

## Events
```
BubbleDisplayed(partOrCharacter: Instance, textChatMessage: TextChatMessage)
ClientToServerMessageReplicateSignalV2(text: string, metadata: string, messageId: string, textSource: TextSource, textChannel: TextChannel)
ClientToServerMessageReplicateSignalV3(text: string, metadata: string, messageId: string, textSource: TextSource, textChannel: TextChannel, verified: bool, isEscapedFlagEnabled: bool)
MessageReceived(textChatMessage: TextChatMessage)
SendingMessage(textChatMessage: TextChatMessage)
ServerToClientMessageReplicateSignal(text: string, prefixText: string, metadata: string, messageId: string, textSource: TextSource, textChannel: TextChannel, timestamp: int64, status: TextChatMessageStatus)
ServerToClientMessageReplicateSignalV2(data: Dictionary)
UpdateChatTimeout(userId: int64, startTime: int64, duration: int64)
```

---

# TextFilterResult
**Extends:** Instance

## Functions
```
GetChatForUserAsync(toUserId: int64) → string [Deprecated]
GetNonChatStringForBroadcastAsync() → string
GetNonChatStringForUserAsync(toUserId: int64) → string
```

---

# TextFilterTranslatedResult
**Extends:** Instance

## Properties
```
SourceLanguage: string [ReadOnly]
SourceText: TextFilterResult [ReadOnly]
```

## Functions
```
GetTranslationForLocale(locale: string) → TextFilterResult
GetTranslations() → Dictionary
```

---

# TextService
**Extends:** Instance

## Functions
```
GetFontMemoryData() → Dictionary
GetTextSize(string: string, fontSize: int, font: Font, frameSize: Vector2) → Vector2
SetResolutionScale(scale: float) → null
FilterAndTranslateStringAsync(stringToFilter: string, fromUserId: int64, targetLocales: Array, textContext: TextFilterContext) → TextFilterTranslatedResult
FilterStringAsync(stringToFilter: string, fromUserId: int64, textContext: TextFilterContext) → TextFilterResult
GetFamilyInfoAsync(assetId: ContentId) → Dictionary
GetTextBoundsAsync(params: GetTextBoundsParams) → Vector2
GetTextSizeOffsetAsync(fontSize: int, font: Font) → float
```

---

# TextSource
**Extends:** Instance

## Properties
```
CanSend: bool
UserId: int64 [ReadOnly]
UserIdReplicated: int64
```

---

# TextureGenerationPartGroup
**Extends:** Instance

## Functions
```
GetInstances() → Instances
GetMeshIdsHash() → string
```

---

# TextureGenerationService
**Extends:** Instance

## Functions
```
CancelGenerationRequest(jobUuid: string) → null
CreatePartGroup(instances: Instances) → TextureGenerationPartGroup
GenerateTexture(previewJobId: string) → Dictionary
PreviewTexture(partGroup: TextureGenerationPartGroup, prompt: string, options: Dictionary) → Dictionary
GetQuotasAsync() → Dictionary
```

## Events
```
GenerationNotificationSignal(notificationData: Dictionary)
PreviewNotificationSignal(notificationData: Dictionary)
```

---

# TextureGenerationUnwrappingRequest
**Extends:** Instance

## Functions
```
ApplyToDataModel(partGroup: TextureGenerationPartGroup) → TextureGenerationPartGroup
GetPartGroup() → TextureGenerationPartGroup
```

---

# ThirdPartyUserService
**Extends:** Instance

## Properties
```
FriendCommunicationRestrictionStatus: ChatRestrictionStatus [ReadOnly]
```

## Functions
```
GetUserPlatformName() → string
GetVoiceChatRestrictionStatus() → ChatRestrictionStatus
HaveActiveUser() → bool
IsChatRestrictionSupported() → bool
ShowAccountPicker() → null
RegisterActiveUser(gamepadId: UserInputType) → int
```

## Events
```
ActiveUserSignedOut(signOutStatus: int)
```

---

# ThreadState
**Extends:** Instance

## Properties
```
FrameCount: int [ReadOnly]
Populated: bool [ReadOnly]
ThreadId: int [ReadOnly]
ThreadName: string [ReadOnly]
```

## Functions
```
GetFrame(index: int) → Instance
```

---

# TimerService
**Extends:** Instance

---

# ToastNotificationService
**Extends:** Instance

## Functions
```
HideNotification(notificationId: string) → null
ShowNotification(message: string, notificationId: string) → null
```

---

# TouchInputService
**Extends:** Instance

---

# TouchTransmitter
**Extends:** Instance

---

# TracerService
**Extends:** Instance

## Functions
```
FinishSpan(spanId: string) → null
StartSpan(name: string, parentId: string) → string
```

---

# TrackerLodController
**Extends:** Instance

## Properties
```
AudioMode: TrackerLodFlagMode
VideoExtrapolationMode: TrackerExtrapolationFlagMode
VideoLodMode: TrackerLodValueMode
VideoMode: TrackerLodFlagMode
```

## Functions
```
getExtrapolation() → int
getVideoLod() → int
isAudioEnabled() → bool
isVideoEnabled() → bool
```

## Events
```
UpdateState()
```

---

# TrackerStreamAnimation
**Extends:** Instance

---

# Trail
**Extends:** Instance

## Properties
```
Attachment0: Attachment
Attachment1: Attachment
Brightness: float
Color: ColorSequence
Enabled: bool
FaceCamera: bool
Lifetime: float
LightEmission: float
LightInfluence: float
LocalTransparencyModifier: float
MaxLength: float
MinLength: float
Texture: ContentId
TextureLength: float
TextureMode: TextureMode
Transparency: NumberSequence
WidthScale: NumberSequence
```

## Functions
```
Clear() → null
```

## Events
```
OnClearRequested()
```

---

# Translator
**Extends:** Instance

## Properties
```
LocaleId: string [ReadOnly]
```

## Functions
```
FormatByKey(key: string, args: Variant) → string
RobloxOnlyTranslate(context: Instance, text: string) → string
Translate(context: Instance, text: string) → string
```

---

# TutorialService
**Extends:** Instance

## Functions
```
GetMainViewSessionId() → string
HasUserCompletedTutorial() → bool
HideWidgets(commaSeparatedNames: string) → bool
PromptClosePlace() → null
SetTutorialCompletionStatus(completed: bool) → null
ShouldLaunchTutorial() → bool
ShowWidgets(commaSeparatedNames: string) → bool
```

---

# TweenBase
**Extends:** Instance

## Properties
```
PlaybackState: PlaybackState [ReadOnly]
```

## Functions
```
Cancel() → null
Pause() → null
Play() → null
```

## Events
```
Completed(playbackState: PlaybackState)
```

---

# Tween
**Extends:** TweenBase

## Properties
```
Instance: Instance [ReadOnly]
TweenInfo: TweenInfo [ReadOnly]
```

---

# TweenService
**Extends:** Instance

## Functions
```
Create(instance: Instance, tweenInfo: TweenInfo, propertyTable: Dictionary) → Tween
GetValue(alpha: float, easingStyle: EasingStyle, easingDirection: EasingDirection) → float
SmoothDamp(current: Variant, target: Variant, velocity: Variant, smoothTime: float, maxSpeed: float?, dt: float?) → void
```

---

# UGCAvatarService
**Extends:** Instance

---

# UGCValidationService
**Extends:** Instance

## Functions
```
CalculateAverageEditableCageMeshDistance(innerCage: EditableMesh, outerCage: EditableMesh, refMesh: EditableMesh, innerTransform: CFrame, outerTransform: CFrame) → float
CalculateBodyPartMaxCageDistance(outerCage: EditableMesh, renderMesh: EditableMesh, outerTransform: CFrame, scale: Vector3) → float
CalculateEditableMeshInsideMeshPercentage(editableMeshRoot: EditableMesh, editableMeshQuery: EditableMesh, meshQueryTransform: CFrame, meshQueryScale: Vector3) → float
CalculateEditableMeshModifiedCageBoundingBox(referenceUVValues: Array, innerCage: EditableMesh, innerTransform: CFrame, outerCage: EditableMesh, outerTransform: CFrame) → Tuple
CalculateEditableMeshNumModifiedCageUVsInSet(referenceUVValues: Array, innerCage: EditableMesh, innerTransform: CFrame, outerCage: EditableMesh, outerTransform: CFrame) → Tuple
CalculateEditableMeshTotalSurfaceArea(editableMesh: EditableMesh, meshScale: Vector3) → float
CalculateEditableMeshUniqueUVCount(editableMesh: EditableMesh) → int
CheckEditableMeshInCameraFrustum(editableMesh: EditableMesh, meshScale: Vector3, handleWorldCF: CFrame, cameraWorldCF: CFrame) → bool
CreateEditableImageFromBinaryStringRobloxOnly(value: BinaryStringValue) → EditableImage
CreateEditableMeshFromBinaryStringRobloxOnly(value: BinaryStringValue) → EditableMesh
GetBoundingBoxManipulationData(partMeshObjects: Array, partCFs: Array, meshScales: Array) → Map
GetDynamicHeadEditableMeshInactiveControls(editableMesh: EditableMesh, controlNames: Array) → Tuple
GetEditableCagingRelevancyMetrics(innerCage: EditableMesh, outerCage: EditableMesh, refMesh: EditableMesh, offsetInner: Vector3, offsetOuter: Vector3) → Tuple
GetEditableImageData(editableImage: EditableImage) → BinaryStringValue
GetEditableImageSize(editableImage: EditableImage) → Vector2
GetEditableMeshMaxNearbyVerticesCollisions(editableMesh: EditableMesh, meshScale: Vector3) → int
GetEditableMeshTriCount(editableMesh: EditableMesh) → int
GetEditableMeshVertColors(editableMesh: EditableMesh) → Array
GetEditableMeshVerticesSimilarityRate(editableMesh: EditableMesh, meshScale: Vector3) → float
GetEditableMeshVerts(editableMesh: EditableMesh) → Array
GetFacsDrivenJointNamesFromEditableMesh(editableMesh: EditableMesh) → Tuple
GetImageTransparencyWithByteString(textureId: string) → float
GetPropertyValue(instance: Instance, property: string) → Variant
GetSkinnedJointNamesFromEditableMesh(editableMesh: EditableMesh) → Tuple
IsEditableMeshNumCoplanarIntersectionsOverLimit(editableMesh: EditableMesh, limit: int, meshScale: Vector3, intersectBackFaces: bool) → bool
RegisterAlternateMesh(alternateId: string, binaryStringValue: BinaryStringValue) → null
RegisterUGCValidationFunction(setFunction: Function) → null
ReportUGCValidationCounter(success: bool, validationType: string) → null
ReportUGCValidationFailureTelemetry(errorType: string) → null
ReportUGCValidationTelemetry(assetType: string, data: Dictionary) → null
ResetCollisionFidelity(meshPart: Instance, collisionFidelity: CollisionFidelity) → null
ResetCollisionFidelityWithEditableMeshDataLua(meshPart: MeshPart, editableMesh: EditableMesh, collisionFidelity: CollisionFidelity) → null
SetMeshIdBlocking(meshPart: Instance, meshId: string) → null
ValidateDynamicHeadEditableMesh(editableMesh: EditableMesh) → bool
ValidateEditableImageSize(editableImage: EditableImage) → bool
ValidateEditableMeshCageMeshIntersection(innerCage: EditableMesh, outerCage: EditableMesh, refMesh: EditableMesh) → Tuple
ValidateEditableMeshCageNonManifoldAndHoles(editableMesh: EditableMesh) → Tuple
ValidateEditableMeshCageUVCoincident(editableMesh: EditableMesh) → bool
ValidateEditableMeshCageUVTriangleArea(editableMesh: EditableMesh) → bool
ValidateEditableMeshFacialBounds(editableMesh: EditableMesh, boundsScale: float, partSize: Vector3) → bool
ValidateEditableMeshFacialExpressiveness(editableMesh: EditableMesh, minDelta: float, partSize: Vector3) → float
ValidateEditableMeshFullBodyCageDeletion(editableMesh: EditableMesh) → bool
ValidateEditableMeshMisMatchUV(innerCage: EditableMesh, outerCage: EditableMesh) → bool
ValidateEditableMeshOverlappingVertices(editableMesh: EditableMesh) → bool
ValidateEditableMeshTriangleArea(editableMesh: EditableMesh) → bool
ValidateEditableMeshTriangles(editableMesh: EditableMesh) → bool
ValidateEditableMeshUVDuplicates(referenceValues: Array, editableMesh: EditableMesh) → int
ValidateEditableMeshUVSpace(editableMesh: EditableMesh) → bool
ValidateEditableMeshUVValuesInReference(referenceValues: Array, editableMesh: EditableMesh) → bool
ValidateEditableMeshUniqueUVCount(editableMesh: EditableMesh, numRequired: int) → bool
ValidateEditableMeshVertColors(editableMesh: EditableMesh, includeAlpha: bool) → bool
ValidatePartBBoxAfterFullFacs(headEditableMesh: EditableMesh, partEditableMesh: EditableMesh, headScale: Vector3, partScale: Vector3, boundsMaxMultiplier: float) → bool
ValidateSkinnedEditableMesh(editableMesh: EditableMesh) → bool
CalculateBodyMaxCageDistance(inputBodyParts: Array) → Tuple
CanLoadAsset(assetId: string) → bool
CompareTextureOverlapByteString(byteStringBaseline: string, byteStringFollowup: string) → Array
CompareTextureOverlapTextureId(textureIdBaseline: string, textureIdFollowup: string) → Array
DoesMeshHaveSkinningData(meshId: string) → bool
FetchAssetWithFormat(url: ContentId, assetFormat: string) → Instances
GetCagingRelevancyMetrics(innerCageMeshId: string, outerCageMeshId: string, refMeshId: string, offsetInner: Vector3, offsetOuter: Vector3) → Tuple
GetDynamicHeadMeshInactiveControls(meshId: string, controlNames: Array) → Tuple
GetFacsDrivenJointNamesFromMeshId(meshId: string) → Tuple
GetImageTransparencyWithTextureID(textureId: string) → float
GetMaxNearbyVerticesCollisions(meshId: string, meshScale: Vector3) → int
GetMeshDataBinaryString(meshId: string) → BinaryStringValue
GetMeshTriCount(meshId: string) → int
GetMeshVertColors(meshId: string) → Array
GetMeshVerts(meshId: string) → Array
GetSkinnedJointNamesFromMeshId(meshId: string) → Tuple
GetTextureSize(textureId: string) → Vector2
IsDeformedLayeredClothingOutOfRenderBounds(accessory: Accessory) → bool
ValidateCageMeshIntersection(innerCageMeshId: string, outerCageMeshId: string, refMeshId: string) → Tuple
ValidateCageUVCoincident(meshId: string) → bool
ValidateCageUVTriangleArea(meshId: string) → bool
ValidateDynamicHeadMesh(meshId: string) → bool
ValidateFacialBounds(meshId: string, boundsScale: float, partSize: Vector3) → bool
ValidateFacialExpressiveness(meshId: string, minDelta: float, partSize: Vector3) → float
ValidateImageTransparencyThresholdByteString(image: string, threshold: float) → bool
ValidateImageTransparencyThresholdByteString_V2(image: string, threshold: float) → bool
ValidateImageTransparencyThresholdTextureID(textureId: string, threshold: float) → bool
ValidateImageTransparencyThresholdTextureID_V2(textureId: string, threshold: float) → bool
ValidateMeshVertColors(meshId: string, includeAlpha: bool) → bool
ValidateOverlappingVertices(meshId: string) → bool
ValidatePartBBoxAfterFullFacsFromMeshIds(headMeshId: string, partMeshId: string, headScale: Vector3, partScale: Vector3, boundsMaxMultiplier: float) → bool
ValidateSkinnedMesh(meshId: string) → bool
ValidateTextureAlpha(textureId: string, pixelWidth: int) → bool
ValidateTextureAlphaByteString(byteString: string, pixelWidth: int) → bool
ValidateUVValuesInReference(referenceValues: Array, meshId: string) → bool
```

---

# UIBase
**Extends:** Instance

---

# UIComponent
**Extends:** UIBase

---

# UIConstraint
**Extends:** UIComponent

---

# UIAspectRatioConstraint
**Extends:** UIConstraint

## Properties
```
AspectRatio: float
AspectType: AspectType
DominantAxis: DominantAxis
```

---

# UISizeConstraint
**Extends:** UIConstraint

## Properties
```
MaxSize: Vector2
MinSize: Vector2
```

---

# UITextSizeConstraint
**Extends:** UIConstraint

## Properties
```
MaxTextSize: int
MinTextSize: int
```

---

# UIContainerQuery
**Extends:** UIComponent

## Properties
```
AspectRatioRange: NumberRange
IsActive: bool
MaxSize: Vector2
MinSize: Vector2
```

---

# UICorner
**Extends:** UIComponent

## Properties
```
CornerRadius: UDim
```

---

# UIDragDetector
**Extends:** UIComponent

## Properties
```
ActivatedCursorIcon: ContentId
BoundingBehavior: UIDragDetectorBoundingBehavior
BoundingUI: GuiBase2d
CursorIcon: ContentId
DragAxis: Vector2
DragRelativity: UIDragDetectorDragRelativity
DragRotation: float
DragSpace: UIDragDetectorDragSpace
DragStyle: UIDragDetectorDragStyle
DragUDim2: UDim2
Enabled: bool
MaxDragAngle: float
MaxDragTranslation: UDim2
MinDragAngle: float
MinDragTranslation: UDim2
ReferenceUIInstance: GuiObject
ResponseStyle: UIDragDetectorResponseStyle
SelectionModeDragSpeed: UDim2
SelectionModeRotateSpeed: float
UIDragSpeedAxisMapping: UIDragSpeedAxisMapping
```

## Functions
```
AddConstraintFunction(priority: int, function: Function) → RBXScriptConnection
GetReferencePosition() → UDim2
GetReferenceRotation() → float
SetDragStyleFunction(function: Function) → null
```

## Events
```
DragContinue(inputPosition: Vector2)
DragEnd(inputPosition: Vector2)
DragStart(inputPosition: Vector2)
```

---

# UIFlexItem
**Extends:** UIComponent

## Properties
```
FlexMode: UIFlexMode
GrowRatio: float
ItemLineAlignment: ItemLineAlignment
ShrinkRatio: float
```

---

# UIGradient
**Extends:** UIComponent

## Properties
```
Color: ColorSequence
Enabled: bool
Offset: Vector2
Rotation: float
Transparency: NumberSequence
```

---

# UILayout
**Extends:** UIComponent

---

# UIGridStyleLayout
**Extends:** UILayout

## Properties
```
AbsoluteContentSize: Vector2 [ReadOnly]
FillDirection: FillDirection
HorizontalAlignment: HorizontalAlignment
SortOrder: SortOrder
VerticalAlignment: VerticalAlignment
```

## Functions
```
ApplyLayout() → null [Deprecated]
SetCustomSortFunction(function: Function) → null [Deprecated]
```

---

# UIGridLayout
**Extends:** UIGridStyleLayout

## Properties
```
AbsoluteCellCount: Vector2 [ReadOnly]
AbsoluteCellSize: Vector2 [ReadOnly]
CellPadding: UDim2
CellSize: UDim2
FillDirectionMaxCells: int
StartCorner: StartCorner
```

---

# UIListLayout
**Extends:** UIGridStyleLayout

## Properties
```
HorizontalFlex: UIFlexAlignment
HorizontalPadding: UDim
ItemLineAlignment: ItemLineAlignment
Padding: UDim
VerticalFlex: UIFlexAlignment
VerticalPadding: UDim
Wraps: bool
```

---

# UIPageLayout
**Extends:** UIGridStyleLayout

## Properties
```
Animated: bool
Circular: bool
CurrentPage: GuiObject [ReadOnly]
EasingDirection: EasingDirection
EasingStyle: EasingStyle
GamepadInputEnabled: bool
Padding: UDim
ScrollWheelInputEnabled: bool
TouchInputEnabled: bool
TweenTime: float
```

## Functions
```
JumpTo(page: Instance) → null
JumpToIndex(index: int) → null
Next() → null
Previous() → null
```

## Events
```
PageEnter(page: Instance)
PageLeave(page: Instance)
Stopped(currentPage: Instance)
```

---

# UITableLayout
**Extends:** UIGridStyleLayout

## Properties
```
FillEmptySpaceColumns: bool
FillEmptySpaceRows: bool
MajorAxis: TableMajorAxis
Padding: UDim2
```

---

# UIPadding
**Extends:** UIComponent

## Properties
```
PaddingBottom: UDim
PaddingLeft: UDim
PaddingRight: UDim
PaddingTop: UDim
```

---

# UIScale
**Extends:** UIComponent

## Properties
```
Scale: float
```

---

# UIStroke
**Extends:** UIComponent

## Properties
```
ApplyStrokeMode: ApplyStrokeMode
BorderOffset: UDim
BorderStrokePosition: BorderStrokePosition
Color: Color3
Enabled: bool
LineJoinMode: LineJoinMode
StrokeSizingMode: StrokeSizingMode
Thickness: float
Transparency: float
ZIndex: int
```

---

# UIDragDetectorService
**Extends:** Instance

---

# UniqueIdLookupService
**Extends:** Instance

## Functions
```
GetInstanceByRfc4122String(id: string) → Instance
```

---

# UnvalidatedAssetService
**Extends:** Instance

## Properties
```
CachedData: string
```

## Functions
```
AppendTempAssetId(userId: int64, id: int64, lookAt: Vector3, camPos: Vector3, usage: string) → null
AppendVantagePoint(userId: int64, id: int64, lookAt: Vector3, camPos: Vector3) → bool
UpgradeTempAssetId(userId: int64, tempId: int64, assetId: int64) → bool
```

---

# UserGameSettings
**Extends:** Instance

## Properties
```
AllTutorialsDisabled: bool
CameraMode: CustomCameraMode
CameraYInverted: bool
ChatTranslationEnabled: bool
ChatTranslationFTUXShown: bool
ChatTranslationLocale: string
ChatTranslationToggleEnabled: bool
ChatVisible: bool
CompletedTutorials: string
ComputerCameraMovementChanged: bool
ComputerCameraMovementMode: ComputerCameraMovementMode
ComputerMovementChanged: bool
ComputerMovementMode: ComputerMovementMode
ControlMode: ControlMode
DefaultCameraID: string
FramerateCap: int
Fullscreen: bool
GamepadCameraSensitivity: float
GraphicsOptimizationMode: GraphicsOptimizationMode
GraphicsQualityLevel: int
HapticStrength: float
HasEverUsedVR: bool
IsUsingCameraYInverted: bool [ReadOnly]
IsUsingGamepadCameraSensitivity: bool [ReadOnly]
MasterVolume: float
MasterVolumeStudio: float
MaxQualityEnabled: bool
MicroProfilerWebServerEnabled: bool
MicroProfilerWebServerIP: string [ReadOnly]
MicroProfilerWebServerPort: int [ReadOnly]
MouseSensitivity: float
MouseSensitivityFirstPerson: Vector2
MouseSensitivityThirdPerson: Vector2
OnScreenProfilerEnabled: bool
OnboardingsCompleted: string
PartyVoiceVolume: float
PerformanceStatsVisible: bool
PlayerHeight: float
PreferredTextSize: PreferredTextSize
PreferredTransparency: float
QualityResetLevel: int
RCCProfilerRecordFrameRate: int
RCCProfilerRecordTimeFrame: int
ReadAloud: bool
ReducedMotion: bool
RotationType: RotationType
SavedQualityLevel: SavedQualitySetting
StartMaximized: bool
StartScreenPosition: Vector2
StartScreenSize: Vector2
TouchCameraMovementChanged: bool
TouchCameraMovementMode: TouchCameraMovementMode
TouchMovementChanged: bool
TouchMovementMode: TouchMovementMode
UiNavigationKeyBindEnabled: bool
UsedCoreGuiIsVisibleToggle: bool
UsedCustomGuiIsVisibleToggle: bool
UsedHideHudShortcut: bool
VRComfortSetting: VRComfortSetting
VREnabled: bool
VRRotationIntensity: int
VRSafetyBubbleMode: VRSafetyBubbleMode
VRSmoothRotationEnabled: bool
VRSmoothRotationEnabledCustomOption: bool
VRThirdPersonFollowCamEnabled: bool
VRThirdPersonFollowCamEnabledCustomOption: bool
VignetteEnabled: bool
VignetteEnabledCustomOption: bool
gaID: string
```

## Functions
```
GetCameraYInvertValue() → int
GetDefaultFramerateCap() → int
GetOnboardingCompleted(onboardingId: string) → bool
GetTutorialState(tutorialId: string) → bool
InFullScreen() → bool
InStudioMode() → bool
ResetOnboardingCompleted(onboardingId: string) → null
SetCameraYInvertVisible() → null
SetGamepadCameraSensitivityVisible() → null
SetOnboardingCompleted(onboardingId: string) → null
SetTutorialState(tutorialId: string, value: bool) → null
```

## Events
```
FullscreenChanged(isFullscreen: bool)
PerformanceStatsVisibleChanged(isPerformanceStatsVisible: bool)
StudioModeChanged(isStudioMode: bool)
```

---

# UserInputService
**Extends:** Instance

## Properties
```
AccelerometerEnabled: bool [ReadOnly]
BottomBarSize: Vector2 [ReadOnly]
GamepadEnabled: bool [ReadOnly]
GyroscopeEnabled: bool [ReadOnly]
KeyboardEnabled: bool [ReadOnly]
LegacyInputEventsEnabled: bool [Deprecated]
ModalEnabled: bool [Deprecated]
MouseBehavior: MouseBehavior
MouseDeltaSensitivity: float
MouseEnabled: bool [ReadOnly]
MouseIcon: ContentId
MouseIconEnabled: bool
NavBarSize: Vector2 [ReadOnly]
OnScreenKeyboardAnimationDuration: double [ReadOnly]
OnScreenKeyboardPosition: Vector2 [ReadOnly]
OnScreenKeyboardSize: Vector2 [ReadOnly]
OnScreenKeyboardVisible: bool [ReadOnly]
OverrideMouseIconBehavior: OverrideMouseIconBehavior
PreferredInput: PreferredInput [ReadOnly]
RightBarSize: Vector2 [ReadOnly]
StatusBarSize: Vector2 [ReadOnly]
TouchEnabled: bool [ReadOnly]
UserHeadCFrame: CFrame [ReadOnly] [Deprecated]
VREnabled: bool [ReadOnly]
```

## Functions
```
GamepadSupports(gamepadNum: UserInputType, gamepadKeyCode: KeyCode) → bool
GetConnectedGamepads() → Array
GetDeviceAcceleration() → InputObject
GetDeviceGravity() → InputObject
GetDeviceLevel() → DeviceLevel
GetDeviceRotation() → Tuple
GetDeviceType() → DeviceType
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
GetPasteText() → string
GetPlatform() → Platform
GetStringForKeyCode(keyCode: KeyCode) → string
GetSupportedGamepadKeyCodes(gamepadNum: UserInputType) → Array
GetUserCFrame(type: UserCFrame) → CFrame [Deprecated]
IsGamepadButtonDown(gamepadNum: UserInputType, gamepadKeyCode: KeyCode) → bool
IsKeyDown(keyCode: KeyCode) → bool
IsMouseButtonPressed(mouseButton: UserInputType) → bool
IsNavigationGamepad(gamepadEnum: UserInputType) → bool
RecenterUserHeadCFrame() → null
SendAppUISizes(statusBarSize: Vector2, navBarSize: Vector2, bottomBarSize: Vector2, rightBarSize: Vector2) → null
SetNavigationGamepad(gamepadEnum: UserInputType, enabled: bool) → null
```

## Events
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
StatusBarTapped(position: Vector2)
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

# UserService
**Extends:** Instance

## Functions
```
GetUserInfosByUserIdsAsync(userIds: Array) → Array
```

---

# VRService
**Extends:** Instance

## Properties
```
AutomaticScaling: VRScaling
AvatarGestures: bool
ControllerModels: VRControllerModelMode
DidPointerHit: bool [ReadOnly]
FadeOutViewOnCollision: bool
GuiInputUserCFrame: UserCFrame
LaserDistance: float [ReadOnly]
LaserPointer: VRLaserPointerMode
PointerHitCFrame: CFrame [ReadOnly]
QuestASWState: bool
QuestDisplayRefreshRate: float
ThirdPersonFollowCamEnabled: bool [ReadOnly]
VRDeviceAvailable: bool [ReadOnly]
VRDeviceName: string [ReadOnly]
VREnabled: bool [ReadOnly]
VRSessionState: VRSessionState [ReadOnly]
```

## Functions
```
GetTouchpadMode(pad: VRTouchpad) → VRTouchpadMode
GetUserCFrame(type: UserCFrame) → CFrame
GetUserCFrameEnabled(type: UserCFrame) → bool
IsMaquettes() → bool
IsVRAppBuild() → bool
RecenterUserHeadCFrame() → null
RequestNavigation(cframe: CFrame, inputUserCFrame: UserCFrame) → null
SetTouchpadMode(pad: VRTouchpad, mode: VRTouchpadMode) → null
```

## Events
```
LaserPointerTriggered(input: InputObject)
NavigationRequested(cframe: CFrame, inputUserCFrame: UserCFrame)
TouchpadModeChanged(pad: VRTouchpad, mode: VRTouchpadMode)
UserCFrameChanged(type: UserCFrame, value: CFrame)
UserCFrameEnabled(type: UserCFrame, enabled: bool)
```

---

# VRStatusService
**Extends:** Instance

---

# ValueBase
**Extends:** Instance

---

# BinaryStringValue
**Extends:** ValueBase

## Properties
```
Value: BinaryString
```

## Events
```
Changed(value: BinaryString)
```

---

# BoolValue
**Extends:** ValueBase

## Properties
```
Value: bool
```

## Events
```
Changed(value: bool)
changed(value: bool)
```

---

# BrickColorValue
**Extends:** ValueBase

## Properties
```
Value: BrickColor
```

## Events
```
Changed(value: BrickColor)
changed(value: BrickColor)
```

---

# CFrameValue
**Extends:** ValueBase

## Properties
```
Value: CFrame
```

## Events
```
Changed(value: CFrame)
changed(value: CFrame)
```

---

# Color3Value
**Extends:** ValueBase

## Properties
```
Value: Color3
```

## Events
```
Changed(value: Color3)
changed(value: Color3)
```

---

# DoubleConstrainedValue
**Extends:** ValueBase

## Properties
```
ConstrainedValue: double
MaxValue: double
MinValue: double
Value: double
value: double
```

## Events
```
Changed(value: double)
changed(value: double)
```

---

# IntConstrainedValue
**Extends:** ValueBase

## Properties
```
ConstrainedValue: int64
MaxValue: int64
MinValue: int64
Value: int64
value: int64
```

## Events
```
Changed(value: int64)
changed(value: int64)
```

---

# IntValue
**Extends:** ValueBase

## Properties
```
Value: int64
```

## Events
```
Changed(value: int64)
changed(value: int64)
```

---

# NumberValue
**Extends:** ValueBase

## Properties
```
Value: double
```

## Events
```
Changed(value: double)
changed(value: double)
```

---

# ObjectValue
**Extends:** ValueBase

## Properties
```
Value: Instance
```

## Events
```
Changed(value: Instance)
changed(value: Instance)
```

---

# RayValue
**Extends:** ValueBase

## Properties
```
Value: Ray
```

## Events
```
Changed(value: Ray)
changed(value: Ray)
```

---

# StringValue
**Extends:** ValueBase

## Properties
```
Value: string
```

## Events
```
Changed(value: string)
changed(value: string)
```

---

# Vector3Value
**Extends:** ValueBase

## Properties
```
Value: Vector3
```

## Events
```
Changed(value: Vector3)
changed(value: Vector3)
```

---

# Vector3Curve
**Extends:** Instance

## Functions
```
GetValueAtTime(time: float) → Array
X() → FloatCurve
Y() → FloatCurve
Z() → FloatCurve
```

---

# VersionControlService
**Extends:** Instance

## Properties
```
ScriptCollabEnabled: bool
ScriptCollabVersionHistoryEnabled: bool
```

## Events
```
BroadcastScriptChangesSubmitted(scriptGuid: string)
CommitRejectedInfo(reason: int)
LockedScriptBatchCommit(scriptGuidTuple: Tuple, scriptTextTuple: Tuple, commitMessage: string)
RequestAllEditorsSignal()
ScriptBatchCommit(scriptGuidTuple: Tuple, scriptHashBaseTuple: Tuple, scriptTextTuple: Tuple, commitMessage: string)
ScriptChangesSubmitted(scriptGuid: string, submitted: bool)
ScriptEditorAdded(scriptGuid: string, editor: Instance)
ScriptEditorRemoved(scriptGuid: string, editor: Instance)
ScriptStartEdit(scriptGuid: string)
ScriptStopEdit(scriptGuid: string)
```

---

# VideoCaptureService
**Extends:** Instance

## Properties
```
Active: bool
CameraID: string
```

## Functions
```
GetCameraDevices() → Map
```

## Events
```
DevicesChanged()
Error(cameraid: string, errorcode: string)
Started(cameraid: string)
Stopped(cameraid: string)
```

---

# VideoDeviceInput
**Extends:** Instance

## Properties
```
Active: bool
CameraId: string
CaptureQuality: VideoDeviceCaptureQuality
IsReady: bool [ReadOnly]
```

---

# VideoPlayer
**Extends:** Instance

## Properties
```
Asset: ContentId
AutoLoadInStudio: bool
AutoPlayInStudio: bool
IsLoaded: bool [ReadOnly]
IsPlaying: bool [ReadOnly]
Looping: bool
PlaybackSpeed: float
Resolution: Vector2 [ReadOnly]
TimeLength: double [ReadOnly]
TimePosition: double
Volume: float
```

## Functions
```
GetConnectedWires(pin: string) → Instances
GetInputPins() → Array
GetOutputPins() → Array
Pause() → null
Play() → null
SetStudioPreview(isPreview: bool) → null
Unload() → null
LoadAsync() → AssetFetchStatus
```

## Events
```
DidEnd()
DidLoop()
PlayFailed(error: AssetFetchStatus)
WiringChanged(connected: bool, pin: string, wire: Wire, instance: Instance)
```

---

# VideoService
**Extends:** Instance

---

# VirtualInputManager
**Extends:** Instance

## Properties
```
AdditionalLuaState: string
```

## Functions
```
Dump() → null
HandleGamepadAxisInput(objectId: int, keyCode: KeyCode, x: float, y: float, z: float) → null
HandleGamepadButtonInput(deviceId: int, keyCode: KeyCode, buttonState: int) → null
HandleGamepadConnect(deviceId: int) → null
HandleGamepadDisconnect(deviceId: int) → null
SendAccelerometerEvent(x: float, y: float, z: float) → null
SendGravityEvent(x: float, y: float, z: float) → null
SendGyroscopeEvent(quatX: float, quatY: float, quatZ: float, quatW: float) → null
SendKeyEvent(isPressed: bool, keyCode: KeyCode, isRepeatedKey: bool, layerCollector: Instance) → null
SendMouseButtonEvent(x: int, y: int, mouseButton: int, isDown: bool, layerCollector: Instance, repeatCount: int) → null
SendMouseMoveDeltaEvent(deltaX: float, deltaY: float, layerCollector: Instance) → null
SendMouseMoveEvent(x: float, y: float, layerCollector: Instance) → null
SendMouseWheelEvent(x: float, y: float, isForwardScroll: bool, layerCollector: Instance) → null
SendScroll(x: float, y: float, deltaX: float, deltaY: float, options: Dictionary, layerCollector: Instance) → null
SendTextInputCharacterEvent(str: string, layerCollector: Instance) → null
SendTouchEvent(touchId: int64, state: int, x: float, y: float) → null
SetInputTypesToIgnore(inputTypesToIgnore: Variant) → null
StartPlaying(fileName: string) → null
StartPlayingJSON(string: string) → null
StartRecording() → null
StopPlaying() → null
StopRecording() → null
sendRobloxEvent(namespace: string, detail: string, detailType: string) → null
sendThemeChangeEvent(themeName: string) → null
WaitForInputEventsProcessed() → null
```

## Events
```
PlaybackCompleted(additionalLuaState: string)
RecordingCompleted(result: string)
```

---

# VirtualUser
**Extends:** Instance

## Functions
```
Button1Down(position: Vector2, camera: CFrame) → null
Button1Up(position: Vector2, camera: CFrame) → null
Button2Down(position: Vector2, camera: CFrame) → null
Button2Up(position: Vector2, camera: CFrame) → null
CaptureController() → null
ClickButton1(position: Vector2, camera: CFrame) → null
ClickButton2(position: Vector2, camera: CFrame) → null
MoveMouse(position: Vector2, camera: CFrame) → null
SetKeyDown(key: string) → null
SetKeyUp(key: string) → null
StartRecording() → null
StopRecording() → string
TypeKey(key: string) → null
```

---

# VisibilityCheckDispatcher
**Extends:** Instance

---

# Visit
**Extends:** Instance

---

# VisualizationMode
**Extends:** Instance

## Properties
```
Enabled: bool
Title: string
ToolTip: string
```

---

# VisualizationModeCategory
**Extends:** Instance

## Properties
```
Enabled: bool
Title: string
```

---

# VisualizationModeService
**Extends:** Instance

---

# VoiceChatInternal
**Extends:** Instance

## Properties
```
VoiceChatState: VoiceChatState [ReadOnly] [Deprecated]
```

## Functions
```
GetAndClearCallFailureMessage() → string [Deprecated]
GetAudioProcessingSettings() → Tuple [Deprecated]
GetChannelId() → string
GetGroupId() → string
GetMicDevices() → Tuple [Deprecated]
GetParticipants() → Array [Deprecated]
GetSessionId() → string
GetSpeakerDevices() → Tuple [Deprecated]
GetVoiceChatApiVersion() → int [Deprecated]
GetVoiceChatAvailable() → int [Deprecated]
GetVoiceExperienceId() → string
IsContextVoiceEnabled() → bool
IsPublishPaused() → bool [Deprecated]
IsSubscribePaused(userId: int64) → bool [Deprecated]
JoinByGroupId(groupId: string, isMicMuted: bool) → bool [Deprecated]
JoinByGroupIdToken(groupId: string, isMicMuted: bool, isRetry: bool) → bool [Deprecated]
Leave() → null [Deprecated]
LogPublisherWebRTCStats() → bool
LogSubscriptionWebRTCStats() → bool
PublishPause(paused: bool) → bool [Deprecated]
SetMicDevice(micDeviceName: string, micDeviceGuid: string) → null [Deprecated]
SetSpeakerDevice(speakerDeviceName: string, speakerDeviceGuid: string) → null [Deprecated]
SubscribeBlock(userId: int64) → bool
SubscribePause(userId: int64, paused: bool) → bool [Deprecated]
SubscribePauseAll(paused: bool) → bool [Deprecated]
SubscribeRetry(userId: int64) → bool
SubscribeUnblock(userId: int64) → bool
IsVoiceEnabledForUserIdAsync(userId: int64) → bool
```

## Events
```
LocalPlayerModerated()
ParticipantsStateChanged(participantsLeft: Array, participantsJoined: Array, updatedStates: Array)
PlayerMicActivitySignalChange(activityInfo: Dictionary)
StateChanged(old: VoiceChatState, new: VoiceChatState)
TempSetMicMutedToggleMic()
```

---

# VoiceChatService
**Extends:** Instance

## Properties
```
DefaultDistanceAttenuation: VoiceChatDistanceAttenuationType
EnableDefaultVoice: bool
UseAudioApi: AudioApiRollout
UseNewAudioApi: bool
UseNewControlPaths: bool
UseNewJoinFlow: bool
UseStreamSwitching: bool
VoiceChatEnabledForPlaceOnRcc: bool
VoiceChatEnabledForUniverseOnRcc: bool
```

## Functions
```
getInternalChannelId() → string
getInternalGroupId() → string
getInternalPublishPause() → bool
getInternalSessionId() → string
getInternalSubscribePause(userId: int64) → bool
getInternalSubscribePauseAll() → bool
getInternalVoiceChatApiVersion() → int
isInternalPublishPaused() → bool
joinVoice() → null
lastVoiceChatStats() → Dictionary
leaveVoice() → null
rejoinVoice() → null
IsVoiceEnabledForUserIdAsync(userId: int64) → bool
```

## Events
```
ClientRetryJoin()
ClientRetryJoinWithConfig(sessionConfigFlags: int64)
FetchUserTurnAuthOperationFailed(sessionId: string)
JoinedVoice(channelName: string, participantId: int64, sessionId: string, channelId: string)
PublishStateChange(muteState: MuteState, sessionId: string)
PublishingHandshakeAcked(handshakeAnswer: string, sessionId: string)
PublishingHandshakeAckedWithBothSdp(fullHandshakeAnswer: string, compressedHandshakeAnswer: string, sessionId: string, compressMode: int)
PublishingHandshakeAckedWithCompressedSdp(compressedHandshakeAnswer: string, sessionId: string, compressMode: int)
PublishingHandshakeCompleted(sessionId: string)
PublishingHandshakeInitiated(handshakeOffer: string, muteState: MuteState, sessionId: string)
PublishingHandshakeInitiatedWithBothSdp(fullHandshakeOffer: string, compressedHandshakeOffer: string, muteState: MuteState, sessionId: string, compressMode: int)
PublishingHandshakeInitiatedWithCompressedSdp(compressedHandshakeOffer: string, muteState: MuteState, sessionId: string, compressMode: int)
ReJoinedVoice(channelName: string, participantId: int64, sessionId: string, channelId: string)
RelayCandidatesGathered(voiceControlPath: VoiceControlPath, serializedIceCandidates: string, isLast: bool, sessionId: string, clientIp: string, clientPort: int)
RuppInitialToken(sessionId: string, token: string, destinationIpAddress: string, destinationPort: int)
RuppPeriodicToken(sessionId: string, token: string, destinationIpAddress: string, destinationPort: int, sourceIpAddress: string, sourcePort: int)
SubscribeStateChange(muteState: MuteState, userIds: string, sessionId: string)
SubscriptionDropped(sessionId: string)
SubscriptionFeedStarted(eventTag: int64, sessionId: string)
SubscriptionHandshakeAcked(eventTag: int64, handshakeAnswer: string, usersToMute: string, sessionId: string)
SubscriptionHandshakeAckedWithBothSdp(eventTag: int64, fullHandshakeAnswer: string, compressedSdpAnswer: string, usersToMute: string, sessionId: string, compressMode: int)
SubscriptionHandshakeAckedWithCompressedSdp(eventTag: int64, compressedSdpAnswer: string, usersToMute: string, sessionId: string, compressMode: int)
SubscriptionHandshakeCompleted(sessionId: string, eventTag: int64)
SubscriptionHandshakeInitiated(handshakeOffer: string, newSubscriptionStates: string, isNewConnection: bool, sessionId: string, eventTag: int64)
SubscriptionHandshakeInitiatedWithBothSdp(fullHandshakeOffer: string, compressedHandshakeOffer: string, newSubscriptionStates: string, isNewConnection: bool, sessionId: string, eventTag: int64, compressMode: int)
SubscriptionHandshakeInitiatedWithCompressedSdp(compressedHandshakeOffer: string, newSubscriptionStates: string, isNewConnection: bool, sessionId: string, eventTag: int64, compressMode: int)
SubscriptionReset(sessionId: string)
UpdateTurnAuthInfoRequest()
UserTurnAuth(sessionId: string, userName: string, password: string, ttl: int, uris: Array)
VoiceChatClientVoiceCapability()
VoiceChatClientVoiceCapabilityWithConfig(sessionConfigFlags: int64)
VoiceChatPlayerMuteStateChangedClientToServer(muteState: MuteState)
VoiceChatPlayerMuteStateChangedServerToClient(muteState: MuteState)
VoiceChatSampleTaggedEventClientToServer(tag: int64, value: string)
VoiceChatSampleTaggedEventServerToClient(tag: int64, value: string)
VoiceChatStatsCollected()
VoiceChatSubscriptionInitialBatchEmpty(sessionId: string)
VoiceChatplayerMuteStatusChangedEvent(userId: int64, muted: bool, sessionId: string)
VoiceSetupFailed(voiceControlPath: VoiceControlPath, serializedFailure: string, sessionId: string)
VoiceUdmuxVip(sessionId: string, udmuxVipAddress: string)
```

---

# WebSocketClient
**Extends:** Instance

## Properties
```
ConnectionState: WebSocketState [ReadOnly]
```

## Functions
```
Close() → null
Send(data: string) → null
```

## Events
```
Closed()
MessageReceived(data: string)
Opened()
```

---

# WebSocketService
**Extends:** Instance

## Functions
```
CreateClient(uri: string) → WebSocketClient
```

---

# WebViewService
**Extends:** Instance

## Functions
```
CloseWindow() → null
MutateWindow(url: string, title: string?, isVisible: bool?, searchType: string?, transitionAnimation: string?, showDomainAsTitle: bool?) → null
OpenWindow(url: string, title: string?, isVisible: bool?, searchType: string?, transitionAnimation: string?, showDomainAsTitle: bool?) → null
IsAvailable() → bool
```

## Events
```
OnJavaScriptCall(content: string)
OnWindowClosed()
```

---

# WeldConstraint
**Extends:** Instance

## Properties
```
Active: bool [ReadOnly]
CFrame0: CFrame
CFrame1: CFrame
Enabled: bool
Part0: BasePart
Part0Internal: BasePart
Part1: BasePart
Part1Internal: BasePart
State: int
```

---

# Wire
**Extends:** Instance

## Properties
```
Connected: bool [ReadOnly]
SourceInstance: Instance
SourceName: string
TargetInstance: Instance
TargetName: string
```

## Functions
```
RenameToDefault() → null
```

---

# MLSession
**Extends:** Object

## Functions
```
ForwardAsync(data: Dictionary) → Dictionary
```

---

# TerrainIterateOperation
**Extends:** Object

## Functions
```
CommitBlock(block: Dictionary) → RBXScriptSignal
```

## Events
```
Ready(block: Dictionary)
```

---

# TerrainModifyOperation
**Extends:** Object

## Functions
```
CommitBlock(block: Dictionary) → RBXScriptSignal
```

## Events
```
Ready(block: Dictionary)
```

---

# TerrainReadOperation
**Extends:** Object

## Events
```
Ready(block: Dictionary)
```

---

# TerrainWriteOperation
**Extends:** Object

## Functions
```
CommitBlock(block: Dictionary) → RBXScriptSignal
GetBlock() → Dictionary
```

---
