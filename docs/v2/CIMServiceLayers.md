


## CIMAGSServiceConnection
#### Represents an ArcGIS Server service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 


### CIMServiceDataConnectionProperties 

|Property | Type | Description | 
|---------|--------|--------|
| customParameters | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | Vendor specific parameters. 


### CIMAGSServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| objectName | string | The object name. 
| objectType | string | The object type. 
| URL | string | The URL. 
| capabilities | string | The capabilities. 
| serverConnection | [ServerConnection](Types.md#serverconnection) | The server connection. 
| gdbVersion | string | The name of the geodatabase version to use in service requests. 






## CIMBuildingDisciplineSceneLayer
#### Represents a building discipline scene layer. 


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
| layerMasks | [string] | The layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
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


### CIMBuildingDisciplineSceneLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| subLayers | [string] | The sublayers. 
| subLayerID | long | Identifier that will be used to identify the layer in a building. 






## CIMBuildingSceneLayer
#### Represents a building composite scene layer. 


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
| layerMasks | [string] | The layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
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


### CIMBuildingSceneLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| subLayers | [string] | The sublayers. 
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection to the workspace. 


### CIMObject3DRenderingFilters 

|Property | Type | Description | 
|---------|--------|--------|
| filters | [[CIMObject3DRenderingFilter]](CIMServiceLayers.md#cimobject3drenderingfilter) | The 3D object rendering filters. 
| activeFilterID | string | The ID of the filter currently used for rendering. 





### Enumeration: ConnectionMode
#### Connection modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Consumer| 0| User. 
| Admin| 1| Administrator. 
| Publisher| 2| Publisher. 




## CIMDynamicServiceCompositeSubLayer
#### Represents a dynamic service composite sublayer. 


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


### CIMDynamicServiceCompositeSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| definitionExpression | string | The definition expression. This property is used for composite layers that are backed by feature classes. 






## CIMDynamicServiceLayer
#### Represents a dynamic service layer. 


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
| layerMasks | [string] | The layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
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


### CIMServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection) | The service connection. 
| subLayers | [[CIMSubLayerBase]](CIMLayer.md#cimsublayerbase) | The sublayers. 
| transparentColor | [Color](Types.md#color) | The transparent color. 
| backgroundColor | [Color](Types.md#color) | The background color. 


### CIMDynamicServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| imageFormat | [enumeration esriImageFormat](ExternalReferences.md#enumeration-esriimageformat) | The image format. 
| useTime | boolean | A value indicating whether or not to use time. 






## CIMDynamicServiceSubLayer
#### Represents a dynamic service sublayer. 


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


### CIMDynamicServiceSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| showLabels | boolean | A value indicating whether or not to show labels. 
| scaleSymbols | boolean | A value indicating whether or not to scale symbols. 
| definitionExpression | string | The definition expression. 
| sourceID | string | The source ID. 
| useTime | boolean | A value indicating whether or not to use time. 
| drawTimeCumulative | boolean | A value indicating whether or not draw time cumulatively. 
| timeOffset | double | The time offset. 
| timeOffsetUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time offset units. 
| styleName | string | The style name. 
| layerDefinition | string | The layer definition. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 






## CIMGlobeServiceLayer
#### Represents a globe service layer. 


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
| layerMasks | [string] | The layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
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


### CIMServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection) | The service connection. 
| subLayers | [[CIMSubLayerBase]](CIMLayer.md#cimsublayerbase) | The sublayers. 
| transparentColor | [Color](Types.md#color) | The transparent color. 
| backgroundColor | [Color](Types.md#color) | The background color. 


### CIMGlobeServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| constantScreenSize | boolean | A value indicating whether or not to use constant screen size. If this property is true, then the size specified in the vector features in the cache are treated as points. Otherwise it is assumed they are meters. 
| snappable | boolean | A value indicating whether or not geometries are snappable. 






## CIMInternetServerConnection
#### Represents an internet server connection. 


### CIMServerConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMInternetServerConnection 

|Property | Type | Description | 
|---------|--------|--------|
| anonymous | boolean | A value indicating whether of not this is an anonymous connection. 
| hideUserProperty | boolean | A value indicating whether of not to hide the user. 
| password | string | The password. 
| URL | string | The URL. 
| user | string | The user. 






## CIMIsosurface
#### Represents a isosurface. 


### CIMIsosurface 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The ID. 
| color | [Color](Types.md#color) | The isosurface color. 
| isCustomColor | boolean | A value indicating whether the color was set by user. 
| value | double | The variable value. 
| variable | string | The variable. 
| name | string | The isosurface name. 
| visible | boolean | A value indicating whether the isosurface is visible. 






## CIMIsosurfaceGroup
#### Represents a isosurface group. 


### CIMIsosurfaceGroup 

|Property | Type | Description | 
|---------|--------|--------|
| isosurfaces | [[CIMIsosurface]](CIMServiceLayers.md#cimisosurface) | A collection of isosurfaces. 
| variable | string | The variable. 






## CIMIsosurfaceGroupContainer
#### Represents a isosurface group container. 


### CIMIsosurfaceGroupContainer 

|Property | Type | Description | 
|---------|--------|--------|
| groups | [[CIMIsosurfaceGroup]](CIMServiceLayers.md#cimisosurfacegroup) | A collection of isosurface groups. 
| visible | boolean | A value indicating whether the isosurface container is visible. 
| expanded | boolean | A value indicating whether the isosurface container is expanded in the contents pane. 






## CIMOGCAPIServiceConnection
#### Represents a OGCAPI service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 


### CIMOGCAPIServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| serviceName | string | The service name. 
| version | string | The version. 
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase) | The server connection. 
| capabilitiesParameters | {JSON_object}| Vendor specific parameters for all OGCAPI requests. 






## CIMObject3DRenderingFilter
#### Represents a 3D object rendering filter. 


### CIMObject3DRenderingFilter 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The ID. 
| name | string | The name. 
| description | string | The description. 
| filterBlocks | [[CIMObject3DRenderingFilterBlock]](CIMServiceLayers.md#cimobject3drenderingfilterblock) | The filter blocks. 
| authoringInfo | [CIMObject3DRenderingFilterAuthoringInfo](CIMServiceLayers.md#cimobject3drenderingfilterauthoringinfo) | The authoring info. 






## CIMObject3DRenderingFilterAuthoringInfo
#### Represents a filter authoring info. 


### CIMObject3DRenderingFilterAuthoringInfo 

|Property | Type | Description | 
|---------|--------|--------|
| isVisible | boolean | A value indicating whether the filter is displayed in the UI or not. 
| filterBlocks | [[CIMObject3DRenderingFilterBlockAuthoringInfo]](CIMServiceLayers.md#cimobject3drenderingfilterblockauthoringinfo) | The filter blocks. 






## CIMObject3DRenderingFilterBlock
#### Represents a 3D object rendering filter block. 


### CIMObject3DRenderingFilterBlock 

|Property | Type | Description | 
|---------|--------|--------|
| title | string | The title. 
| mode | [enumeration Object3DRenderingMode](CIMServiceLayers.md#enumeration-object3drenderingmode) | The rendering mode. 
| expression | string | The expression. 






## CIMObject3DRenderingFilterBlockAuthoringInfo
#### Represents a filter block authoring info. 


### CIMObject3DRenderingFilterBlockAuthoringInfo 

|Property | Type | Description | 
|---------|--------|--------|
| filterStates | [[CIMObject3DRenderingFilterState]](CIMServiceLayers.md#cimobject3drenderingfilterstate) | The filter state. 






## CIMObject3DRenderingFilterState
#### Represents a 3D object rendering filter value. 


### CIMObject3DRenderingFilterState 

|Property | Type | Description | 
|---------|--------|--------|
| filterType | string | The filter type. 
| selectedValues | [string] | The selected values. 





### Enumeration: Object3DRenderingMode
#### Specified how features are drawn. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Features drawn normally. 
| Wireframe| 1| Features are drawn as wireframe. 




## CIMProjectServerConnection
#### Represents a project server connection. 


### CIMServerConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMInternetServerConnection 

|Property | Type | Description | 
|---------|--------|--------|
| anonymous | boolean | A value indicating whether of not this is an anonymous connection. 
| hideUserProperty | boolean | A value indicating whether of not to hide the user. 
| password | string | The password. 
| URL | string | The URL. 
| user | string | The user. 


### CIMProjectServerConnection 

|Property | Type | Description | 
|---------|--------|--------|
| connectionMode | [enumeration ConnectionMode](CIMServiceLayers.md#enumeration-connectionmode) | The connection mode. 
| name | string | The name. 
| serverType | [enumeration ServerType](CIMServiceLayers.md#enumeration-servertype) | The server type. 
| stagingFolder | string | The staging folder. 
| useDefaultStagingFolder | boolean | A value indicating whether or not to use the default staging folder. 






## CIMSceneServiceLayer
#### Represents a scene service layer. 


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
| layerMasks | [string] | The layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
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


### CIMSceneServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMAGSServiceConnection](CIMServiceLayers.md#cimagsserviceconnection) | The service connection. 
| snappable | boolean | A value indicating whether the geometries are snappable. 
| renderer | [Renderer](Types.md#renderer) | The primary symbol renderer. 
| featureElevationExpression | string | The feature elevation expression. 
| labelClasses | [[CIMLabelClass]](CIMLabelPlacement.md#cimlabelclass) | The collection of label class definitions. 
| labelVisibility | boolean | A value indicating whether to display labels for this layer's label classes. 
| dataConnection | [CIMSceneDataConnection](CIMTerrainLayers.md#cimscenedataconnection) | The data connection. Currently used only when loading local scene layer packages. 
| useRealWorldSymbolSizes | boolean | A value indicating whether to use real world symbols sizes (meters) vs. points. 
| exclusionSet | [long long] | The set of excluded features. 
| definitionExpression | string | The definition expression that can subset the features. 
| definitionExpressionName | string | The Name of definition expression. 
| definitionFilterChoices | [[CIMDefinitionFilter]](CIMLayer.md#cimdefinitionfilter) | The definition filter choices. 
| associatedFeatureLayerURI | string | The URI to the associated feature layer. 
| sceneServiceLayerType | [enumeration SceneServiceLayerType](CIMServiceLayers.md#enumeration-sceneservicelayertype) | The scene service layer type. Typically set by the system and should not be modified. 
| selectable | boolean | A value indicating whether the layer is selectable. 
| selectionSetURI | string | The URI of the selection set for the layer. 
| modificationLayerURI | string | The URI of the modification layer. 
| modificationLayerEnabled | boolean | A value indicating whether the integrated mesh modification is enabled. 
| usePredefinedMaxScreenThreshold | boolean | A value indicating whether to use predefined max screen threshold as defined in the integrated mesh layer. 





### Enumeration: SceneServiceLayerType
#### Scene service layer types. 

|Property | Value | Description | 
|---------|--------|--------|
| IntegratedMesh| 0| Represents integrated mesh scene service layer type. 
| Point| 1| Represents point scene service layer type. 
| Object3D| 2| Represents 3D object scene service layer type. 



### Enumeration: ServerType
#### Server types. 

|Property | Value | Description | 
|---------|--------|--------|
| AGS| 0| ArcGIS Server. 
| WMS| 1| WMS. 
| WCS| 2| WCS. 
| WMTS| 3| WMTS. 
| WFS| 4| WFS. 
| OGCAPI| 5| OGCAPI. 




## CIMStandardServiceConnection
#### Represents a standard service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 


### CIMStandardServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| serviceProvider | string | The service provider. 
| serviceType | string | The service type. 
| URL | string | The service URL. 
| culture | string | The service culture. 






## CIMTiledServiceLayer
#### Represents a tiled service layer. 


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
| layerMasks | [string] | The layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
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


### CIMServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection) | The service connection. 
| subLayers | [[CIMSubLayerBase]](CIMLayer.md#cimsublayerbase) | The sublayers. 
| transparentColor | [Color](Types.md#color) | The transparent color. 
| backgroundColor | [Color](Types.md#color) | The background color. 


### CIMTiledServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| associatedFeatureLayerURI | string | The URI for a feature service or portal item that provides pop-up support for the layer. 






## CIMVoxelColorUniqueValue
#### Represents a voxel color unique value. 


### CIMVoxelColorUniqueValue 

|Property | Type | Description | 
|---------|--------|--------|
| value | long | The class value as a integer. 
| label | string | The class label. 
| color | [Color](Types.md#color) | The class color. 
| visible | boolean | A value indicating whether this class is visible. 
| description | string | The description. 






## CIMVoxelContinuousStatistics
#### Represents continuous voxel volume statistics. 


### CIMVoxelStatistics 

|Property | Type | Description | 
|---------|--------|--------|
| status | [enumeration VoxelStatisticsStatus](CIMServiceLayers.md#enumeration-voxelstatisticsstatus) | A value indicating whether the voxel section container is visible. 
| revision | long | A value indicating the statistics revision. 
| variable | string | The variable that the statistics are associated with. 
| minimumValue | double | The minimum value of the data. 
| maximumValue | double | The maximum value of the data. 


### CIMVoxelContinuousStatistics 

|Property | Type | Description | 
|---------|--------|--------|
| distributionMinimumValue | double | The minimum value of the quantized data. 
| distributionMaximumValue | double | The maximum value of the quantized data. 
| distribution | [double] | The quantized values of the data. 
| mean | double | The average value. 
| standardDeviation | double | The standard deviation value. 






## CIMVoxelDataConnection
#### Represents a voxel data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMVoxelDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string | The URI. 






## CIMVoxelDiscreteStatistics
#### Represents discrete voxel volume statistics. 


### CIMVoxelStatistics 

|Property | Type | Description | 
|---------|--------|--------|
| status | [enumeration VoxelStatisticsStatus](CIMServiceLayers.md#enumeration-voxelstatisticsstatus) | A value indicating whether the voxel section container is visible. 
| revision | long | A value indicating the statistics revision. 
| variable | string | The variable that the statistics are associated with. 
| minimumValue | double | The minimum value of the data. 
| maximumValue | double | The maximum value of the data. 


### CIMVoxelDiscreteStatistics 

|Property | Type | Description | 
|---------|--------|--------|
| mostFrequentValues | [long] | An array of the most frequently occurring values. 
| mostFrequentValuesCounts | [long] | An array of the counts of the most frequently occurring values. 






## CIMVoxelFormat
#### Represents a voxel format. 


### CIMVoxelFormat 

|Property | Type | Description | 
|---------|--------|--------|
| scale | double | The scaling factor for fixed point encoded data. 
| offset | double | The offset for fixed point encoded data. 
| useNoDataValue | boolean | A value indicating whether the native no data value should be used. 
| noDataValue | double | The native no data value. 
| scalarFormat | [enumeration VoxelScalarFormat](CIMServiceLayers.md#enumeration-voxelscalarformat) | The scalar format. 





### Enumeration: VoxelInterpolationMode
#### Voxel interpolation mode. 

|Property | Value | Description | 
|---------|--------|--------|
| Linear| 0| Linear interpolation 
| Nearest| 1| Nearest interpolation 




## CIMVoxelLayer
#### Represents a voxel layer. 


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
| layerMasks | [string] | The layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
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


### CIMVoxelLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| snappable | boolean | A value indicating whether this layer participates in snapping in the editor. 
| selectedVariableProfileIndex | long | The selected variable profile index. 
| variableProfiles | [[CIMVoxelVariableProfile]](CIMServiceLayers.md#cimvoxelvariableprofile) | The variable profiles. 
| optimization | [enumeration VoxelLayerOptimization](CIMServiceLayers.md#enumeration-voxellayeroptimization) | The voxel layer optimization. 
| isosurfaceGroupContainer | [CIMIsosurfaceGroupContainer](CIMServiceLayers.md#cimisosurfacegroupcontainer) | The isosurface group container. 
| sliceContainer | [CIMVoxelSliceContainer](CIMServiceLayers.md#cimvoxelslicecontainer) | The slice container. 
| sectionContainer | [CIMVoxelSectionContainer](CIMServiceLayers.md#cimvoxelsectioncontainer) | The section container. 
| staticSectionContainer | [CIMVoxelStaticSectionContainer](CIMServiceLayers.md#cimvoxelstaticsectioncontainer) | The static section container. 
| visualization | [enumeration VoxelVisualization](CIMServiceLayers.md#enumeration-voxelvisualization) | The voxel visualization. 
| surfaceContainerExpanded | boolean | A value indicating whether the surface container is expanded in the contents pane. 
| lighting | [CIMVoxelLighting](CIMServiceLayers.md#cimvoxellighting) | The lighting. 





### Enumeration: VoxelLayerOptimization
#### Represents voxel layer optimization. 

|Property | Value | Description | 
|---------|--------|--------|
| Visualization| 0| Voxel layer is optimized to maximize visualization performance. 
| Size| 1| Voxel layer is optimized to minimize size on disk. 




## CIMVoxelLighting
#### Represents voxel lighting. 


### CIMVoxelLighting 

|Property | Type | Description | 
|---------|--------|--------|
| isDiffuseEnabled | boolean | A value indicating whether diffuse lighting is enabled. 
| diffuse | double | The diffuse value. This property can have a value between 0 and 1. 
| isSpecularEnabled | boolean | A value indicating whether specular lighting is enabled. 
| specular | double | The specular value. This property can have a value between 0 and 1. 






## CIMVoxelPlane
#### Represents a voxel plane. 


### CIMVoxelPlane 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The ID. 
| name | string | The plane's name. 
| visible | boolean | A value indicating whether the plane is visible. 
| position | [Point](ExternalReferences.md#point) | A point on the plane, specified in voxel coordinates. 
| normal | [Point](ExternalReferences.md#point) | The direction vector of the plane, which is a unit vector representing the normal to the plane. This vector is perpendicular to the plane you are defining, and it points in the direction of what you want to remove with the plane. The X, Y, and Z values should all be between 0 and 1. For example a Normal of (0,0,1) is pointing away from the earth's surface, and this defines a horizontal plane. 






## CIMVoxelRangeValueFilter
#### Represents a voxel value filter. Filter based on the value of an specified variable. 


### CIMVoxelFilter 

|Property | Type | Description | 
|---------|--------|--------|
| variable | string | The variable. 


### CIMVoxelRangeValueFilter 

|Property | Type | Description | 
|---------|--------|--------|
| min | double | The min value. 
| max | double | The max value. 





### Enumeration: VoxelScalarFormat
#### Voxel scalar formats. 

|Property | Value | Description | 
|---------|--------|--------|
| I1| 0| 1 byte signed integer 
| U1| 1| 1 byte unsigned integer 
| I2| 2| 2 byte signed integer 
| U2| 3| 2 byte unsigned integer 
| I4| 4| 4 byte signed integer 
| U4| 5| 4 byte unsigned integer 
| I8| 6| 8 byte signed integer 
| U8| 7| 8 byte unsigned integer 
| F4| 8| 4 byte floating point 
| F8| 9| 8 byte floating point 




## CIMVoxelSectionContainer
#### Represents a voxel section container. 


### CIMVoxelSectionContainer 

|Property | Type | Description | 
|---------|--------|--------|
| dynamicSections | [[CIMVoxelPlane]](CIMServiceLayers.md#cimvoxelplane) | A collection of dynamic sections. 
| expanded | boolean | A value indicating whether this voxel section container is expanded in the contents pane. 
| visible | boolean | A value indicating whether the voxel section container is visible. 






## CIMVoxelSliceContainer
#### Represents a voxel slice container. 


### CIMVoxelSliceContainer 

|Property | Type | Description | 
|---------|--------|--------|
| slices | [[CIMVoxelPlane]](CIMServiceLayers.md#cimvoxelplane) | A collection of slices. 
| expanded | boolean | A value indicating whether this voxel slice container is expanded in the contents pane. 
| visible | boolean | A value indicating whether the voxel slice container is visible. 






## CIMVoxelStaticSection
#### Represents a voxel static section. 


### CIMVoxelStaticSection 

|Property | Type | Description | 
|---------|--------|--------|
| ID | long | The section ID, which must be unique among all sections in the layer. 
| name | string | The section name. 
| visible | boolean | A value indicating whether the section is visible. 
| expanded | boolean | A value indicating whether this section is expanded in the contents pane. 
| variable | string | The variable that the section is associated with. 
| slices | [[CIMVoxelPlane]](CIMServiceLayers.md#cimvoxelplane) | A collection of slices which define the volume for the section. 
| plane | [CIMVoxelPlane](CIMServiceLayers.md#cimvoxelplane) | The section plane. 
| rasterURI | string | The URI of the binary reference containing the raster. 
| format | [CIMVoxelFormat](CIMServiceLayers.md#cimvoxelformat) | The section format. 
| height | long | The height. 
| width | long | The width. 
| timeIndex | long | The time index that this section was created from for the variable. 






## CIMVoxelStaticSectionContainer
#### Represents a voxel static section container. 


### CIMVoxelStaticSectionContainer 

|Property | Type | Description | 
|---------|--------|--------|
| staticSections | [[CIMVoxelStaticSection]](CIMServiceLayers.md#cimvoxelstaticsection) | A collection of static sections. 
| expanded | boolean | A value indicating whether this voxel section container is expanded in the contents pane. 
| visible | boolean | A value indicating whether the voxel section container is visible. 





### Enumeration: VoxelStatisticsStatus
#### Specifies the status of statistics creation. 

|Property | Value | Description | 
|---------|--------|--------|
| Final| 0| Finalized statistics. 
| Partial| 1| Partial statistics. 
| NotSet| 2| Uninitialized statistics. 




## CIMVoxelStretchRenderer
#### Represents a stretch renderer. 


### CIMVoxelRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMVoxelStretchRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp of the renderer. 
| minLabel | string | The legend label for the minimum color range value. 
| maxLabel | string | The legend label for the maximum color range value. 
| isDataFilterEnabled | boolean | A value indicating whether data filter is enabled. 
| dataFilterMin | double | The minimum value. 
| dataFilterMax | double | The maximum value. 
| colorRangeMin | double | The minimum value. 
| colorRangeMax | double | The maximum value. 
| useTransparencyStops | boolean | A value indicating whether transparency stops are used. 
| transparencyStopPositions | [double] | The transparency stop positions. 
| transparencyStopValues | [double] | The transparency stop values. 
| heading | string | The heading. 
| interpolation | [enumeration VoxelInterpolationMode](CIMServiceLayers.md#enumeration-voxelinterpolationmode) | The interpolation mode. 
| showFullDataRange | boolean | A value indicating whether the histogram shows the full data range. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 






## CIMVoxelUniqueValueRenderer
#### Represents a unique value renderer. 


### CIMVoxelRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMVoxelUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| classes | [[CIMVoxelColorUniqueValue]](CIMServiceLayers.md#cimvoxelcoloruniquevalue) | The unique color classes of the renderer. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| heading | string | The heading. 
| useDefaultColor | boolean | A value indicating whether of not to use the default color. 
| defaultColor | [Color](Types.md#color) | The default color. 
| defaultLabel | string | The default label. 
| defaultDescription | string | The default description. 






## CIMVoxelValueFilter
#### Represents a voxel value filter. Filter based on the value of an specified variable. 


### CIMVoxelFilter 

|Property | Type | Description | 
|---------|--------|--------|
| variable | string | The variable. 


### CIMVoxelValueFilter 

|Property | Type | Description | 
|---------|--------|--------|
| values | [double] | The values used as exclude or include list. 
| mode | [enumeration VoxelValueFilterMode](CIMServiceLayers.md#enumeration-voxelvaluefiltermode) | The mode that determines if the ValueList is an include list or an exclude list. 





### Enumeration: VoxelValueFilterMode
#### Voxel value filter modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Exclude| 0| List of values in the exclude list 
| Include| 1| List of values in the include list 



### Enumeration: VoxelVariableDataType
#### Voxel variable data types. 

|Property | Value | Description | 
|---------|--------|--------|
| Continuous| 0| Continuous 
| Discrete| 1| Discrete 



### Enumeration: VoxelVariablePrecision
#### Voxel variable precision. The lower the precision the smaller the data size of the voxel layer. 

|Property | Value | Description | 
|---------|--------|--------|
| InputData| 0| Variable data is unchanged. 
| Low| 1| Low precision. 
| Medium| 2| Medium precision. 
| High| 3| High precision. 




## CIMVoxelVariableProfile
#### Represents a voxel layer variable profile. 


### CIMVoxelVariableProfile 

|Property | Type | Description | 
|---------|--------|--------|
| variable | string | The variable that the profile is associated with. 
| description | string | The variable description. 
| dataType | [enumeration VoxelVariableDataType](CIMServiceLayers.md#enumeration-voxelvariabledatatype) | The variable data type. 
| filters | [[CIMVoxelFilter]](Types.md#voxelfilter) | The filters. 
| renderer | [VoxelRenderer](Types.md#voxelrenderer) | The symbol renderer. 
| precision | [enumeration VoxelVariablePrecision](CIMServiceLayers.md#enumeration-voxelvariableprecision) | The variable precision. 
| statistics | [VoxelStatistics](Types.md#voxelstatistics) | The statistics for the variable. 
| signature | string | The signature for the variable. 
| signatureVersion | long | The signature version for the variable. 





### Enumeration: VoxelVisualization
#### Represents voxel visualization. 

|Property | Value | Description | 
|---------|--------|--------|
| Volume| 0| Voxel is visualized using volume mode. 
| Surface| 1| Voxel is visualized using surface mode. 




## CIMWCSServiceConnection
#### Represents a WCS service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 


### CIMWCSServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| coverageName | string | The coverage name. 
| version | string | The version. 
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase) | The server connection. 






## CIMWFSServiceConnection
#### Represents a WFS service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 


### CIMWFSServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| layerName | string | The layer name. 
| version | string | The version. 
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase) | The server connection. 
| capabilitiesParameters | {JSON_object}| Vendor specific parameters for all WFS requests. 






## CIMWMSServiceConnection
#### Represents a WMS service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 


### CIMWMSServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| layerName | string | The layer name. 
| version | string | The version. 
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase) | The server connection. 
| capabilitiesParameters | {JSON_object}| Vendor specific parameters for GetCapabilities, GetMap and GetFeatureInfo requests. 
| mapParameters | {JSON_object}| Vendor specific parameters for GetMap and GetFeatureInfo requests. 






## CIMWMSSubLayer
#### Represents a WMS service sublayer. 


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


### CIMWMSSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| styleName | string | The style name. 






## CIMWMTSServiceConnection
#### Represents a WMTS service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 


### CIMWMTSServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| layerName | string | The layer name. 
| version | string | The version. 
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase) | The server connection. 
| style | string | The style. 
| dimensions | {JSON_object}| The dimensions as a property set. 
| imageFormat | string | The image format. 
| tileMatrixSet | string | The tile matrix set. 
| capabilitiesParameters | {JSON_object}| The connection capabilities parameters as a property set. 
| mapParameters | {JSON_object}| The custom map parameters as a property set. 
| templateUrl | string | The template url that can be used for tile requests. 



