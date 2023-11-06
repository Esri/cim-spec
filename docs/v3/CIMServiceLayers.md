


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




## CIMIndexedSceneLayer
#### Represents a indexed scene layer. 


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


### CIMIndexedSceneLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| snappable | boolean | A value indicating whether the geometries are snappable. 
| renderer | [Renderer](Types.md#renderer) | The primary symbol renderer. 
| featureElevationExpression | string | The feature elevation expression. 
| labelClasses | [[CIMLabelClass]](CIMLabelPlacement.md#cimlabelclass) | The collection of label class definitions. 
| labelVisibility | boolean | A value indicating whether to display labels for this layer's label classes. 
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| useRealWorldSymbolSizes | boolean | A value indicating whether to use real world symbols sizes (meters) vs. points. This value should always be in sync with the UseRealWorldSymbolSizes property at the symbol level. 
| exclusionSet | [long long] | The set of excluded features. 
| definitionExpression | string | The definition expression that can subset the features. 
| definitionExpressionName | string | The Name of definition expression. 
| definitionFilterChoices | [[CIMDefinitionFilter]](CIMLayer.md#cimdefinitionfilter) | The definition filter choices. 
| associatedFeatureLayerURI | string | The URI to the associated feature layer. 
| indexedSceneLayerType | [enumeration IndexedSceneLayerType](CIMServiceLayers.md#enumeration-indexedscenelayertype) | The indexed scene layer type. Typically set by the system and should not be modified. 
| selectable | boolean | A value indicating whether the layer is selectable. 
| selectionSetURI | string | The URI of the selection set for the layer. 
| modificationLayerURI | string | The URI of the modification layer. 
| modificationLayerEnabled | boolean | A value indicating whether the integrated mesh modification is enabled. 
| usePredefinedMaxScreenThreshold | boolean | A value indicating whether to use predefined max screen threshold as defined in the integrated mesh layer. 
| floorAwareTableProperties | [CIMFloorAwareTableProperties](CIMVectorLayers.md#cimfloorawaretableproperties) | Floor-aware properties if the scene layer is used in floor filtering. 
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition) | The time fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition) | The time definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition) | The time display definition. 





### Enumeration: IndexedSceneLayerType
#### Indexed scene layer types. 

|Property | Value | Description | 
|---------|--------|--------|
| IntegratedMesh| 0| Represents integrated mesh indexed scene layer type. 
| Point| 1| Represents point indexed scene layer type. 
| Object3D| 2| Represents 3D object indexed scene layer type. 




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
| name | string | The isosurface name. 
| visible | boolean | A value indicating whether the isosurface is visible. 






## CIMMapImageLayer
#### Represents an ArcGIS Map Service layer. 


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


### CIMServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection) | The service connection. 
| subLayers | [[CIMSubLayerBase]](CIMLayer.md#cimsublayerbase) | The sublayers. 
| transparentColor | [Color](Types.md#color) | The transparent color. 
| backgroundColor | [Color](Types.md#color) | The background color. 
| subTables | [[CIMServiceSubTable]](CIMServiceLayers.md#cimservicesubtable) | The subtables. 


### CIMDynamicServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| imageFormat | [enumeration esriImageFormat](ExternalReferences.md#enumeration-esriimageformat) | The image format. 
| useTime | boolean | A value indicating whether or not to use time. 


### CIMMapImageLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|






## CIMOGCAPIMapTilesServiceConnection
#### Represents a OGC API Map Tiles service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 


### CIMOGCAPIMapTilesServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| layerName | string | The layer name. 
| version | string | The version. 
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase) | The server connection. 
| style | string | The style. 
| imageFormat | string | The image format. 
| tileMatrixSet | string | The tile matrix set. 
| capabilitiesParameters | {JSON_object}| The connection capabilities parameters as a property set. 
| templateUrl | string | The template url that can be used for tile requests. 






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




## CIMServiceCompositeSubLayer
#### Represents a service composite sublayer. 


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


### CIMServiceCompositeSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| definitionExpression | string | The definition expression. This property is used for composite layers that are backed by feature classes. 
| URI | string | The URI of the backing layer. Used when feature layer capabilities are enabled. 






## CIMServiceSubLayer
#### Represents a service sublayer. 


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


### CIMServiceSubLayer 

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
| layerDefinition | string | The layer definition for dynamic service layer. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| floorAwareTableProperties | [CIMFloorAwareTableProperties](CIMVectorLayers.md#cimfloorawaretableproperties) | Floor-aware properties if the sublayer is used in floor filtering. 
| URI | string | The URI of the backing layer. Used when feature layer capabilities are enabled. 






## CIMServiceSubTable
#### Represents a service subtable. 


### CIMServiceSubTable 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| subTableID | string | The sub table ID. 






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


### CIMServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection) | The service connection. 
| subLayers | [[CIMSubLayerBase]](CIMLayer.md#cimsublayerbase) | The sublayers. 
| transparentColor | [Color](Types.md#color) | The transparent color. 
| backgroundColor | [Color](Types.md#color) | The background color. 
| subTables | [[CIMServiceSubTable]](CIMServiceLayers.md#cimservicesubtable) | The subtables. 


### CIMTiledServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| associatedFeatureLayerURI | string | The URI for a feature layer (feature service-based or portal item-based) that provides pop-up support for the tiled service layer. 






## CIMTiles3DDataConnection
#### Represents a 3D Tiles data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceDataConnectionProperties 

|Property | Type | Description | 
|---------|--------|--------|
| customParameters | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | Vendor specific parameters. 


### CIMTiles3DDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string | The URI. 






## CIMTiles3DLayer
#### Represents a 3D Tiles layer. 


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


### CIMTiles3DLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| snappable | boolean | A value indicating whether the geometries are snappable. 
| tiles3DLayerType | [enumeration Tiles3DLayerType](CIMServiceLayers.md#enumeration-tiles3dlayertype) | The 3D Tiles layer type. Typically set by the system and should not be modified. 





### Enumeration: Tiles3DLayerType
#### 3D Tiles layer types. 

|Property | Value | Description | 
|---------|--------|--------|
| IntegratedMesh| 0| Represents integrated mesh 3D Tiles layer type. 
| Object3D| 1| Represents 3D object 3D Tiles layer type. 



### Enumeration: VoxelAlignment
#### Represents voxel alignment. 

|Property | Value | Description | 
|---------|--------|--------|
| Origin| 0| Values are at voxel origin. 
| Center| 1| Values are at voxel center. 




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






## CIMVoxelDataConnection
#### Represents a voxel data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMVoxelDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string | The URI. 






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


### CIMVoxelLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| lighting | [CIMVoxelLighting](CIMServiceLayers.md#cimvoxellighting) | The lighting. 
| isosurfaceContainerExpanded | boolean | A value indicating whether the isosurface container is expanded in the contents pane. 
| isosurfaceContainerVisible | boolean | A value indicating whether the isosurface container is visible. 
| optimization | [enumeration VoxelLayerOptimization](CIMServiceLayers.md#enumeration-voxellayeroptimization) | The voxel layer optimization. 
| sectionContainerExpanded | boolean | A value indicating whether this voxel section container is expanded in the contents pane. 
| sectionContainerVisible | boolean | A value indicating whether the voxel section container is visible. 
| selectedVariable | string | The selected variable. 
| sliceContainerExpanded | boolean | A value indicating whether this voxel slice container is expanded in the contents pane. 
| sliceContainerVisible | boolean | A value indicating whether the voxel slice container is visible. 
| snappable | boolean | A value indicating whether this layer participates in snapping in the editor. 
| staticSections | [[CIMVoxelStaticSection]](CIMServiceLayers.md#cimvoxelstaticsection) | A collection of static sections. 
| staticSectionContainerExpanded | boolean | A value indicating whether this voxel static section container is expanded in the contents pane. 
| staticSectionContainerVisible | boolean | A value indicating whether the voxel static section container is visible. 
| surfaceContainerExpanded | boolean | A value indicating whether the surface container is expanded in the contents pane. 
| visualization | [enumeration VoxelVisualization](CIMServiceLayers.md#enumeration-voxelvisualization) | The voxel visualization. 
| alignment | [enumeration VoxelAlignment](CIMServiceLayers.md#enumeration-voxelalignment) | The voxel alignment. 
| volumes | [[CIMVoxelVolume]](CIMServiceLayers.md#cimvoxelvolume) | The volumes. 





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
| unlistedValues | [long] | The unlisted values. 






## CIMVoxelValueFilter
#### Represents a voxel value filter. Filter based on the value of an specified variable. 


### CIMVoxelFilter 

|Property | Type | Description | 
|---------|--------|--------|


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
| signature | string | The signature for the variable. 
| signatureVersion | long | The signature version for the variable. 
| isosurfaces | [[CIMIsosurface]](CIMServiceLayers.md#cimisosurface) | A collection of isosurfaces. 





### Enumeration: VoxelVisualization
#### Represents voxel visualization. 

|Property | Value | Description | 
|---------|--------|--------|
| Volume| 0| Voxel is visualized using volume mode. 
| Surface| 1| Voxel is visualized using surface mode. 




## CIMVoxelVolume
#### Represents a voxel layer volume. 


### CIMVoxelVolume 

|Property | Type | Description | 
|---------|--------|--------|
| ID | long | The volume ID, which must be unique among all volumes in the layer. 
| sections | [[CIMVoxelPlane]](CIMServiceLayers.md#cimvoxelplane) | A collection of sections. 
| slices | [[CIMVoxelPlane]](CIMServiceLayers.md#cimvoxelplane) | A collection of slices. 
| variableProfiles | [[CIMVoxelVariableProfile]](CIMServiceLayers.md#cimvoxelvariableprofile) | The variable profiles. 






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
| capabilitiesParameters | {JSON_object}| Vendor specific parameters for all WCS requests. 






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






## CIMWMSLayer
#### Represents an OGC WMS layer. 


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


### CIMServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection) | The service connection. 
| subLayers | [[CIMSubLayerBase]](CIMLayer.md#cimsublayerbase) | The sublayers. 
| transparentColor | [Color](Types.md#color) | The transparent color. 
| backgroundColor | [Color](Types.md#color) | The background color. 
| subTables | [[CIMServiceSubTable]](CIMServiceLayers.md#cimservicesubtable) | The subtables. 


### CIMDynamicServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| imageFormat | [enumeration esriImageFormat](ExternalReferences.md#enumeration-esriimageformat) | The image format. 
| useTime | boolean | A value indicating whether or not to use time. 


### CIMWMSLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|






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



