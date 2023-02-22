


## CIM3DLayerProperties
#### Represents 3D layer properties which contain properties used for 3D draw. 


### CIM3DLayerProperties 

|Property | Type | Description | 
|---------|--------|--------|
| castShadows | boolean | A value indicating whether shadows are enabled. If true, this layer's features contribute to shadows. 
| isLayerLit | boolean | A value indicating whether this layer is lit. This property determines whether an object in 3D is shaded based on the angle of its normal compared to the lighting properties of the scene (where the "sun" is) or is lit uniformly as if by only ambient light (light with no distinct directionality). 
| layerFaceCulling | [enumeration FaceCulling3D](CIMEnumerations.md#enumeration-faceculling3d) | The layer's face culling setting. 
| maxDistance | double | The maximum distance at which objects in view are visible. Objects beyond this point don't get rendered. 
| maxPreloadDistance | double | The maximum radius from the camera at which objects outside the view are loaded. Values are in Meters. 
| minDistance | double | The minimum distance at which objects in view are visible. Objects closer than this don't get rendered. 
| minPreloadDistance | double | The minimum radius from the camera at which objects at which objects outside the view are loaded. Values are in Meters. 
| preloadTextureCutoffHigh | double | The distance (in visible range) at which high resolution textures change to low resolution textures for objects outside the view. Range is 0 to 1. 
| preloadTextureCutoffLow | double | The distance (in visible range) at which low resolution textures change to solid colors for objects outside the view. Range is 0 to 1. 
| textureCutoffHigh | double | The distance (in visible range) at which the high resolution textures change to low resolution textures. Range is 0 to 1. 
| textureCutoffLow | double | The distance (in visible range) at which the high resolution textures change to solid colors. Range is 0 to 1. 
| textureDownscalingFactor | long | The downscaling factor. All textures for this layer are downscaled by this additional factor on loading. 
| useCompressedTextures | boolean | A value indicating whether uncompressed textures are compressed using DXT5 at load time. 
| verticalExaggeration | double | The layer's vertical exaggeration. 
| exaggerationMode | [enumeration ExaggerationMode](CIMLayer.md#enumeration-exaggerationmode) | The layer's exaggeration mode. 
| verticalUnit | [Unit](ExternalReferences.md#unit) | The layer's vertical unit. 
| depthPriority | long | The depth priority of a 3D layer. 
| lighting | [enumeration Lighting3D](CIMLayer.md#enumeration-lighting3d) | The layer's lighting setting. 
| optimizeMarkerTransparency | boolean | A value indicating whether true alpha is quantized to fully opaque or transparent when false, actual values are used in marker drawing. 
| useDepthWritingForTransparency | boolean | A value indicating whether to use depth writing for transparency. This should be set to true if anomalies are seen in drawing order of transparent features in the same feature class. 






## CIMCompositeSubLayer
#### Represents a composite sublayer. 


### CIMSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| name | string | The name. 
| showLegends | boolean | A value indicating whether or not to show legends. 
| subLayerID | string | The sublayer ID. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 


### CIMCompositeSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| subLayers | [[CIMSubLayerBase]](CIMLayer.md#cimsublayerbase) | The composite sublayers. 






## CIMDefinitionFilter
#### Contains filters so that only features satisfying these definitions will be displayed. 


### CIMDefinitionFilter 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the Definition Filter item. 
| definitionExpression | string | The definition expression to filter features in the dataset. 





### Enumeration: DisplayCacheType
#### Display cache types. 

|Property | Value | Description | 
|---------|--------|--------|
| Permanent| 0| Cache is permanent. 
| InSession| 1| Cache is maintained in session. 
| None| 2| No cache. 
| MaxAge| 3| Cache expires when it reaches the set maximum age. 




## CIMElementStorage
#### Represents a series of graphic elements stored offline. 


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMElementStorage 

|Property | Type | Description | 
|---------|--------|--------|
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The graphics' spatial reference. 
| symbols | [[CIMSymbolIdentifier]](CIMVectorLayers.md#cimsymbolidentifier) | The symbols used by graphic elements. The symbol reference inside graphic elements will have a null Symbol, and instead refer to a symbol in this collection by name. The names are generated programmatically. 






## CIMElevationSurfaceLayer
#### Represents an elevation surface layer. 


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


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The URIs of the layers used as masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 


### CIMElevationSurfaceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| elevationSourceLayers | [string] | The sublayers. 
| elevationMode | [enumeration ElevationMode](CIMEnumerations.md#enumeration-elevationmode) | The elevation mode. 
| verticalExaggeration | double | The vertical exaggeration. 
| color | [Color](Types.md#color) | The surface color. 
| enableSurfaceShading | boolean | A value indicating whether this elevation surface has shadows. 
| surfaceTINShadingMode | [enumeration SurfaceTINShadingMode](CIMMap.md#enumeration-surfacetinshadingmode) | The elevation surface shading mode for TIN elevation sources. 
| useSurfaceEffect | boolean | A value indicating whether the current surface effect should be applied in 3D views. 
| surfaceEffect | [SurfaceEffect](Types.md#surfaceeffect) | The surface effect definition for the elevation surface. 





### Enumeration: ExaggerationMode
#### Represents the exaggeration modes. 

|Property | Value | Description | 
|---------|--------|--------|
| ScaleZ| 0| Multiply z-coordinate by the exaggeration factor. 
| ScaleVoxelHeight| 1| Multiply the height (z-dimension) of a voxel by the exaggeration factor. The origin of the layer will remain unchanged. This option is valid for Voxel layer. 




## CIMEyeDomeLighting
#### Represents eye-dome lighting properties. 


### CIMEyeDomeLighting 

|Property | Type | Description | 
|---------|--------|--------|
| isEnabled | boolean | A value indicating whether eye-dome lighting is enabled. 
| strength | double | The strength of the eye-dome lighting. This property can have a value between 0 and 1. 
| radius | double | The radius of the eye-dome lighting. This property can have a value between 1 and 5. 






## CIMGeodatabaseErrorLayer
#### Represents GDB Error tables as a composite layer and draws the errors. 


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


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The URIs of the layers used as masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 


### CIMStandaloneTableContainer 

|Property | Type | Description | 
|---------|--------|--------|
| standaloneTables | [string] | The standalone tables as an array of table repository paths. 


### CIMGeodatabaseErrorLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| pointLayer | string | The path of the point layer in the Geodatabase Error layer. 
| lineLayer | string | The path of the line layer in the Geodatabase Error layer. 
| polygonLayer | string | The path of the polygon layer in the Geodatabase Error layer. 
| objectTable | string | The path of the object table in the Geodatabase Error layer. 
| workspaceConnection | [CIMWorkspaceConnection](CIMVectorLayers.md#cimworkspaceconnection) | The Geodatabase Errors data connection to the parent workspace. 






## CIMGraphicsLayer
#### Represents a layer of simple graphic elements. 


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


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The URIs of the layers used as masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 


### CIMGraphicsLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| elementStorageURI | string | The URI of the storage for the graphic elements themselves. 
| referenceScale | double | The graphics' reference scale. This value takes precedence over any reference scale on the map. 
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight) | The weight of graphics in this layer when considered as barriers to labeling. 
| snappable | boolean | A value indicating whether this layer participates in snapping. 
| selectable | boolean | A value indicating whether this layer is selectable. 
| showInvisibleGraphics | boolean | A value indicating whether this layer should show invisible graphics. 
| invisibleGraphicsColor | [Color](Types.md#color) | The color of invisible graphics. 






## CIMGroupLayer
#### Represents a group layer which is a simple ordered collection of other layers. 


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


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The URIs of the layers used as masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 


### CIMStandaloneTableContainer 

|Property | Type | Description | 
|---------|--------|--------|
| standaloneTables | [string] | The standalone tables as an array of table repository paths. 


### CIMGroupLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| layers | [string] | The layer URIs of the layers in the group layer. 
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing) | The symbol layer drawing definition. 






## CIMKMLDataConnection
#### Represents a KML data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceDataConnectionProperties 

|Property | Type | Description | 
|---------|--------|--------|
| customParameters | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | Vendor specific parameters. 


### CIMKMLDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| KMLURI | string | The URI of the KML file or resource. 






## CIMKMLLayer
#### Represents a KML layer. 


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


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The URIs of the layers used as masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 


### CIMKMLLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [CIMKMLDataConnection](CIMLayer.md#cimkmldataconnection) | The data connection to the KML resource. 
| selectable | boolean | A value indicating whether the layer is selectable. 
| selectionColor | [Color](Types.md#color) | The selection color. 
| useSelectionColor | boolean | A value indicating whether to use the selection color. 
| labelVisibility | boolean | A value indicating whether to display labels for this KML layer's placemarks. 
| textSymbol | [CIMTextSymbol](CIMSymbols.md#cimtextsymbol) | The text symbol used to label placemarks. 






## CIMLayerElevationSurface
#### Represents a layer elevation surface. 


### CIMLayerElevationSurface 

|Property | Type | Description | 
|---------|--------|--------|
| offsetZ | double | Z offset. 
| elevationSurfaceLayerURI | string | The elevation surface layer URI. 
| isRelativeToScene | boolean | A value indicating whether to display the data relative to scene. 






## CIMLayerTemplate
#### Represents a layer template. 


### CIMLayerTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| layerTemplateId | string | The layer template ID. 
| parameters | {JSON_object}| The layer template parameters. 





### Enumeration: Lighting3D
#### The types of lighting. 

|Property | Value | Description | 
|---------|--------|--------|
| OneSideDataNormal| 0| Lights one side of each face using the original data normals. 
| OneSideResetNormal| 1| Lights one side of each face using recalculated normals. 
| TwoSideDataNormal| 2| Lights both sides of each face using original data normals. 
| TwoSideResetNormal| 3| Lights both sides of each face using recalculated normals. 
| TwoSideDataNormalFromWindingOrder| 4| Lights both sides of each face using original data normals, and the winding order for the "out" direction. 
| TwoSideResetNormalFromWindingOrder| 5| Lights both sides of each face using recalculated normal, and the winding order for the "out" direction. 



### Enumeration: SortOrderType
#### Options to choose sort order type. 

|Property | Value | Description | 
|---------|--------|--------|
| Ascending| 0| Sort ascending. 
| Descending| 1| Sort descending. 




## CIMSubLayer
#### Represents sublayer. Defines a sublayer for a containing parent layer. The parent layer is a full-fledged layer, and it controls the sublayer, which is subordinate to the parent. The sublayer is not a layer definition itself rather, it is a property of its parent layer. 


### CIMSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| name | string | The name. 
| showLegends | boolean | A value indicating whether or not to show legends. 
| subLayerID | string | The sublayer ID. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 






## CIMSymbolLayerDrawing
#### Represents symbol layer drawing properties. 


### CIMSymbolLayerDrawing 

|Property | Type | Description | 
|---------|--------|--------|
| symbolLayers | [[CIMSymbolLayerIdentifier]](CIMLayer.md#cimsymbollayeridentifier) | The symbol layer identifiers. 
| useSymbolLayerDrawing | boolean | A value indicating whether symbol layer drawing is enabled. 






## CIMSymbolLayerIdentifier
#### Represents symbol layer identifier. 


### CIMSymbolLayerIdentifier 

|Property | Type | Description | 
|---------|--------|--------|
| symbolLayerName | string | The symbol layer name. 






## CIMTopologyLayer
#### Represents a topology dataset as a layer and draws its errors, exceptions, and areas in need of validation. 


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


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The URIs of the layers used as masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 


### CIMTopologyLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| allLayers | [string] | The paths of the layers in the topology layer. 
| topologyConnection | [DataConnection](Types.md#dataconnection) | The topology data connection. 



