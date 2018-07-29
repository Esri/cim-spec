


## CIMAnnotationLayer
Represents an annotation layer used to draw annotation feature classes.


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


### CIMFeatureLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| autoGenerateFeatureTemplates | boolean|A boolean option indicating whether to automatically generate feature templates from the renderer.
| extrusion | [CIMFeatureExtrusion](CIMVectorLayers.md#cimfeatureextrusion)|The feature extrusion.
| featureElevationExpression | string|The feature elevation expression.
| featureHyperlinks | [CIMFeatureHyperlink](CIMVectorLayers.md#cimfeaturehyperlink) |The feature hyperlinks.
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable)|The feature table.
| featureTemplates | [CIMEditingTemplate](Types.md#cimeditingtemplate) |The feature templates.
| hotlinkField | string|The field containing hotlink URLs.
| htmlPopupEnabled | boolean|A boolean option indicating whether HTML popups are enabled.
| htmlPopupFormat | [CIMHtmlPopupFormat](CIMVectorLayers.md#cimhtmlpopupformat)|The HTML popups format.
| isFlattened | boolean|A boolean option indicating whether the layer is flattened.
| selectable | boolean|A boolean option indicating whether the layer is selectable.
| selectionColor | [Color](Types.md#color)|The selection color.
| selectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The selection symbol.
| useSelectionSymbol | boolean|A boolean option indicating whether to use the selection symbol.
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition)|Use current map series page to select features.
| featureCacheType | [enumeration FeatureCacheType](CIMVectorLayers.md#enumeration-featurecachetype)|The feature cache type.
| enableDisplayFilters | boolean|A boolean option indicating whether the current set of display filters are honored during drawing.
| displayFilters | [CIMDisplayFilter](CIMVectorLayers.md#cimdisplayfilter) |The current set of display filters.
| featureElevationExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The expression for setting the feature elevation


### CIMAnnotationLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight)|The weight of features in this layer when considered as barriers to labeling.
| drawGeometry | boolean|A Boolean property designating whether the geometry of the text graphics should be drawn.
| drawUnplacedAnnotation | boolean|A Boolean property designating whether unplaced annotation should be drawn.
| drawGeometryLineSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The line symbol used to draw text graphic line geometries when the DrawGeometry option is true.
| drawGeometryPointSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The point symbol used to draw text graphic line geometries when the DrawGeometry option is true.
| unplacedAnnotationColor | [Color](Types.md#color)|The color that unplaced text graphics will be drawn with when Unplaced Annotation is drawn.
| symbolSubstitutionType | [enumeration SymbolSubstitutionType](CIMVectorLayers.md#enumeration-symbolsubstitutiontype)|The type of symbol substitution this layer uses.
| massColorSubstitute | [Color](Types.md#color)|The mass color substitute. When using the SymbolSubstitutionColor substitution type this is the color that all text graphics will be overridden with.
| inlineColor | [Color](Types.md#color)|The inline color. When using the SymbolSubstitutionIndividualSubordinate or SymbolSubstitutionIndividualDominant substitution types this is the color that all text graphics that are stored inline (bloated) will be overridden with.
| substitutionSymbolCollection | [CIMSymbolIdentifier](CIMVectorLayers.md#cimsymbolidentifier) |A symbol substitution collection. When using the SymbolSubstitutionIndividualSubordinate or SymbolSubstitutionIndividualDominant substitution types this collection defines which symbols in the symbol collection are substituted and what their substitute values are. The symbol substitution properties allow the users to swap out symbols/colors of annotation stored in the geodatabase at the layer level. This allows annotation to be repurposed in maps without duplicating the annotation. The classic case for this behavior is when a user wishes to utilize black text generated for standard parcel maps on top of a map with raster imagery. By substituting the color or symbol collection of the annotation the user is allowed to change the appearance for this one map without a large performance or data management overhead. One complex aspect of symbol substitution is how overrides are treated when it is enabled. When this feature was originally added some wanted overrides to be respected and others did not, so options were added for this (dominant and subordinate substitution types). When the dominant type is chosen overrides are ignored. When the subordinate type is chosen overrides are applied on top of the new symbols.
| subLayers | [CIMAnnotationSubLayer](CIMVectorLayers.md#cimannotationsublayer) |A collection of AnnotationSubLayers, corresponding to the annotation subclasses defined by the annotation feature class.






## CIMAnnotationSubLayer
Represents an annotation sublayer used to draw annotation feature classes subclasses.


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


### CIMAnnotationSubLayer

|Property | Type | Description |
|---------|--------|--------|





### Enumeration: AttachmentDisplayType
Attachment display types.

|Property | Value | Description |
|---------|--------|--------|
| PreviewFirst| 0| Preview first.
| PreviewAll| 1| Preview all.
| List| 2| List.




## CIMAttachmentsMediaInfo
Represents attachment media info.


### CIMMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| row | number //int32|The row.
| column | number //int32|The column.
| refreshRate | number //double|The amount of time in RefreshRateUnit to wait between refreshing the media info.
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media.


### CIMAttachmentMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| caption | string|The caption.
| title | string|The title.
| contentType | string|The content MIME type. Example: (image/png, image/jpeg, audio/mp3
| displayType | [enumeration AttachmentDisplayType](CIMVectorLayers.md#enumeration-attachmentdisplaytype)|The display type.






## CIMAttributeCondition
Represents an attribute condition.


### CIMCondition

|Property | Type | Description |
|---------|--------|--------|


### CIMAttributeCondition

|Property | Type | Description |
|---------|--------|--------|
| whereClause | string|The where clause.






## CIMBarChartMediaInfo
Represents bar chart media info.


### CIMMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| row | number //int32|The row.
| column | number //int32|The column.
| refreshRate | number //double|The amount of time in RefreshRateUnit to wait between refreshing the media info.
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media.


### CIMChartMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| fields | [string,]|The fields.
| normalizeField | string|The normalization field.
| caption | string|The caption.
| title | string|The title.


### CIMBarChartMediaInfo

|Property | Type | Description |
|---------|--------|--------|





### Enumeration: BarrierWeight
Barrier weights.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| No weight.
| Low| 1| Low weight.
| Medium| 2| Medium weight.
| High| 3| High weight.



### Enumeration: BindVariableType
Bind variable types.

|Property | Value | Description |
|---------|--------|--------|
| String| 0| String variable type.
| Integer| 1| Integer variable type.
| number //double| 2| Double variable type.
| Date| 3| Date variable type.




## CIMColumnChartMediaInfo
Represents column chart media info.


### CIMMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| row | number //int32|The row.
| column | number //int32|The column.
| refreshRate | number //double|The amount of time in RefreshRateUnit to wait between refreshing the media info.
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media.


### CIMChartMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| fields | [string,]|The fields.
| normalizeField | string|The normalization field.
| caption | string|The caption.
| title | string|The title.


### CIMColumnChartMediaInfo

|Property | Type | Description |
|---------|--------|--------|





### Enumeration: DataSearchMode
Field search modes.

|Property | Value | Description |
|---------|--------|--------|
| Contains| 0| Search for values that contain the search text.
| Exact| 1| Search for values that are the exact match with the search text.




## CIMDimensionLayer
Represents an dimension layer used to draw dimension feature classes.


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


### CIMFeatureLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| autoGenerateFeatureTemplates | boolean|A boolean option indicating whether to automatically generate feature templates from the renderer.
| extrusion | [CIMFeatureExtrusion](CIMVectorLayers.md#cimfeatureextrusion)|The feature extrusion.
| featureElevationExpression | string|The feature elevation expression.
| featureHyperlinks | [CIMFeatureHyperlink](CIMVectorLayers.md#cimfeaturehyperlink) |The feature hyperlinks.
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable)|The feature table.
| featureTemplates | [CIMEditingTemplate](Types.md#cimeditingtemplate) |The feature templates.
| hotlinkField | string|The field containing hotlink URLs.
| htmlPopupEnabled | boolean|A boolean option indicating whether HTML popups are enabled.
| htmlPopupFormat | [CIMHtmlPopupFormat](CIMVectorLayers.md#cimhtmlpopupformat)|The HTML popups format.
| isFlattened | boolean|A boolean option indicating whether the layer is flattened.
| selectable | boolean|A boolean option indicating whether the layer is selectable.
| selectionColor | [Color](Types.md#color)|The selection color.
| selectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The selection symbol.
| useSelectionSymbol | boolean|A boolean option indicating whether to use the selection symbol.
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition)|Use current map series page to select features.
| featureCacheType | [enumeration FeatureCacheType](CIMVectorLayers.md#enumeration-featurecachetype)|The feature cache type.
| enableDisplayFilters | boolean|A boolean option indicating whether the current set of display filters are honored during drawing.
| displayFilters | [CIMDisplayFilter](CIMVectorLayers.md#cimdisplayfilter) |The current set of display filters.
| featureElevationExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The expression for setting the feature elevation


### CIMDimensionLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight)|The weight of features in this layer when considered as barriers to labeling.





### Enumeration: DimensionMarkerFit
Dimension marker fit options.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| Do not fit markers with text.
| Tolerance| 1| Fit markers with text using the length of the dimension line.
| Text| 2| Fit markers when overlapping the text.



### Enumeration: DimensionPartOptions
Dimension part options.

|Property | Value | Description |
|---------|--------|--------|
| Begin| 0| Only display the beginning dimension part.
| End| 1| Only display the end dimension part.
| None| 2| Do not display any dimension parts.
| Both| 3| Display both dimension parts.




## CIMDimensionStyle
Represents an dimension style which defines dimension appearance.


### CIMDimensionStyle

|Property | Type | Description |
|---------|--------|--------|
| align | boolean|A boolean property which indicates if the text should be aligned with the dimension line.
| baselineHeight | number //double|The height of the construction for creating baseline dimensions with this style.
| beginMarkerSymbol | [CIMPointSymbol](CIMSymbols.md#cimpointsymbol)|The symbol used for the begin arrow.
| convertUnits | boolean|A boolean property which indicates if the length of the dimension needs to be converted for display.
| dimensionLineOption | [enumeration DimensionPartOptions](CIMVectorLayers.md#enumeration-dimensionpartoptions)|The dimension line display of the style.
| dimensionLineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol)|The symbol used for the dimension line.
| displayPrecision | number //int32|The precision for the value displayed by the dimension text.
| displayUnits | [Unit](ExternalReferences.md#unit)|The units the length of the dimension text is displayed in.
| drawLineOnFit | boolean|A boolean value which indicates if a dimension line should be drawn between the extension lines for an inward dimension.
| endMarkerSymbol | [CIMPointSymbol](CIMSymbols.md#cimpointsymbol)|The symbol used for the end arrow.
| expression | string|The text expression for the style.
| expressionParserName | string|The text expression parser for the text expression for the style.
| extendLineOnFit | boolean|A boolean property which indicates if the dimension line will be extended to underline the text on inward dimensions.
| extensionLineOffset | number //double|The length of the extension line offset.
| extensionLineOption | [enumeration DimensionPartOptions](CIMVectorLayers.md#enumeration-dimensionpartoptions)|The extension line display options of the style.
| extensionLineOvershot | number //double|The length of the extension line overshot.
| extensionLineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol)|The symbol used for extension lines.
| ID | number //int32|The ID of the style.
| markerFit | [enumeration DimensionMarkerFit](CIMVectorLayers.md#enumeration-dimensionmarkerfit)|The arrow fit policy of the style.
| markerFitTolerance | number //double|The arrow fit tolerance of the style.
| markerOption | [enumeration DimensionPartOptions](CIMVectorLayers.md#enumeration-dimensionpartoptions)|The arrow display properties of the style.
| name | string|The name of the style.
| prefix | string|The prefix for the text expression for the style.
| suffix | string|The suffix for the text expression for the style.
| textFit | [enumeration DimensionTextFit](CIMVectorLayers.md#enumeration-dimensiontextfit)|The text fit policy for the style.
| textOption | [enumeration DimensionTextOption](CIMVectorLayers.md#enumeration-dimensiontextoption)|The text display option for the style.
| textSymbol | [CIMTextSymbol](CIMSymbols.md#cimtextsymbol)|The text symbol used for the text.





### Enumeration: DimensionTextFit
Dimension text fit options.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| Do not fit the text.
| MoveBegin| 1| Move the text outside the begin extension line.
| MoveEnd| 2| Move the text outside the end extension line.



### Enumeration: DimensionTextOption
Dimension text options.

|Property | Value | Description |
|---------|--------|--------|
| Only| 0| Only display the value of the dimension length.
| Suffix| 1| Display the value of the dimension length with a prefix and suffix.
| Expression| 2| Display a text string derived from a custom expression.
| None| 3| Do not display any text.




## CIMDiscreteVariable
Represents a single bind variable.


### CIMBindVariable

|Property | Type | Description |
|---------|--------|--------|
| variableName | string|The name of the variable. The name must be unique among all variables.
| alias | string|The alias of the variable.
| dataType | [enumeration BindVariableType](CIMVectorLayers.md#enumeration-bindvariabletype)|The type of the variable.


### CIMDiscreteVariable

|Property | Type | Description |
|---------|--------|--------|
| defaultValue | ["<string>" / <number> / Object]|The variable's required default value. The array can have multiple values only if AllowMultiple is true.
| boundValue | ["<string>" / <number> / Object]|The variable's currently-bound value. The array can have multiple values only if AllowMultiple is true.
| allowMultiple | boolean|A boolean indicating whether the variable will accept an array of values.






## CIMDisplayFilter
Represents a display filter used to restrict the display of features across scale ranges.


### CIMDisplayFilter

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name of the display filter.
| whereClause | string|The where clause that filters features for a given scale range.
| minScale | number //double|The minimum scale for this display filter.
| maxScale | number //double|The maximum scale for this display filter.






## CIMEditingTemplateRelationship
Represents an editing template relationship.


### CIMEditingTemplateRelationship

|Property | Type | Description |
|---------|--------|--------|
| tableURI | string|The table URI of the table the relationship corresponds to.
| name | string|The name.
| relationshipID | number //int32|The relationship ID.






## CIMEditingTemplateToolOptions
####


### CIMEditingTemplateToolOptions

|Property | Type | Description |
|---------|--------|--------|
| toolProgID | string|The tool ProgID.
| options | Object|The options for the specified creation tool.





### Enumeration: FeatureCacheType
Feature cache type options.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| No cache.
| Session| 1| Cache is maintained in session.




## CIMFeatureDatasetDataConnection
Represents a feature dataset data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


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





### Enumeration: FeatureExpirationMethod
Stream service feature expiration method.

|Property | Value | Description |
|---------|--------|--------|
| MaximumFeatureCount| 0| The oldest features will expire after a threshold number of features has been reached.
| MaximumFeatureAge| 1| Features will expire after the specified time since the beginning of their lifetime.




## CIMFeatureExtrusion
Represents feature extrusion.


### CIMFeatureExtrusion

|Property | Type | Description |
|---------|--------|--------|
| extrusionType | [enumeration ExtrusionType](CIMEnumerations.md#enumeration-extrusiontype)|The extrusion type.
| extrusionExpression | string|The extrusion expression.
| extrusionUnit | [LinearUnit](ExternalReferences.md#linearunit)|The feature layer's extrusion unit.
| extrusionExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The ExpressionInfo that contains Arcade expresion that returns a numeric value.






## CIMFeatureHyperlink
Represents feature hyperlink.


### CIMFeatureHyperlink

|Property | Type | Description |
|---------|--------|--------|
| featureID | number //int32|The feature ID.
| link | string|The link URL.






## CIMFeatureLayer
Represents feature layer used to draw data from feature classes. A feature layer displays a set of geographic features. A geographic feature represents a real-world object on the earth. It has a spatially- referenced location, stored as a point, line, or polygon, and a set of attributes that describe the feature. Its position is accurate and relevant within a particular scale range. Geographic features are the core spatial data holdings of an organization. They can serve as official records, are used in spatial analysis, and are used as source data for cartography. Feature layers draw their features by using a feature renderer to transform the geographic feature into one or more graphic entities. Feature renderers read the feature's geometry and attribute values to generate graphic entities that graphically depict the feature on a map.


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


### CIMFeatureLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| autoGenerateFeatureTemplates | boolean|A boolean option indicating whether to automatically generate feature templates from the renderer.
| extrusion | [CIMFeatureExtrusion](CIMVectorLayers.md#cimfeatureextrusion)|The feature extrusion.
| featureElevationExpression | string|The feature elevation expression.
| featureHyperlinks | [CIMFeatureHyperlink](CIMVectorLayers.md#cimfeaturehyperlink) |The feature hyperlinks.
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable)|The feature table.
| featureTemplates | [CIMEditingTemplate](Types.md#cimeditingtemplate) |The feature templates.
| hotlinkField | string|The field containing hotlink URLs.
| htmlPopupEnabled | boolean|A boolean option indicating whether HTML popups are enabled.
| htmlPopupFormat | [CIMHtmlPopupFormat](CIMVectorLayers.md#cimhtmlpopupformat)|The HTML popups format.
| isFlattened | boolean|A boolean option indicating whether the layer is flattened.
| selectable | boolean|A boolean option indicating whether the layer is selectable.
| selectionColor | [Color](Types.md#color)|The selection color.
| selectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The selection symbol.
| useSelectionSymbol | boolean|A boolean option indicating whether to use the selection symbol.
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition)|Use current map series page to select features.
| featureCacheType | [enumeration FeatureCacheType](CIMVectorLayers.md#enumeration-featurecachetype)|The feature cache type.
| enableDisplayFilters | boolean|A boolean option indicating whether the current set of display filters are honored during drawing.
| displayFilters | [CIMDisplayFilter](CIMVectorLayers.md#cimdisplayfilter) |The current set of display filters.
| featureElevationExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The expression for setting the feature elevation


### CIMGeoFeatureLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| actions | [CIMLayerAction](CIMVectorLayers.md#cimlayeraction) |The layer actions.
| exclusionSet | [number], //[int64],|The set of excluded features.
| featureMasks | [CIMDataConnection](Types.md#cimdataconnection) |The data connection os the masking data.
| labelClasses | [CIMLabelClass](CIMLabelPlacement.md#cimlabelclass) |The collection of label class definitions.
| labelVisibility | boolean|A boolean option indicating whether to display labels for this layer's label classes.
| maskedSymbolLayers | [CIMSymbolLayerMasking](CIMVectorLayers.md#cimsymbollayermasking) |The masked symbol layers. Each SymbolLayerMasking gives the symbol layers that are masked by that masking layer.
| mostCurrentRenderer | [Renderer](Types.md#renderer)|The renderer used for the most current features when displaying tracks.
| renderer | [Renderer](Types.md#renderer)|The primary symbol renderer.
| scaleSymbols | boolean|A boolean option indicating whether to scale the symbols in this layer based on the map's reference scale.
| snappable | boolean|A boolean option indicating whether this layer participates in snapping in the editor.
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing)|The symbol layer drawing properties.
| trackLinesRenderer | [Renderer](Types.md#renderer)|The track renderer when displaying tracks.
| useRealWorldSymbolSizes | boolean|A boolean option indicating whether to use real world symbols sizes (meters) vs. points.






## CIMFeatureTable
Represents a feature table.


### CIMDisplayTableDefinition

|Property | Type | Description |
|---------|--------|--------|
| definitionExpression | string|The definition expression that can subset the rows in the virtual table.
| displayField | string|The name of the attribute field that will be used as a label that represents each row in the table. The display field must be able to be represented as a string (string or numeric).
| editable | boolean|A boolean option indicating whether or not the table can be edited.
| relates | [CIMRelateInfoBase](CIMVectorLayers.md#cimrelateinfobase) |The relates.
| fieldDescriptions | [CIMFieldDescription](CIMVectorLayers.md#cimfielddescription) |The field descriptions. Field descriptions for fields may only be written if values are overridden from defaults.
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition)|The time fields.
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|The time definition.
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|The time display definition.
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition)|The time definition fields.
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |The range defintions.
| activeRangeName | string|The active range name.
| selectRelatedData | boolean|A value indicating if related data should be selected when creating a new selection.
| bindVariables | [CIMBindVariable](Types.md#cimbindvariable) |The bind variables.
| subtypeValue | number //int32|The subtype value that should be used in the feature layer definition. This property is honored only when feature layer is a member of SubtypeLayer.
| useSubtypeValue | boolean|A boolean option indicating whether or not the SubtypeValue should be used.
| displayExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The expression information used for coming up with a string that represents a row or a feature.
| selectionSetURI | string|The URI of the selection set for the table.


### CIMFeatureTableDefinition

|Property | Type | Description |
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|The data connection.
| studyArea | [Area](ExternalReferences.md#area)|An area that can be used to subset the rows in the virtual table.
| studyAreaSpatialRel | [enumeration esriSpatialRelEnum](ExternalReferences.md#enumeration-esrispatialrelenum)|The study area spatial relationship.
| searchOrder | [enumeration esriSearchOrder](ExternalReferences.md#enumeration-esrisearchorder)|The search order option.
| isLicensedDataSource | boolean|A boolean option indicating whether the data source is licensed.
| definitionSetURI | string|The DefinitionSet for the table.






## CIMFeatureTemplate
Represents a feature template.


### CIMEditingTemplate

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| name | string|The name.
| tags | string|The tags.
| toolProgID | string|The tool ProgID.
| toolFilter | [string,]|The tool filter.
| toolOptions | [CIMEditingTemplateToolOptions](CIMVectorLayers.md#cimeditingtemplatetooloptions) |The per-tool options.


### CIMBasicFeatureTemplate  

|Property | Type | Description |
|---------|--------|--------|
| defaultValues | Object|The default values.
| requiredFields | [string,]|The required fields.
| hiddenFields | [string,]|The hidden fields.
| relationships | [CIMEditingTemplateRelationship](CIMVectorLayers.md#cimeditingtemplaterelationship) |The template relationships.


### CIMFeatureTemplate

|Property | Type | Description |
|---------|--------|--------|






## CIMFieldDescription
Represents a field description.


### CIMFieldDescription

|Property | Type | Description |
|---------|--------|--------|
| alias | string|The field alias.
| fieldName | string|The field name.
| highlight | boolean|A boolean option indicating whether the field is highlighted.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format.
| readOnly | boolean|A boolean option indicating whether the field is read only.
| visible | boolean|A boolean option indicating whether the field is visible.
| valueAsRatio | boolean|A boolean option indicating whether the field value is a ratio (used only by geoprocessing).
| searchable | boolean|A boolean indicating whether the values from this field should be included in the search.
| searchMode | [enumeration DataSearchMode](CIMVectorLayers.md#enumeration-datasearchmode)|The search mode to use when searching for values in this field.






## CIMFolderConnection
Represents a folder connection.


### CIMFolderConnection

|Property | Type | Description |
|---------|--------|--------|
| folderConnectionString | string|The folder connection string.
| alias | string|The connection alias.






## CIMGeometryLocationCondition
Represents geometry location condition.


### CIMCondition

|Property | Type | Description |
|---------|--------|--------|


### CIMLocationCondition

|Property | Type | Description |
|---------|--------|--------|
| conditionType | [enumeration LocationConditionType](CIMVectorLayers.md#enumeration-locationconditiontype)|The location condition type.


### CIMGeometryLocationCondition

|Property | Type | Description |
|---------|--------|--------|
| geometries | [GeometryArray](ExternalReferences.md#geometryarray)|The geometries.






## CIMGroupEditingTemplate
Represents a group editing template.


### CIMEditingTemplate

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| name | string|The name.
| tags | string|The tags.
| toolProgID | string|The tool ProgID.
| toolFilter | [string,]|The tool filter.
| toolOptions | [CIMEditingTemplateToolOptions](CIMVectorLayers.md#cimeditingtemplatetooloptions) |The per-tool options.


### CIMGroupEditingTemplate

|Property | Type | Description |
|---------|--------|--------|
| baseName | string|The base name.
| basePart | [CIMGroupEditingTemplatePart](CIMVectorLayers.md#cimgroupeditingtemplatepart)|The base part.
| parts | [CIMGroupEditingTemplatePart](CIMVectorLayers.md#cimgroupeditingtemplatepart) |The parts.






## CIMGroupEditingTemplatePart
Represents a group editing template part.


### CIMGroupEditingTemplatePart

|Property | Type | Description |
|---------|--------|--------|
| layerURI | string|The URI of the layer this template is defined for.
| name | string|The name.
| transformationID | string|The transformation ID.
| options | Object|The options.






## CIMHighlightActivity
Represents a highlight activity.


### CIMActivity

|Property | Type | Description |
|---------|--------|--------|


### CIMHighlightActivity

|Property | Type | Description |
|---------|--------|--------|
| highlightSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The highlight symbol.






## CIMHtmlPopupFormat
Represents an HTML popup format.


### CIMHtmlPopupFormat

|Property | Type | Description |
|---------|--------|--------|
| htmlRedirectField | string|The redirect field.
| htmlRedirectFieldPrefix | string|The redirect field prefix.
| htmlRedirectFieldSuffix | string|The redirect field suffix.
| htmlXSLStyleSheet | string|The XSL style sheet.
| htmlHideFieldNameColumn | boolean|A boolean value indicating whether of not to hide the field name column.
| htmlUseCodedDomainValues | boolean|A boolean value indicating whether of not to use coded domain values.
| htmlPresentationStyle | [enumeration HtmlPopupStyle](CIMVectorLayers.md#enumeration-htmlpopupstyle)|The presentation style.





### Enumeration: HtmlPopupStyle
HTML popup styles.

|Property | Value | Description |
|---------|--------|--------|
| TwoColumnTable| 0| A two column table.
| RedirectedHTML| 1| Redirected HTML.
| XSLStyleSheet| 2| An XSL style sheet.




## CIMImageMediaInfo
Represents image media info.


### CIMMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| row | number //int32|The row.
| column | number //int32|The column.
| refreshRate | number //double|The amount of time in RefreshRateUnit to wait between refreshing the media info.
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media.


### CIMImageMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| sourceURL | string|The source URL.
| linkURL | string|The link URL.
| caption | string|The caption.
| title | string|The title.






## CIMLayerAction
Represents a layer action


### CIMLayerAction

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| activities | [CIMActivity](Types.md#cimactivity) |The activities.
| conditions | [CIMCondition](Types.md#cimcondition) |The conditions.






## CIMLayerRange
Represents a layer range.


### CIMLayerRange

|Property | Type | Description |
|---------|--------|--------|
| layerURI | string|The URI of the layer this range is defined for.
| rangeName | string|The range name.
| currentRange | [CIMRange](CIMVectorLayers.md#cimrange)|The current range.
| isExclusion | boolean|A boolean value indicating whether or not this is an exclusion range.






## CIMLineChartMediaInfo
Represents line chart media info.


### CIMMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| row | number //int32|The row.
| column | number //int32|The column.
| refreshRate | number //double|The amount of time in RefreshRateUnit to wait between refreshing the media info.
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media.


### CIMChartMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| fields | [string,]|The fields.
| normalizeField | string|The normalization field.
| caption | string|The caption.
| title | string|The title.


### CIMLineChartMediaInfo

|Property | Type | Description |
|---------|--------|--------|





### Enumeration: LocationConditionType
Location condition types.

|Property | Value | Description |
|---------|--------|--------|
| In| 0| In.
| Depart| 1| Depart.
| Out| 2| Out.
| Arrive| 3| Arrive.
| Cross| 4| Cross.
| Crossover| 5| Crossover.




## CIMMultipatchFeatureTemplate
Represents a multipatch feature template.


### CIMEditingTemplate

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| name | string|The name.
| tags | string|The tags.
| toolProgID | string|The tool ProgID.
| toolFilter | [string,]|The tool filter.
| toolOptions | [CIMEditingTemplateToolOptions](CIMVectorLayers.md#cimeditingtemplatetooloptions) |The per-tool options.


### CIMBasicFeatureTemplate  

|Property | Type | Description |
|---------|--------|--------|
| defaultValues | Object|The default values.
| requiredFields | [string,]|The required fields.
| hiddenFields | [string,]|The hidden fields.
| relationships | [CIMEditingTemplateRelationship](CIMVectorLayers.md#cimeditingtemplaterelationship) |The template relationships.


### CIMMultipatchFeatureTemplate

|Property | Type | Description |
|---------|--------|--------|
| galleryMode | boolean|A boolean value indicating whether or not this is gallery mode.
| models | [CIMMultipatchFeatureTemplateModel](CIMVectorLayers.md#cimmultipatchfeaturetemplatemodel) |The models.






## CIMMultipatchFeatureTemplateModel
Represents a multipatch feature template model.


### CIMMultipatchTemplateModel

|Property | Type | Description |
|---------|--------|--------|
| isActive | boolean|A boolean value indicating whether or not this is active.
| modelURI | string|The model URI.
| modelSourceURI | string|The model source URI.
| thumbnailURI | string|The thumbnail URI.
| camera | [CIMViewCamera](CIMMap.md#cimviewcamera)|The camera.






## CIMNetCDFRasterDataConnection
Represents a NetCDF raster data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMNetCDFRasterDataConnection

|Property | Type | Description |
|---------|--------|--------|
| bandDimension | string|The band dimension.
| extent | [Envelope](ExternalReferences.md#envelope)|The extent.
| invertRows | boolean|A boolean value indicating whether or not to invert rows.
| selectedDimensionIndexes | [long]|The selected dimension indexes.
| selectedDimensions | [string,]|The selected dimensions.
| selectedDimensionValues | ["<string>" / <number> / Object]|The selected dimension values.
| variable | string|The variable.
| verticalDimension | string|The vertical dimension.
| verticalDimensionUnit | string|The vertical dimension unit.
| XDimension | string|The X dimension.
| YDimension | string|The Y dimension.


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.






## CIMNetCDFStandardDataConnection
Represents a NetCDF standard data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMNetCDFStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| variableList | [string,]|The variable list.
| rowDimensionList | [string,]|The row dimension list.
| XDimension | string|The X dimension.
| YDimension | string|The Y dimension.
| ZDimension | string|The Z dimension.
| MDimension | string|The M dimension.
| selectedDimensions | [string,]|The selected dimensions.
| selectedDimensionIndexes | [long]|The selected dimension indexes.
| selectedDimensionValues | ["<string>" / <number> / Object]|The selected dimension values.
| shapeFieldName | string|The shape field name.
| verticalDimension | string|The vertical dimension.
| verticalDimensionUnit | string|The vertical dimension unit.


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.






## CIMPageDefinition
Represents page definition.


### CIMPageDefinition

|Property | Type | Description |
|---------|--------|--------|
| pageFieldName | string|Show features where the value of this field either matches or doesn't match the current map series page name. Match versus don't match is controlled by ExcludePages.
| excludePages | boolean|Specify false to show features that match or true to show features that don't match.






## CIMParcelFabricLayer
Represents a parcel fabric layer.


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


### CIMParcelFabricLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| accuracyTable | string|The path of the accuracy table.
| allLayers | [string,]|The paths of the layers in the parcel fabric layer.
| adjustmentsTable | string|The path of the adjustments table.
| cadastralFabricConnection | [DataConnection](Types.md#dataconnection)|The data connection to the fabric.
| controlPointLayer | string|The path of the control point layer.
| controlPointSelectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The control point selection symbol.
| jobsTable | string|The path to the jobs table.
| lineLayer | string|The path to the line layer.
| linePointLayer | string|The path to the line point layer.
| lockedParcelSelectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The locked parcel selection symbol.
| parcelLayer | string|The path to the parcel layer.
| plansTable | string|The path to the plans table.
| pointLayer | string|The path to the point layer.
| unlockedParcelSelectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The unlocked parcel selection symbol.






## CIMParcelLayer
Represents a parcel fabric layer.


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


### CIMParcelLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| recordsLayer | string|The path to the parcel polygon records layer. The records layer links parcel polygons and lines to the legal record that created / retired it as well as integration point to business systems.
| dirtyAreaLayer | string|The path to the parcel dirty area layer. A dirty area is an area that has been modified and needs to be validated against the topology rules and parcel rules. Validation may yield error features (points, lines, polygons).
| pointErrorLayer | string|The path to the parcel point error layer.
| lineErrorLayer | string|The path to the parcel line error layer.
| polygonErrorLayer | string|The path to the parcel polygon error layer.
| parcelConnection | [DataConnection](Types.md#dataconnection)|The data connection to the Parcel Fabric. A Parcel Fabric controls simple feature classes and uses topology rules and parcel rules. Parcel geometry is edited using feature services The Parcel Layer provides additional services to control the fabric classes such as validate.






## CIMPieChartMediaInfo
Represents pie chart media info.


### CIMMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| row | number //int32|The row.
| column | number //int32|The column.
| refreshRate | number //double|The amount of time in RefreshRateUnit to wait between refreshing the media info.
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media.


### CIMChartMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| fields | [string,]|The fields.
| normalizeField | string|The normalization field.
| caption | string|The caption.
| title | string|The title.


### CIMPieChartMediaInfo

|Property | Type | Description |
|---------|--------|--------|






## CIMPopupInfo
Represents popup info.


### CIMPopupInfo

|Property | Type | Description |
|---------|--------|--------|
| title | string|The title.
| expressionInfos | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo) |The media infos.
| mediaInfos | [CIMMediaInfo](Types.md#cimmediainfo) |The media infos.






## CIMRange
Represents a range.


### CIMRange

|Property | Type | Description |
|---------|--------|--------|
| min | number //double|The min,
| max | number //double|The max.






## CIMRangeDefinition
Represents a range definition.


### CIMRangeDefinition

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| fieldName | string|The field name.
| currentRange | [CIMRange](CIMVectorLayers.md#cimrange)|The current range.
| customFullExtent | [CIMRange](CIMVectorLayers.md#cimrange)|The custom full extent.
| isExclusion | boolean|A boolean value indicating whether or not range is exclusion.
| aliasExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The ExpressionInfo that contains the Arcade expression that returns a string representing range alias value






## CIMRangeVariable
Represents a range variable.


### CIMBindVariable

|Property | Type | Description |
|---------|--------|--------|
| variableName | string|The name of the variable. The name must be unique among all variables.
| alias | string|The alias of the variable.
| dataType | [enumeration BindVariableType](CIMVectorLayers.md#enumeration-bindvariabletype)|The type of the variable.


### CIMRangeVariable

|Property | Type | Description |
|---------|--------|--------|
| fieldExpression | string|The field for which the value range will be specified.
| optional | boolean|A boolean indicating whether this variable is optional. If not, default values must be provided.
| defaultMin | VARIANT|The default minimum value.
| defaultMax | VARIANT|The default maximum value.
| tableName | string|The name of the table to which the field in FieldExpression belongs.
| valueIfMissing | boolean|The value the resulting expression should take if the variable is optional and no value is passed.






## CIMRasterTable
Represents a raster table.


### CIMDisplayTableDefinition

|Property | Type | Description |
|---------|--------|--------|
| definitionExpression | string|The definition expression that can subset the rows in the virtual table.
| displayField | string|The name of the attribute field that will be used as a label that represents each row in the table. The display field must be able to be represented as a string (string or numeric).
| editable | boolean|A boolean option indicating whether or not the table can be edited.
| relates | [CIMRelateInfoBase](CIMVectorLayers.md#cimrelateinfobase) |The relates.
| fieldDescriptions | [CIMFieldDescription](CIMVectorLayers.md#cimfielddescription) |The field descriptions. Field descriptions for fields may only be written if values are overridden from defaults.
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition)|The time fields.
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|The time definition.
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|The time display definition.
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition)|The time definition fields.
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |The range defintions.
| activeRangeName | string|The active range name.
| selectRelatedData | boolean|A value indicating if related data should be selected when creating a new selection.
| bindVariables | [CIMBindVariable](Types.md#cimbindvariable) |The bind variables.
| subtypeValue | number //int32|The subtype value that should be used in the feature layer definition. This property is honored only when feature layer is a member of SubtypeLayer.
| useSubtypeValue | boolean|A boolean option indicating whether or not the SubtypeValue should be used.
| displayExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The expression information used for coming up with a string that represents a row or a feature.
| selectionSetURI | string|The URI of the selection set for the table.


### CIMRasterTableDefinition

|Property | Type | Description |
|---------|--------|--------|
| joins | [DataConnection](Types.md#dataconnection)|The joins as a data connection.






## CIMRelQueryTableDataConnection
Represents a RelQuery table data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMRelQueryTableDataConnection

|Property | Type | Description |
|---------|--------|--------|
| sourceTable | [DataConnection](Types.md#dataconnection)|The source table data connection.
| destinationTable | [DataConnection](Types.md#dataconnection)|The destination table.
| primaryKey | string|The primary key.
| foreignKey | string|The foreign key.
| name | string|The name.
| cardinality | [enumeration esriRelCardinality](ExternalReferences.md#enumeration-esrirelcardinality)|The join cardinality.
| joinType | [enumeration esriJoinType](ExternalReferences.md#enumeration-esrijointype)|The join type.
| joinForward | boolean|A boolean value indicating whether or not this is a forward join.






## CIMRelateInfo
Represents relate info.


### CIMRelateInfo

|Property | Type | Description |
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|The relate data connection.
| foreignKey | string|The foreign key.
| primaryKey | string|The primary key.
| cardinality | [enumeration esriRelCardinality](ExternalReferences.md#enumeration-esrirelcardinality)|The relate cardinality.
| name | string|The name.






## CIMRouteEventDataConnection
Represents a route event data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMRouteEventDataConnection

|Property | Type | Description |
|---------|--------|--------|
| routeFeatureClass | [DataConnection](Types.md#dataconnection)|The data connection for the route feature class.
| routeIDFieldName | string|The route identifier field of the route feature class.
| routeWhereClause | string|The where clause that limits the routes that events can be located on.
| routeMeasureUnit | [Unit](ExternalReferences.md#unit)|The route measure units.
| eventMeasureUnit | [Unit](ExternalReferences.md#unit)|The units of the event measure(s).
| eventRouteIDFieldName | string|The route identifier field name.
| isLineEvent | boolean|A boolean value indicating whether or not this is a line event.
| lateralOffsetFieldName | string|The lateral offset field name.
| MDirectionOffsetting | boolean|A boolean value indicating if the offset should based on the M direction or the digitized direction.
| errorFieldName | string|The error field name.
| addErrorField | boolean|The add error field.
| fromMeasureFieldName | string|The from measure field name.
| toMeasureFieldName | string|The to measure field name.
| addAngleField | boolean|A boolean value indicating if an angle field should be added to the field set.
| angleFieldName | string|The angle field name.
| asPointFeature | boolean|A boolean value indicating if the point event shape should be output as a multipoint or a point.
| complementAngle | boolean|A boolean value indicating if 180 degres should be added to the angle field value.
| normalAngle | boolean|A boolean value indicating if the angle field should be the normal or the tangent anglea.
| eventTable | [DataConnection](Types.md#dataconnection)|The data connection for the route events.






## CIMSqlQueryDataConnection
Represents a SQL query data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMSqlQueryDataConnection

|Property | Type | Description |
|---------|--------|--------|
| sqlQuery | string|The SQL query.
| srid | string|The SRID of the spatial reference.
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference)|The spatial reference.
| OIDFields | string|The OID fields.
| geometryType | [enumeration esriGeometryType](ExternalReferences.md#enumeration-esrigeometrytype)|The geometry type.
| extent | [Envelope](ExternalReferences.md#envelope)|The extent.
| queryFields | [Fields](ExternalReferences.md#fields)|The query fields.
| spatialStorageType | number //int32|The spatial storage type.


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.






## CIMStandaloneTable
Represents a standalone table.


### CIMDefinition

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| URI | string|The URI of the definition. Typically set by the system and used as an identifier.
| sourceURI | string|The source URI of the item. Set if sourced from an external item such as an item on a portal.
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|The time the definition was last modfied.
| metadataURI | string|The metadata URI.
| useSourceMetadata | boolean|A boolean indicating if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project.


### CIMStandaloneTableDefinition

|Property | Type | Description |
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|The data connection for the table.
| description | string|The description.
| autoGenerateRowTemplates | boolean|A boolean option indicating whether to automatically generate row templates from the renderer.
| rowTemplates | [CIMEditingTemplate](Types.md#cimeditingtemplate) |The row templates.
| serviceTableID | number //int32|The identifier that will be used to identify the layer in server
| showPopups | boolean|A boolean indicating whether or not to show popups.
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo)|The popup info.
| charts | [CIMChart](CIMLayer.md#cimchart) |


### CIMDisplayTableDefinition

|Property | Type | Description |
|---------|--------|--------|
| definitionExpression | string|The definition expression that can subset the rows in the virtual table.
| displayField | string|The name of the attribute field that will be used as a label that represents each row in the table. The display field must be able to be represented as a string (string or numeric).
| editable | boolean|A boolean option indicating whether or not the table can be edited.
| relates | [CIMRelateInfoBase](CIMVectorLayers.md#cimrelateinfobase) |The relates.
| fieldDescriptions | [CIMFieldDescription](CIMVectorLayers.md#cimfielddescription) |The field descriptions. Field descriptions for fields may only be written if values are overridden from defaults.
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition)|The time fields.
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|The time definition.
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|The time display definition.
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition)|The time definition fields.
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |The range defintions.
| activeRangeName | string|The active range name.
| selectRelatedData | boolean|A value indicating if related data should be selected when creating a new selection.
| bindVariables | [CIMBindVariable](Types.md#cimbindvariable) |The bind variables.
| subtypeValue | number //int32|The subtype value that should be used in the feature layer definition. This property is honored only when feature layer is a member of SubtypeLayer.
| useSubtypeValue | boolean|A boolean option indicating whether or not the SubtypeValue should be used.
| displayExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The expression information used for coming up with a string that represents a row or a feature.
| selectionSetURI | string|The URI of the selection set for the table.






## CIMStandardDataConnection
Represents a standard data connection, the most common data connection type.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.






## CIMStreamServiceDataConnection
Represents a stream service data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMStreamServiceDataConnection

|Property | Type | Description |
|---------|--------|--------|
| featureExpirationMethod | [enumeration FeatureExpirationMethod](CIMVectorLayers.md#enumeration-featureexpirationmethod)|The feature expiration method used at dataset level.
| maximumFeatureCount | __int64|The maximum number of features that are held in memory before features are discarded.
| maximumFeatureAge | __int64|The maximum age for each feature before the feature is discarded.


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.






## CIMSubtypeGroupLayer
Represents a subtype group layer that works with feature classes enabled with subtypes. A subtype layer is a group layer that contains feature layers, each of which represents a subtype in a feature class.


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


### CIMFeatureLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| autoGenerateFeatureTemplates | boolean|A boolean option indicating whether to automatically generate feature templates from the renderer.
| extrusion | [CIMFeatureExtrusion](CIMVectorLayers.md#cimfeatureextrusion)|The feature extrusion.
| featureElevationExpression | string|The feature elevation expression.
| featureHyperlinks | [CIMFeatureHyperlink](CIMVectorLayers.md#cimfeaturehyperlink) |The feature hyperlinks.
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable)|The feature table.
| featureTemplates | [CIMEditingTemplate](Types.md#cimeditingtemplate) |The feature templates.
| hotlinkField | string|The field containing hotlink URLs.
| htmlPopupEnabled | boolean|A boolean option indicating whether HTML popups are enabled.
| htmlPopupFormat | [CIMHtmlPopupFormat](CIMVectorLayers.md#cimhtmlpopupformat)|The HTML popups format.
| isFlattened | boolean|A boolean option indicating whether the layer is flattened.
| selectable | boolean|A boolean option indicating whether the layer is selectable.
| selectionColor | [Color](Types.md#color)|The selection color.
| selectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The selection symbol.
| useSelectionSymbol | boolean|A boolean option indicating whether to use the selection symbol.
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition)|Use current map series page to select features.
| featureCacheType | [enumeration FeatureCacheType](CIMVectorLayers.md#enumeration-featurecachetype)|The feature cache type.
| enableDisplayFilters | boolean|A boolean option indicating whether the current set of display filters are honored during drawing.
| displayFilters | [CIMDisplayFilter](CIMVectorLayers.md#cimdisplayfilter) |The current set of display filters.
| featureElevationExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The expression for setting the feature elevation


### CIMSubtypeGroupLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| subtypeLayers | [string,]|The layer URI corresponding to each subtype value.






## CIMSuppressActivity
Represents suppress activity.


### CIMActivity

|Property | Type | Description |
|---------|--------|--------|


### CIMSuppressActivity

|Property | Type | Description |
|---------|--------|--------|






## CIMSymbolIdentifier
Represents a symbol identifier.


### CIMSymbolIdentifier

|Property | Type | Description |
|---------|--------|--------|
| ID | number //int32|The ID which identifies the symbol in the collection.
| name | string|The name of the symbol in the symbol collection.
| symbol | [Symbol](Types.md#symbol)|The symbol.






## CIMSymbolLayerMasking
Represents symbol layer masking.


### CIMSymbolLayerMasking

|Property | Type | Description |
|---------|--------|--------|
| symbolLayers | [CIMSymbolLayerIdentifier](CIMLayer.md#cimsymbollayeridentifier) |The symbol layer identifiers





### Enumeration: SymbolSubstitutionType
Symbol substitution types.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| No symbol substitution.
| Color| 1| Substitute color.
| IndividualSubordinate| 2| Substitute individual symbols in the collection with overrides taking precedence to symbols.
| IndividualDominant| 3| Substitute individual symbols in the collection with the symbol taking precedence to overrides.




## CIMTableMediaInfo
Represents table media info.


### CIMMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| row | number //int32|The row.
| column | number //int32|The column.
| refreshRate | number //double|The amount of time in RefreshRateUnit to wait between refreshing the media info.
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media.


### CIMTableMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| fields | [string,]|The fields.






## CIMTableQueryNameDataConnection
Represents a table query name data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMTableQueryNameDataConnection

|Property | Type | Description |
|---------|--------|--------|
| subFields | string|The subfields.
| tables | string|The tables.
| whereClause | string|The where clause.
| primaryKeyFields | string|The primary key fields.
| copyLocally | boolean|A boolean value indicating whether or not to copy data locally.
| shapeType | [enumeration esriGeometryType](ExternalReferences.md#enumeration-esrigeometrytype)|The shape type.
| featureType | [enumeration esriFeatureType](ExternalReferences.md#enumeration-esrifeaturetype)|The feature type.
| extent | [Envelope](ExternalReferences.md#envelope)|The extent.
| shapeFieldName | string|The shape field name.


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.






## CIMTemporalDataConnection
Represents a temporal data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMTemporalDataConnection

|Property | Type | Description |
|---------|--------|--------|
| timeFieldLocaleID | number //int32|The time field locale ID.
| timeFieldAmFormat | string|The custom string representation of the AM symbol.
| timeFieldPmFormat | string|The custom string representation of the PM symbol.
| cachingMode | [enumeration TemporalFeatureClassCachingMode](CIMVectorLayers.md#enumeration-temporalfeatureclasscachingmode)|The caching mode.
| startTimeField | string|The start time field.
| endTimeField | string|The end time field.
| timeValueFormat | string|The time value format.
| trackIDField | string|The track ID field.


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.





### Enumeration: TemporalFeatureClassCachingMode
Temporal feature class caching modes.

|Property | Value | Description |
|---------|--------|--------|
| All| 0| All.
| None| 1| None.



### Enumeration: TemporalFeatureClassPurgeRule
Temporal feature class purge rules.

|Property | Value | Description |
|---------|--------|--------|
| KeepLatestPerTrack| 0| Keep latest per track.
| PurgeOldest| 1| Purge oldest.




## CIMTextMediaInfo
Represents text media info.


### CIMMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| row | number //int32|The row.
| column | number //int32|The column.
| refreshRate | number //double|The amount of time in RefreshRateUnit to wait between refreshing the media info.
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units for the amount of time to wait between refreshing the media.


### CIMTextMediaInfo

|Property | Type | Description |
|---------|--------|--------|
| text | string|The text.






## CIMTimeDataDefinition
Represents a time data definition.


### CIMTimeDataDefinition

|Property | Type | Description |
|---------|--------|--------|
| useTime | boolean|A boolean indicating whether or not to use time for animation purposes.
| timeReference | [TimeReference](ExternalReferences.md#timereference)|The time reference.
| customTimeExtent | [TimeExtent](ExternalReferences.md#timeextent)|The custom time extent.
| hasLiveData | boolean|A boolean indicating whether or not this dataset has live data.
| timeExtentCanChange | boolean|The data regularly changes, so the extent needs recalculated.






## CIMTimeDimensionDefinition
Represents a time dimension definition.


### CIMTimeDimensionDefinition

|Property | Type | Description |
|---------|--------|--------|
| timeDimensionName | string|The time dimension name.
| timeDimensionFormat | string|The time dimension format.






## CIMTimeDisplayDefinition
Represents a time display definition.


### CIMTimeDisplayDefinition

|Property | Type | Description |
|---------|--------|--------|
| cumulative | boolean|A boolean value indicating whether time is cumulative.
| timeInterval | number //double|The time interval.
| timeIntervalUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The time interval units.
| timeOffset | number //double|The time offset.
| timeOffsetUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The time offset units.






## CIMTimeTableDefinition
Represents a time table definition.


### CIMTimeTableDefinition

|Property | Type | Description |
|---------|--------|--------|
| startTimeField | string|The start time field.
| endTimeField | string|The end time field.
| timeValueFormat | string|The time value format.
| trackIDField | string|The track ID field.






## CIMTrackingServerDataConnection
Represents a tracking server data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMTrackingServerDataConnection

|Property | Type | Description |
|---------|--------|--------|
| autoPurge | boolean|A boolean value indicating whether to automatically purge data.
| purgeThreshold | number //int32|The purge threshold.
| purgePercentage | number //double|The percentage of the maximum allowed number of records to delete when the purge occurs.
| keepPerTrack | number //int32|The minimum number of features to keep per track.
| purgeRule | [enumeration TemporalFeatureClassPurgeRule](CIMVectorLayers.md#enumeration-temporalfeatureclasspurgerule)|The purge rule.


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.






## CIMVectorTileDataConnection
Represents a VectorTile layer data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMVectorTileDataConnection

|Property | Type | Description |
|---------|--------|--------|
| URI | string|The URI of the VectorTile files or resources.






## CIMVectorTileLayer
Represents a VectorTile layer. A VectorTileServiceLayer provides rich cartographic content in a fast and efficient vector tile format. It may have multiple styles and if so users can choose which style to use to display the layer's vector geometries. Logically a VectorTileServiceLayer is more like a basemap layer in that it is typically composed of several distinct data sources (e.g. roads, cities, hydrology, buildings) that can provide context and background but in a way that is typically more performant than raster tile layers.


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


### CIMVectorTileLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| dataConnection | [CIMVectorTileDataConnection](CIMVectorLayers.md#cimvectortiledataconnection)|The data connection to the VectorTile resource.
| currentStyle | string|The current style the vector tile layer features should be rendered with.






## CIMWorkspaceConnection
Represents a workspace connection.


### CIMWorkspaceConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.





### Enumeration: WorkspaceFactory
Workspace factory types.

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
Represents an XY event data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMXYEventDataConnection

|Property | Type | Description |
|---------|--------|--------|
| XFieldName | string|The X field name.
| YFieldName | string|The Y field name.
| ZFieldName | string|The Z field name.
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference)|The spatial reference.
| XYEventTableDataConnection | [DataConnection](Types.md#dataconnection)|The data connection to the table events are created from.
