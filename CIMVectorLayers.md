


## CIMAnnotationLayer
#### Represents an annotation layer used to draw annotation feature classes. 


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


### CIMFeatureLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| autoGenerateFeatureTemplates | boolean|Gets and sets a boolean option indicating whether to automatically generate feature templates from the renderer. 
| extrusion | [CIMFeatureExtrusion](CIMVectorLayers.md#cimfeatureextrusion)|Gets and sets the feature extrusion. 
| featureElevationExpression | string|Gets and sets the feature elevation expression. 
| featureHyperlinks | [CIMFeatureHyperlink](CIMVectorLayers.md#cimfeaturehyperlink) |Gets and sets the feature hyperlinks. 
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable)|Gets and sets the feature table. 
| featureTemplates | [CIMEditingTemplate](Types.md#cimeditingtemplate) |Gets and sets the feature templates. 
| hotlinkField | string|Gets and sets the field containing hotlink URLs. 
| htmlPopupEnabled | boolean|Gets and sets a boolean option indicating whether HTML popups are enabled. 
| htmlPopupFormat | [CIMHtmlPopupFormat](CIMVectorLayers.md#cimhtmlpopupformat)|Gets and sets the HTML popups format. 
| isFlattened | boolean|Gets and sets a boolean option indicating whether the layer is flattened. 
| selectable | boolean|Gets and sets a boolean option indicating whether the layer is selectable. 
| selectionColor | [Color](Types.md#color)|Gets and sets the selection color. 
| selectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the selection symbol. 
| useSelectionSymbol | boolean|Gets and sets a boolean option indicating whether to use the selection symbol. 
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition)|Use current map series page to select features. 
| featureCacheType | [enumeration FeatureCacheType](CIMVectorLayers.md#enumeration-featurecachetype)|Gets and sets the feature cache type. 
| enableDisplayFilters | boolean|Gets and sets a boolean option indicating whether the current set of display filters are honored during drawing. 
| displayFilters | [CIMDisplayFilter](CIMVectorLayers.md#cimdisplayfilter) |Gets and sets the current set of display filters. 
| featureElevationExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets the expression for setting the feature elevation 


### CIMAnnotationLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight)|Gets and sets the weight of features in this layer when considered as barriers to labeling. 
| drawGeometry | boolean|Gets and sets a Boolean property designating whether the geometry of the text graphics should be drawn. 
| drawUnplacedAnnotation | boolean|Gets and sets a Boolean property designating whether unplaced annotation should be drawn. 
| drawGeometryLineSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the line symbol used to draw text graphic line geometries when the DrawGeometry option is true. 
| drawGeometryPointSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the point symbol used to draw text graphic line geometries when the DrawGeometry option is true. 
| unplacedAnnotationColor | [Color](Types.md#color)|Gets and sets the color that unplaced text graphics will be drawn with when Unplaced Annotation is drawn. 
| symbolSubstitutionType | [enumeration SymbolSubstitutionType](CIMVectorLayers.md#enumeration-symbolsubstitutiontype)|Gets and sets the type of symbol substitution this layer uses. 
| massColorSubstitute | [Color](Types.md#color)|Gets and sets the mass color substitute. When using the SymbolSubstitutionColor substitution type this is the color that all text graphics will be overridden with. 
| inlineColor | [Color](Types.md#color)|Gets and sets the inline color. When using the SymbolSubstitutionIndividualSubordinate or SymbolSubstitutionIndividualDominant substitution types this is the color that all text graphics that are stored inline (bloated) will be overridden with. 
| substitutionSymbolCollection | [CIMSymbolIdentifier](CIMVectorLayers.md#cimsymbolidentifier) |Gets and sets a symbol substitution collection. When using the SymbolSubstitutionIndividualSubordinate or SymbolSubstitutionIndividualDominant substitution types this collection defines which symbols in the symbol collection are substituted and what their substitute values are. The symbol substitution properties allow the users to swap out symbols/colors of annotation stored in the geodatabase at the layer level. This allows annotation to be repurposed in maps without duplicating the annotation. The classic case for this behavior is when a user wishes to utilize black text generated for standard parcel maps on top of a map with raster imagery. By substituting the color or symbol collection of the annotation the user is allowed to change the appearance for this one map without a large performance or data management overhead. One complex aspect of symbol substitution is how overrides are treated when it is enabled. When this feature was originally added some wanted overrides to be respected and others did not, so options were added for this (dominant and subordinate substitution types). When the dominant type is chosen overrides are ignored. When the subordinate type is chosen overrides are applied on top of the new symbols. 
| subLayers | [CIMAnnotationSubLayer](CIMVectorLayers.md#cimannotationsublayer) |Gets and sets a collection of AnnotationSubLayers, corresponding to the annotation subclasses defined by the annotation feature class. 






## CIMAnnotationSubLayer
#### Represents an annotation sublayer used to draw annotation feature classes subclasses. 


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


### CIMAnnotationSubLayer 

|Property | Type | Description | 
|---------|--------|--------|





### Enumeration: AttachmentDisplayType
#### Attachment display types. 

|Property | Value | Description | 
|---------|--------|--------|
| PreviewFirst| 0| Preview first. 
| PreviewAll| 1| Preview all. 
| List| 2| List. 




## CIMAttachmentsMediaInfo
#### Represents attachment media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long|Gets and sets the row. 
| column | long|Gets and sets the column. 
| refreshRate | double|The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media. 


### CIMAttachmentMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| caption | string|Gets and sets the caption. 
| title | string|Gets and sets the title. 
| contentType | string|Gets and sets the content MIME type. Example: (image/png, image/jpeg, audio/mp3 
| displayType | [enumeration AttachmentDisplayType](CIMVectorLayers.md#enumeration-attachmentdisplaytype)|Gets and sets the display type. 






## CIMAttributeCondition
#### Represents an attribute condition. 


### CIMCondition 

|Property | Type | Description | 
|---------|--------|--------|


### CIMAttributeCondition 

|Property | Type | Description | 
|---------|--------|--------|
| whereClause | string|Gets and sets the where clause. 






## CIMBarChartMediaInfo
#### Represents bar chart media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long|Gets and sets the row. 
| column | long|Gets and sets the column. 
| refreshRate | double|The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media. 


### CIMChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| fields | IStringArray|Gets and sets the fields. 
| normalizeField | string|Gets and sets the normalization field. 
| caption | string|Gets and sets the caption. 
| title | string|Gets and sets the title. 


### CIMBarChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|





### Enumeration: BarrierWeight
#### Barrier weights. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No weight. 
| Low| 1| Low weight. 
| Medium| 2| Medium weight. 
| High| 3| High weight. 



### Enumeration: BindVariableType
#### Bind variable types. 

|Property | Value | Description | 
|---------|--------|--------|
| String| 0| String variable type. 
| Integer| 1| Integer variable type. 
| Double| 2| Double variable type. 
| Date| 3| Date variable type. 




## CIMColumnChartMediaInfo
#### Represents column chart media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long|Gets and sets the row. 
| column | long|Gets and sets the column. 
| refreshRate | double|The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media. 


### CIMChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| fields | IStringArray|Gets and sets the fields. 
| normalizeField | string|Gets and sets the normalization field. 
| caption | string|Gets and sets the caption. 
| title | string|Gets and sets the title. 


### CIMColumnChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|





### Enumeration: DataSearchMode
#### Field search modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Contains| 0| Search for values that contain the search text. 
| Exact| 1| Search for values that are the exact match with the search text. 




## CIMDimensionLayer
#### Represents an dimension layer used to draw dimension feature classes. 


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


### CIMFeatureLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| autoGenerateFeatureTemplates | boolean|Gets and sets a boolean option indicating whether to automatically generate feature templates from the renderer. 
| extrusion | [CIMFeatureExtrusion](CIMVectorLayers.md#cimfeatureextrusion)|Gets and sets the feature extrusion. 
| featureElevationExpression | string|Gets and sets the feature elevation expression. 
| featureHyperlinks | [CIMFeatureHyperlink](CIMVectorLayers.md#cimfeaturehyperlink) |Gets and sets the feature hyperlinks. 
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable)|Gets and sets the feature table. 
| featureTemplates | [CIMEditingTemplate](Types.md#cimeditingtemplate) |Gets and sets the feature templates. 
| hotlinkField | string|Gets and sets the field containing hotlink URLs. 
| htmlPopupEnabled | boolean|Gets and sets a boolean option indicating whether HTML popups are enabled. 
| htmlPopupFormat | [CIMHtmlPopupFormat](CIMVectorLayers.md#cimhtmlpopupformat)|Gets and sets the HTML popups format. 
| isFlattened | boolean|Gets and sets a boolean option indicating whether the layer is flattened. 
| selectable | boolean|Gets and sets a boolean option indicating whether the layer is selectable. 
| selectionColor | [Color](Types.md#color)|Gets and sets the selection color. 
| selectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the selection symbol. 
| useSelectionSymbol | boolean|Gets and sets a boolean option indicating whether to use the selection symbol. 
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition)|Use current map series page to select features. 
| featureCacheType | [enumeration FeatureCacheType](CIMVectorLayers.md#enumeration-featurecachetype)|Gets and sets the feature cache type. 
| enableDisplayFilters | boolean|Gets and sets a boolean option indicating whether the current set of display filters are honored during drawing. 
| displayFilters | [CIMDisplayFilter](CIMVectorLayers.md#cimdisplayfilter) |Gets and sets the current set of display filters. 
| featureElevationExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets the expression for setting the feature elevation 


### CIMDimensionLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight)|Gets and sets the weight of features in this layer when considered as barriers to labeling. 





### Enumeration: DimensionMarkerFit
#### Dimension marker fit options. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Do not fit markers with text. 
| Tolerance| 1| Fit markers with text using the length of the dimension line. 
| Text| 2| Fit markers when overlapping the text. 



### Enumeration: DimensionPartOptions
#### Dimension part options. 

|Property | Value | Description | 
|---------|--------|--------|
| Begin| 0| Only display the beginning dimension part. 
| End| 1| Only display the end dimension part. 
| None| 2| Do not display any dimension parts. 
| Both| 3| Display both dimension parts. 




## CIMDimensionStyle
#### Represents an dimension style which defines dimension appearance. 


### CIMDimensionStyle 

|Property | Type | Description | 
|---------|--------|--------|
| align | boolean|Gets and sets a boolean property which indicates if the text should be aligned with the dimension line. 
| baselineHeight | double|Gets and sets the height of the construction for creating baseline dimensions with this style. 
| beginMarkerSymbol | [CIMPointSymbol](CIMSymbols.md#cimpointsymbol)|Gets and sets the symbol used for the begin arrow. 
| convertUnits | boolean|Gets and sets a boolean property which indicates if the length of the dimension needs to be converted for display. 
| dimensionLineOption | [enumeration DimensionPartOptions](CIMVectorLayers.md#enumeration-dimensionpartoptions)|Gets and sets the dimension line display of the style. 
| dimensionLineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol)|Gets and sets the symbol used for the dimension line. 
| displayPrecision | long|Gets and sets the precision for the value displayed by the dimension text. 
| displayUnits | [Unit](ExternalReferences.md#unit)|Gets and sets the units the length of the dimension text is displayed in. 
| drawLineOnFit | boolean|Gets and sets a boolean value which indicates if a dimension line should be drawn between the extension lines for an inward dimension. 
| endMarkerSymbol | [CIMPointSymbol](CIMSymbols.md#cimpointsymbol)|Gets and sets the symbol used for the end arrow. 
| expression | string|Gets and sets the text expression for the style. 
| expressionParserName | string|Gets and sets the text expression parser for the text expression for the style. 
| extendLineOnFit | boolean|Gets and sets a boolean property which indicates if the dimension line will be extended to underline the text on inward dimensions. 
| extensionLineOffset | double|Gets and sets the length of the extension line offset. 
| extensionLineOption | [enumeration DimensionPartOptions](CIMVectorLayers.md#enumeration-dimensionpartoptions)|Gets and sets the extension line display options of the style. 
| extensionLineOvershot | double|Gets and sets the length of the extension line overshot. 
| extensionLineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol)|Gets and sets the symbol used for extension lines. 
| ID | long|Gets and sets the ID of the style. 
| markerFit | [enumeration DimensionMarkerFit](CIMVectorLayers.md#enumeration-dimensionmarkerfit)|Gets and sets the arrow fit policy of the style. 
| markerFitTolerance | double|Gets and sets the arrow fit tolerance of the style. 
| markerOption | [enumeration DimensionPartOptions](CIMVectorLayers.md#enumeration-dimensionpartoptions)|Gets and sets the arrow display properties of the style. 
| name | string|Gets and sets the name of the style. 
| prefix | string|Gets and sets the prefix for the text expression for the style. 
| suffix | string|Gets and sets the suffix for the text expression for the style. 
| textFit | [enumeration DimensionTextFit](CIMVectorLayers.md#enumeration-dimensiontextfit)|Gets and sets the text fit policy for the style. 
| textOption | [enumeration DimensionTextOption](CIMVectorLayers.md#enumeration-dimensiontextoption)|Gets and sets the text display option for the style. 
| textSymbol | [CIMTextSymbol](CIMSymbols.md#cimtextsymbol)|Gets and sets the text symbol used for the text. 





### Enumeration: DimensionTextFit
#### Dimension text fit options. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Do not fit the text. 
| MoveBegin| 1| Move the text outside the begin extension line. 
| MoveEnd| 2| Move the text outside the end extension line. 



### Enumeration: DimensionTextOption
#### Dimension text options. 

|Property | Value | Description | 
|---------|--------|--------|
| Only| 0| Only display the value of the dimension length. 
| Suffix| 1| Display the value of the dimension length with a prefix and suffix. 
| Expression| 2| Display a text string derived from a custom expression. 
| None| 3| Do not display any text. 




## CIMDiscreteVariable
#### Represents a single bind variable. 


### CIMBindVariable 

|Property | Type | Description | 
|---------|--------|--------|
| variableName | string|Gets and sets the name of the variable. The name must be unique among all variables. 
| alias | string|Gets and sets the alias of the variable. 
| dataType | [enumeration BindVariableType](CIMVectorLayers.md#enumeration-bindvariabletype)|Gets and sets the type of the variable. 


### CIMDiscreteVariable 

|Property | Type | Description | 
|---------|--------|--------|
| defaultValue | ["<string>" / <number> / {JSON_object}]|Gets and sets the variable's required default value. The array can have multiple values only if AllowMultiple is true. 
| boundValue | ["<string>" / <number> / {JSON_object}]|Gets and sets the variable's currently-bound value. The array can have multiple values only if AllowMultiple is true. 
| allowMultiple | bool|Gets and sets whether the variable will accept an array of values. 






## CIMDisplayFilter
#### Represents a display filter used to restrict the display of features across scale ranges. 


### CIMDisplayFilter 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name of the display filter. 
| whereClause | string|Gets and sets the where clause that filters features for a given scale range. 
| minScale | double|Gets and sets the minimum scale for this display filter. 
| maxScale | double|Gets and sets the maximum scale for this display filter. 






## CIMEditingTemplateRelationship
#### Represents an editing template relationship. 


### CIMEditingTemplateRelationship 

|Property | Type | Description | 
|---------|--------|--------|
| tableURI | string|Gets and sets the table URI of the table the relationship corresponds to. 
| name | string|Gets and sets the name. 
| relationshipID | long|Gets and sets the relationship ID. 






## CIMEditingTemplateToolOptions
#### 


### CIMEditingTemplateToolOptions 

|Property | Type | Description | 
|---------|--------|--------|
| toolProgID | string|Gets and sets the tool ProgID. 
| options | {JSON_object}|Gets and sets the options for the specified creation tool. 





### Enumeration: FeatureCacheType
#### Feature cache type options. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No cache. 
| Session| 1| Cache is maintained in session. 




## CIMFeatureDatasetDataConnection
#### Represents a feature dataset data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


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





### Enumeration: FeatureExpirationMethod
#### Stream service feature expiration method. 

|Property | Value | Description | 
|---------|--------|--------|
| MaximumFeatureCount| 0| The oldest features will expire after a threshold number of features has been reached. 
| MaximumFeatureAge| 1| Features will expire after the specified time since the beginning of their lifetime. 




## CIMFeatureExtrusion
#### Represents feature extrusion. 


### CIMFeatureExtrusion 

|Property | Type | Description | 
|---------|--------|--------|
| extrusionType | [enumeration ExtrusionType](CIMEnumerations.md#enumeration-extrusiontype)|Gets and sets the extrusion type. 
| extrusionExpression | string|Gets and sets the extrusion expression. 
| extrusionUnit | [LinearUnit](ExternalReferences.md#linearunit)|Gets and sets the feature layer's extrusion unit. 
| extrusionExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets the ExpressionInfo that contains Arcade expresion that returns a numeric value. 






## CIMFeatureHyperlink
#### Represents feature hyperlink. 


### CIMFeatureHyperlink 

|Property | Type | Description | 
|---------|--------|--------|
| featureID | long|Gets and sets the feature ID. 
| link | string|Gets and sets the link URL. 






## CIMFeatureLayer
#### Represents feature layer used to draw data from feature classes. A feature layer displays a set of geographic features. A geographic feature represents a real-world object on the earth. It has a spatially- referenced location, stored as a point, line, or polygon, and a set of attributes that describe the feature. Its position is accurate and relevant within a particular scale range. Geographic features are the core spatial data holdings of an organization. They can serve as official records, are used in spatial analysis, and are used as source data for cartography. Feature layers draw their features by using a feature renderer to transform the geographic feature into one or more graphic entities. Feature renderers read the feature's geometry and attribute values to generate graphic entities that graphically depict the feature on a map. 


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


### CIMFeatureLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| autoGenerateFeatureTemplates | boolean|Gets and sets a boolean option indicating whether to automatically generate feature templates from the renderer. 
| extrusion | [CIMFeatureExtrusion](CIMVectorLayers.md#cimfeatureextrusion)|Gets and sets the feature extrusion. 
| featureElevationExpression | string|Gets and sets the feature elevation expression. 
| featureHyperlinks | [CIMFeatureHyperlink](CIMVectorLayers.md#cimfeaturehyperlink) |Gets and sets the feature hyperlinks. 
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable)|Gets and sets the feature table. 
| featureTemplates | [CIMEditingTemplate](Types.md#cimeditingtemplate) |Gets and sets the feature templates. 
| hotlinkField | string|Gets and sets the field containing hotlink URLs. 
| htmlPopupEnabled | boolean|Gets and sets a boolean option indicating whether HTML popups are enabled. 
| htmlPopupFormat | [CIMHtmlPopupFormat](CIMVectorLayers.md#cimhtmlpopupformat)|Gets and sets the HTML popups format. 
| isFlattened | boolean|Gets and sets a boolean option indicating whether the layer is flattened. 
| selectable | boolean|Gets and sets a boolean option indicating whether the layer is selectable. 
| selectionColor | [Color](Types.md#color)|Gets and sets the selection color. 
| selectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the selection symbol. 
| useSelectionSymbol | boolean|Gets and sets a boolean option indicating whether to use the selection symbol. 
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition)|Use current map series page to select features. 
| featureCacheType | [enumeration FeatureCacheType](CIMVectorLayers.md#enumeration-featurecachetype)|Gets and sets the feature cache type. 
| enableDisplayFilters | boolean|Gets and sets a boolean option indicating whether the current set of display filters are honored during drawing. 
| displayFilters | [CIMDisplayFilter](CIMVectorLayers.md#cimdisplayfilter) |Gets and sets the current set of display filters. 
| featureElevationExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets the expression for setting the feature elevation 


### CIMGeoFeatureLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| actions | [CIMLayerAction](CIMVectorLayers.md#cimlayeraction) |Gets and sets the layer actions. 
| exclusionSet | [LongLongArray](ExternalReferences.md#longlongarray)|Gets and sets the set of excluded features. 
| featureMasks | [CIMDataConnection](Types.md#cimdataconnection) |Gets and sets the data connection os the masking data. 
| labelClasses | [CIMLabelClass](CIMLabelPlacement.md#cimlabelclass) |Gets and sets the collection of label class definitions. 
| labelVisibility | boolean|Gets and sets a boolean option indicating whether to display labels for this layer's label classes. 
| maskedSymbolLayers | [CIMSymbolLayerMasking](CIMVectorLayers.md#cimsymbollayermasking) |Gets and sets the masked symbol layers. Each SymbolLayerMasking gives the symbol layers that are masked by that masking layer. 
| mostCurrentRenderer | [Renderer](Types.md#renderer)|Gets and sets the renderer used for the most current features when displaying tracks. 
| renderer | [Renderer](Types.md#renderer)|Gets and sets the primary symbol renderer. 
| scaleSymbols | boolean|Gets and sets a boolean option indicating whether to scale the symbols in this layer based on the map's reference scale. 
| snappable | boolean|Gets and sets a boolean option indicating whether this layer participates in snapping in the editor. 
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing)|Gets and sets the symbol layer drawing properties. 
| trackLinesRenderer | [Renderer](Types.md#renderer)|Gets and sets the track renderer when displaying tracks. 
| useRealWorldSymbolSizes | boolean|Gets and sets a boolean option indicating whether to use real world symbols sizes (meters) vs. points. 






## CIMFeatureTable
#### Represents a feature table. 


### CIMDisplayTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| definitionExpression | string|Gets and sets the definition expression that can subset the rows in the virtual table. 
| displayField | string|Gets and sets the name of the attribute field that will be used as a label that represents each row in the table. The display field must be able to be represented as a string (string or numeric). 
| editable | boolean|Gets and sets a boolean option indicating whether or not the table can be edited. 
| relates | [CIMRelateInfoBase](CIMVectorLayers.md#cimrelateinfobase) |Gets and sets the relates. 
| fieldDescriptions | [CIMFieldDescription](CIMVectorLayers.md#cimfielddescription) |Gets and sets the field descriptions. Field descriptions for fields may only be written if values are overridden from defaults. 
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition)|Gets and sets the time fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|Gets and sets the time definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|Gets and sets the time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition)|Gets and sets the time definition fields. 
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |Gets and sets the range defintions. 
| activeRangeName | string|Gets and sets the active range name. 
| selectRelatedData | boolean|Gets or sets a value indicating if related data should be selected when creating a new selection. 
| bindVariables | [CIMBindVariable](Types.md#cimbindvariable) |Gets and sets the bind variables. 
| subtypeValue | long|Gets and sets the subtype value that should be used in the feature layer definition. This property is honored only when feature layer is a member of SubtypeLayer. 
| useSubtypeValue | boolean|Gets and sets a boolean option indicating whether or not the SubtypeValue should be used. 
| displayExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets the expression information used for coming up with a string that represents a row or a feature. 
| selectionSetURI | string|Gets and sets the URI of the selection set for the table. 


### CIMFeatureTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection. 
| studyArea | [Area](ExternalReferences.md#area)|Gets and sets sn area that can be used to subset the rows in the virtual table. 
| studyAreaSpatialRel | [enumeration esriSpatialRelEnum](ExternalReferences.md#enumeration-esrispatialrelenum)|Gets and sets the study area spatial relationship. 
| searchOrder | [enumeration esriSearchOrder](ExternalReferences.md#enumeration-esrisearchorder)|Gets and sets the search order option. 
| isLicensedDataSource | boolean|Gets and sets a boolean option indicating whether the data source is licensed. 
| definitionSetURI | string|Gets or sets the DefinitionSet for the table. 






## CIMFeatureTemplate
#### Represents a feature template. 


### CIMEditingTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| name | string|Gets and sets the name. 
| tags | string|Gets and sets the tags. 
| toolProgID | string|Gets and sets the tool ProgID. 
| toolFilter | IStringArray|Gets and sets the tool filter. 
| toolOptions | [CIMEditingTemplateToolOptions](CIMVectorLayers.md#cimeditingtemplatetooloptions) |Gets and sets the per-tool options. 


### CIMBasicFeatureTemplate  

|Property | Type | Description | 
|---------|--------|--------|
| defaultValues | {JSON_object}|Gets and sets the default values. 
| requiredFields | IStringArray|Gets and sets the required fields. 
| hiddenFields | IStringArray|Gets and sets the hidden fields. 
| relationships | [CIMEditingTemplateRelationship](CIMVectorLayers.md#cimeditingtemplaterelationship) |Gets and sets the template relationships. 


### CIMFeatureTemplate 

|Property | Type | Description | 
|---------|--------|--------|






## CIMFieldDescription
#### Represents a field description. 


### CIMFieldDescription 

|Property | Type | Description | 
|---------|--------|--------|
| alias | string|Gets and sets the field alias. 
| fieldName | string|Gets and sets the field name. 
| highlight | boolean|Gets and sets a boolean option indicating whether the field is highlighted. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format. 
| readOnly | boolean|Gets and sets a boolean option indicating whether the field is read only. 
| visible | boolean|Gets and sets a boolean option indicating whether the field is visible. 
| valueAsRatio | boolean|Gets and sets a boolean option indicating whether the field value is a ratio (used only by geoprocessing). 
| searchable | boolean|Gets and sets a boolean indicating whether the values from this field should be included in the search. 
| searchMode | [enumeration DataSearchMode](CIMVectorLayers.md#enumeration-datasearchmode)|Gets and sets search mode to use when searching for values in this field. 






## CIMFolderConnection
#### Represents a folder connection. 


### CIMFolderConnection 

|Property | Type | Description | 
|---------|--------|--------|
| folderConnectionString | string|Gets and sets the folder connection string. 
| alias | string|Gets and sets the connection alias. 






## CIMGeometryLocationCondition
#### Represents geometry location condition. 


### CIMCondition 

|Property | Type | Description | 
|---------|--------|--------|


### CIMLocationCondition 

|Property | Type | Description | 
|---------|--------|--------|
| conditionType | [enumeration LocationConditionType](CIMVectorLayers.md#enumeration-locationconditiontype)|Gets and sets the location condition type. 


### CIMGeometryLocationCondition 

|Property | Type | Description | 
|---------|--------|--------|
| geometries | [GeometryArray](ExternalReferences.md#geometryarray)|Gets and sets the geometries. 






## CIMGroupEditingTemplate
#### Represents a group editing template. 


### CIMEditingTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| name | string|Gets and sets the name. 
| tags | string|Gets and sets the tags. 
| toolProgID | string|Gets and sets the tool ProgID. 
| toolFilter | IStringArray|Gets and sets the tool filter. 
| toolOptions | [CIMEditingTemplateToolOptions](CIMVectorLayers.md#cimeditingtemplatetooloptions) |Gets and sets the per-tool options. 


### CIMGroupEditingTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| baseName | string|Gets and sets the base name. 
| basePart | [CIMGroupEditingTemplatePart](CIMVectorLayers.md#cimgroupeditingtemplatepart)|Gets and sets the base part. 
| parts | [CIMGroupEditingTemplatePart](CIMVectorLayers.md#cimgroupeditingtemplatepart) |Gets and sets the parts. 






## CIMGroupEditingTemplatePart
#### Represents a group editing template part. 


### CIMGroupEditingTemplatePart 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string|Gets and sets the URI of the layer this template is defined for. 
| name | string|Gets and sets the name. 
| transformationID | string|Gets and sets the transformation ID. 
| options | {JSON_object}|Gets and sets the options. 






## CIMHighlightActivity
#### Represents a highlight activity. 


### CIMActivity 

|Property | Type | Description | 
|---------|--------|--------|


### CIMHighlightActivity 

|Property | Type | Description | 
|---------|--------|--------|
| highlightSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the highlight symbol. 






## CIMHtmlPopupFormat
#### Represents an HTML popup format. 


### CIMHtmlPopupFormat 

|Property | Type | Description | 
|---------|--------|--------|
| htmlRedirectField | string|Gets and sets the redirect field. 
| htmlRedirectFieldPrefix | string|Gets and sets the redirect field prefix. 
| htmlRedirectFieldSuffix | string|Gets and sets the redirect field suffix. 
| htmlXSLStyleSheet | string|Gets and sets the XSL style sheet. 
| htmlHideFieldNameColumn | boolean|Gets and sets a boolean value indicating whether of not to hide the field name column. 
| htmlUseCodedDomainValues | boolean|Gets and sets a boolean value indicating whether of not to use coded domain values. 
| htmlPresentationStyle | [enumeration HtmlPopupStyle](CIMVectorLayers.md#enumeration-htmlpopupstyle)|Gets and sets the presentation style. 





### Enumeration: HtmlPopupStyle
#### HTML popup styles. 

|Property | Value | Description | 
|---------|--------|--------|
| TwoColumnTable| 0| A two column table. 
| RedirectedHTML| 1| Redirected HTML. 
| XSLStyleSheet| 2| An XSL style sheet. 




## CIMImageMediaInfo
#### Represents image media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long|Gets and sets the row. 
| column | long|Gets and sets the column. 
| refreshRate | double|The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media. 


### CIMImageMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| sourceURL | string|Gets and sets the source URL. 
| linkURL | string|Gets and sets the link URL. 
| caption | string|Gets and sets the caption. 
| title | string|Gets and sets the title. 






## CIMLayerAction
#### Represents a layer action 


### CIMLayerAction 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| activities | [CIMActivity](Types.md#cimactivity) |Gets and sets activities. 
| conditions | [CIMCondition](Types.md#cimcondition) |Gets and sets conditions. 






## CIMLayerRange
#### Represents a layer range. 


### CIMLayerRange 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string|Gets and sets the URI of the layer this range is defined for. 
| rangeName | string|Gets and sets the range name. 
| currentRange | [CIMRange](CIMVectorLayers.md#cimrange)|Gets and sets the current range. 
| isExclusion | boolean|Gets and sets a boolean value indicating whether or not this is an exclusion range. 






## CIMLineChartMediaInfo
#### Represents line chart media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long|Gets and sets the row. 
| column | long|Gets and sets the column. 
| refreshRate | double|The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media. 


### CIMChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| fields | IStringArray|Gets and sets the fields. 
| normalizeField | string|Gets and sets the normalization field. 
| caption | string|Gets and sets the caption. 
| title | string|Gets and sets the title. 


### CIMLineChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|





### Enumeration: LocationConditionType
#### Location condition types. 

|Property | Value | Description | 
|---------|--------|--------|
| In| 0| In. 
| Depart| 1| Depart. 
| Out| 2| Out. 
| Arrive| 3| Arrive. 
| Cross| 4| Cross. 
| Crossover| 5| Crossover. 




## CIMMultipatchFeatureTemplate
#### Represents a multipatch feature template. 


### CIMEditingTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| name | string|Gets and sets the name. 
| tags | string|Gets and sets the tags. 
| toolProgID | string|Gets and sets the tool ProgID. 
| toolFilter | IStringArray|Gets and sets the tool filter. 
| toolOptions | [CIMEditingTemplateToolOptions](CIMVectorLayers.md#cimeditingtemplatetooloptions) |Gets and sets the per-tool options. 


### CIMBasicFeatureTemplate  

|Property | Type | Description | 
|---------|--------|--------|
| defaultValues | {JSON_object}|Gets and sets the default values. 
| requiredFields | IStringArray|Gets and sets the required fields. 
| hiddenFields | IStringArray|Gets and sets the hidden fields. 
| relationships | [CIMEditingTemplateRelationship](CIMVectorLayers.md#cimeditingtemplaterelationship) |Gets and sets the template relationships. 


### CIMMultipatchFeatureTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| galleryMode | boolean|Gets and sets a boolean value indicating whether or not this is gallery mode. 
| models | [CIMMultipatchFeatureTemplateModel](CIMVectorLayers.md#cimmultipatchfeaturetemplatemodel) |Gets and sets the models. 






## CIMMultipatchFeatureTemplateModel
#### Represents a multipatch feature template model. 


### CIMMultipatchTemplateModel 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean|Gets and sets a boolean value indicating whether or not this is active. 
| modelURI | string|Gets and sets the model URI. 
| modelSourceURI | string|Gets and sets the model source URI. 
| thumbnailURI | string|Gets and sets the thumbnail URI. 
| camera | [CIMViewCamera](CIMMap.md#cimviewcamera)|Gets and sets the camera. 






## CIMNetCDFRasterDataConnection
#### Represents a NetCDF raster data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMNetCDFRasterDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| bandDimension | string|Gets and sets the band dimension. 
| extent | [Envelope](ExternalReferences.md#envelope)|Gets and sets the extent. 
| invertRows | bool|Gets and sets a boolean value indicating whether or not to invert rows. 
| selectedDimensionIndexes | [long]|Gets and sets the selected dimension indexes. 
| selectedDimensions | IStringArray|Gets and sets the selected dimensions. 
| selectedDimensionValues | ["<string>" / <number> / {JSON_object}]|Gets and sets the selected dimension values. 
| variable | string|Gets and sets the variable. 
| verticalDimension | string|Gets and sets the vertical dimension. 
| verticalDimensionUnit | string|Gets and sets the vertical dimension unit. 
| XDimension | string|Gets and sets the X dimension. 
| YDimension | string|Gets and sets the Y dimension. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 






## CIMNetCDFStandardDataConnection
#### Represents a NetCDF standard data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMNetCDFStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| variableList | IStringArray|Gets and sets the variable list. 
| rowDimensionList | IStringArray|Gets and sets the row dimension list. 
| XDimension | string|Gets and sets the X dimension. 
| YDimension | string|Gets and sets the Y dimension. 
| ZDimension | string|Gets and sets the Z dimension. 
| MDimension | string|Gets and sets the M dimension. 
| selectedDimensions | IStringArray|Gets and sets the selected dimensions. 
| selectedDimensionIndexes | [long]|Gets and sets the selected dimension indexes. 
| selectedDimensionValues | ["<string>" / <number> / {JSON_object}]|Gets and sets the selected dimension values. 
| shapeFieldName | string|Gets and sets the shape field name. 
| verticalDimension | string|Gets and sets the vertical dimension. 
| verticalDimensionUnit | string|Gets and sets the vertical dimension unit. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 






## CIMPageDefinition
#### Represents page definition. 


### CIMPageDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| pageFieldName | string|Show features where the value of this field either matches or doesn't match the current map series page name. Match versus don't match is controlled by ExcludePages. 
| excludePages | boolean|Specify false to show features that match or true to show features that don't match. 






## CIMParcelFabricLayer
#### Represents a parcel fabric layer. 


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


### CIMParcelFabricLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| accuracyTable | string|Gets and sets the path of the accuracy table. 
| allLayers | IStringArray|Gets and sets the paths of the layers in the parcel fabric layer. 
| adjustmentsTable | string|Gets and sets the path of the adjustments table. 
| cadastralFabricConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection to the fabric. 
| controlPointLayer | string|Gets and sets the path of the control point layer. 
| controlPointSelectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the control point selection symbol. 
| jobsTable | string|Gets and sets the path to the jobs table. 
| lineLayer | string|Gets and sets the path to the line layer. 
| linePointLayer | string|Gets and sets the path to the line point layer. 
| lockedParcelSelectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the locked parcel selection symbol. 
| parcelLayer | string|Gets and sets the path to the parcel layer. 
| plansTable | string|Gets and sets the path to the plans table. 
| pointLayer | string|Gets and sets the path to the point layer. 
| unlockedParcelSelectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the unlocked parcel selection symbol. 






## CIMParcelLayer
#### Represents a parcel fabric layer. 


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


### CIMParcelLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| recordsLayer | string|Gets and sets the path to the parcel polygon records layer. The records layer links parcel polygons and lines to the legal record that created / retired it as well as integration point to business systems. 
| dirtyAreaLayer | string|Gets and sets the path to the parcel dirty area layer. A dirty area is an area that has been modified and needs to be validated against the topology rules and parcel rules. Validation may yield error features (points, lines, polygons). 
| pointErrorLayer | string|Gets and sets the path to the parcel point error layer. 
| lineErrorLayer | string|Gets and sets the path to the parcel line error layer. 
| polygonErrorLayer | string|Gets and sets the path to the parcel polygon error layer. 
| parcelConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection to the Parcel Fabric. A Parcel Fabric controls simple feature classes and uses topology rules and parcel rules. Parcel geometry is edited using feature services The Parcel Layer provides additional services to control the fabric classes such as validate. 






## CIMPieChartMediaInfo
#### Represents pie chart media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long|Gets and sets the row. 
| column | long|Gets and sets the column. 
| refreshRate | double|The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media. 


### CIMChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| fields | IStringArray|Gets and sets the fields. 
| normalizeField | string|Gets and sets the normalization field. 
| caption | string|Gets and sets the caption. 
| title | string|Gets and sets the title. 


### CIMPieChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|






## CIMPopupInfo
#### Represents popup info. 


### CIMPopupInfo 

|Property | Type | Description | 
|---------|--------|--------|
| title | string|Gets and sets the title. 
| expressionInfos | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo) |Gets and sets the media infos. 
| mediaInfos | [CIMMediaInfo](Types.md#cimmediainfo) |Gets and sets the media infos. 






## CIMRange
#### Represents a range. 


### CIMRange 

|Property | Type | Description | 
|---------|--------|--------|
| min | double|Gets and sets the min, 
| max | double|Gets and sets the max. 






## CIMRangeDefinition
#### Represents a range definition. 


### CIMRangeDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| fieldName | string|Gets and sets the field name. 
| currentRange | [CIMRange](CIMVectorLayers.md#cimrange)|Gets and sets the current range. 
| customFullExtent | [CIMRange](CIMVectorLayers.md#cimrange)|Gets and sets the custom full extent. 
| isExclusion | boolean|Gets and sets a boolean value indicating whether or not range is exclusion. 
| aliasExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets ExpressionInfo that contains the Arcade expression that returns a string representing range alias value 






## CIMRangeVariable
#### Represents a range variable. 


### CIMBindVariable 

|Property | Type | Description | 
|---------|--------|--------|
| variableName | string|Gets and sets the name of the variable. The name must be unique among all variables. 
| alias | string|Gets and sets the alias of the variable. 
| dataType | [enumeration BindVariableType](CIMVectorLayers.md#enumeration-bindvariabletype)|Gets and sets the type of the variable. 


### CIMRangeVariable 

|Property | Type | Description | 
|---------|--------|--------|
| fieldExpression | string|Gets and sets the field for which the value range will be specified. 
| optional | bool|Gets and sets whether this variable is optional. If not, default values must be provided. 
| defaultMin | VARIANT|Gets and sets the default minimum value. 
| defaultMax | VARIANT|Gets and sets the default maximum value. 
| tableName | string|Gets and sets the name of the table to which the field in FieldExpression belongs. 
| valueIfMissing | bool|Gets and sets the value the resulting expression should take if the variable is optional and no value is passed. 






## CIMRasterTable
#### Represents a raster table. 


### CIMDisplayTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| definitionExpression | string|Gets and sets the definition expression that can subset the rows in the virtual table. 
| displayField | string|Gets and sets the name of the attribute field that will be used as a label that represents each row in the table. The display field must be able to be represented as a string (string or numeric). 
| editable | boolean|Gets and sets a boolean option indicating whether or not the table can be edited. 
| relates | [CIMRelateInfoBase](CIMVectorLayers.md#cimrelateinfobase) |Gets and sets the relates. 
| fieldDescriptions | [CIMFieldDescription](CIMVectorLayers.md#cimfielddescription) |Gets and sets the field descriptions. Field descriptions for fields may only be written if values are overridden from defaults. 
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition)|Gets and sets the time fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|Gets and sets the time definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|Gets and sets the time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition)|Gets and sets the time definition fields. 
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |Gets and sets the range defintions. 
| activeRangeName | string|Gets and sets the active range name. 
| selectRelatedData | boolean|Gets or sets a value indicating if related data should be selected when creating a new selection. 
| bindVariables | [CIMBindVariable](Types.md#cimbindvariable) |Gets and sets the bind variables. 
| subtypeValue | long|Gets and sets the subtype value that should be used in the feature layer definition. This property is honored only when feature layer is a member of SubtypeLayer. 
| useSubtypeValue | boolean|Gets and sets a boolean option indicating whether or not the SubtypeValue should be used. 
| displayExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets the expression information used for coming up with a string that represents a row or a feature. 
| selectionSetURI | string|Gets and sets the URI of the selection set for the table. 


### CIMRasterTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| joins | [DataConnection](Types.md#dataconnection)|Gets and sets the joins as a data connection. 






## CIMRelQueryTableDataConnection
#### Represents a RelQuery table data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMRelQueryTableDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| sourceTable | [DataConnection](Types.md#dataconnection)|Gets and sets the source table data connection. 
| destinationTable | [DataConnection](Types.md#dataconnection)|Gets and sets the destination table. 
| primaryKey | string|Gets and sets the primary key. 
| foreignKey | string|Gets and sets the foreign key. 
| name | string|Gets and sets the name. 
| cardinality | [enumeration esriRelCardinality](ExternalReferences.md#enumeration-esrirelcardinality)|Gets and sets the join cardinality. 
| joinType | [enumeration esriJoinType](ExternalReferences.md#enumeration-esrijointype)|Gets and sets the join type. 
| joinForward | boolean|Gets and sets a boolean value indicating whether or not this is a forward join. 






## CIMRelateInfo
#### Represents relate info. 


### CIMRelateInfo 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the relate data connection. 
| foreignKey | string|Gets and sets the foreign key. 
| primaryKey | string|Gets and sets the primary key. 
| cardinality | [enumeration esriRelCardinality](ExternalReferences.md#enumeration-esrirelcardinality)|Gets and sets the relate cardinality. 
| name | string|Gets and sets the name. 






## CIMRouteEventDataConnection
#### Represents a route event data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMRouteEventDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| routeFeatureClass | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection for the route feature class. 
| routeIDFieldName | string|Gets and sets the route identifier field of the route feature class. 
| routeWhereClause | string|Gets and sets the where clause that limits the routes that events can be located on. 
| routeMeasureUnit | [Unit](ExternalReferences.md#unit)|Gets and sets the route measure units. 
| eventMeasureUnit | [Unit](ExternalReferences.md#unit)|Gets and sets the units of the event measure(s). 
| eventRouteIDFieldName | string|Gets and sets the route identifier field name. 
| isLineEvent | boolean|Gets and sets a boolean value indicating whether or not this is a line event. 
| lateralOffsetFieldName | string|Gets and sets the lateral offset field name. 
| MDirectionOffsetting | boolean|Gets and sets a boolean value indicating if the offset should based on the M direction or the digitized direction. 
| errorFieldName | string|Gets and sets the error field name. 
| addErrorField | boolean|Gets and sets the add error field. 
| fromMeasureFieldName | string|Gets and sets the from measure field name. 
| toMeasureFieldName | string|Gets and sets the to measure field name. 
| addAngleField | boolean|Gets and sets a boolean value indicating if an angle field should be added to the field set. 
| angleFieldName | string|Gets and sets the angle field name. 
| asPointFeature | boolean|Gets and sets a boolean value indicating if the point event shape should be output as a multipoint or a point. 
| complementAngle | boolean|Gets and sets a boolean value indicating if 180 degres should be added to the angle field value. 
| normalAngle | boolean|Gets and sets a boolean value indicating if the angle field should be the normal or the tangent anglea. 
| eventTable | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection for the route events. 






## CIMSqlQueryDataConnection
#### Represents a SQL query data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMSqlQueryDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| sqlQuery | string|Gets and sets the SQL query. 
| srid | string|Gets and sets the SRID of the spatial reference. 
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference)|Gets and sets the spatial reference. 
| OIDFields | string|Gets and sets the OID fields. 
| geometryType | [enumeration esriGeometryType](ExternalReferences.md#enumeration-esrigeometrytype)|Gets and sets the geometry type. 
| extent | [Envelope](ExternalReferences.md#envelope)|Gets and sets the extent. 
| queryFields | [Fields](ExternalReferences.md#fields)|Gets and sets the query fields. 
| spatialStorageType | long|Gets and sets the spatial storage type. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 






## CIMStandaloneTable
#### Represents a standalone table. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| URI | string|Gets and sets the URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string|Gets and sets the source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|Gets and sets the time the definition was last modfied. 
| metadataURI | string|Gets and sets the metadata URI. 
| useSourceMetadata | bool|Gets and sets if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


### CIMStandaloneTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection for the table. 
| description | string|Gets and sets the description. 
| autoGenerateRowTemplates | bool|Gets and sets a boolean option indicating whether to automatically generate row templates from the renderer. 
| rowTemplates | [CIMEditingTemplate](Types.md#cimeditingtemplate) |Gets and sets the row templates. 
| serviceTableID | long|Gets and sets identifier that will be used to identify the layer in server 
| showPopups | boolean|Gets and sets a boolean indicating whether or not to show popups. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo)|Gets and sets the popup info. 
| charts | [CIMChart](CIMLayer.md#cimchart) | 


### CIMDisplayTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| definitionExpression | string|Gets and sets the definition expression that can subset the rows in the virtual table. 
| displayField | string|Gets and sets the name of the attribute field that will be used as a label that represents each row in the table. The display field must be able to be represented as a string (string or numeric). 
| editable | boolean|Gets and sets a boolean option indicating whether or not the table can be edited. 
| relates | [CIMRelateInfoBase](CIMVectorLayers.md#cimrelateinfobase) |Gets and sets the relates. 
| fieldDescriptions | [CIMFieldDescription](CIMVectorLayers.md#cimfielddescription) |Gets and sets the field descriptions. Field descriptions for fields may only be written if values are overridden from defaults. 
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition)|Gets and sets the time fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|Gets and sets the time definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|Gets and sets the time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition)|Gets and sets the time definition fields. 
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |Gets and sets the range defintions. 
| activeRangeName | string|Gets and sets the active range name. 
| selectRelatedData | boolean|Gets or sets a value indicating if related data should be selected when creating a new selection. 
| bindVariables | [CIMBindVariable](Types.md#cimbindvariable) |Gets and sets the bind variables. 
| subtypeValue | long|Gets and sets the subtype value that should be used in the feature layer definition. This property is honored only when feature layer is a member of SubtypeLayer. 
| useSubtypeValue | boolean|Gets and sets a boolean option indicating whether or not the SubtypeValue should be used. 
| displayExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets the expression information used for coming up with a string that represents a row or a feature. 
| selectionSetURI | string|Gets and sets the URI of the selection set for the table. 






## CIMStandardDataConnection
#### Represents a standard data connection, the most common data connection type. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 






## CIMStreamServiceDataConnection
#### Represents a stream service data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMStreamServiceDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| featureExpirationMethod | [enumeration FeatureExpirationMethod](CIMVectorLayers.md#enumeration-featureexpirationmethod)|Gets and sets feature expiration method used at dataset level. 
| maximumFeatureCount | __int64|Gets or sets the maximum number of features that are held in memory before features are discarded. 
| maximumFeatureAge | __int64|Gets or sets the maximum age for each feature before the feature is discarded. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 






## CIMSubtypeGroupLayer
#### Represents a subtype group layer that works with feature classes enabled with subtypes. A subtype layer is a group layer that contains feature layers, each of which represents a subtype in a feature class. 


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


### CIMFeatureLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| autoGenerateFeatureTemplates | boolean|Gets and sets a boolean option indicating whether to automatically generate feature templates from the renderer. 
| extrusion | [CIMFeatureExtrusion](CIMVectorLayers.md#cimfeatureextrusion)|Gets and sets the feature extrusion. 
| featureElevationExpression | string|Gets and sets the feature elevation expression. 
| featureHyperlinks | [CIMFeatureHyperlink](CIMVectorLayers.md#cimfeaturehyperlink) |Gets and sets the feature hyperlinks. 
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable)|Gets and sets the feature table. 
| featureTemplates | [CIMEditingTemplate](Types.md#cimeditingtemplate) |Gets and sets the feature templates. 
| hotlinkField | string|Gets and sets the field containing hotlink URLs. 
| htmlPopupEnabled | boolean|Gets and sets a boolean option indicating whether HTML popups are enabled. 
| htmlPopupFormat | [CIMHtmlPopupFormat](CIMVectorLayers.md#cimhtmlpopupformat)|Gets and sets the HTML popups format. 
| isFlattened | boolean|Gets and sets a boolean option indicating whether the layer is flattened. 
| selectable | boolean|Gets and sets a boolean option indicating whether the layer is selectable. 
| selectionColor | [Color](Types.md#color)|Gets and sets the selection color. 
| selectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the selection symbol. 
| useSelectionSymbol | boolean|Gets and sets a boolean option indicating whether to use the selection symbol. 
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition)|Use current map series page to select features. 
| featureCacheType | [enumeration FeatureCacheType](CIMVectorLayers.md#enumeration-featurecachetype)|Gets and sets the feature cache type. 
| enableDisplayFilters | boolean|Gets and sets a boolean option indicating whether the current set of display filters are honored during drawing. 
| displayFilters | [CIMDisplayFilter](CIMVectorLayers.md#cimdisplayfilter) |Gets and sets the current set of display filters. 
| featureElevationExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets the expression for setting the feature elevation 


### CIMSubtypeGroupLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| subtypeLayers | IStringArray|Gets or sets the layer URI corresponding to each subtype value. 






## CIMSuppressActivity
#### Represents suppress activity. 


### CIMActivity 

|Property | Type | Description | 
|---------|--------|--------|


### CIMSuppressActivity 

|Property | Type | Description | 
|---------|--------|--------|






## CIMSymbolIdentifier
#### Represents a symbol identifier. 


### CIMSymbolIdentifier 

|Property | Type | Description | 
|---------|--------|--------|
| ID | long|Gets and sets the ID which identifies the symbol in the collection. 
| name | string|Gets and sets the name of the symbol in the symbol collection. 
| symbol | [Symbol](Types.md#symbol)|Gets and sets the symbol. 






## CIMSymbolLayerMasking
#### Represents symbol layer masking. 


### CIMSymbolLayerMasking 

|Property | Type | Description | 
|---------|--------|--------|
| symbolLayers | [CIMSymbolLayerIdentifier](CIMLayer.md#cimsymbollayeridentifier) |Gets and sets the symbol layer identifiers 





### Enumeration: SymbolSubstitutionType
#### Symbol substitution types. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No symbol substitution. 
| Color| 1| Substitute color. 
| IndividualSubordinate| 2| Substitute individual symbols in the collection with overrides taking precedence to symbols. 
| IndividualDominant| 3| Substitute individual symbols in the collection with the symbol taking precedence to overrides. 




## CIMTableMediaInfo
#### Represents table media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long|Gets and sets the row. 
| column | long|Gets and sets the column. 
| refreshRate | double|The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media. 


### CIMTableMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| fields | IStringArray|Gets and sets the fields. 






## CIMTableQueryNameDataConnection
#### Represents a table query name data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMTableQueryNameDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| subFields | string|Gets and sets the subfields. 
| tables | string|Gets and sets the tables. 
| whereClause | string|Gets and sets the where clause. 
| primaryKeyFields | string|Gets and sets the primary key fields. 
| copyLocally | boolean|Gets and sets a boolean value indicating whether or not to copy data locally. 
| shapeType | [enumeration esriGeometryType](ExternalReferences.md#enumeration-esrigeometrytype)|Gets and sets the shape type. 
| featureType | [enumeration esriFeatureType](ExternalReferences.md#enumeration-esrifeaturetype)|Gets and sets the feature type. 
| extent | [Envelope](ExternalReferences.md#envelope)|Gets and sets the extent. 
| shapeFieldName | string|Gets and sets the shape field name. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 






## CIMTemporalDataConnection
#### Represents a temporal data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMTemporalDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| timeFieldLocaleID | long|Gets and sets the time field locale ID. 
| timeFieldAmFormat | string|Gets and sets the custom string representation of the AM symbol. 
| timeFieldPmFormat | string|Gets and sets the custom string representation of the PM symbol. 
| cachingMode | [enumeration TemporalFeatureClassCachingMode](CIMVectorLayers.md#enumeration-temporalfeatureclasscachingmode)|Gets and sets the caching mode. 
| startTimeField | string|Gets and sets the start time field. 
| endTimeField | string|Gets and sets the end time field. 
| timeValueFormat | string|Gets and sets the time value format. 
| trackIDField | string|Gets and sets the track ID field. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 





### Enumeration: TemporalFeatureClassCachingMode
#### Temporal feature class caching modes. 

|Property | Value | Description | 
|---------|--------|--------|
| All| 0| All. 
| None| 1| None. 



### Enumeration: TemporalFeatureClassPurgeRule
#### Temporal feature class purge rules. 

|Property | Value | Description | 
|---------|--------|--------|
| KeepLatestPerTrack| 0| Keep latest per track. 
| PurgeOldest| 1| Purge oldest. 




## CIMTextMediaInfo
#### Represents text media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long|Gets and sets the row. 
| column | long|Gets and sets the column. 
| refreshRate | double|The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media. 


### CIMTextMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| text | string|Gets and sets the text. 






## CIMTimeDataDefinition
#### Represents a time data definition. 


### CIMTimeDataDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| useTime | boolean|Gets and sets a boolean indicating whether or not to use time for animation purposes. 
| timeReference | [TimeReference](ExternalReferences.md#timereference)|Gets and sets the time reference. 
| customTimeExtent | [TimeExtent](ExternalReferences.md#timeextent)|Gets and sets the custom time extent. 
| hasLiveData | boolean|Gets and sets a boolean indicating whether or not this dataset has live data. 
| timeExtentCanChange | boolean|The data regularly changes, so the extent needs recalculated. 






## CIMTimeDimensionDefinition
#### Represents a time dimension definition. 


### CIMTimeDimensionDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| timeDimensionName | string|Gets and sets the time dimension name. 
| timeDimensionFormat | string|Gets and sets the time dimension format. 






## CIMTimeDisplayDefinition
#### Represents a time display definition. 


### CIMTimeDisplayDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| cumulative | boolean|Gets and sets a boolean value indicating whether time is cumulative. 
| timeInterval | double|Gets and sets the time interval. 
| timeIntervalUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|Gets and sets the time interval units. 
| timeOffset | double|Gets and sets the time offset. 
| timeOffsetUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|Gets and sets the time offset units. 






## CIMTimeTableDefinition
#### Represents a time table definition. 


### CIMTimeTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| startTimeField | string|Gets and sets the start time field. 
| endTimeField | string|Gets and sets the end time field. 
| timeValueFormat | string|Gets and sets the time value format. 
| trackIDField | string|Gets and sets the track ID field. 






## CIMTrackingServerDataConnection
#### Represents a tracking server data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMTrackingServerDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| autoPurge | boolean|Gets and sets a boolean value indicating whether to automatically purge data. 
| purgeThreshold | long|Gets and sets the purge threshold. 
| purgePercentage | double|Gets and sets the percentage of the maximum allowed number of records to delete when the purge occurs. 
| keepPerTrack | long|Gets and sets the minimum number of features to keep per track. 
| purgeRule | [enumeration TemporalFeatureClassPurgeRule](CIMVectorLayers.md#enumeration-temporalfeatureclasspurgerule)|Gets and sets the purge rule. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 






## CIMVectorTileDataConnection
#### Represents a VectorTile layer data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMVectorTileDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string|Gets and sets the URI of the VectorTile files or resources. 






## CIMVectorTileLayer
#### Represents a VectorTile layer. A VectorTileServiceLayer provides rich cartographic content in a fast and efficient vector tile format. It may have multiple styles and if so users can choose which style to use to display the layer's vector geometries. Logically a VectorTileServiceLayer is more like a basemap layer in that it is typically composed of several distinct data sources (e.g. roads, cities, hydrology, buildings) that can provide context and background but in a way that is typically more performant than raster tile layers. 


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


### CIMVectorTileLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [CIMVectorTileDataConnection](CIMVectorLayers.md#cimvectortiledataconnection)|Gets and sets the data connection to the VectorTile resource. 
| currentStyle | string|Gets and sets the current style the vector tile layer features should be rendered with. 






## CIMWorkspaceConnection
#### Represents a workspace connection. 


### CIMWorkspaceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 





### Enumeration: WorkspaceFactory
#### Workspace factory types. 

|Property | Value | Description | 
|---------|--------|--------|
| SDE| 0| Enterprise geodatabase. 
| FileGDB| 1| File geodatabase. 
| Raster| 2| Raster. 
| Shapefile| 3| Shapefile. 
| OLEDB| 4| OLEDB. 
| Access| 5| Microsoft Access. 
| DelimitedTextFile| 6| Delimited text file. 
| Custom| 7| Custom. 
| Sql| 8| SQL query layer. 
| Tin| 9| TIN. 
| TrackingServer| 10| Tracking server. 
| NetCDF| 11| NetCDF. 
| LASDataset| 12| LAS dataset. 
| SqlLite| 13| SQLite. 
| FeatureService| 14| Feature service. 
| ArcInfo| 15| Arc/INFO Coverage. 
| Cad| 16| CAD. 
| Excel| 17| Microsoft Excel. 
| WFS| 18| Web feature service. 
| StreamService| 19| Stream service 




## CIMXYEventDataConnection
#### Represents an XY event data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMXYEventDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| XFieldName | string|Gets and sets the X field name. 
| YFieldName | string|Gets and sets the Y field name. 
| ZFieldName | string|Gets and sets the Z field name. 
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference)|Gets and sets the spatial reference. 
| XYEventTableDataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection to the table events are created from. 



