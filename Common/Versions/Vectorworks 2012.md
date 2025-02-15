# New Functions

[VS:Vectorworks 2012 New Functions](VS:Vectorworks 2012 New Functions)

# Changes

* Parametric objects no longer reset when moved inside a viewport, or when a viewport is moved. This was done for optimization purposes. However, if your parametric object needs to reset, you can specify the **kObjXPropResetOnMoveInViewport** extended property.

## List of deprecated functions

### Criteria

* __BotBound__
* __CriteriaArea__
* __CriteriaSurfaceArea__
* __CriteriaVolume__
* __LeftBound__
* __Length__
* __Perim__
* __RightBound__
* __TopBound__
* __XCenter__
* __YCenter__
* __ZCenter__

### Dialogs - Modern

* __CreateIconPushButton__
* __InsertEnhancedPullDownMenuItem__
* __InsertProposedClassOrLayerItem__

### Dialogs - Modern - Browser

* __AddLBImage__
* __SetLBMultImageIndexes__

### Objects - Walls

* __GetLayerDeltaZOffset__
* __GetLinkHeightToLayerDeltaZ__
* __HWallHeight__
* __SetLayerDeltaZOffset__
* __SetLinkHeightToLayerDeltaZ__
* __SetWallHeights__
* __WallHeight__

# Table with replacement functions

| Deprecated function | Replacement function |
|---------------------|----------------------|
| __CreateControl__ <br> * controlKind = 1  {PICT image} <br> * controlKind = 26 {PNG image} | [CreateImageControl2](../../Function%20Reference/Functions/pages/CreateImageControl2.md) |
| __CreateControl__ <br> * controlKind = 10 {image popup} | [CreateThumbnailPopup](../../Function%20Reference/Functions/pages/CreateThumbnailPopup.md) |
| __CreateIconPushButton__ | [CreateImagePushButton](../../Function%20Reference/Functions/pages/CreateImagePushButton.md) |
| __InsertEnhancedPullDownMenuItem__ | [InsertEnhanPullDownMenuItem](../../Function%20Reference/Functions/pages/InsertEnhanPullDownMenuItem.md) |
| __InsertProposedClassOrLayerItem__ | [InsertPropClassOrLayerItem](../../Function%20Reference/Functions/pages/InsertPropClassOrLayerItem.md) |
| __AddLBImage__ | [AddListBrowserImage](../../Function%20Reference/Functions/pages/AddListBrowserImage.md) |
| __SetLBMultImageIndexes__ | [SetLBImageIndexes](../../Function%20Reference/Functions/pages/SetLBImageIndexes.md) |
| __BotBound__ | [BotBoundN](../../Function%20Reference/Functions/pages/BotBoundN.md) |
| __CriteriaArea__ | [AreaN](../../Function%20Reference/Functions/pages/AreaN.md) |
| __CriteriaSurfaceArea__ | [SurfaceAreaN](../../Function%20Reference/Functions/pages/SurfaceAreaN.md) |
| __CriteriaVolume__ | [VolumeN](../../Function%20Reference/Functions/pages/VolumeN.md) |
| __LeftBound__ | [LeftBoundN](../../Function%20Reference/Functions/pages/LeftBoundN.md) |
| __Length__ | [LengthN](../../Function%20Reference/Functions/pages/LengthN.md) |
| __Perim__ | [PerimN](../../Function%20Reference/Functions/pages/PerimN.md) |
| __RightBound__ | [RightBoundN](../../Function%20Reference/Functions/pages/RightBoundN.md) |
| __TopBound__ | [TopBoundN](../../Function%20Reference/Functions/pages/TopBoundN.md) |
| __XCenter__ | [XCenterN](../../Function%20Reference/Functions/pages/XCenterN.md) |
| __YCenter__ | [YCenterN](../../Function%20Reference/Functions/pages/YCenterN.md) |
| __ZCenter__ | [ZCenterN](../../Function%20Reference/Functions/pages/ZCenterN.md) |
