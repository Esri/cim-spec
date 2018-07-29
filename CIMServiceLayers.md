


## CIMAGSServiceConnection
Represents an ArcGIS Server service connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMServiceConnection

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.


### CIMAGSServiceConnection

|Property | Type | Description |
|---------|--------|--------|
| objectName | string|The object name.
| objectType | string|The object type.
| URL | string|The URL.
| capabilities | string|The capabilities.
| serverConnection | [ServerConnection](Types.md#serverconnection)|The server connection.
| gdbVersion | string|The name of the geodatabase version to use in service requests.





### Enumeration: ConnectionMode
Connection modes.

|Property | Value | Description |
|---------|--------|--------|
| Consumer| 0| User.
| Admin| 1| Administrator.
| Publisher| 2| Publisher.




## CIMDCOMServerConnection
Represents a DCOM server connection.


### CIMServerConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMDCOMServerConnection

|Property | Type | Description |
|---------|--------|--------|
| domain | string|The domain.
| hideUserProperty | boolean|A boolean value indicating whether of not to hide the user.
| machine | string|The machine.
| managerURL | string|The manager URL.
| password | string|The password.
| user | string|The user.






## CIMDynamicServiceCompositeSubLayer
Represents a dynamic service composite sublayer.


### CIMSubLayer

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| expanded | boolean|A boolean indicating whether this layer is expanded in the contents pane.
| maxScale | number //double|The maximum scale for layer draw (set as the denominator of the scale's representative fraction)
| minScale | number //double|The minimum scale for layer draw (set as the denominator of the scale's representative fraction)
| name | string|The name.
| showLegends | boolean|A boolean indicating whether or not to show legends.
| subLayerID | string|The sublayer ID.
| visibility | boolean|A boolean indicating whether or not this layer is visibile.
| serviceLayerID | number //int32|The identifier that will be used to identify the layer in server


### CIMDynamicServiceCompositeSubLayer

|Property | Type | Description |
|---------|--------|--------|
| definitionExpression | string|The definition expression. This property is used for composite layers that are backed by feature classes.


### CIMCompositeSubLayer

|Property | Type | Description |
|---------|--------|--------|
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) |The composite sublayers.






## CIMDynamicServiceLayer
Represents a dynamic service layer.


### CIMDefinition

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| URI | string|The URI of the definition. Typically set by the system and used as an identifier.
| sourceURI | string|The source URI of the item. Set if sourced from an external item such as an item on a portal.
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|The time the definition was last modfied.
| metadataURI | string|The metadata URI.
| useSourceMetadata | boolean|A boolean indicating if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project.


### CIMLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| attribution | string|The attribution text that appears on a map that draws this layer.
| description | string|The description.
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface)|The layer elevation.
| expanded | boolean|A boolean indicating whether this layer is expanded in the contents pane.
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties)|The 3D layer properties.
| layerMasks | [string,]|The layer masks.
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype)|The map layer type.
| maxScale | number //double|The maximum scale for layer draw (set as the denominator of the scale's representative fraction)
| minScale | number //double|The minimum scale for layer draw (set as the denominator of the scale's representative fraction)
| showLegends | boolean|A boolean indicating whether or not to show legends.
| transparency | number //double|The transparency of the layer.
| visibility | boolean|A boolean indicating whether or not this layer is visibile.
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype)|The display cache type.
| maxDisplayCacheAge | number //double|The max display cache age.
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate)|The layer template.
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo)|The popup info.
| showPopups | boolean|A boolean indicating whether or not to show popups.
| serviceLayerID | number //int32|The identifier that will be used to identify the layer in server
| charts | [CIMChart](CIMLayer.md#cimchart) |
| searchable | boolean|A boolean indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search.
| refreshRate | number //double|the amount of time to wait between refreshing the layer
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the layer


### CIMServiceLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection)|The service connection.
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) |The sublayers.
| transparentColor | [Color](Types.md#color)|The transparent color.
| backgroundColor | [Color](Types.md#color)|The background color.


### CIMDynamicServiceLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| imageFormat | [enumeration esriImageFormat](ExternalReferences.md#enumeration-esriimageformat)|The image format.
| useTime | boolean|A boolean indicating whether or not to use time.






## CIMDynamicServiceSubLayer
Represents a dynamic service sublayer.


### CIMSubLayer

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| expanded | boolean|A boolean indicating whether this layer is expanded in the contents pane.
| maxScale | number //double|The maximum scale for layer draw (set as the denominator of the scale's representative fraction)
| minScale | number //double|The minimum scale for layer draw (set as the denominator of the scale's representative fraction)
| name | string|The name.
| showLegends | boolean|A boolean indicating whether or not to show legends.
| subLayerID | string|The sublayer ID.
| visibility | boolean|A boolean indicating whether or not this layer is visibile.
| serviceLayerID | number //int32|The identifier that will be used to identify the layer in server


### CIMDynamicServiceSubLayer

|Property | Type | Description |
|---------|--------|--------|
| showLabels | boolean|A boolean indicating whether or not to show labels.
| scaleSymbols | boolean|A boolean indicating whether or not to scale symbols.
| definitionExpression | string|The definition expression.
| sourceID | string|The source ID.
| useTime | boolean|A boolean indicating whether or not to use time.
| drawTimeCumulative | boolean|A boolean indicating whether or not draw time cumulatively.
| timeOffset | number //double|The time offset.
| timeOffsetUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The time offset units.
| styleName | string|The style name.
| layerDefinition | string|The layer definition.
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo)|The popup info.
| showPopups | boolean|A boolean indicating whether or not to show popups.






## CIMGlobeServiceLayer
Represents a globe service layer.


### CIMDefinition

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| URI | string|The URI of the definition. Typically set by the system and used as an identifier.
| sourceURI | string|The source URI of the item. Set if sourced from an external item such as an item on a portal.
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|The time the definition was last modfied.
| metadataURI | string|The metadata URI.
| useSourceMetadata | boolean|A boolean indicating if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project.


### CIMLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| attribution | string|The attribution text that appears on a map that draws this layer.
| description | string|The description.
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface)|The layer elevation.
| expanded | boolean|A boolean indicating whether this layer is expanded in the contents pane.
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties)|The 3D layer properties.
| layerMasks | [string,]|The layer masks.
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype)|The map layer type.
| maxScale | number //double|The maximum scale for layer draw (set as the denominator of the scale's representative fraction)
| minScale | number //double|The minimum scale for layer draw (set as the denominator of the scale's representative fraction)
| showLegends | boolean|A boolean indicating whether or not to show legends.
| transparency | number //double|The transparency of the layer.
| visibility | boolean|A boolean indicating whether or not this layer is visibile.
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype)|The display cache type.
| maxDisplayCacheAge | number //double|The max display cache age.
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate)|The layer template.
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo)|The popup info.
| showPopups | boolean|A boolean indicating whether or not to show popups.
| serviceLayerID | number //int32|The identifier that will be used to identify the layer in server
| charts | [CIMChart](CIMLayer.md#cimchart) |
| searchable | boolean|A boolean indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search.
| refreshRate | number //double|the amount of time to wait between refreshing the layer
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the layer


### CIMServiceLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection)|The service connection.
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) |The sublayers.
| transparentColor | [Color](Types.md#color)|The transparent color.
| backgroundColor | [Color](Types.md#color)|The background color.


### CIMGlobeServiceLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| constantScreenSize | boolean|A boolean value indicating whether or not to use constant screen size. If this property is true, then the size specified in the vector features in the cache are treated as points. Otherwise it is assumed they are meters.
| snappable | boolean|A boolean value indicating whether or not geometries are snappable.






## CIMInternetServerConnection
Represents an internet server connection.


### CIMServerConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMInternetServerConnection

|Property | Type | Description |
|---------|--------|--------|
| anonymous | boolean|A boolean value indicating whether of no this is an anonymous connection.
| hideUserProperty | boolean|A boolean value indicating whether of not to hide the user.
| password | string|The password.
| URL | string|The URL.
| user | string|The user.






## CIMLANServerConnection
Represents a LAN service connection.


### CIMServerConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMLANServerConnection

|Property | Type | Description |
|---------|--------|--------|
| machine | string|The machine.






## CIMProjectServerConnection
Represents a project server connection.


### CIMServerConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMInternetServerConnection

|Property | Type | Description |
|---------|--------|--------|
| anonymous | boolean|A boolean value indicating whether of no this is an anonymous connection.
| hideUserProperty | boolean|A boolean value indicating whether of not to hide the user.
| password | string|The password.
| URL | string|The URL.
| user | string|The user.


### CIMProjectServerConnection

|Property | Type | Description |
|---------|--------|--------|
| connectionMode | [enumeration ConnectionMode](CIMServiceLayers.md#enumeration-connectionmode)|The connection mode.
| name | string|The name.
| serverType | [enumeration ServerType](CIMServiceLayers.md#enumeration-servertype)|The server type.
| stagingFolder | string|The staging folder.
| useDefaultStagingFolder | boolean|A boolean value indicating whether or not to use the default staging folder.






## CIMSceneServiceLayer
Represents a scene service layer.


### CIMDefinition

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| URI | string|The URI of the definition. Typically set by the system and used as an identifier.
| sourceURI | string|The source URI of the item. Set if sourced from an external item such as an item on a portal.
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|The time the definition was last modfied.
| metadataURI | string|The metadata URI.
| useSourceMetadata | boolean|A boolean indicating if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project.


### CIMLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| attribution | string|The attribution text that appears on a map that draws this layer.
| description | string|The description.
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface)|The layer elevation.
| expanded | boolean|A boolean indicating whether this layer is expanded in the contents pane.
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties)|The 3D layer properties.
| layerMasks | [string,]|The layer masks.
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype)|The map layer type.
| maxScale | number //double|The maximum scale for layer draw (set as the denominator of the scale's representative fraction)
| minScale | number //double|The minimum scale for layer draw (set as the denominator of the scale's representative fraction)
| showLegends | boolean|A boolean indicating whether or not to show legends.
| transparency | number //double|The transparency of the layer.
| visibility | boolean|A boolean indicating whether or not this layer is visibile.
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype)|The display cache type.
| maxDisplayCacheAge | number //double|The max display cache age.
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate)|The layer template.
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo)|The popup info.
| showPopups | boolean|A boolean indicating whether or not to show popups.
| serviceLayerID | number //int32|The identifier that will be used to identify the layer in server
| charts | [CIMChart](CIMLayer.md#cimchart) |
| searchable | boolean|A boolean indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search.
| refreshRate | number //double|the amount of time to wait between refreshing the layer
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the layer


### CIMSceneServiceLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| serviceConnection | [CIMAGSServiceConnection](CIMServiceLayers.md#cimagsserviceconnection)|The service connection.
| snappable | boolean|A boolean value indicating if the geometries are snappable.
| renderer | [Renderer](Types.md#renderer)|The primary symbol renderer.
| featureElevationExpression | string|The feature elevation expression.
| labelClasses | [CIMLabelClass](CIMLabelPlacement.md#cimlabelclass) |The collection of label class definitions.
| labelVisibility | boolean|A boolean option indicating whether to display labels for this layer's label classes.
| dataConnection | [CIMSceneDataConnection](CIMTerrainLayers.md#cimscenedataconnection)|The data connection. Currently used only when loading local spk's.
| useRealWorldSymbolSizes | boolean|A boolean option indicating whether to use real world symbols sizes (meters) vs. points.
| exclusionSet | [number], //[int64],|The set of excluded features.
| definitionExpression | string|The definition expression that can subset the features.





### Enumeration: ServerType
Server types.

|Property | Value | Description |
|---------|--------|--------|
| AGS| 0| ArcGIS Server.
| WMS| 1| WMS.
| WCS| 2| WCS.
| WMTS| 3| WMTS.
| WFS| 4| WFS.




## CIMStandardServiceConnection
Represents a standard service connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMServiceConnection

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.


### CIMStandardServiceConnection

|Property | Type | Description |
|---------|--------|--------|
| serviceProvider | string|The service provider.
| serviceType | string|The service type.
| URL | string|The service URL.
| culture | string|The service culture.






## CIMTiledServiceLayer
Represents a tiled service layer.


### CIMDefinition

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| URI | string|The URI of the definition. Typically set by the system and used as an identifier.
| sourceURI | string|The source URI of the item. Set if sourced from an external item such as an item on a portal.
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|The time the definition was last modfied.
| metadataURI | string|The metadata URI.
| useSourceMetadata | boolean|A boolean indicating if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project.


### CIMLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| attribution | string|The attribution text that appears on a map that draws this layer.
| description | string|The description.
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface)|The layer elevation.
| expanded | boolean|A boolean indicating whether this layer is expanded in the contents pane.
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties)|The 3D layer properties.
| layerMasks | [string,]|The layer masks.
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype)|The map layer type.
| maxScale | number //double|The maximum scale for layer draw (set as the denominator of the scale's representative fraction)
| minScale | number //double|The minimum scale for layer draw (set as the denominator of the scale's representative fraction)
| showLegends | boolean|A boolean indicating whether or not to show legends.
| transparency | number //double|The transparency of the layer.
| visibility | boolean|A boolean indicating whether or not this layer is visibile.
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype)|The display cache type.
| maxDisplayCacheAge | number //double|The max display cache age.
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate)|The layer template.
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo)|The popup info.
| showPopups | boolean|A boolean indicating whether or not to show popups.
| serviceLayerID | number //int32|The identifier that will be used to identify the layer in server
| charts | [CIMChart](CIMLayer.md#cimchart) |
| searchable | boolean|A boolean indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search.
| refreshRate | number //double|the amount of time to wait between refreshing the layer
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the layer


### CIMServiceLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection)|The service connection.
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) |The sublayers.
| transparentColor | [Color](Types.md#color)|The transparent color.
| backgroundColor | [Color](Types.md#color)|The background color.


### CIMTiledServiceLayerDefinition

|Property | Type | Description |
|---------|--------|--------|






## CIMWCSServiceConnection
Represents a WCS service connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMServiceConnection

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.


### CIMWCSServiceConnection

|Property | Type | Description |
|---------|--------|--------|
| coverageName | string|The coverage name.
| version | string|The version.
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase)|The server connection.






## CIMWFSServiceConnection
Represents a WFS service connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMServiceConnection

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.


### CIMWFSServiceConnection

|Property | Type | Description |
|---------|--------|--------|
| layerName | string|The layer name.
| version | string|The version.
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase)|The server connection.
| capabilitiesParameters | Object|The vendor specific parameters for all WFS requests






## CIMWMSServiceConnection
Represents a WMS service connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMServiceConnection

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.


### CIMWMSServiceConnection

|Property | Type | Description |
|---------|--------|--------|
| layerName | string|The layer name.
| version | string|The version.
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase)|The server connection.
| capabilitiesParameters | Object|The vendor specific parameters for GetCapabilities, GetMap and GetFeatureInfo requests
| mapParameters | Object|The vendor specific parameters for GetMap and GetFeatureInfo requests






## CIMWMSSubLayer
Represents a WMS service sublayer.


### CIMSubLayer

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| expanded | boolean|A boolean indicating whether this layer is expanded in the contents pane.
| maxScale | number //double|The maximum scale for layer draw (set as the denominator of the scale's representative fraction)
| minScale | number //double|The minimum scale for layer draw (set as the denominator of the scale's representative fraction)
| name | string|The name.
| showLegends | boolean|A boolean indicating whether or not to show legends.
| subLayerID | string|The sublayer ID.
| visibility | boolean|A boolean indicating whether or not this layer is visibile.
| serviceLayerID | number //int32|The identifier that will be used to identify the layer in server


### CIMWMSSubLayer

|Property | Type | Description |
|---------|--------|--------|
| styleName | string|The style name.






## CIMWMTSServiceConnection
Represents a WMTS service connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMServiceConnection

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.


### CIMWMTSServiceConnection

|Property | Type | Description |
|---------|--------|--------|
| layerName | string|The layer name.
| version | string|The version.
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase)|The server connection.
| style | string|The style.
| dimensions | Object|The dimensions as a property set.
| imageFormat | string|The image format.
| tileMatrixSet | string|The tile matrix set.
| capabilitiesParameters | Object|The connection capabilities parameters as a property set.
| mapParameters | Object|The custom map parameters as a property set.
| templateUrl | string|The template url that can be used for tile requests.
