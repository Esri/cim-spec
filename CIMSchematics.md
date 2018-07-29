


## CIMSchematicAlgorithm
Represents a schematic algorithm.


### CIMSchematicAlgorithm

|Property | Type | Description |
|---------|--------|--------|
| algorihmPropertySet | Object|An algorithm property set.
| algorithmCLSID | string|The algorithm CLSID.
| available | boolean|A boolean inndicating if the algorithm is currently available.
| label | string|The label of the algorithm.
| overridable | boolean|A boolean which indicates if the algorithm properties page is editable.
| useEndNode | boolean|A boolean which indicates if the algorithm uses end nodes.
| useRootNode | boolean|A boolean which indicates if the algorithm uses root nodes.






## CIMSchematicAttribute
Represents a schematic attribute.


### CIMSchematicAttribute

|Property | Type | Description |
|---------|--------|--------|
| attributeCLSID | string|The CLSID of the schematic attribute.
| description | string|The description of the schematic attribute.
| evaluationMode | [enumeration SchematicAttributeEvaluationMode](CIMSchematics.md#enumeration-schematicattributeevaluationmode)|The evaluation mode of the schematic attribute.
| isPredefined | boolean|A boolean indicating whether or not the schematic attribute is predefined.
| name | string|The name of the schematic attribute.
| parameters | Object|The schematic attribute parameters.
| storageFieldDescription | [CIMFieldDescription](CIMVectorLayers.md#cimfielddescription)|The storage field description.
| storageMode | [enumeration SchematicAttributeStorage](CIMSchematics.md#enumeration-schematicattributestorage)|The storage mode.
| storageName | string|The storage name.
| storagePropertyName | string|The storage property name.





### Enumeration: SchematicAttributeEvaluationMode
Schematic attribute evaluation modes.

|Property | Value | Description |
|---------|--------|--------|
| OnTheFlyEvaluation| 0| On the fly evaluation.
| BuildEvaluation| 1| Build time evaluation.
| LoadEvaluation| 2| Load time evaluation.
| DrawEvaluation| 3| Draw time evaluation.



### Enumeration: SchematicAttributeStorage
Schematic attribute storage modes.

|Property | Value | Description |
|---------|--------|--------|
| NoStorage| 0| No storage.
| FieldStorage| 1| Field storage.
| PropertySetStorage| 2| Property set storage.




## CIMSchematicBuilder
Represents a schematic builder.


### CIMSchematicBuilder

|Property | Type | Description |
|---------|--------|--------|
| autoCreateFeatureClasses | boolean|A boolean indicating whether or not to autocreate feature classes.
| builderCLSID | string|The builder CLSID.
| builderPropertySet | Object|The builder property set.
| initializeLinkVertices | boolean|A boolean indicating whether or not to initialize link verticies.
| name | string|The name.






## CIMSchematicDataConnection
Represents a schematic data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMSchematicDataConnection

|Property | Type | Description |
|---------|--------|--------|
| schematicDataset | string|The schematic dataset path.
| diagramTemplate | string|The diagram template.
| diagram | string|The diagram.


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.






## CIMSchematicDataSource
Represents a schematic data source.


### CIMSchematicDataSource

|Property | Type | Description |
|---------|--------|--------|
| dataSourceCLSID | string|The data source CLSID.
| dataSourceID | number //int32|The data source ID.
| initString | string|The data source init string.
| name | string|The data source name.






## CIMSchematicDataset
Represents a schematic dataset.


### CIMSchematicDataset

|Property | Type | Description |
|---------|--------|--------|
| is9xDataset | boolean|A boolean indicating whether or not this is an ArcGIS 9.x dataset.
| name | string|The dataset name.
| schematicDataSources | [CIMSchematicDataSource](CIMSchematics.md#cimschematicdatasource) |The schematic data sources.
| schematicDiagramTemplate | [CIMSchematicDiagramTemplate](CIMSchematics.md#cimschematicdiagramtemplate) |The schematic diagram template.
| schematicFeatureClasses | [CIMSchematicFeatureClass](CIMSchematics.md#cimschematicfeatureclass) |The schematic feature classes.
| workspace | [CIMWorkspaceConnection](CIMVectorLayers.md#cimworkspaceconnection)|The workspace connection.






## CIMSchematicDiagramTemplate
Represents a diagram template.


### CIMSchematicDiagramTemplate

|Property | Type | Description |
|---------|--------|--------|
| alwaysLoadDiagram | boolean|A boolean which indicates if the diagram is always loaded.
| associatedSchematicFeatureClasses | [string,]|The associated schematic feature classes.
| defaultSchematicAlgorithm | [CIMSchematicAlgorithm](CIMSchematics.md#cimschematicalgorithm)|The default schematic algorithm.
| defaultSchematicNodeClassName | string|The default schematic noce class name.
| externalQueryEvaluationMode | [enumeration SchematicExternalQueryEvaluationMode](CIMSchematics.md#enumeration-schematicexternalqueryevaluationmode)|The external query evaluation mode.
| diagramTemplateID | number //int32|The diagram template ID.
| identifierFieldNames | [string,]|The identifier field names.
| name | string|The name.
| predefinedAttributeNames | [string,]|The predefined attribute names.
| queryString | string|The query string.
| schematicAlgorithms | [CIMSchematicAlgorithm](CIMSchematics.md#cimschematicalgorithm) |The schematic algorithms.
| schematicAttributes | [CIMSchematicAttribute](CIMSchematics.md#cimschematicattribute) |The schematic attributes.
| schematicBuilder | [CIMSchematicBuilder](CIMSchematics.md#cimschematicbuilder)|The schematic builder.
| schematicDataSourceID | number //int32|The schematic data source ID.
| schematicLayerTemplate | [CIMSchematicLayer](CIMSchematics.md#cimschematiclayer)|The schematic layer template.
| schematicQueryParameters | [CIMSchematicQueryParameter](CIMSchematics.md#cimschematicqueryparameter) |The schematic query parameters.
| schematicRules | [CIMSchematicRule](CIMSchematics.md#cimschematicrule) |The schematic rules.
| schematicTraces | [CIMSchematicAlgorithm](CIMSchematics.md#cimschematicalgorithm) |The schematic traces.
| tableName | string|The table name.





### Enumeration: SchematicElementType
Schematic element types

|Property | Value | Description |
|---------|--------|--------|
| NodeType| 0| Node type.
| LinkType| 1| Link type.
| DrawingType| 2| Drawing type.
| NodeOnLinkType| 3| Node on link type.
| SubLinkType| 4| Sub link type.



### Enumeration: SchematicExternalQueryEvaluationMode
Schematic external query evaluation modes.

|Property | Value | Description |
|---------|--------|--------|
| NoQuery| 0| No query.
| BuilderEvaluation| 1| Builder evaluation.
| LoadEvaluation| 2| Load evaluation.




## CIMSchematicFeatureClass
Represents a schematic feature class.


### CIMSchematicFeatureClass

|Property | Type | Description |
|---------|--------|--------|
| associatedObjectClassDataSourceID | number //int32|The ID of the associated object class data source.
| associatedObjectClassID | number //int32|The ID of the associated object class.
| externalQueryEvaluationMode | [enumeration SchematicExternalQueryEvaluationMode](CIMSchematics.md#enumeration-schematicexternalqueryevaluationmode)|The external query evaluation mode.
| geometryType | [enumeration esriGeometryType](ExternalReferences.md#enumeration-esrigeometrytype)|The geometry type.
| featureClassID | number //int32|The feature class ID.
| identifierFieldNames | [string,]|The identifier field names.
| name | string|The name.
| parent | string|The parent.
| predefinedAttributeNames | [string,]|The predefined attribute names.
| queryString | string|The query string.
| schematicAttributes | [CIMSchematicAttribute](CIMSchematics.md#cimschematicattribute) |The schematic attributes.
| schematicDataSourceID | number //int32|The schematic data source ID.
| schematicElementType | [enumeration SchematicElementType](CIMSchematics.md#enumeration-schematicelementtype)|The schematic element type.
| schematicQueryParameters | [CIMSchematicQueryParameter](CIMSchematics.md#cimschematicqueryparameter) |The schematic query parameters.
| shapeFieldDescription | [CIMFieldDescription](CIMVectorLayers.md#cimfielddescription)|The shape field description.
| tableName | string|The table name.






## CIMSchematicLayer
Represents a schematic layer.


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


### CIMSchematicLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| layers | [string,]|The layers (as paths).
| schematicDiagram | [DataConnection](Types.md#dataconnection)|The data connection to the schematic diagram.
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing)|The symbol layer drawing configuration.
| referenceScale | number //double|The reference scale.
| isTemplate | boolean|A boolean indicating if this definition is a template.






## CIMSchematicQueryParameter
Represents a schematic query parameter.


### CIMSchematicQueryParameter

|Property | Type | Description |
|---------|--------|--------|
| isTextual | boolean|A boolean indicating whether or not the query parameter is textual.
| name | string|The name.






## CIMSchematicRule
Represents a schematic rule.


### CIMSchematicRule

|Property | Type | Description |
|---------|--------|--------|
| isActive | boolean|A boolean indicating if the rule is active.
| orderNumber | number //int32|The order number.
| ruleCLSID | string|The rule CLSID.
| rulePropertySet | Object|The rule property set.
