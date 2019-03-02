


## CIMAGSServiceConnection
#### Represents an ArcGIS Server service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 


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
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the definition was last modified. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


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
| charts | [CIMChart](CIMLayer.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [CIMStringMap](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 


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
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the definition was last modified. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


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
| charts | [CIMChart](CIMLayer.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [CIMStringMap](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 


### CIMBuildingSceneLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| subLayers | [string] | The sublayers. 
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection to the workspace. 


### CIMObject3DRenderingFilters 

|Property | Type | Description | 
|---------|--------|--------|
| filters | [CIMObject3DRenderingFilter](CIMServiceLayers.md#cimobject3drenderingfilter) | The filters. 
| activeFilterID | string | The active filter id. 





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
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) | The composite sublayers. 


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
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the definition was last modified. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


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
| charts | [CIMChart](CIMLayer.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [CIMStringMap](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 


### CIMServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection) | The service connection. 
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) | The sublayers. 
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
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the definition was last modified. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


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
| charts | [CIMChart](CIMLayer.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [CIMStringMap](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 


### CIMServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection) | The service connection. 
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) | The sublayers. 
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






## CIMObject3DRenderingFilter
#### Represents a 3D object rendering filter. 


### CIMObject3DRenderingFilter 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The ID. 
| name | string | The name. 
| description | string | The description. 
| filterBlocks | [CIMObject3DRenderingFilterBlock](CIMServiceLayers.md#cimobject3drenderingfilterblock) | The filter blocks. 
| authoringInfo | [CIMObject3DRenderingFilterAuthoringInfo](CIMServiceLayers.md#cimobject3drenderingfilterauthoringinfo) | The authoring info. 






## CIMObject3DRenderingFilterAuthoringInfo
#### Represents a filter authoring info. 


### CIMObject3DRenderingFilterAuthoringInfo 

|Property | Type | Description | 
|---------|--------|--------|
| isVisible | boolean | A value indicating whether the filter is displayed in the UI or not. 
| filterBlocks | [CIMObject3DRenderingFilterBlockAuthoringInfo](CIMServiceLayers.md#cimobject3drenderingfilterblockauthoringinfo) | The filter blocks. 






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
| filterStates | [CIMObject3DRenderingFilterState](CIMServiceLayers.md#cimobject3drenderingfilterstate) | The filter state. 






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
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the definition was last modified. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


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
| charts | [CIMChart](CIMLayer.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [CIMStringMap](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 


### CIMSceneServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMAGSServiceConnection](CIMServiceLayers.md#cimagsserviceconnection) | The service connection. 
| snappable | boolean | A value indicating whether the geometries are snappable. 
| renderer | [Renderer](Types.md#renderer) | The primary symbol renderer. 
| featureElevationExpression | string | The feature elevation expression. 
| labelClasses | [CIMLabelClass](CIMLabelPlacement.md#cimlabelclass) | The collection of label class definitions. 
| labelVisibility | boolean | A value indicating whether to display labels for this layer's label classes. 
| dataConnection | [CIMSceneDataConnection](CIMTerrainLayers.md#cimscenedataconnection) | The data connection. Currently used only when loading local scene layer packages. 
| useRealWorldSymbolSizes | boolean | A value indicating whether to use real world symbols sizes (meters) vs. points. 
| exclusionSet | [long64] | The set of excluded features. 
| definitionExpression | string | The definition expression that can subset the features. 
| definitionExpressionName | string | The Name of definition expression. 
| definitionFilterChoices | [CIMDefinitionFilter](CIMLayer.md#cimdefinitionfilter) | The definition filter choices. 
| associatedFeatureLayerURI | string | The URI to the associated feature layer. 
| sceneServiceLayerType | [enumeration SceneServiceLayerType](CIMServiceLayers.md#enumeration-sceneservicelayertype) | The scene service layer type. Typically set by the system and should not be modified. 
| selectable | boolean | A value indicating whether the layer is selectable. 
| selectionSetURI | string | The URI of the selection set for the layer. 





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
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the definition was last modified. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


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
| charts | [CIMChart](CIMLayer.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [CIMStringMap](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 


### CIMServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection) | The service connection. 
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) | The sublayers. 
| transparentColor | [Color](Types.md#color) | The transparent color. 
| backgroundColor | [Color](Types.md#color) | The background color. 


### CIMTiledServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| associatedFeatureLayerURI | string | The URI for a feature service or portal item that provides pop-up support for the layer. 






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



