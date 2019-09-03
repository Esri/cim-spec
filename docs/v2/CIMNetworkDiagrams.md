


## CIMDiagramBuilderDefinition
#### Represents a diagram builder definition. 


### CIMDiagramBuilderDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| rules | [[CIMDiagramRuleDefinition]](CIMNetworkDiagrams.md#cimdiagramruledefinition) | The diagram rules. 
| layouts | [[CIMDiagramLayoutDefinition]](CIMNetworkDiagrams.md#cimdiagramlayoutdefinition) | The diagram layouts. 
| keepEdgeVertices | boolean | A value indicating whether to keep edge vertices. 
| containerMargin | double | The container margin. 
| network | string | The network. 






## CIMDiagramDatasetDataConnection
#### Represents a diagram dataset data connection. 


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


### CIMDiagramDatasetDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| diagramDataset | string | The diagram dataset name. 






## CIMDiagramLayer
#### Represents a diagram layer. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the definition was last modified. 
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
| charts | [[CIMChart]](CIMLayer.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 


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






## CIMDiagramLayoutDefinition
#### Represents a diagram layout definition. 


### CIMDiagramLayoutDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The diagram layout name. 
| description | string | The diagram layout description. 
| properties | {JSON_object}| The diagram layout properties. 






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






## CIMDiagramRuleDefinition
#### Represents a diagram rule definition. 


### CIMDiagramRuleDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The diagram rule name. 
| description | string | The diagram rule description. 
| isActive | boolean | A value indicating whether the rule is active. 
| properties | {JSON_object}| The diagram rule properties. 






## CIMNetworkDiagram
#### Represents a network diagram. 


### CIMNetworkDiagram 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The network diagram name. 
| ID | string | The network diagram id. 
| isTransient | boolean | A value indicating whether the diagram is transient. 
| isConsistent | boolean | A value indicating whether the diagram is consistent. 
| templateString | string | The template string. 
| network | string | The network name. 
| layerURI | string | The layer URI. 






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



