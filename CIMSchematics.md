


## CIMSchematicAlgorithm
#### Represents a schematic algorithm. 


### CIMSchematicAlgorithm 

|Property | Type | Description | 
|---------|--------|--------|
| algorihmPropertySet | {JSON_object}|Gets and sets an algorithm property set. 
| algorithmCLSID | string|Gets and sets the algorithm CLSID. 
| available | boolean|Gets and sets a boolean inndicating if the algorithm is currently available. 
| label | string|Gets and sets the label of the algorithm. 
| overridable | boolean|Gets and sets a boolean which indicates if the algorithm properties page is editable. 
| useEndNode | boolean|Gets and sets a boolean which indicates if the algorithm uses end nodes. 
| useRootNode | boolean|Gets and sets a boolean which indicates if the algorithm uses root nodes. 






## CIMSchematicAttribute
#### Represents a schematic attribute. 


### CIMSchematicAttribute 

|Property | Type | Description | 
|---------|--------|--------|
| attributeCLSID | string|Gets and sets the CLSID of the schematic attribute. 
| description | string|Gets and sets the description of the schematic attribute. 
| evaluationMode | [enumeration SchematicAttributeEvaluationMode](CIMSchematics.md#enumeration-schematicattributeevaluationmode)|Gets and sets the evaluation mode of the schematic attribute. 
| isPredefined | boolean|Gets and sets a boolean indicating whether or not the schematic attribute is predefined. 
| name | string|Gets and sets the name of the schematic attribute. 
| parameters | {JSON_object}|Gets and sets the schematic attribute parameters. 
| storageFieldDescription | [CIMFieldDescription](CIMVectorLayers.md#cimfielddescription)|Gets and sets the storage field description. 
| storageMode | [enumeration SchematicAttributeStorage](CIMSchematics.md#enumeration-schematicattributestorage)|Gets and sets the storage mode. 
| storageName | string|Gets and sets the storage name. 
| storagePropertyName | string|Gets and sets the storage property name. 





### Enumeration: SchematicAttributeEvaluationMode
#### Schematic attribute evaluation modes. 

|Property | Value | Description | 
|---------|--------|--------|
| OnTheFlyEvaluation| 0| On the fly evaluation. 
| BuildEvaluation| 1| Build time evaluation. 
| LoadEvaluation| 2| Load time evaluation. 
| DrawEvaluation| 3| Draw time evaluation. 



### Enumeration: SchematicAttributeStorage
#### Schematic attribute storage modes. 

|Property | Value | Description | 
|---------|--------|--------|
| NoStorage| 0| No storage. 
| FieldStorage| 1| Field storage. 
| PropertySetStorage| 2| Property set storage. 




## CIMSchematicBuilder
#### Represents a schematic builder. 


### CIMSchematicBuilder 

|Property | Type | Description | 
|---------|--------|--------|
| autoCreateFeatureClasses | boolean|Gets and sets a boolean indicating whether or not to autocreate feature classes. 
| builderCLSID | string|Gets and sets the builder CLSID. 
| builderPropertySet | {JSON_object}|Gets and sets the builder property set. 
| initializeLinkVertices | boolean|Gets and sets a boolean indicating whether or not to initialize link verticies. 
| name | string|Gets and sets the name. 






## CIMSchematicDataConnection
#### Represents a schematic data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMSchematicDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| schematicDataset | string|Gets and sets the schematic dataset path. 
| diagramTemplate | string|Gets and sets the diagram template. 
| diagram | string|Gets and sets the diagram. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 






## CIMSchematicDataSource
#### Represents a schematic data source. 


### CIMSchematicDataSource 

|Property | Type | Description | 
|---------|--------|--------|
| dataSourceCLSID | string|Gets and sets the data source CLSID. 
| dataSourceID | long|Gets and sets the data source ID. 
| initString | string|Gets and sets the data source init string. 
| name | string|Gets and sets the data source name. 






## CIMSchematicDataset
#### Represents a schematic dataset. 


### CIMSchematicDataset 

|Property | Type | Description | 
|---------|--------|--------|
| is9xDataset | boolean|Gets and sets a boolean indicating whether or not this is an ArcGIS 9.x dataset. 
| name | string|Gets and sets the dataset name. 
| schematicDataSources | [CIMSchematicDataSource](CIMSchematics.md#cimschematicdatasource) |Gets and sets the schematic data sources. 
| schematicDiagramTemplate | [CIMSchematicDiagramTemplate](CIMSchematics.md#cimschematicdiagramtemplate) |Gets and sets the schematic diagram template. 
| schematicFeatureClasses | [CIMSchematicFeatureClass](CIMSchematics.md#cimschematicfeatureclass) |Gets and sets the schematic feature classes. 
| workspace | [CIMWorkspaceConnection](CIMVectorLayers.md#cimworkspaceconnection)|Gets and sets the workspace connection. 






## CIMSchematicDiagramTemplate
#### Represents a diagram template. 


### CIMSchematicDiagramTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| alwaysLoadDiagram | boolean|Gets and sets a boolean which indicates if the diagram is always loaded. 
| associatedSchematicFeatureClasses | IStringArray|Gets and sets the associated schematic feature classes. 
| defaultSchematicAlgorithm | [CIMSchematicAlgorithm](CIMSchematics.md#cimschematicalgorithm)|Gets and sets the default schematic algorithm. 
| defaultSchematicNodeClassName | string|Gets and sets the default schematic noce class name. 
| externalQueryEvaluationMode | [enumeration SchematicExternalQueryEvaluationMode](CIMSchematics.md#enumeration-schematicexternalqueryevaluationmode)|Gets and sets the external query evaluation mode. 
| diagramTemplateID | long|Gets and sets the diagram template ID. 
| identifierFieldNames | IStringArray|Gets and sets the identifier field names. 
| name | string|Gets and sets the name. 
| predefinedAttributeNames | IStringArray|Gets and sets the predefined attribute names. 
| queryString | string|Gets and sets the query string. 
| schematicAlgorithms | [CIMSchematicAlgorithm](CIMSchematics.md#cimschematicalgorithm) |Gets and sets the schematic algorithms. 
| schematicAttributes | [CIMSchematicAttribute](CIMSchematics.md#cimschematicattribute) |Gets and sets the schematic attributes. 
| schematicBuilder | [CIMSchematicBuilder](CIMSchematics.md#cimschematicbuilder)|Gets and sets the schematic builder. 
| schematicDataSourceID | long|Gets and sets the schematic data source ID. 
| schematicLayerTemplate | [CIMSchematicLayer](CIMSchematics.md#cimschematiclayer)|Gets and sets the schematic layer template. 
| schematicQueryParameters | [CIMSchematicQueryParameter](CIMSchematics.md#cimschematicqueryparameter) |Gets and sets the schematic query parameters. 
| schematicRules | [CIMSchematicRule](CIMSchematics.md#cimschematicrule) |Gets and sets the schematic rules. 
| schematicTraces | [CIMSchematicAlgorithm](CIMSchematics.md#cimschematicalgorithm) |Gets and sets the schematic traces. 
| tableName | string|Gets and sets the table name. 





### Enumeration: SchematicElementType
#### Schematic element types 

|Property | Value | Description | 
|---------|--------|--------|
| NodeType| 0| Node type. 
| LinkType| 1| Link type. 
| DrawingType| 2| Drawing type. 
| NodeOnLinkType| 3| Node on link type. 
| SubLinkType| 4| Sub link type. 



### Enumeration: SchematicExternalQueryEvaluationMode
#### Schematic external query evaluation modes. 

|Property | Value | Description | 
|---------|--------|--------|
| NoQuery| 0| No query. 
| BuilderEvaluation| 1| Builder evaluation. 
| LoadEvaluation| 2| Load evaluation. 




## CIMSchematicFeatureClass
#### Represents a schematic feature class. 


### CIMSchematicFeatureClass 

|Property | Type | Description | 
|---------|--------|--------|
| associatedObjectClassDataSourceID | long|Gets and sets the ID of the associated object class data source. 
| associatedObjectClassID | long|Gets and sets the ID of the associated object class. 
| externalQueryEvaluationMode | [enumeration SchematicExternalQueryEvaluationMode](CIMSchematics.md#enumeration-schematicexternalqueryevaluationmode)|Gets and sets the external query evaluation mode. 
| geometryType | [enumeration esriGeometryType](ExternalReferences.md#enumeration-esrigeometrytype)|Gets and sets the geometry type. 
| featureClassID | long|Gets and sets the feature class ID. 
| identifierFieldNames | IStringArray|Gets and sets the identifier field names. 
| name | string|Gets and sets the name. 
| parent | string|Gets and sets the parent. 
| predefinedAttributeNames | IStringArray|Gets and sets the predefined attribute names. 
| queryString | string|Gets and sets the query string. 
| schematicAttributes | [CIMSchematicAttribute](CIMSchematics.md#cimschematicattribute) |Gets and sets the schematic attributes. 
| schematicDataSourceID | long|Gets and sets the schematic data source ID. 
| schematicElementType | [enumeration SchematicElementType](CIMSchematics.md#enumeration-schematicelementtype)|Gets and sets the schematic element type. 
| schematicQueryParameters | [CIMSchematicQueryParameter](CIMSchematics.md#cimschematicqueryparameter) |Gets and sets the schematic query parameters. 
| shapeFieldDescription | [CIMFieldDescription](CIMVectorLayers.md#cimfielddescription)|Gets and sets the shape field description. 
| tableName | string|Gets and sets the table name. 






## CIMSchematicLayer
#### Represents a schematic layer. 


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


### CIMSchematicLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| layers | IStringArray|Gets and sets the layers (as paths). 
| schematicDiagram | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection to the schematic diagram. 
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing)|Gets and sets the symbol layer drawing configuration. 
| referenceScale | double|Gets and sets the reference scale. 
| isTemplate | boolean|Gets and sets a boolean indicating if this definition is a template. 






## CIMSchematicQueryParameter
#### Represents a schematic query parameter. 


### CIMSchematicQueryParameter 

|Property | Type | Description | 
|---------|--------|--------|
| isTextual | boolean|Gets and sets a boolean indicating whether or not the query parameter is textual. 
| name | string|Gets and sets the name. 






## CIMSchematicRule
#### Represents a schematic rule. 


### CIMSchematicRule 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean|Gets and sets a boolean indicating if the rule is active. 
| orderNumber | long|Gets and sets the order number. 
| ruleCLSID | string|Gets and sets the rule CLSID. 
| rulePropertySet | {JSON_object}|Gets and sets the rule property set. 



