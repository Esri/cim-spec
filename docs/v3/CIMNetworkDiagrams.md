


## CIMDiagramLayer
#### Represents a diagram layer. 


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


### CIMStandaloneTableContainer 

|Property | Type | Description | 
|---------|--------|--------|
| standaloneTables | [string] | The standalone tables as an array of table repository paths. 


### CIMGroupLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| layers | [string] | The layer URIs of the layers in the group layer. 
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing) | The symbol layer drawing definition. 


### CIMDiagramLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| referenceScale | double | The digram layer's reference scale. 
| dataConnection | [CIMNetworkDiagramDataConnection](CIMNetworkDiagrams.md#cimnetworkdiagramdataconnection) | The data connection to the network diagram. 






## CIMDiagramRelQueryDataConnection
#### Represents a diagram rel query data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string | The workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory) | The workspace factory. 
| customWorkspaceFactoryCLSID | string | The classID of the custom workspace factory. 
| dataset | string | The dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype) | The dataset type. 


### CIMFeatureDatasetDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| featureDataset | string | Feature dataset. 


### CIMDiagramRelQueryDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| diagramDatasetFeatureClass | [enumeration esriDiagramDatasetFeatureClass](ExternalReferences.md#enumeration-esridiagramdatasetfeatureclass) | The diagram dataset feature class. 
| networkSourceID | long | The network source id. 






## CIMNetworkDiagramDataConnection
#### Represents a network diagram data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string | The workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory) | The workspace factory. 
| customWorkspaceFactoryCLSID | string | The classID of the custom workspace factory. 
| dataset | string | The dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype) | The dataset type. 


### CIMFeatureDatasetDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| featureDataset | string | Feature dataset. 


### CIMNetworkDiagramDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| diagram | string | The diagram. 
| isStored | boolean | A value indicating whether or not the diagram is stored. 
| table | string | The diagram table name. 



