


## CIMDiagramBuilderDefinition
####


### CIMDiagramBuilderDefinition

|Property | Type | Description |
|---------|--------|--------|
| rules | [CIMDiagramRuleDefinition](CIMNetworkDiagrams.md#cimdiagramruledefinition) |
| layouts | [CIMDiagramLayoutDefinition](CIMNetworkDiagrams.md#cimdiagramlayoutdefinition) |
| keepEdgeVertices | boolean|
| containerMargin | number //double|
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
| featureDataset | string|The feature dataset.


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.






## CIMDiagramLayer
####


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


### CIMGroupLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| layers | [string,]|The paths of the layers in the group layer.
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing)|The symbol layer drawing definition.


### CIMDiagramLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| referenceScale | number //double|
| dataConnection | [CIMNetworkDiagramDataConnection](CIMNetworkDiagrams.md#cimnetworkdiagramdataconnection)|






## CIMDiagramLayoutDefinition
####


### CIMDiagramLayoutDefinition

|Property | Type | Description |
|---------|--------|--------|
| name | string|
| description | string|
| properties | Object|






## CIMDiagramRelQueryDataConnection
####


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMDiagramRelQueryDataConnection

|Property | Type | Description |
|---------|--------|--------|
| diagramDatasetFeatureClass | [enumeration esriDiagramDatasetFeatureClass](ExternalReferences.md#enumeration-esridiagramdatasetfeatureclass)|
| networkSourceID | number //int32|


### CIMFeatureDatasetDataConnection

|Property | Type | Description |
|---------|--------|--------|
| featureDataset | string|The feature dataset.


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.






## CIMDiagramRuleDefinition
####


### CIMDiagramRuleDefinition

|Property | Type | Description |
|---------|--------|--------|
| name | string|
| description | string|
| isActive | boolean|
| properties | Object|






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
| table | string|The diagram table name.


### CIMFeatureDatasetDataConnection

|Property | Type | Description |
|---------|--------|--------|
| featureDataset | string|The feature dataset.


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.
