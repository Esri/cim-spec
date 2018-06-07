


## CIMDiagramBuilderDefinition
#### 


### CIMDiagramBuilderDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| rules | [CIMDiagramRuleDefinition](CIMNetworkDiagrams.md#cimdiagramruledefinition) |
| layouts | [CIMDiagramLayoutDefinition](CIMNetworkDiagrams.md#cimdiagramlayoutdefinition) |
| keepEdgeVertices | boolean|
| containerMargin | double|
| network | string|






## CIMDiagramDatasetDataConnection
#### 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDiagramDatasetDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| diagramDataset | string|


### CIMFeatureDatasetDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| featureDataset | string|Gets and sets feature dataset. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 






## CIMDiagramLayer
#### 


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


### CIMGroupLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| layers | IStringArray|Gets and sets the paths of the layers in the group layer. 
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing)|Gets and sets the symbol layer drawing definition. 


### CIMDiagramLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| referenceScale | double|
| dataConnection | [CIMNetworkDiagramDataConnection](CIMNetworkDiagrams.md#cimnetworkdiagramdataconnection)|






## CIMDiagramLayoutDefinition
#### 


### CIMDiagramLayoutDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|
| description | string|
| properties | {JSON_object}|






## CIMDiagramRelQueryDataConnection
#### 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDiagramRelQueryDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| diagramDatasetFeatureClass | [enumeration esriDiagramDatasetFeatureClass](ExternalReferences.md#enumeration-esridiagramdatasetfeatureclass)|
| networkSourceID | long|


### CIMFeatureDatasetDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| featureDataset | string|Gets and sets feature dataset. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 






## CIMDiagramRuleDefinition
#### 


### CIMDiagramRuleDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|
| description | string|
| isActive | boolean|
| properties | {JSON_object}|






## CIMNetworkDiagram
#### 


### CIMNetworkDiagram 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|
| ID | string|
| isTransient | boolean|
| isConsistent | boolean|
| templateString | string|
| network | string|
| layerURI | string|






## CIMNetworkDiagramDataConnection
#### 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMNetworkDiagramDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| diagram | string|
| isStored | boolean|
| table | string|Gets and sets the diagram table name. 


### CIMFeatureDatasetDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| featureDataset | string|Gets and sets feature dataset. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 



