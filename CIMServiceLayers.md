


## CIMAGSServiceConnection
#### Represents an ArcGIS Server service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 


### CIMAGSServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| objectName | string|Gets and sets the object name. 
| objectType | string|Gets and sets the object type. 
| URL | string|Gets and sets the URL. 
| capabilities | string|Gets and sets the capabilities. 
| serverConnection | [ServerConnection](Types.md#serverconnection)|Gets and sets the server connection. 
| gdbVersion | string|Gets and sets the name of the geodatabase version to use in service requests. 





### Enumeration: ConnectionMode
#### Connection modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Consumer| 0| User. 
| Admin| 1| Administrator. 
| Publisher| 2| Publisher. 




## CIMDCOMServerConnection
#### Represents a DCOM server connection. 


### CIMServerConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDCOMServerConnection 

|Property | Type | Description | 
|---------|--------|--------|
| domain | string|Gets and sets the domain. 
| hideUserProperty | boolean|Gets and sets a boolean value indicating whether of not to hide the user. 
| machine | string|Gets and sets the machine. 
| managerURL | string|Gets and sets the manager URL. 
| password | string|Gets and sets the password. 
| user | string|Gets and sets the user. 






## CIMDynamicServiceCompositeSubLayer
#### Represents a dynamic service composite sublayer. 


### CIMSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| expanded | boolean|Gets and sets whether this layer is expanded in the contents pane. 
| maxScale | double|Gets and sets the maximum scale for layer draw (set as the denominator of the scale's representative fraction) 
| minScale | double|Gets and sets the minimum scale for layer draw (set as the denominator of the scale's representative fraction) 
| name | string|Gets and sets the name. 
| showLegends | boolean|Gets and sets a boolean indicating whether or not to show legends. 
| subLayerID | string|Gets and sets the sublayer ID. 
| visibility | boolean|Gets and sets a boolean indicating whether or not this layer is visibile. 
| serviceLayerID | long|Gets and sets identifier that will be used to identify the layer in server 


### CIMDynamicServiceCompositeSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| definitionExpression | string|Gets and sets the definition expression. This property is used for composite layers that are backed by feature classes. 


### CIMCompositeSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) |Gets and sets the composite sublayers. 






## CIMDynamicServiceLayer
#### Represents a dynamic service layer. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| URI | string|Gets and sets the URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string|Gets and sets the source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|Gets and sets the time the definition was last modfied. 
| metadataURI | string|Gets and sets the metadata URI. 
| useSourceMetadata | bool|Gets and sets if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string|Gets and sets the attribution text that appears on a map that draws this layer. 
| description | string|Gets and sets the description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface)|Gets and sets the layer elevation. 
| expanded | boolean|Gets and sets whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties)|Gets and sets the 3D layer properties. 
| layerMasks | IStringArray|Gets and sets the layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype)|Gets and sets the map layer type. 
| maxScale | double|Gets and sets the maximum scale for layer draw (set as the denominator of the scale's representative fraction) 
| minScale | double|Gets and sets the minimum scale for layer draw (set as the denominator of the scale's representative fraction) 
| showLegends | boolean|Gets and sets a boolean indicating whether or not to show legends. 
| transparency | double|Gets and sets the transparency of the layer. 
| visibility | boolean|Gets and sets a boolean indicating whether or not this layer is visibile. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype)|Gets and sets the display cache type. 
| maxDisplayCacheAge | double|Gets and sets the max display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate)|Gets and sets the layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo)|Gets and sets the popup info. 
| showPopups | boolean|Gets and sets a boolean indicating whether or not to show popups. 
| serviceLayerID | long|Gets and sets identifier that will be used to identify the layer in server 
| charts | [CIMChart](CIMLayer.md#cimchart) | 
| searchable | boolean|Gets and sets a boolean indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double|the amount of time to wait between refreshing the layer 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the layer 


### CIMServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection)|Gets and sets the service connection. 
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) |Gets and sets the sublayers. 
| transparentColor | [Color](Types.md#color)|Gets and sets the transparent color. 
| backgroundColor | [Color](Types.md#color)|Gets and sets the background color. 


### CIMDynamicServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| imageFormat | [enumeration esriImageFormat](ExternalReferences.md#enumeration-esriimageformat)|Gets and sets the image format. 
| useTime | boolean|Gets and sets a boolean indicating whether or not to use time. 






## CIMDynamicServiceSubLayer
#### Represents a dynamic service sublayer. 


### CIMSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| expanded | boolean|Gets and sets whether this layer is expanded in the contents pane. 
| maxScale | double|Gets and sets the maximum scale for layer draw (set as the denominator of the scale's representative fraction) 
| minScale | double|Gets and sets the minimum scale for layer draw (set as the denominator of the scale's representative fraction) 
| name | string|Gets and sets the name. 
| showLegends | boolean|Gets and sets a boolean indicating whether or not to show legends. 
| subLayerID | string|Gets and sets the sublayer ID. 
| visibility | boolean|Gets and sets a boolean indicating whether or not this layer is visibile. 
| serviceLayerID | long|Gets and sets identifier that will be used to identify the layer in server 


### CIMDynamicServiceSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| showLabels | boolean|Gets and sets a boolean indicating whether or not to show labels. 
| scaleSymbols | boolean|Gets and sets a boolean indicating whether or not to scale symbols. 
| definitionExpression | string|Gets and sets the definition expression. 
| sourceID | string|Gets and sets the source ID. 
| useTime | boolean|Gets and sets a boolean indicating whether or not to use time. 
| drawTimeCumulative | boolean|Gets and sets a boolean indicating whether or not draw time cumulatively. 
| timeOffset | double|Gets and sets the time offset. 
| timeOffsetUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|Gets and sets the time offset units. 
| styleName | string|Gets and sets the style name. 
| layerDefinition | string|Gets and sets the layer definition. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo)|Gets and sets the popup info. 
| showPopups | boolean|Gets and sets a boolean indicating whether or not to show popups. 






## CIMGlobeServiceLayer
#### Represents a globe service layer. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| URI | string|Gets and sets the URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string|Gets and sets the source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|Gets and sets the time the definition was last modfied. 
| metadataURI | string|Gets and sets the metadata URI. 
| useSourceMetadata | bool|Gets and sets if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string|Gets and sets the attribution text that appears on a map that draws this layer. 
| description | string|Gets and sets the description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface)|Gets and sets the layer elevation. 
| expanded | boolean|Gets and sets whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties)|Gets and sets the 3D layer properties. 
| layerMasks | IStringArray|Gets and sets the layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype)|Gets and sets the map layer type. 
| maxScale | double|Gets and sets the maximum scale for layer draw (set as the denominator of the scale's representative fraction) 
| minScale | double|Gets and sets the minimum scale for layer draw (set as the denominator of the scale's representative fraction) 
| showLegends | boolean|Gets and sets a boolean indicating whether or not to show legends. 
| transparency | double|Gets and sets the transparency of the layer. 
| visibility | boolean|Gets and sets a boolean indicating whether or not this layer is visibile. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype)|Gets and sets the display cache type. 
| maxDisplayCacheAge | double|Gets and sets the max display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate)|Gets and sets the layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo)|Gets and sets the popup info. 
| showPopups | boolean|Gets and sets a boolean indicating whether or not to show popups. 
| serviceLayerID | long|Gets and sets identifier that will be used to identify the layer in server 
| charts | [CIMChart](CIMLayer.md#cimchart) | 
| searchable | boolean|Gets and sets a boolean indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double|the amount of time to wait between refreshing the layer 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the layer 


### CIMServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection)|Gets and sets the service connection. 
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) |Gets and sets the sublayers. 
| transparentColor | [Color](Types.md#color)|Gets and sets the transparent color. 
| backgroundColor | [Color](Types.md#color)|Gets and sets the background color. 


### CIMGlobeServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| constantScreenSize | boolean|Gets and sets a boolean value indicating whether or not to use constant screen size. If this property is true, then the size specified in the vector features in the cache are treated as points. Otherwise it is assumed they are meters. 
| snappable | boolean|Gets and sets a boolean value indicating whether or not geometries are snappable. 






## CIMInternetServerConnection
#### Represents an internet server connection. 


### CIMServerConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMInternetServerConnection 

|Property | Type | Description | 
|---------|--------|--------|
| anonymous | boolean|Gets and sets a boolean value indicating whether of no this is an anonymous connection. 
| hideUserProperty | boolean|Gets and sets a boolean value indicating whether of not to hide the user. 
| password | string|Gets and sets the password. 
| URL | string|Gets and sets the URL. 
| user | string|Gets and sets the user. 






## CIMLANServerConnection
#### Represents a LAN service connection. 


### CIMServerConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMLANServerConnection 

|Property | Type | Description | 
|---------|--------|--------|
| machine | string|Gets and sets the machine. 






## CIMProjectServerConnection
#### Represents a project server connection. 


### CIMServerConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMInternetServerConnection 

|Property | Type | Description | 
|---------|--------|--------|
| anonymous | boolean|Gets and sets a boolean value indicating whether of no this is an anonymous connection. 
| hideUserProperty | boolean|Gets and sets a boolean value indicating whether of not to hide the user. 
| password | string|Gets and sets the password. 
| URL | string|Gets and sets the URL. 
| user | string|Gets and sets the user. 


### CIMProjectServerConnection 

|Property | Type | Description | 
|---------|--------|--------|
| connectionMode | [enumeration ConnectionMode](CIMServiceLayers.md#enumeration-connectionmode)|Gets and sets the connection mode. 
| name | string|Gets and sets the name. 
| serverType | [enumeration ServerType](CIMServiceLayers.md#enumeration-servertype)|Gets and sets the server type. 
| stagingFolder | string|Gets and sets the staging folder. 
| useDefaultStagingFolder | boolean|Gets and sets a boolean value indicating whether or not to use the default staging folder. 






## CIMSceneServiceLayer
#### Represents a scene service layer. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| URI | string|Gets and sets the URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string|Gets and sets the source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|Gets and sets the time the definition was last modfied. 
| metadataURI | string|Gets and sets the metadata URI. 
| useSourceMetadata | bool|Gets and sets if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string|Gets and sets the attribution text that appears on a map that draws this layer. 
| description | string|Gets and sets the description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface)|Gets and sets the layer elevation. 
| expanded | boolean|Gets and sets whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties)|Gets and sets the 3D layer properties. 
| layerMasks | IStringArray|Gets and sets the layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype)|Gets and sets the map layer type. 
| maxScale | double|Gets and sets the maximum scale for layer draw (set as the denominator of the scale's representative fraction) 
| minScale | double|Gets and sets the minimum scale for layer draw (set as the denominator of the scale's representative fraction) 
| showLegends | boolean|Gets and sets a boolean indicating whether or not to show legends. 
| transparency | double|Gets and sets the transparency of the layer. 
| visibility | boolean|Gets and sets a boolean indicating whether or not this layer is visibile. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype)|Gets and sets the display cache type. 
| maxDisplayCacheAge | double|Gets and sets the max display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate)|Gets and sets the layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo)|Gets and sets the popup info. 
| showPopups | boolean|Gets and sets a boolean indicating whether or not to show popups. 
| serviceLayerID | long|Gets and sets identifier that will be used to identify the layer in server 
| charts | [CIMChart](CIMLayer.md#cimchart) | 
| searchable | boolean|Gets and sets a boolean indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double|the amount of time to wait between refreshing the layer 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the layer 


### CIMSceneServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMAGSServiceConnection](CIMServiceLayers.md#cimagsserviceconnection)|Gets and sets the service connection. 
| snappable | boolean|Gets and sets a boolean value indicating if the geometries are snappable. 
| renderer | [Renderer](Types.md#renderer)|Gets and sets the primary symbol renderer. 
| featureElevationExpression | string|Gets and sets the feature elevation expression. 
| labelClasses | [CIMLabelClass](CIMLabelPlacement.md#cimlabelclass) |Gets and sets the collection of label class definitions. 
| labelVisibility | boolean|Gets and sets a boolean option indicating whether to display labels for this layer's label classes. 
| dataConnection | [CIMSceneDataConnection](CIMTerrainLayers.md#cimscenedataconnection)|Gets and sets the data connection. Currently used only when loading local spk's. 
| useRealWorldSymbolSizes | boolean|Gets and sets a boolean option indicating whether to use real world symbols sizes (meters) vs. points. 
| exclusionSet | [LongLongArray](ExternalReferences.md#longlongarray)|Gets and sets the set of excluded features. 
| definitionExpression | string|Gets and sets the definition expression that can subset the features. 





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
| description | string|Gets and sets the description. 


### CIMStandardServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| serviceProvider | string|Gets and sets the service provider. 
| serviceType | string|Gets and sets the service type. 
| URL | string|Gets and sets the service URL. 
| culture | string|Gets and sets the service culture. 






## CIMTiledServiceLayer
#### Represents a tiled service layer. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| URI | string|Gets and sets the URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string|Gets and sets the source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|Gets and sets the time the definition was last modfied. 
| metadataURI | string|Gets and sets the metadata URI. 
| useSourceMetadata | bool|Gets and sets if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string|Gets and sets the attribution text that appears on a map that draws this layer. 
| description | string|Gets and sets the description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface)|Gets and sets the layer elevation. 
| expanded | boolean|Gets and sets whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties)|Gets and sets the 3D layer properties. 
| layerMasks | IStringArray|Gets and sets the layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype)|Gets and sets the map layer type. 
| maxScale | double|Gets and sets the maximum scale for layer draw (set as the denominator of the scale's representative fraction) 
| minScale | double|Gets and sets the minimum scale for layer draw (set as the denominator of the scale's representative fraction) 
| showLegends | boolean|Gets and sets a boolean indicating whether or not to show legends. 
| transparency | double|Gets and sets the transparency of the layer. 
| visibility | boolean|Gets and sets a boolean indicating whether or not this layer is visibile. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype)|Gets and sets the display cache type. 
| maxDisplayCacheAge | double|Gets and sets the max display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate)|Gets and sets the layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo)|Gets and sets the popup info. 
| showPopups | boolean|Gets and sets a boolean indicating whether or not to show popups. 
| serviceLayerID | long|Gets and sets identifier that will be used to identify the layer in server 
| charts | [CIMChart](CIMLayer.md#cimchart) | 
| searchable | boolean|Gets and sets a boolean indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double|the amount of time to wait between refreshing the layer 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the layer 


### CIMServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| serviceConnection | [CIMServiceConnection](CIMServiceLayers.md#cimserviceconnection)|Gets and sets the service connection. 
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) |Gets and sets the sublayers. 
| transparentColor | [Color](Types.md#color)|Gets and sets the transparent color. 
| backgroundColor | [Color](Types.md#color)|Gets and sets the background color. 


### CIMTiledServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|






## CIMWCSServiceConnection
#### Represents a WCS service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 


### CIMWCSServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| coverageName | string|Gets and sets the coverage name. 
| version | string|Gets and sets the version. 
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase)|Gets and sets the server connection. 






## CIMWFSServiceConnection
#### Represents a WFS service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 


### CIMWFSServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| layerName | string|Gets and sets the layer name. 
| version | string|Gets and sets the version. 
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase)|Gets and sets the server connection. 
| capabilitiesParameters | {JSON_object}|Gets and sets vendor specific parameters for all WFS requests 






## CIMWMSServiceConnection
#### Represents a WMS service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 


### CIMWMSServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| layerName | string|Gets and sets the layer name. 
| version | string|Gets and sets the version. 
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase)|Gets and sets the server connection. 
| capabilitiesParameters | {JSON_object}|Gets and sets vendor specific parameters for GetCapabilities, GetMap and GetFeatureInfo requests 
| mapParameters | {JSON_object}|Gets and sets vendor specific parameters for GetMap and GetFeatureInfo requests 






## CIMWMSSubLayer
#### Represents a WMS service sublayer. 


### CIMSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| expanded | boolean|Gets and sets whether this layer is expanded in the contents pane. 
| maxScale | double|Gets and sets the maximum scale for layer draw (set as the denominator of the scale's representative fraction) 
| minScale | double|Gets and sets the minimum scale for layer draw (set as the denominator of the scale's representative fraction) 
| name | string|Gets and sets the name. 
| showLegends | boolean|Gets and sets a boolean indicating whether or not to show legends. 
| subLayerID | string|Gets and sets the sublayer ID. 
| visibility | boolean|Gets and sets a boolean indicating whether or not this layer is visibile. 
| serviceLayerID | long|Gets and sets identifier that will be used to identify the layer in server 


### CIMWMSSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| styleName | string|Gets and sets the style name. 






## CIMWMTSServiceConnection
#### Represents a WMTS service connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 


### CIMWMTSServiceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| layerName | string|Gets and sets the layer name. 
| version | string|Gets and sets the version. 
| serverConnection | [CIMInternetServerConnectionBase](CIMServiceLayers.md#ciminternetserverconnectionbase)|Gets and sets the server connection. 
| style | string|Gets and sets the style. 
| dimensions | {JSON_object}|Gets and sets the dimensions as a property set. 
| imageFormat | string|Gets and sets the image format. 
| tileMatrixSet | string|Gets and sets the tile matrix set. 
| capabilitiesParameters | {JSON_object}|Gets and sets the connection capabilities parameters as a property set. 
| mapParameters | {JSON_object}|Gets and sets the custom map parameters as a property set. 
| templateUrl | string|Gets or sets the template url that can be used for tile requests. 



