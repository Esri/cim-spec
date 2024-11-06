


## CIMAspectRatio
#### Represents an aspect ratio. 


### CIMAspectRatio 

|Property | Type | Description | 
|---------|--------|--------|
| width | double | The width component of the aspect ratio. 
| height | double | The height component of the aspect ratio. 






## CIMImagePresentationPage
#### Represents an image media presentation page. 


### CIMPresentationPage 

|Property | Type | Description | 
|---------|--------|--------|
| transition | [CIMPresentationTransition](CIMPresentation.md#cimpresentationtransition) | The transition used to display the page. 
| holdTime | double | The hold time in seconds. 
| isAutomaticAdvancement | boolean | A value indicating whether to automatically advance to the next page after the specified hold time. 
| backgroundColor | [Color](Types.md#color) | The background color. 
| showBackgroundBorder | boolean | A value indicating whether to show the border around the background content. 
| margin | [CIMMargin](CIMLayout.md#cimmargin) | The page margin. 
| elementStorageURI | string | The URI of the storage for the graphic elements that will be overlaid on this presentation page. 
| extent | [Envelope](ExternalReferences.md#envelope) | The spatial extent to zoom to for the graphic elements that will be overlaid on this presentation page. 
| thumbnailURI | string | The URI of the binary reference containing the thumbnail image. 
| visibility | boolean | A value indicating whether this page is visible. 
| locked | boolean | A value indicating whether this page is locked. 
| colorVisionDeficiencyMode | [enumeration ColorVisionDeficiencyType](CIMEnumerations.md#enumeration-colorvisiondeficiencytype) | The color vision deficiency mode. 


### CIMImagePresentationPage 

|Property | Type | Description | 
|---------|--------|--------|
| imageURI | string | The URI of the binary reference containing the image. 
| sourceURL | string | The source URL of the image. Typically the source of the image copied into the ImageURI. 
| fitType | [enumeration PresentationMediaContentFitType](CIMPresentation.md#enumeration-presentationmediacontentfittype) | The image content fit type. 






## CIMMapPresentationPage
#### Represents a map presentation page. 


### CIMPresentationPage 

|Property | Type | Description | 
|---------|--------|--------|
| transition | [CIMPresentationTransition](CIMPresentation.md#cimpresentationtransition) | The transition used to display the page. 
| holdTime | double | The hold time in seconds. 
| isAutomaticAdvancement | boolean | A value indicating whether to automatically advance to the next page after the specified hold time. 
| backgroundColor | [Color](Types.md#color) | The background color. 
| showBackgroundBorder | boolean | A value indicating whether to show the border around the background content. 
| margin | [CIMMargin](CIMLayout.md#cimmargin) | The page margin. 
| elementStorageURI | string | The URI of the storage for the graphic elements that will be overlaid on this presentation page. 
| extent | [Envelope](ExternalReferences.md#envelope) | The spatial extent to zoom to for the graphic elements that will be overlaid on this presentation page. 
| thumbnailURI | string | The URI of the binary reference containing the thumbnail image. 
| visibility | boolean | A value indicating whether this page is visible. 
| locked | boolean | A value indicating whether this page is locked. 
| colorVisionDeficiencyMode | [enumeration ColorVisionDeficiencyType](CIMEnumerations.md#enumeration-colorvisiondeficiencytype) | The color vision deficiency mode. 


### CIMMapPresentationPage 

|Property | Type | Description | 
|---------|--------|--------|
| mapView | [CIMPresentationMapView](CIMPresentation.md#cimpresentationmapview) | The map view. 
| restingState | [PresentationMapRestingState](Types.md#presentationmaprestingstate) | The map resting state. 
| autoPlayAnimationName | string | The name of the animation that will automatically play when this map page becomes active. 






## CIMPresentation
#### Represents a presentation. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the source was last modified, as of the last sync. Used to detect when another sync is needed. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 
| sourcePortalUrl | string | The source portal URI of the item. Set if sourced from an external item such as an item on a portal. 


### CIMPresentation 

|Property | Type | Description | 
|---------|--------|--------|
| pageSettings | [CIMPage](CIMLayout.md#cimpage) | The page settings for the presentation. 
| pages | [string] | The presentation pages as an array of repository URIs. Each string in the array represents a repository URI that points to the storage of a presentation page in the form of an object reference. 
| aspectRatio | [CIMAspectRatio](CIMPresentation.md#cimaspectratio) | The aspect ratio. 
| colorModel | [enumeration ColorModel](CIMEnumerations.md#enumeration-colormodel) | The color model for a presentation. 
| RGBColorProfile | string | The name of the RGB color profile for a presentation. 
| CMYKColorProfile | string | The name of the CMYK color profile for a presentation. 






## CIMPresentationGravityWellRestingState
#### Presentation map gravity well resting state. When a presentation map page has an active gravity well resting state, the camera will be pulled back to the specified view point within the given time (travel time) if left idle. 


### CIMPresentationMapRestingState 

|Property | Type | Description | 
|---------|--------|--------|
| startDelay | double | The number of seconds to delay before starting. 
| enabled | boolean | A value indicating whether this resting state is enabled. 
| viewpoint | [CIMViewCamera](CIMMap.md#cimviewcamera) | The camera. 


### CIMPresentationGravityWellRestingState 

|Property | Type | Description | 
|---------|--------|--------|
| travelTime | double | The number of seconds that it will take to travel back to the viewpoint. 






## CIMPresentationLayerOverrideSet
#### Represents a presentation layer property override set. 


### CIMPresentationLayerOverrideSet 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string | The path to the associated map layer. 
| visibility | boolean | A value indicating whether this layer is visible. It overrides the visibility property on the associated map layer. 






## CIMPresentationMapView
#### Represents a map view in a map presentation page. 


### CIMPresentationMapView 

|Property | Type | Description | 
|---------|--------|--------|
| mapView | [CIMMapView](CIMDocument.md#cimmapview) | The map view. 
| layerOverrides | [[CIMPresentationLayerOverrideSet]](CIMPresentation.md#cimpresentationlayeroverrideset) | The array of layer overrides. 





### Enumeration: PresentationMediaContentFitType
#### Media content (image/video) fit types. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| The media content preserves its original size. 
| Fill| 1| The media content is stretched proportionally to fill the available space. 
| StretchToFill| 2| The media content is stretched to fill the available space. 
| Center| 3| The media content is centered. 




## CIMPresentationPage
#### Represents a presentation page. 


### CIMPresentationPage 

|Property | Type | Description | 
|---------|--------|--------|
| transition | [CIMPresentationTransition](CIMPresentation.md#cimpresentationtransition) | The transition used to display the page. 
| holdTime | double | The hold time in seconds. 
| isAutomaticAdvancement | boolean | A value indicating whether to automatically advance to the next page after the specified hold time. 
| backgroundColor | [Color](Types.md#color) | The background color. 
| showBackgroundBorder | boolean | A value indicating whether to show the border around the background content. 
| margin | [CIMMargin](CIMLayout.md#cimmargin) | The page margin. 
| elementStorageURI | string | The URI of the storage for the graphic elements that will be overlaid on this presentation page. 
| extent | [Envelope](ExternalReferences.md#envelope) | The spatial extent to zoom to for the graphic elements that will be overlaid on this presentation page. 
| thumbnailURI | string | The URI of the binary reference containing the thumbnail image. 
| visibility | boolean | A value indicating whether this page is visible. 
| locked | boolean | A value indicating whether this page is locked. 
| colorVisionDeficiencyMode | [enumeration ColorVisionDeficiencyType](CIMEnumerations.md#enumeration-colorvisiondeficiencytype) | The color vision deficiency mode. 






## CIMPresentationRotateRestingState
#### Presentation map rotate resting state. When a presentation map page has an active rotate resting state, the camera will be rotated around the specified view point at the given rotational velocity. 


### CIMPresentationMapRestingState 

|Property | Type | Description | 
|---------|--------|--------|
| startDelay | double | The number of seconds to delay before starting. 
| enabled | boolean | A value indicating whether this resting state is enabled. 
| viewpoint | [CIMViewCamera](CIMMap.md#cimviewcamera) | The camera. 


### CIMPresentationRotateRestingState 

|Property | Type | Description | 
|---------|--------|--------|
| rotationRate | double | The rotational velocity in degrees per second. A negative value indicates counterclockwise rotation. 






## CIMPresentationTransition
#### Represents a transition. 


### CIMPresentationTransition 

|Property | Type | Description | 
|---------|--------|--------|
| duration | double | The transition duration in seconds. 
| transitionType | [enumeration PresentationTransitionType](CIMPresentation.md#enumeration-presentationtransitiontype) | The transition type. 
| swipeDirection | [enumeration SwipeDirection](CIMMap.md#enumeration-swipedirection) | The swipe transition direction. 





### Enumeration: PresentationTransitionType
#### Presentation transition types. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No transition. 
| Swipe| 1| Swipe transition. 
| Fade| 2| Fade in/out transition. 




## CIMVideoPresentationPage
#### Represents an video media presentation page. 


### CIMPresentationPage 

|Property | Type | Description | 
|---------|--------|--------|
| transition | [CIMPresentationTransition](CIMPresentation.md#cimpresentationtransition) | The transition used to display the page. 
| holdTime | double | The hold time in seconds. 
| isAutomaticAdvancement | boolean | A value indicating whether to automatically advance to the next page after the specified hold time. 
| backgroundColor | [Color](Types.md#color) | The background color. 
| showBackgroundBorder | boolean | A value indicating whether to show the border around the background content. 
| margin | [CIMMargin](CIMLayout.md#cimmargin) | The page margin. 
| elementStorageURI | string | The URI of the storage for the graphic elements that will be overlaid on this presentation page. 
| extent | [Envelope](ExternalReferences.md#envelope) | The spatial extent to zoom to for the graphic elements that will be overlaid on this presentation page. 
| thumbnailURI | string | The URI of the binary reference containing the thumbnail image. 
| visibility | boolean | A value indicating whether this page is visible. 
| locked | boolean | A value indicating whether this page is locked. 
| colorVisionDeficiencyMode | [enumeration ColorVisionDeficiencyType](CIMEnumerations.md#enumeration-colorvisiondeficiencytype) | The color vision deficiency mode. 


### CIMVideoPresentationPage 

|Property | Type | Description | 
|---------|--------|--------|
| videoSource | [CIMVideoDataConnection](CIMImageLayers.md#cimvideodataconnection) | The data connection of the video. 
| fitType | [enumeration PresentationMediaContentFitType](CIMPresentation.md#enumeration-presentationmediacontentfittype) | The video content fit type. 
| startTime | double | The number of seconds in the video at which to start playing. 
| endTime | double | The number of seconds in the video at which to end playing. 
| loop | boolean | A value indicating whether to play the video in a loop. 



