


## CIMAltitudeParams
#### Represents altitude parameters. 


### CIMAltitudeParams 

|Property | Type | Description | 
|---------|--------|--------|
| altitudeValue | double | The altitude value. 
| mode | [enumeration AltitudeMode](CIMEnumerations.md#enumeration-altitudemode) | The altitude mode. 






## CIMAnimationScreenGraphic
#### Represents a graphic and list of keyframes indicating properties that can be changed during the animation. 


### CIMAnimationScreenGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| graphic | [Graphic](Types.md#graphic) | The graphic to be displayed. 
| alias | string | An identifier for the user. 
| keyframes | [CIMAnimationScreenGraphicKeyframe](CIMMap.md#cimanimationscreengraphickeyframe) | The graphic properties keyframes. 






## CIMAnimationScreenGraphicKeyframe
#### Properties defining the graphic at a single point in time for the animation. 


### CIMAnimationScreenGraphicKeyframe 

|Property | Type | Description | 
|---------|--------|--------|
| trackTime | double | The time in seconds relative to the beginning of the track. 
| anchorX | double | The horizontal placement percent of the graphic anchor position on the viewer (0 is left edge, 1 is right edge). 
| anchorY | double | The vertical placement percent of the graphic anchor position on the viewer (0 is top edge, 1 is bottom edge). 
| transparency | double | The transparency of the graphic. 
| scale | double | The size multiplier for the graphic. 






## CIMBookmark
#### Represents a spatial bookmark. 


### CIMBookmark 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The bookmark name. 
| thumbnailImagePath | string | The thumbnail image path. 
| camera | [CIMViewCamera](CIMMap.md#cimviewcamera) | The camera. 
| location | [Envelope](ExternalReferences.md#envelope) | The location. 
| timeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The time extent. 
| description | string | The bookmark description. 
| videoURI | string | The URI to the standalone video. 
| videoElapsedTime | double | The video elapsed time in seconds. 





### Enumeration: ClipDistanceMode
#### Specifies the clipping mode used for the map. 

|Property | Value | Description | 
|---------|--------|--------|
| Automatic| 0| Calculate clip distance automatically. 
| Manual| 1| Use the specified clip distance. 



### Enumeration: ClippingMode
#### Specifies the clipping mode used for the map. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No clipping applied. 
| MapExtent| 1| Clip to the custom extent defined for the map. 
| CustomShape| 2| Clip to a custom shape. 



### Enumeration: ComparisonOperator
#### Query builder comparison operator between fields. 

|Property | Value | Description | 
|---------|--------|--------|
| IsEqual| 1| Is Equal to comparison operator. 
| NotEqual| 2| Does not equal to comparison operator. 
| LessThanOrEqualTo| 3| Less than or equal to comparison operator. 
| LessThan| 4| Less than comparison operator. 
| GreaterThanOrEqualTo| 5| Greater than or equal to comparison operator. 
| GreaterThan| 6| Greater than comparison operator. 



### Enumeration: CullDirection
#### Represents the direction for clipping. 

|Property | Value | Description | 
|---------|--------|--------|
| Inward| 0| Clip the inside or forward. 
| Outward| 1| Clip the outside or backwards. 
| Camera| 2| Clip from the side that is closest to the camera. 




## CIMDatumTransform
#### Represents a datum transform. 


### CIMDatumTransform 

|Property | Type | Description | 
|---------|--------|--------|
| forward | boolean | A value indicating whether or not this is a forward transformation. 
| geoTransformation | [GeoTransformation](ExternalReferences.md#geotransformation) | The transformation. 






## CIMElevationSource
#### Represents an elevation source. 


### CIMElevationSource 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| verticalUnit | [Unit](ExternalReferences.md#unit) | The vertical unit. 
| visibility | boolean | A value indicating whether the elevation source is visible. 
| name | string | The name of the elevation source. 
| metadataURI | string | The metadata URI of the elevation source. 
| elevationSourceID | string | The elevation source ID. 






## CIMGroundToGridCorrection
#### Defines the properties needed to perform a COGO ground to grid correction when adding new features. 


### CIMGroundToGridCorrection 

|Property | Type | Description | 
|---------|--------|--------|
| enabled | boolean | A value indicating whether ground to grid corrections are currently in operation for the map. 
| useDirection | boolean | A value indicating whether the direction angle will be used in the ground to grid correction. 
| useScale | boolean | A value indicating whether the distance scale will be used in the ground to grid correction. 
| direction | double | The direction angle (in degrees) that will be used in ground to grid calculations. 
| scaleType | [enumeration GroundToGridScaleType](CIMMap.md#enumeration-groundtogridscaletype) | The type of scale that will be used in ground to grid calculations. 
| constantScaleFactor | double | The constant scale factor used in ground to grid calculations, only when . 





### Enumeration: GroundToGridScaleType
#### Defines modes for specifying Scale for ground to grid corrections. 

|Property | Value | Description | 
|---------|--------|--------|
| ConstantFactor| 0| A constant scale factor will be used to specify scale for ground to grid corrections. 
| ComputeUsingElevation| 1| The scale will be computed using the current Editing ElevationCapturing mode. 




## CIMIlluminationProperties
#### Represents illumination properties. 


### CIMIlluminationProperties 

|Property | Type | Description | 
|---------|--------|--------|
| ambientLight | double | The ambient light value. 
| sunPositionX | double | The sun position X. 
| sunPositionY | double | The sun position Y. 
| sunPositionZ | double | The sun position Z. 
| showAtmosphericEffects | boolean | A value indicating whether or not to show atmospheric effects. 
| showShadows3D | boolean | A value indicating whether or not to show shadows in 3D. 
| dateTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time instant. 
| illuminationSource | [enumeration IlluminationSource](CIMMap.md#enumeration-illuminationsource) | The illumination source. 
| sunAzimuth | double | The sun azimuth. 
| sunAltitude | double | The sun altitude. 
| showStars | boolean | A value indicating whether to show the stars and the atmospheric halo for a global scene. 





### Enumeration: IlluminationSource
#### Illumination source types. 

|Property | Value | Description | 
|---------|--------|--------|
| NoonAtCameraPosition| 0| Noon at the camera position. 
| DateTime| 1| Set for a specific date and time. 
| AbsoluteSunPosition| 2| An absolute sun position. 
| MapTime| 3| Synchronized with the current map time. 



### Enumeration: JoinOperator
#### Query builder Boolean operator types. 

|Property | Value | Description | 
|---------|--------|--------|
| And| 1| And Boolean operator. 
| Or| 2| Or Boolean operator. 
| None| 3| No Boolean operator used. Used for the first item in a collection of Comparisons. 




## CIMKeyframeAnalysis
#### Represents an exploratory analysis keyframe. 


### CIMKeyframeAnalysis 

|Property | Type | Description | 
|---------|--------|--------|
| analysis | [ExploratoryAnalysisDefinition](Types.md#exploratoryanalysisdefinition) | The exploratory analysis definition. 
| transition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the exploratory analysis item. 






## CIMKeyframeCamera
#### Represents a camera keyframe. 


### CIMKeyframeCamera 

|Property | Type | Description | 
|---------|--------|--------|
| camera | [CIMViewCamera](CIMMap.md#cimviewcamera) | The camera for the keyframe. 
| headingTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the heading of the camera. 
| pitchTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the pitch of the camera. 
| rollTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the roll of the camera. 
| scaleTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the scale of the camera. 
| XTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the x of the camera. 
| YTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the y of the camera. 
| ZTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the z of the camera. 
| transitionScale | double | The value of adjustable transitions. The value must be between 0.0 and 1.0. Smaller values will result in a tighter / smaller curve than larger values. 
| cameraTransitionMode | [enumeration esriAnimationTransitionMode](ExternalReferences.md#enumeration-esrianimationtransitionmode) | The transition mode determines whether the camera path follows a Geodesic or Cartesian interpolation. 






## CIMKeyframeLayer
#### Represents a layer keyframe. 


### CIMKeyframeLayer 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string | The path to the layer. 
| transparency | double | The method of transition for the visibility of the layer. 
| transparencyTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the transparency of the layer. 
| visible | boolean | A value indicating whether the layer is visible. 
| swipeDirection | [enumeration SwipeDirection](CIMMap.md#enumeration-swipedirection) | The direction to clip from an edge. 
| swipePercent | double | The amount of the visible area to clip. 
| verticalExaggeration | double | The vertical exaggeration. 
| ZOffset | double | The vertical exaggeration. 






## CIMKeyframeRange
#### Represents a range keyframe. 


### CIMKeyframeRange 

|Property | Type | Description | 
|---------|--------|--------|
| range | [CIMRange](CIMVectorLayers.md#cimrange) | The value of the range. 
| minTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the minimum value of the range. 
| maxTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the maximum value of the range. 
| isExclusion | boolean | A value indicating whether the range should be all values less than the minimum value and greater than the maximum value. 






## CIMKeyframeSurface
#### Represents a surface keyframe. 


### CIMKeyframeSurface 

|Property | Type | Description | 
|---------|--------|--------|
| surfaceID | string | The id for the surface. 
| transition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the surface. 
| verticalExaggeration | double | The vertical exaggeration for the surface. 
| visible | boolean | A value indicating whether the surface is visible. 
| swipeDirection | [enumeration SwipeDirection](CIMMap.md#enumeration-swipedirection) | The direction to clip from an edge. 
| swipePercent | double | The amount of the visible area to clip. 






## CIMKeyframeTime
#### Represents a time keyframe. 


### CIMKeyframeTime 

|Property | Type | Description | 
|---------|--------|--------|
| time | [TimeExtent](ExternalReferences.md#timeextent) | The value of the time extent. 
| endTimeTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the end value of the time extent. 
| startTimeTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition) | The method of transition for the start value of the time extent. 






## CIMLineOfSightEADefinition
#### Represents a line of sight exploratory analysis definition. 


### CIMExploratoryAnalysisDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| ID | long | The id. 


### CIMLineOfSightEADefinition 

|Property | Type | Description | 
|---------|--------|--------|
| observer | [Point](ExternalReferences.md#point) | The observer position. 
| targets | [Multipoint](ExternalReferences.md#multipoint) | The target positions. 
| maximumDistance | double | The maximum distance to be analyzed. 
| minimumDistance | double | The minimum distance to be analyzed. 






## CIMLocator
#### Represents properties of locator for the map. 


### CIMLocator 

|Property | Type | Description | 
|---------|--------|--------|
| locatorType | [enumeration LocatorType](CIMMap.md#enumeration-locatortype) | The type of locator for the LocatorURI specified. 
| name | string | The name of the locator. 
| locatorURI | string | Locator source URI. It can either be a local path, URL or a layer URI from this map. e.g. file://&lt;folder_path&gt;, http://&lt;url&gt;, CIMPATH=&lt;cim_layer_UR&gt;. 
| suggestionsEnabled | boolean | A value indicating whether or not to suggestions should enabled if the locator supports suggestions. 
| enabled | boolean | A value indicating whether or not to this locator is enabled. 
| suggestionsSupported | boolean | A value indicating whether the locator supports suggestions. 





### Enumeration: LocatorType
#### Type of locators. 

|Property | Value | Description | 
|---------|--------|--------|
| Locator| 0| Locator is based on local locator file or URL. 
| Layer| 1| LocatorURI is based on a Layer in the map 




## CIMMap
#### Represents a map or scene. A map is a container of geographic information. There are different kinds of geographic information within a map: imagery, terrain, and different kinds of vector data. The information in a map is organized into layers. A map contains an ordered list of layers, and draws each layer on top of its preceding layers. In 3D layers may be drawn in Z order and not layer order. A map has a single spatial reference system. Each of its layers can be stored natively in different spatial reference systems. If a layer has a different spatial reference system than a map it is displayed in, the map reprojects the data to its spatial reference system before drawing it. A map can dynamically place labels for its features. It finds optimal label locations for each map extent to maximize typographic clarity and to avoid overlaps. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the definition was last modified. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


### CIMMap 

|Property | Type | Description | 
|---------|--------|--------|
| defaultCamera | [CIMViewCamera](CIMMap.md#cimviewcamera) | The default camera. 
| illumination | [CIMIlluminationProperties](CIMMap.md#cimilluminationproperties) | The illumination properties. 
| layers | [string] | The layers as an array of layer repository paths. 
| standaloneTables | [string] | The standalone tables as an array of table repository paths. 
| stereoProperties | [CIMMapStereoProperties](CIMMap.md#cimmapstereoproperties) | The stereo properties. 
| defaultViewingMode | [enumeration MapViewingMode](CIMEnumerations.md#enumeration-mapviewingmode) | The default viewing mode. 
| mapType | [enumeration MapType](CIMMap.md#enumeration-maptype) | The map type. 
| rangeSliderSettings | [CIMSliderSettings](CIMMap.md#cimslidersettings) | The range slider settings. 
| timeSliderSettings | [CIMSliderSettings](CIMMap.md#cimslidersettings) | The time slider settings. 
| animationViewTracks | [CIMViewTrack](CIMMap.md#cimviewtrack) | The collection of view tracks in the animation. 
| locators | [CIMLocator](CIMMap.md#cimlocator) | The locators as an ordered array. 
| mapContexts | [string] | An array string values used to provide a hint for the intended context for the map. 
| standaloneVideos | [string] | The standalone videos as an array of video repository paths. 


### CIMMapDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundColor | [Color](Types.md#color) | The background color. 
| bookmarks | [CIMBookmark](CIMMap.md#cimbookmark) | The bookmarks. 
| clipToFullExtent | boolean | A value indicating whether or not to clip to full extent. 
| attribution | string | The attribution text that will appear on the map when it is drawn. 
| customFullExtent | [Polygon](ExternalReferences.md#polygon) | The custom full extent as a polygon. 
| datumTransforms | [CIMDatumTransform](CIMMap.md#cimdatumtransform) | The set of geographic transformations used by the map for spatial references that do not have vertical coordinate system. 
| defaultExtent | [Envelope](ExternalReferences.md#envelope) | The extent shown when you open new views of the map. The application automatically updates this property whenever you save a project with an active map view. 
| defaultScale | double | The scale used when you open new views of the map. When set, the application automatically applies this property after DefaultExtent to ensure the view is at the correct scale. 
| defaultGlobeTransparency | double | The transparency of the spheroid's combined terrain mesh and draped content. 
| defaultRotation | double | The default rotation. 
| description | string | The long description of the map. 
| elevationSurfaces | [CIMMapElevationSurface](CIMMap.md#cimmapelevationsurface) | The elevation surfaces. 
| generalPlacementProperties | [GeneralPlacementProperties](Types.md#generalplacementproperties) | The general label placement properties for dynamic labels in the map. 
| scaleLevels | [double] | The scale levels of the map. 
| snappingProperties | [CIMSnappingProperties](CIMMap.md#cimsnappingproperties) | The snapping properties of the map. 
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The map's spatial reference. 
| surfaceColor | [Color](Types.md#color) | The color of the default spheroid. 
| timeDisplay | [CIMMapTimeDisplay](CIMMap.md#cimmaptimedisplay) | The time display properties. 
| enableNavigationBelowGround | boolean | A value indicating whether or to enable navigation below the ground. 
| referenceScale | double | The map reference scale. 
| enableWraparound | boolean | A value indicating whether or to enable wraparound when the coordinate system supports it. 
| includeMaximumInScaleRanges | boolean | A value indicating whether or not to draw up to and including the maximum scale in scale ranges. 
| colorModel | [enumeration ColorModel](CIMEnumerations.md#enumeration-colormodel) | The color model for a map. 
| scales | [CIMScale](CIMMap.md#cimscale) | An array of CIMScale objects, describing the full list of named scales for the map. 
| scaleFormat | [CIMScaleFormat](CIMMap.md#cimscaleformat) | The scale format describing the formatting of the scale value. 
| scaleDisplayFormat | [enumeration ScaleDisplayFormat](CIMMap.md#enumeration-scaledisplayformat) | The display mode for the map's Scales in the user interface. 
| HVDatumTransforms | [ArrayOfCompositeHVDatumTransformation](ExternalReferences.md#arrayofcompositehvdatumtransformation) | The set of geographic transformations used by the map for spatial references with vertical coordinate system. 
| useServiceLayerIDs | boolean | A value indicating whether to allow the use of unique numeric IDs on layers that will be used when publishing services. 
| groundToGridCorrection | [CIMGroundToGridCorrection](CIMMap.md#cimgroundtogridcorrection) | The Ground To Grid Correction properties. 
| clippingMode | [enumeration ClippingMode](CIMMap.md#enumeration-clippingmode) | The clipping mode for a map. 
| customClippingShapeURI | string | The URI of the custom clipping shape used when the clipping mode is set to CustomShape. 
| layersExcludedFromClipping | [string] | The layers to be excluded from clipping. The layers are defined as an array of layer repository paths. 
| surfacesExcludedFromClipping | [string] | The surfaces to be excluded from clipping. The surfaces are defined as an array of surface IDs. 
| clippingAreaBorderSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The border symbol used for displaying the clipping area. 
| nearPlaneClipDistanceMode | [enumeration ClipDistanceMode](CIMMap.md#enumeration-clipdistancemode) | The near plane clipping mode for a scene. This property applies to only local and global viewing modes. 
| nearPlaneClipDistance | double | The near plane clip distance in meters for a scene. This property applies to only local and global viewing modes. 






## CIMMapElevationSurface
#### Represents a map elevation surface. 


### CIMMapElevationSurface 

|Property | Type | Description | 
|---------|--------|--------|
| baseSources | [CIMElevationSource](CIMMap.md#cimelevationsource) | The elevation sources. 
| elevationMode | [enumeration ElevationMode](CIMEnumerations.md#enumeration-elevationmode) | The elevation mode. 
| name | string | The elevation name. 
| verticalExaggeration | double | The vertical exaggeration. 
| mapElevationID | string | The map elevation ID. 
| color | [Color](Types.md#color) | The surface color. 
| enableSurfaceShading | boolean | A value indicating whether this elevation surface has shadows. 
| surfaceTINShadingMode | [enumeration SurfaceTINShadingMode](CIMMap.md#enumeration-surfacetinshadingmode) | The elevation surface shading mode for TIN elevation sources. 
| visibility | boolean | A value indicating whether the elevation surface is visible. 
| metadataURI | string | The elevation metadata URI. 
| offset | double | The vertical exaggeration. 
| expanded | boolean | A value indicating whether the elevation surface is expanded in the contents pane. 






## CIMMapStereoProperties
#### Represents map stereo properties. 


### CIMMapStereoProperties 

|Property | Type | Description | 
|---------|--------|--------|
| leftImage | [DataConnection](Types.md#dataconnection) | The left image of the stereo pair. 
| rightImage | [DataConnection](Types.md#dataconnection) | The right image of the stereo pair. 
| sourceType | [enumeration StereoSourceType](CIMMap.md#enumeration-stereosourcetype) | The stereo source type. 
| stereoModelCollection | [DataConnection](Types.md#dataconnection) | The data connection to the source stereo model collection. 
| leftImageID | long64 | The OID of the left image of the current stereo model in a collection. 
| rightImageID | long64 | The OID of the right image of the current stereo model in a collection. 
| leftImageColorizer | [CIMRasterColorizer](CIMImageLayers.md#cimrastercolorizer) | The colorizer for the left image. 
| rightImageColorizer | [CIMRasterColorizer](CIMImageLayers.md#cimrastercolorizer) | The colorizer for the right image. 
| adjustColorizersInSync | boolean | A value indicating whether adjustments to either colorizer should be synced to the other. 
| isInverted | boolean | A value indicating whether the left and right images of the stereo model should be swapped. 
| stereoModelDisplayMode | [enumeration StereoModelDisplayMode](CIMMap.md#enumeration-stereomodeldisplaymode) | The stereo model display mode. 






## CIMMapTimeDisplay
#### Represents map time display. 


### CIMMapTimeDisplay 

|Property | Type | Description | 
|---------|--------|--------|
| currentTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The current time extent. 
| defaultTimeInterval | double | The default time interval. 
| defaultTimeIntervalUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The default time interval units. 
| defaultTimeWindow | double | The default time window. 
| fullTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The full time extent. 
| timeReference | [TimeReference](ExternalReferences.md#timereference) | The time reference. 
| timeValue | [TimeValue](ExternalReferences.md#timevalue) | The time value. 
| hasLiveData | boolean | A value indicating whether or not this map has live data. 
| timeRelation | [enumeration esriTimeRelation](ExternalReferences.md#enumeration-esritimerelation) | The time relation. 





### Enumeration: MapType
#### Types of maps. 

|Property | Value | Description | 
|---------|--------|--------|
| Map| 0| A 2D map. 
| Scene| 1| A scene. 
| Basemap| 2| A basemap. 
| NetworkDiagram| 3| A network diagram. 
| ContainmentMap| 4| A containment map. 




## CIMScale
#### Represents a 2D scale or 3D Distance. 


### CIMScale 

|Property | Type | Description | 
|---------|--------|--------|
| value | double | The numeric value representing the 2D scale or 3D distance. 
| alias | string | The string value for the alias name of the Scale. 





### Enumeration: ScaleDisplayFormat
#### Scale display formats. 

|Property | Value | Description | 
|---------|--------|--------|
| Value| 0| Show just the Scale value. 
| Alias| 1| Show just the Scale alias name. 
| ValueAndAlias| 2| Show the Scale value, and then the Scale alias name. 
| AliasAndValue| 3| Show the Scale alias name, and then the Scale value. 




## CIMScaleFormat
#### Represents the scale formatting options. 


### CIMScaleFormat 

|Property | Type | Description | 
|---------|--------|--------|
| formatType | [enumeration ScaleFormatType](CIMMap.md#enumeration-scaleformattype) | The format used to display scale, i.e., 1:20000 or 1 inch equals 5 miles. 
| separator | string | The character(s) used to separate '1' from the scale in an absolute scale, e.g ':' in 1:20000. 
| reverseOrder | boolean | A value indicating whether to reverse the standard order. e.g. [1:1000] becomes [1000:1] and [1 in=10 mi] becomes [10 mi=1 in]. 
| decimalPlacesThreshold | double | The number the scale has to be less than or equal to display decimal places. 
| decimalPlaces | long | The number decimal places. 
| showThousandSeparator | boolean | A value indicating whether to show the thousands separator, e.g., 1:20,000. 
| pageUnits | [LinearUnit](ExternalReferences.md#linearunit) | The page units used to display a scale,e.g, the 'inch' in 1 inch=5 miles. 
| pageUnitValue | double | The number preceding the page units in a scale, i.e., the '1' in 1 inch=5 miles. 
| equalsSign | string | The text used for 'equals', e.g, '=' in 1 inch=5 miles. 
| mapUnits | [LinearUnit](ExternalReferences.md#linearunit) | The map units used to display a scale, e.g, the 'miles' in 1 inch=5 miles. 
| capitalizeUnits | boolean | A value indicating whether to capitalize the units in the scale string. 
| abbreviateUnits | boolean | A value indicating whether to abbreviate the units in the scale string. 





### Enumeration: ScaleFormatType
#### Scale format types. 

|Property | Value | Description | 
|---------|--------|--------|
| Absolute| 0| Display absolute format, e.g. 1:20000. 
| Imperial| 1| Display imperial format, e.g. 1 in = 1 mi. 




## CIMSliceBoxEADefinition
#### Represents a slice box exploratory analysis definition. 


### CIMExploratoryAnalysisDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| ID | long | The id. 


### CIMSliceBoxEADefinition 

|Property | Type | Description | 
|---------|--------|--------|
| centerPoint | [Point](ExternalReferences.md#point) | The center position. 
| heading | double | The heading in degrees from North. 0 is North, 90 is West, 180 is South, -90 is East, etc. 
| height | double | The height. 
| width | double | The width. 
| depth | double | The depth. 
| cullDirection | [enumeration CullDirection](CIMMap.md#enumeration-culldirection) | The depth. 






## CIMSliceCylinderEADefinition
#### Represents a slice cylinder exploratory analysis definition. 


### CIMExploratoryAnalysisDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| ID | long | The id. 


### CIMSliceCylinderEADefinition 

|Property | Type | Description | 
|---------|--------|--------|
| centerPoint | [Point](ExternalReferences.md#point) | The observer position. 
| heading | double | The heading in degrees from North. 0 is North, 90 is West, 180 is South, -90 is East, etc. 
| pitch | double | The pitch in degrees from horizontal. 0 is horizontal, 90 is looking directly up and -90 is looking directly down. 
| height | double | The height. 
| width | double | The width. 
| cullDirection | [enumeration CullDirection](CIMMap.md#enumeration-culldirection) | The direction that is clipped. 






## CIMSlicePlaneEADefinition
#### Represents a slice plane exploratory analysis definition. 


### CIMExploratoryAnalysisDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| ID | long | The id. 


### CIMSlicePlaneEADefinition 

|Property | Type | Description | 
|---------|--------|--------|
| centerPoint | [Point](ExternalReferences.md#point) | The observer position. 
| heading | double | The heading in degrees from North. 0 is North, 90 is West, 180 is South, -90 is East, etc. 
| pitch | double | The pitch in degrees from horizontal. 0 is horizontal, 90 is looking directly up and -90 is looking directly down. 
| height | double | The height. 
| width | double | The width. 
| cullDirection | [enumeration CullDirection](CIMMap.md#enumeration-culldirection) | The direction that is clipped. 






## CIMSliceSphereEADefinition
#### Represents a slice sphere exploratory analysis definition. 


### CIMExploratoryAnalysisDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| ID | long | The id. 


### CIMSliceSphereEADefinition 

|Property | Type | Description | 
|---------|--------|--------|
| centerPoint | [Point](ExternalReferences.md#point) | The observer position. 
| radius | double | The analysis distance from the center position. 
| cullDirection | [enumeration CullDirection](CIMMap.md#enumeration-culldirection) | The direction that is clipped. 





### Enumeration: SliderExtentType
#### Slider extent types. 

|Property | Value | Description | 
|---------|--------|--------|
| AllLayers| 0| All layers. 
| VisibleLayers| 1| Visible layers. 
| SingleLayer| 2| A single layer. 
| CustomRange| 3| A custom range. 



### Enumeration: SliderInteractionMode
#### Slider interaction modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Slider| 0| Present the values on a slider as a range 
| Picker| 1| Present the values individually 




## CIMSliderSettings
#### Represents slider settings. 


### CIMSliderSettings 

|Property | Type | Description | 
|---------|--------|--------|
| sliderExtent | [CIMRange](CIMVectorLayers.md#cimrange) | The extent shown on the slider. 
| sliderExtentLocked | boolean | A value indicating whether the slider extent will not change due to scrolling or using the mouse wheel. 
| startValueLocked | boolean | A value indicating whether the slider's start thumb will not accept mouse events. 
| endValueLocked | boolean | A value indicating whether the slider's end thumb will not accept mouse events. 
| flipVertically | boolean | A value indicating whether the slider is flipped vertically to put larger values at the bottom and smaller values at the top. 
| useWindowValue | boolean | A value indicating whether the distance between the start and end thumbs will remain constant. 
| windowValue | double | The value of the window on the slider. 
| windowUnit | string | The unit of the window on the slider (for time it could be days, weeks, months, etc.). 
| stepUsesWindow | boolean | A value indicating whether the step interval value will stay in sync with the sliders value window when possible. 
| stepIntervalValue | double | The specific distance to move the thumbs by when stepping or playing. 
| stepIntervalUnit | string | The unit the interval value is in (for time it could by days, weeks, months, etc..) 
| stepCount | double | The number of steps to divide the slider extent into. 
| stepOption | [enumeration SliderStepType](CIMMap.md#enumeration-slidersteptype) | The chosen method of determining the step size. 
| playWaitSeconds | double | The amount of time to wait between steps. 
| playForward | boolean | A value indicating whether the play direction is forward. 
| playRepeats | boolean | A value indicating whether play continuously repeats until interrupted by user interaction. 
| playReverses | boolean | A value indicating whether play direction will reverse after playing to the end (if repeat is false play will move each direction once then stop). 
| fullExtentOption | [enumeration SliderExtentType](CIMMap.md#enumeration-sliderextenttype) | The option that determines the extent used by the full extent button. 
| fullExtentLayerURI | string | The URI of the layer used for the full extent with single layer full extent option. 
| fullExtentCustomRange | [CIMRange](CIMVectorLayers.md#cimrange) | The custom full extent used with the custom range full extent option. 
| interactionMode | [enumeration SliderInteractionMode](CIMMap.md#enumeration-sliderinteractionmode) | Slider interaction mode. 
| useTimeSnapping | boolean | A value indicating whether automatic snapping for the map's current time settings is enabled. 
| timeSnapMode | [enumeration TimeSnapMode](CIMMap.md#enumeration-timesnapmode) | The option that determines mode used for snapping the map's current time settings. 
| singleTimeSnapUnit | string | The time unit to snap to when in 'Single' time snapping mode. 
| aliasExpressionLayerURI | string | The string containing URI of the layer that contains the alias definition. 
| isMinimized | boolean | A value indicating whether to collapse the slider over the map view. 





### Enumeration: SliderStepType
#### Slider step types. 

|Property | Value | Description | 
|---------|--------|--------|
| Interval| 0| Interval. 
| Count| 1| Count. 
| Feature| 2| Feature. 



### Enumeration: SnapRequestType
#### Snap request types. 

|Property | Value | Description | 
|---------|--------|--------|
| SnapRequestType_None| 0| No snapping. 
| SnapRequestType_GeometricSnapping| 1| Geometric snapping. 
| SnapRequestType_VisualSnapping| 2| Visual snapping. 
| SnapRequestType_GeometricAndVisualSnapping| 3| Geometric and visual snapping. 



### Enumeration: SnapXYToleranceUnit
#### Snap XY tolerance units. 

|Property | Value | Description | 
|---------|--------|--------|
| SnapXYToleranceUnitPixel| 0| Pixels. 
| SnapXYToleranceUnitMap| 1| Map units. 




## CIMSnappingProperties
#### Represents snapping properties. 


### CIMSnappingProperties 

|Property | Type | Description | 
|---------|--------|--------|
| XYTolerance | double | The XY tolerance. 
| XYToleranceUnit | [enumeration SnapXYToleranceUnit](CIMMap.md#enumeration-snapxytoleranceunit) | The XY tolerance unit. 
| ZTolerance | double | The Z tolerance. 
| ZToleranceEnabled | boolean | A value indicating whether Z tolerance is enabled. 
| snapToSketchEnabled | boolean | A value indicating whether snapping to the sketch is enabled. 
| snapRequestType | [enumeration SnapRequestType](CIMMap.md#enumeration-snaprequesttype) | The snap request type. 
| geometricFeedbackColor | [Color](Types.md#color) | Geometric feedback color. 
| visualFeedbackColor | [Color](Types.md#color) | The visual feedback color. 





### Enumeration: StereoModelDisplayMode
#### Stereo model display modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Default| 0| Display both the left and right images of the stereo model. 
| OnlyLeftImage| 1| Display only the left image of the stereo model. 
| OnlyRightImage| 2| Display only the right image of the stereo model. 
| None| 3| Turn off stereo model. 



### Enumeration: StereoSourceType
#### Stereo source types. 

|Property | Value | Description | 
|---------|--------|--------|
| StereoModel| 0| Stereo source is a single stereo model (image pair). 
| StereoModelCollection| 1| Stereo source is a collection of stereo models (image pairs). 



### Enumeration: SurfaceTINShadingMode
#### Surface TIN shading modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Smooth| 0| Smooth shading. 
| Flat| 1| Flat shading. 



### Enumeration: SwipeDirection
#### Represents the direction from an edge of the view used to clip a layer. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| None 
| Top| 1| Top 
| Bottom| 2| Bottom 
| Left| 3| Left 
| Right| 4| Right 



### Enumeration: TimeSnapMode
#### Mode used for snapping the map's current time settings. 

|Property | Value | Description | 
|---------|--------|--------|
| Automatic| 0| Snap to an automatically-calculated time unit, based on the map's full time extent and view window size 
| Single| 1| Snap to a user-specified time unit, such as "Minute" or "Year" 
| Interval| 2| Snap to the time-interval value that has been defined for the Range Slider 




## CIMViewCamera
#### Represents a view camera. 


### CIMViewCamera 

|Property | Type | Description | 
|---------|--------|--------|
| heading | double | The heading. 
| pitch | double | The pitch. 
| roll | double | The roll. 
| scale | double | The scale. 
| x | double | X. 
| y | double | Y. 
| z | double | Z. 
| viewportHeight | double | The height of the viewport in meters. Viewport height and width are used for consistent camera positioning in isometric 3D views, eye separation in 3D stereo views and defines the focal distance in perspective views. 
| viewportWidth | double | The width of the viewport in meters. Viewport height and width are used for consistent camera positioning in isometric 3D views, eye separation in 3D stereo views and defines the focal distance in perspective views. 






## CIMViewDomeEADefinition
#### Represents a view dome exploratory analysis definition. 


### CIMExploratoryAnalysisDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| ID | long | The id. 


### CIMViewDomeEADefinition 

|Property | Type | Description | 
|---------|--------|--------|
| observer | [Point](ExternalReferences.md#point) | The observer position. 
| maximumDistance | double | The maximum distance to be analyzed. 
| minimumDistance | double | The maximum distance to be analyzed. 






## CIMViewKeyframe
#### Represents a view keyframe. 


### CIMViewKeyframe 

|Property | Type | Description | 
|---------|--------|--------|
| trackTime | double | The value of time in seconds that the keyframe exists in the track. 
| camera | [CIMKeyframeCamera](CIMMap.md#cimkeyframecamera) | The camera keyframe. 
| layers | [CIMKeyframeLayer](CIMMap.md#cimkeyframelayer) | The collection of layer keyframes. 
| range | [CIMKeyframeRange](CIMMap.md#cimkeyframerange) | The range keyframe. 
| time | [CIMKeyframeTime](CIMMap.md#cimkeyframetime) | The time keyframe. 
| surfaces | [CIMKeyframeSurface](CIMMap.md#cimkeyframesurface) | The collection of surface keyframes. 
| exploratoryAnalysis | [CIMKeyframeAnalysis](CIMMap.md#cimkeyframeanalysis) | The collection of exploratory analysis. 






## CIMViewTrack
#### Represents a animation view track. 


### CIMViewTrack 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the track. 
| keyframes | [CIMViewKeyframe](CIMMap.md#cimviewkeyframe) | The collection of view keyframes. 
| screenGraphics | [CIMAnimationScreenGraphic](CIMMap.md#cimanimationscreengraphic) | The list of graphic overlays used in the animation. 
| referenceResolutionWidth | long | The desired pixel width the animation was made to export at. 
| referenceResolutionHeight | long | The desired pixel height the animation was made to export at. 






## CIMViewshedEADefinition
#### Represents a viewshed exploratory analysis definition. 


### CIMExploratoryAnalysisDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| ID | long | The id. 


### CIMViewshedEADefinition 

|Property | Type | Description | 
|---------|--------|--------|
| observer | [Point](ExternalReferences.md#point) | The observer position. 
| heading | double | The heading in degrees from North. 0 is North, 90 is West, 180 is South, -90 is East, etc. 
| pitch | double | The pitch in degrees from horizontal. 0 is horizontal, 90 is looking directly up and -90 is looking directly down. 
| horizontalAngle | double | The horizontal viewing angle. 
| verticalAngle | double | The vertical viewing angle. 
| maximumDistance | double | The maximum distance to be analyzed. 
| minimumDistance | double | The minimum distance to be analyzed. 



