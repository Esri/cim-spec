


## CIMAreaLegendPatch
#### Represents an area legend patch, small rectangles used to display legend classes. 


### CIMLegendPatch 

|Property | Type | Description | 
|---------|--------|--------|
| geometryURI | string | The URI of the binary reference containing the geometry of the legend patch. 


### CIMAreaLegendPatch 

|Property | Type | Description | 
|---------|--------|--------|






## CIMBivariateFieldInfo
#### Contains a collection of properties that describe a bivariate attribute field. 


### CIMDataNormalization 

|Property | Type | Description | 
|---------|--------|--------|
| normalizationField | string | The normalization field. 
| normalizationTotal | double | The normalization total. 
| normalizationType | [enumeration DataNormalizationMethod](CIMRenderers.md#enumeration-datanormalizationmethod) | The normalization type. 


### CIMBivariateFieldInfo 

|Property | Type | Description | 
|---------|--------|--------|
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method. 
| field | string | The field for rendering. 
| valueExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns value as a number. When both Field and ValueExpressionInfo are present ValueExpressionInfo is used. 
| defaultLabel | string | The default label used for the legend. 
| minimumBreak | double | The minimum break. 
| upperBounds | [double] | The collection of upper bounds. 
| numberOfHistogramBins | long | The number of bins displayed in the histogram. 





### Enumeration: BivariateGridLegendLabelStrategy
#### Bivariate grid label strategy. 

|Property | Value | Description | 
|---------|--------|--------|
| Corners| 0| The labels for the legend are placed at each corner of the grid. 
| Sides| 1| The labels for the legend are placed at bottom and left side of the grid. 



### Enumeration: BivariateGridLegendOrientationType
#### Bivariate grid orientation type. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| The legend is a square without focusing on any particular corner. 
| High| 1| The legend is a diamond with focus on features with high values for both bivariate fields. 
| Low| 2| The legend is a diamond with focus on features with low values for both bivariate fields. 
| HighLow| 3| The legend is a diamond with focus on features with high values in the first bivariate field and low values in the second bivariate field. 
| LowHigh| 4| The legend is a diamond with focus on features with low values in the first bivariate field and high values in the second bivariate field. 



### Enumeration: BivariateGridSizeOption
#### Bivariate grid size option. 

|Property | Value | Description | 
|---------|--------|--------|
| TwoByTwo| 0| A grid with two rows and two columns. 
| ThreeByThree| 1| A grid with three rows and three columns. 
| FourByFour| 2| A grid with four rows and four columns. 




## CIMBivariateRendererAuthoringInfo
#### Represents additional authoring properties used by a bivariate choropleth renderer. 


### CIMRendererAuthoringInfo 

|Property | Type | Description | 
|---------|--------|--------|


### CIMUniqueValueRendererAuthoringInfo 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDataSampling 

|Property | Type | Description | 
|---------|--------|--------|
| sampleSize | long | The maximum number of records to sample. 


### CIMBivariateRendererAuthoringInfo 

|Property | Type | Description | 
|---------|--------|--------|
| fieldInfos | [[CIMBivariateFieldInfo]](CIMRenderers.md#cimbivariatefieldinfo) | The field related properties used to generate the breaks. 
| gridSize | [enumeration BivariateGridSizeOption](CIMRenderers.md#enumeration-bivariategridsizeoption) | The grid size. 
| gridOrientation | [enumeration BivariateGridLegendOrientationType](CIMRenderers.md#enumeration-bivariategridlegendorientationtype) | The grid orientation. 
| gridLabelOption | [enumeration BivariateGridLegendLabelStrategy](CIMRenderers.md#enumeration-bivariategridlegendlabelstrategy) | The grid label option. 
| templateSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The template symbol. 






## CIMChartRenderer
#### Represents chart renderer which contains properties common to all symbolizers that depict some feature value as a chart drawn on top of the feature itself. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDataNormalization 

|Property | Type | Description | 
|---------|--------|--------|
| normalizationField | string | The normalization field. 
| normalizationTotal | double | The normalization total. 
| normalizationType | [enumeration DataNormalizationMethod](CIMRenderers.md#enumeration-datanormalizationmethod) | The normalization type. 


### CIMChartRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight) | The barrier weight for chart label collision. 
| baseSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The base symbol features are drawn with. 
| chartSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The chart symbol. 
| fieldNames | [string] | Field names used to populate the chart. 
| fieldTotals | [double] | The field totals. 
| label | string | The renderer label. 
| maxValue | double | Maximum value. 
| preventChartOverlap | boolean | A value indicating whether or not to prevent chart overlap. 
| proportionalPieSizeOptions | [CIMProportionalPieSizeOptions](CIMRenderers.md#cimproportionalpiesizeoptions) | The proportional pie size options. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| fieldLabels | [string] | The labels that will be shown next to fields in the legend. 
| showSizeLegend | boolean | A value indicating whether or not to show a legend group illustrating the chart's size. 
| sizeLegendOutlineColor | [Color](Types.md#color) | The color of the outline for the size legend group. 
| sizeLegendLeaderlineColor | [Color](Types.md#color) | The color of the leader line for the size legend group. 
| drawChartSymbolsAboveAllLayers | boolean | A value indicating whether or not to draw chart symbols for line or polygon features above all layers. This option applies when drawing charts for line or polygon layer. The background will be drawn in contents order and this option indicates if the charts should be drawn in contents order or above all other layers. 


### CIMDataExclusion 

|Property | Type | Description | 
|---------|--------|--------|
| exclusionClause | string | The exclusion clause. 
| exclusionDescription | string | The exclusion description. 
| exclusionLabel | string | The exclusion label. 
| exclusionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The exclusion symbol. 
| useExclusionSymbol | boolean | A value indicating whether or not to use the exclusion symbol. 
| exclusionSymbolPatch | [enumeration PatchShape](CIMRenderers.md#enumeration-patchshape) | The patch shape for the exclusion symbol. 
| exclusionSymbolCustomPatch | [LegendPatch](Types.md#legendpatch) | The custom patch for the exclusion symbol. 






## CIMClassBreak
#### Represents a class break. 


### CIMClassBreak 

|Property | Type | Description | 
|---------|--------|--------|
| criticalBreak | boolean | A value indicating whether or not this is a critical break. 
| description | string | The description. 
| label | string | The label. 
| patch | [enumeration PatchShape](CIMRenderers.md#enumeration-patchshape) | The patch shape for this class. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol for the class. 
| upperBound | double | The upper bound of the class. 
| alternateSymbols | [[CIMSymbolReference]](CIMRenderers.md#cimsymbolreference) | An array of symbol references that are intended to be used at specific scale ranges. 
| customPatch | [LegendPatch](Types.md#legendpatch) | The custom patch for this class. 





### Enumeration: ClassBreakType
#### Class break types. 

|Property | Value | Description | 
|---------|--------|--------|
| GraduatedColor| 0| Graduated color. 
| GraduatedSymbol| 1| Graduated symbol. 
| UnclassedColor| 2| Unclassed color. Applies only to Polygons and Multi Patches. 



### Enumeration: ClassBreaksLegendVisualVariableOptions
#### Legend display options for class breaks visual variables. 

|Property | Value | Description | 
|---------|--------|--------|
| ShowVisualVariableSymbolClasses| 0| Show classes separately from the primary symbols. 
| ShowClassesForEachPrimarySymbol| 1| Show classes for each primary symbol. 




## CIMClassBreaksRenderer
#### Represents a class break renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMClassBreaksRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The background symbol used for graduated symbols. 
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight) | The barrier weight used for graduated symbols to avoid labels. 
| classBreakType | [enumeration ClassBreakType](CIMRenderers.md#enumeration-classbreaktype) | The class break type. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| field | string | The field for rendering. 
| heading | string | The heading. 
| minimumLabel | string | The minimum label. 
| valueExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns value as a number. When both Fields and ValueExpressionInfo are present ValueExpressionInfo is used. 
| polygonSymbolColorTarget | [enumeration PolygonSymbolColorTarget](CIMRenderers.md#enumeration-polygonsymbolcolortarget) | The property that controls how the color ramp is applied to polygon symbols. 
| drawGraduatedSymbolsAboveAllLayers | boolean | A value indicating whether or not to draw graduated symbols for polygon features above all layers. This option applies when drawing graduated symbols for polygon layers. The background will be drawn in contents order and this option indicates if the graduated symbols should be drawn in contents order or above all other layers. 
| authoringInfo | [CIMClassBreaksRendererAuthoringInfo](CIMRenderers.md#cimclassbreaksrendererauthoringinfo) | The additional authoring information used by the renderer. 


### CIMClassBreaksProperties 

|Property | Type | Description | 
|---------|--------|--------|
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method. 
| breaks | [[CIMClassBreak]](CIMRenderers.md#cimclassbreak) | The class breaks. 
| minimumBreak | double | The minimum break. 
| showClassGaps | boolean | A value indicating whether or not to show class gaps. 
| showInAscendingOrder | boolean | A value indicating whether or not to show classes in ascending order. 
| useDefaultSymbol | boolean | A value indicating whether or not to use the default symbol. 
| defaultSymbolPatch | [enumeration PatchShape](CIMRenderers.md#enumeration-patchshape) | The patch shape for the default symbol. 
| defaultSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The default symbol. 
| defaultLabel | string | The default label. 
| defaultDescription | string | The default description. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| defaultSymbolCustomPatch | [LegendPatch](Types.md#legendpatch) | The custom patch for the default symbol. 
| alwaysUpdateClassLabels | boolean | A value indicating whether or not to automatically update class labels whenever a class upper value is changed. 


### CIMDataSampling 

|Property | Type | Description | 
|---------|--------|--------|
| sampleSize | long | The maximum number of records to sample. 


### CIMDataNormalization 

|Property | Type | Description | 
|---------|--------|--------|
| normalizationField | string | The normalization field. 
| normalizationTotal | double | The normalization total. 
| normalizationType | [enumeration DataNormalizationMethod](CIMRenderers.md#enumeration-datanormalizationmethod) | The normalization type. 


### CIMDataExclusion 

|Property | Type | Description | 
|---------|--------|--------|
| exclusionClause | string | The exclusion clause. 
| exclusionDescription | string | The exclusion description. 
| exclusionLabel | string | The exclusion label. 
| exclusionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The exclusion symbol. 
| useExclusionSymbol | boolean | A value indicating whether or not to use the exclusion symbol. 
| exclusionSymbolPatch | [enumeration PatchShape](CIMRenderers.md#enumeration-patchshape) | The patch shape for the exclusion symbol. 
| exclusionSymbolCustomPatch | [LegendPatch](Types.md#legendpatch) | The custom patch for the exclusion symbol. 


### CIMVisualVariableRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariables | [[CIMVisualVariable]](Types.md#visualvariable) | The visual variables. 






## CIMClassBreaksRendererAuthoringInfo
#### Represents additional authoring properties used by a class breaks renderer. 


### CIMRendererAuthoringInfo 

|Property | Type | Description | 
|---------|--------|--------|


### CIMClassBreaksRendererAuthoringInfo 

|Property | Type | Description | 
|---------|--------|--------|
| numberOfHistogramBins | long | The number of bins displayed in the histogram. 
| templateSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The template symbol. 





### Enumeration: ClassificationMethod
#### Classification methods. 

|Property | Value | Description | 
|---------|--------|--------|
| DefinedInterval| 0| Defined interval. 
| EqualInterval| 1| Equal interval. 
| GeometricalInterval| 2| Geometrical interval. 
| Manual| 3| Manual. 
| NaturalBreaks| 4| Natural breaks. 
| Quantile| 5| Quantile. 
| StandardDeviation| 6| Standard deviation. 



### Enumeration: ColorChannelTarget
#### Indicates the target color channel overridden by the class breaks color visual variable. 

|Property | Value | Description | 
|---------|--------|--------|
| SV| 0| S and V channels of the HSV color model. 
| All| 1| All channels. 




## CIMColorClassBreaksVisualVariable
#### Represents a classified color visual variable. 


### CIMVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMRenderers.md#cimvisualvariableauthoringinfo) | The authoring info. 


### CIMColorVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| expression | string | Expression. This property is used for Python or VBScript expressions. Arcade expressions will use the ValueExpressionInfo property. 
| minValue | double | The minimum value. 
| maxValue | double | The maximum value. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| normalizationField | string | The normalization field. 
| normalizationType | [enumeration DataNormalizationMethod](CIMRenderers.md#enumeration-datanormalizationmethod) | The data normalization method. 
| valueExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns value as a number. 
| polygonSymbolColorTarget | [enumeration PolygonSymbolColorTarget](CIMRenderers.md#enumeration-polygonsymbolcolortarget) | The property that controls how the color ramp is applied to polygon symbols. 


### CIMClassBreaksProperties 

|Property | Type | Description | 
|---------|--------|--------|
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method. 
| breaks | [[CIMClassBreak]](CIMRenderers.md#cimclassbreak) | The class breaks. 
| minimumBreak | double | The minimum break. 
| showClassGaps | boolean | A value indicating whether or not to show class gaps. 
| showInAscendingOrder | boolean | A value indicating whether or not to show classes in ascending order. 
| useDefaultSymbol | boolean | A value indicating whether or not to use the default symbol. 
| defaultSymbolPatch | [enumeration PatchShape](CIMRenderers.md#enumeration-patchshape) | The patch shape for the default symbol. 
| defaultSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The default symbol. 
| defaultLabel | string | The default label. 
| defaultDescription | string | The default description. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| defaultSymbolCustomPatch | [LegendPatch](Types.md#legendpatch) | The custom patch for the default symbol. 
| alwaysUpdateClassLabels | boolean | A value indicating whether or not to automatically update class labels whenever a class upper value is changed. 


### CIMColorClassBreaksVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| colorChannelTarget | [enumeration ColorChannelTarget](CIMRenderers.md#enumeration-colorchanneltarget) | A value indicating which channels of the color model will be overridden by the visual variable. 


### CIMClassBreaksVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| classBreaksLegendVisualVariableOptions | [enumeration ClassBreaksLegendVisualVariableOptions](CIMRenderers.md#enumeration-classbreakslegendvisualvariableoptions) | The legend display options. 
| useClassBreaks | boolean | A value indicating whether or not to use class breaks. 






## CIMColorVisualVariable
#### Represents a color visual variable. 


### CIMVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMRenderers.md#cimvisualvariableauthoringinfo) | The authoring info. 


### CIMColorVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| expression | string | Expression. This property is used for Python or VBScript expressions. Arcade expressions will use the ValueExpressionInfo property. 
| minValue | double | The minimum value. 
| maxValue | double | The maximum value. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| normalizationField | string | The normalization field. 
| normalizationType | [enumeration DataNormalizationMethod](CIMRenderers.md#enumeration-datanormalizationmethod) | The data normalization method. 
| valueExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns value as a number. 
| polygonSymbolColorTarget | [enumeration PolygonSymbolColorTarget](CIMRenderers.md#enumeration-polygonsymbolcolortarget) | The property that controls how the color ramp is applied to polygon symbols. 





### Enumeration: DataNormalizationMethod
#### Data normalization methods. 

|Property | Value | Description | 
|---------|--------|--------|
| Field| 0| Normalize by field. 
| Log| 1| Log normalization. 
| PercentOfTotal| 2| Percent of total. 
| Nothing| 3| None. 




## CIMDictionaryRenderer
#### Represents a dictionary renderer where symbols are drawn from a symbol dictionary. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDictionaryRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| dictionaryName | string | The dictionary name. 
| fieldMap | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The field map between expected fields and actual fields. 
| scalingExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns the symbol scaling ratio as a number. 






## CIMDotDensityRenderer
#### Represents a dot density renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDataSampling 

|Property | Type | Description | 
|---------|--------|--------|
| sampleSize | long | The maximum number of records to sample. 


### CIMVisualVariableRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariables | [[CIMVisualVariable]](Types.md#visualvariable) | The visual variables. 


### CIMDataExclusion 

|Property | Type | Description | 
|---------|--------|--------|
| exclusionClause | string | The exclusion clause. 
| exclusionDescription | string | The exclusion description. 
| exclusionLabel | string | The exclusion label. 
| exclusionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The exclusion symbol. 
| useExclusionSymbol | boolean | A value indicating whether or not to use the exclusion symbol. 
| exclusionSymbolPatch | [enumeration PatchShape](CIMRenderers.md#enumeration-patchshape) | The patch shape for the exclusion symbol. 
| exclusionSymbolCustomPatch | [LegendPatch](Types.md#legendpatch) | The custom patch for the exclusion symbol. 


### CIMDotDensityRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| dotDensitySymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The dot density symbol. 
| dotSize | double | The dot size. 
| dotValue | double | The dot value. 
| excludeDotsFromMaskedArea | boolean | A value indicating whether or not the exclude dots from masked areas. 
| fieldNames | [string] | The field names dot data comes from. 
| fieldLabels | [string] | The label for each selected field name. 
| maintainDensity | boolean | A value indicating whether or not to maintain density. 
| maskingLayer | string | A path to the layer that supplies masks. 
| randomSeed | long | A random seed. 
| referenceScale | double | The reference scale. If specified, dots are calibrated from this scale. 
| useMasking | boolean | A value indicating whether or not to use masking. 
| valueExpressionInfos | [[CIMExpressionInfo]](CIMRenderers.md#cimexpressioninfo) | The arcade expressions the dot data comes from. If this array is populated it takes precedence over the FieldNames array. 
| symbolLabel | string | The legend label indicating what the symbol is (e.g. "dot"). 
| unitLabel | string | The legend label indicating what the dots represent (e.g. "people"). 






## CIMExpressionInfo
#### Represents the properties required for authoring an Arcade expression. 


### CIMExpressionInfo 

|Property | Type | Description | 
|---------|--------|--------|
| title | string | The human readable text that describes the expression. 
| expression | string | The Arcade expression used to evaluate and return the value that a property expects. 
| name | string | The Name of the expression. 
| returnType | [enumeration ExpressionReturnType](CIMRenderers.md#enumeration-expressionreturntype) | The ReturnType of the expression. 





### Enumeration: ExpressionReturnType
#### Visual variable info types. 

|Property | Value | Description | 
|---------|--------|--------|
| Default| 0| The return type of the expression is determined by the consumer using the expression. 
| String| 1| The return type of the expression is treated as a string by all consumers. 
| Numeric| 2| The return type of the expression is treated as a numeric value by all consumers. 




## CIMHeatMapRenderer
#### Represents a heat map renderer. The Heat Map Renderer draws point features as a continuous color gradient representing the density of the points. The resulting density surface represents the physical proximity between points, optionally weighted by a specified attribute value. The displayed raster surface is dynamic and morphs according to the zoom level and updates if the source point features are edited. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMHeatMapRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorScheme | [ColorRamp](Types.md#colorramp) | The color scheme of the heat map. Controls how smooth the color gradient appears. Must be either a continuous or multipart color ramp. If no color scheme is specified, a default color ramp will be used. 
| field | string | The name of the field denoting weighting values for each feature. The field's value is the count or quantity to be spread across the landscape to create a continuous surface. Values in the field may be integer or floating point. The options for the field are listed below. Specify the name of a numeric field in the feature table Use "" if no item or special value will be used and each feature will be counted once. Use Shape if input features contains Z. 
| radius | long | The radius which defines how far the heat spreads away from the points. Specified and stored in Points and translates to Pixels at draw time. 
| rendererQuality | long | The renderer quality which controls the pixelation of the raster. This is an arbitrary range that goes from Best (10) to Fastest (0). 
| heading | string | The legend heading. 
| minLabel | string | The legend label for the minimum density value. 
| maxLabel | string | The legend label for the maximum density value. 
| maxPixelIntensity | double | The maximum pixel intensity. 
| pixelIntensityStops | [double] | The pixel intensity stops. 
| autoAdjustPixelIntensity | boolean | A value indicating whether to update renderers pixel intensity range automatically. When set to True renderer's pixel intensity range will change based on the features with in the visible extent. 
| maxPixelIntensityReferenceScale | double | Base scale at which the maximum pixel intensity should be used. This value is used only when the auto adjust pixel intensity is set to false. 
| referenceScale | double | The scale at which the search radius (in screen units - points) is converted to map units. 






## CIMLineLegendPatch
#### Represents a line legend patch, small lines used to display legend classes. 


### CIMLegendPatch 

|Property | Type | Description | 
|---------|--------|--------|
| geometryURI | string | The URI of the binary reference containing the geometry of the legend patch. 


### CIMLineLegendPatch 

|Property | Type | Description | 
|---------|--------|--------|






## CIMMultilevelColorVisualVariable
#### Represents a color visual variable with different levels-of-detail. 


### CIMVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMRenderers.md#cimvisualvariableauthoringinfo) | The authoring info. 


### CIMMultilevelVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| levels | [[CIMVisualVariableLevel]](CIMRenderers.md#cimvisualvariablelevel) | The levels that hold the minimum and maximum values of the data. 


### CIMMultilevelColorVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| normalizationField | string | The normalization field. 
| normalizationType | [enumeration DataNormalizationMethod](CIMRenderers.md#enumeration-datanormalizationmethod) | The data normalization method. 
| valueExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns value as a number. 
| polygonSymbolColorTarget | [enumeration PolygonSymbolColorTarget](CIMRenderers.md#enumeration-polygonsymbolcolortarget) | The property that controls how the color ramp is applied to polygon symbols. 





### Enumeration: PatchShape
#### Patch shapes. 

|Property | Value | Description | 
|---------|--------|--------|
| Default| 0| Default patch shape. 
| Point| 1| A point. 
| LineHorizontal| 2| A horizontal line. 
| LineZigZag| 3| A zig zag line. 
| LineAngles| 4| An angled line. 
| LineArc| 5| A line arc. 
| LineCurve| 6| A curved line. 
| LineTrail| 7| A line representing a trail. 
| LineHydro| 8| A hydro line. 
| LineVertical3D| 9| A vertical 3D line. 
| LineZigZag3D| 10| A 3D zig zag line. 
| LineCorkscrew3D| 11| A 3D corkscrew line. 
| AreaRectangle| 12| An area rectangle. 
| AreaRoundedRectangle| 13| An area rounded rectangle. 
| AreaPolygon| 14| An area polygon. 
| AreaCircle| 15| An area circle. 
| AreaEllipse| 16| An area ellipse. 
| AreaFootprint| 17| An area footprint. 
| AreaBoundary| 18| An area boundary. 
| AreaHydroPoly| 19| An area hydro polygon. 
| AreaNaturalPoly| 20| A natural area polygon. 
| AreaSquare| 21| A square polygon. 
| AreaHexagonFlat| 22| A flat hexagon. 
| AreaHexagonPointy| 23| A pointy hexagon. 
| AreaTrapezium| 24| A trapezium. 
| Custom| 100| Custom shape. 



### Enumeration: PolygonSymbolColorTarget
#### Polygon symbol color apply targets. 

|Property | Value | Description | 
|---------|--------|--------|
| Fill| 0| The color is applied only to the fill of the polygon symbol. 
| Outline| 1| The color is applied only to the outline of the polygon symbol. 
| FillOutline| 2| The color is applied to the fill and the outline of the polygon symbol. 




## CIMPrimitiveOverride
#### Represents a primitive override. 


### CIMPrimitiveOverride 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name this override applies to. 
| propertyName | string | The property name in the primitive this override applies to. 
| expression | string | The expression. This property is used for Python or VBScript expressions. Arcade expressions will use the ValueExpressionInfo property. 
| valueExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns value as a number or a string depending on the PropertyName. 






## CIMProportionalPieSizeOptions
#### Represents proportional pie size options. 


### CIMProportionalPieSizeOptions 

|Property | Type | Description | 
|---------|--------|--------|
| flanneryCompensation | boolean | A value indicating whether or not to use Flannery compensation. 
| minimumSize | double | The minimum size. 
| minimumValue | double | The data value that corresponds to the minimum size. 
| maximumSize | double | The maximum size. This value is optional. 
| maximumValue | double | The data value that corresponds to the maximum size. This value is optional. 
| proportionalBySum | boolean | A value indicating whether to size the pie chart proportionally by the sum of field values. 
| proportionalFieldName | string | The field that is used to size the pie chart proportionally. 
| proportionalExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The Arcade expression that is used to size the pie chart proportionally. This property is mutually exclusive with ProportionalBySum and ProportionalFieldName. 






## CIMProportionalRenderer
#### Represents a proportional renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDataSampling 

|Property | Type | Description | 
|---------|--------|--------|
| sampleSize | long | The maximum number of records to sample. 


### CIMVisualVariableRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariables | [[CIMVisualVariable]](Types.md#visualvariable) | The visual variables. 


### CIMDataNormalization 

|Property | Type | Description | 
|---------|--------|--------|
| normalizationField | string | The normalization field. 
| normalizationTotal | double | The normalization total. 
| normalizationType | [enumeration DataNormalizationMethod](CIMRenderers.md#enumeration-datanormalizationmethod) | The normalization type. 


### CIMDataExclusion 

|Property | Type | Description | 
|---------|--------|--------|
| exclusionClause | string | The exclusion clause. 
| exclusionDescription | string | The exclusion description. 
| exclusionLabel | string | The exclusion label. 
| exclusionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The exclusion symbol. 
| useExclusionSymbol | boolean | A value indicating whether or not to use the exclusion symbol. 
| exclusionSymbolPatch | [enumeration PatchShape](CIMRenderers.md#enumeration-patchshape) | The patch shape for the exclusion symbol. 
| exclusionSymbolCustomPatch | [LegendPatch](Types.md#legendpatch) | The custom patch for the exclusion symbol. 


### CIMProportionalRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | Background symbol features are drawn with underneath the proportional symbols. 
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight) | The barrier weight used for graduated symbols to avoid labels. 
| field | string | The field the renderer is using. 
| flanneryCompensation | boolean | A value indicating whether or not to use Flannery compensation. 
| legendSymbolCount | long | The legend symbol count. 
| maxDataValue | double | The maximum data value. 
| minDataValue | double | The minimum data value. 
| minSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The minimum symbol. 
| unitSymbolization | [CIMUnitSymbolization](CIMRenderers.md#cimunitsymbolization) | The unit symbolization. 
| heading | string | The heading. 
| useDefaultSymbol | boolean | A value indicating whether or not to use the default symbol. 
| defaultSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The default symbol. 
| defaultSymbolPatch | [enumeration PatchShape](CIMRenderers.md#enumeration-patchshape) | The patch shape for the default symbol. 
| defaultLabel | string | The default label. 
| defaultDescription | string | The default description. 
| showInAscendingOrder | boolean | A value indicating whether or not to show classes in ascending order. 
| valueExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns value as a number. When both Fields and ValueExpressionInfo are present ValueExpressionInfo is used. 
| drawProportionalSymbolsAboveAllLayers | boolean | A value indicating whether or not to draw proportional symbols for polygon features above all layers. This option applies when drawing proportional symbols for polygon layers. The background will be drawn in contents order and this option indicates if the proportional symbols should be drawn in contents order or above all other layers. 
| defaultSymbolCustomPatch | [LegendPatch](Types.md#legendpatch) | The custom patch for the default symbol. 
| authoringInfo | [CIMProportionalRendererAuthoringInfo](CIMRenderers.md#cimproportionalrendererauthoringinfo) | The additional authoring information used by the renderer. 






## CIMProportionalRendererAuthoringInfo
#### Represents additional authoring properties used by a proportional renderer. 


### CIMRendererAuthoringInfo 

|Property | Type | Description | 
|---------|--------|--------|


### CIMProportionalRendererAuthoringInfo 

|Property | Type | Description | 
|---------|--------|--------|
| numberOfHistogramBins | long | The number of bins displayed in the histogram. 






## CIMRepresentationRenderer
#### Represents a representation renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMRepresentationRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| drawInvalidRule | boolean | A value indicating whether or not the draw invalid rules. 
| drawInvisibleRepresentation | boolean | A value indicating whether or not the draw invisible representations. 
| invalidRuleColor | [Color](Types.md#color) | The invalid rule color. 
| invisibleRepresentationColor | [Color](Types.md#color) | The invisible representation color. 
| representationClassName | string | The representation class name. 
| ruleLegendVisibility | [long] | The rule legend visibility. 
| symbolLayerNameMapping | [[CIMRuleSymbolLayerNames]](CIMRenderers.md#cimrulesymbollayernames) | The symbol layer name mapping. 






## CIMRotationVisualVariable
#### Represents a rotation visual variable. 


### CIMVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMRenderers.md#cimvisualvariableauthoringinfo) | The authoring info. 


### CIMRotationVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariableInfoX | [CIMVisualVariableInfo](CIMRenderers.md#cimvisualvariableinfo) | The visual variable info for the X dimension. 
| visualVariableInfoY | [CIMVisualVariableInfo](CIMRenderers.md#cimvisualvariableinfo) | The visual variable info for the Y dimension. 
| visualVariableInfoZ | [CIMVisualVariableInfo](CIMRenderers.md#cimvisualvariableinfo) | The visual variable info for the Z dimension. 
| rotationTypeZ | [enumeration SymbolRotationType](CIMRenderers.md#enumeration-symbolrotationtype) | The Z rotation type. 
| normalToSurface | boolean | A value indicating whether the normal to surface value which applies to 3D views. If true, rotation is applied after marker is rotated normal to the 3D surface. If false, all rotations are applied starting from zeroed X, Y, Z rotation. 






## CIMRuleSymbolLayerNames
#### Represents rule symbol layer names. 


### CIMRuleSymbolLayerNames 

|Property | Type | Description | 
|---------|--------|--------|
| ruleID | long | The rule ID. 
| symbolLayerNames | [string] | The symbol layer names. 






## CIMScaleDependentSizeVariation
#### Represents the scale dependent size variations for a symbol reference. Applies to point symbols, line symbols and the outline of polygon symbols. When the symbol reference is rendered at an intermediate scale a linearly scaled size is used. 


### CIMScaleDependentSizeVariation 

|Property | Type | Description | 
|---------|--------|--------|
| scale | double | The scale the size is associated with. 
| size | double | The size for the associated scale. 






## CIMSimpleRenderer
#### Represents a simple renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDataSampling 

|Property | Type | Description | 
|---------|--------|--------|
| sampleSize | long | The maximum number of records to sample. 


### CIMVisualVariableRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariables | [[CIMVisualVariable]](Types.md#visualvariable) | The visual variables. 


### CIMSimpleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| label | string | The legend label. 
| patch | [enumeration PatchShape](CIMRenderers.md#enumeration-patchshape) | The patch. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 
| alternateSymbols | [[CIMSymbolReference]](CIMRenderers.md#cimsymbolreference) | An array of symbol references that are intended to be used at specific scale ranges. 
| customPatch | [LegendPatch](Types.md#legendpatch) | The custom patch. 






## CIMSizeClassBreaksVisualVariable
#### Represents a classified size visual variable. 


### CIMVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMRenderers.md#cimvisualvariableauthoringinfo) | The authoring info. 


### CIMSizeVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| expression | string | The expression. This property is used for Python or VBScript expressions. Arcade expressions will use the ValueExpressionInfo property. 
| randomMin | double | The random minimum. 
| randomMax | double | The random maximum. 
| minSize | double | The minimum size. 
| maxSize | double | The maximum size. 
| minValue | double | The minimum value. 
| maxValue | double | The maximum value. 
| valueUnits | [LinearUnit](ExternalReferences.md#linearunit) | The size visual variable type. 
| valueRepresentation | [enumeration ValueRepresentations](CIMRenderers.md#enumeration-valuerepresentations) | The value representations. 
| variableType | [enumeration SizeVisualVariableType](CIMRenderers.md#enumeration-sizevisualvariabletype) | Size visual variable type. 
| valueShape | [enumeration SymbolShapes](CIMRenderers.md#enumeration-symbolshapes) | The value shape. 
| axis | [enumeration SizeVisualVariableAxis](CIMRenderers.md#enumeration-sizevisualvariableaxis) | Size visual variable axis. 
| target | string | Size visual variable target which specifies the portion of the symbol targeted for sizing. 
| normalizationField | string | The normalization field. 
| normalizationType | [enumeration DataNormalizationMethod](CIMRenderers.md#enumeration-datanormalizationmethod) | The data normalization method. 
| sizeValues | [double] | The size values that correspond to data values. 
| dataValues | [double] | The data values. 
| valueExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns value as a number. 


### CIMClassBreaksVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| classBreaksLegendVisualVariableOptions | [enumeration ClassBreaksLegendVisualVariableOptions](CIMRenderers.md#enumeration-classbreakslegendvisualvariableoptions) | The legend display options. 
| useClassBreaks | boolean | A value indicating whether or not to use class breaks. 


### CIMClassBreaksProperties 

|Property | Type | Description | 
|---------|--------|--------|
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method. 
| breaks | [[CIMClassBreak]](CIMRenderers.md#cimclassbreak) | The class breaks. 
| minimumBreak | double | The minimum break. 
| showClassGaps | boolean | A value indicating whether or not to show class gaps. 
| showInAscendingOrder | boolean | A value indicating whether or not to show classes in ascending order. 
| useDefaultSymbol | boolean | A value indicating whether or not to use the default symbol. 
| defaultSymbolPatch | [enumeration PatchShape](CIMRenderers.md#enumeration-patchshape) | The patch shape for the default symbol. 
| defaultSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The default symbol. 
| defaultLabel | string | The default label. 
| defaultDescription | string | The default description. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| defaultSymbolCustomPatch | [LegendPatch](Types.md#legendpatch) | The custom patch for the default symbol. 
| alwaysUpdateClassLabels | boolean | A value indicating whether or not to automatically update class labels whenever a class upper value is changed. 


### CIMSizeClassBreaksVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| templateSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The template symbol. 
| drawSizeMarkerSymbolsAboveAllLayers | boolean | A value indicating whether or not to draw size marker symbols for polygon features above all layers. This option applies when drawing size marker symbols for polygon layers. The background will be drawn in contents order and this option indicates if the size marker symbols should be drawn in contents order or above all other layers. 






## CIMSizeVisualVariable
#### Represents a size visual variable. VariableType = Graduated use expression, Minimum/Maximum size, Minimum/Maximum value. VariableType = Proportional, unit defined use Expression, ValueUnit, ValueShape, ValueRepresentation. VariableType = Proportional, unit NOT defined use Expression, MinSize, MinValue, could use MaxSize. 


### CIMVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMRenderers.md#cimvisualvariableauthoringinfo) | The authoring info. 


### CIMSizeVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| expression | string | The expression. This property is used for Python or VBScript expressions. Arcade expressions will use the ValueExpressionInfo property. 
| randomMin | double | The random minimum. 
| randomMax | double | The random maximum. 
| minSize | double | The minimum size. 
| maxSize | double | The maximum size. 
| minValue | double | The minimum value. 
| maxValue | double | The maximum value. 
| valueUnits | [LinearUnit](ExternalReferences.md#linearunit) | The size visual variable type. 
| valueRepresentation | [enumeration ValueRepresentations](CIMRenderers.md#enumeration-valuerepresentations) | The value representations. 
| variableType | [enumeration SizeVisualVariableType](CIMRenderers.md#enumeration-sizevisualvariabletype) | Size visual variable type. 
| valueShape | [enumeration SymbolShapes](CIMRenderers.md#enumeration-symbolshapes) | The value shape. 
| axis | [enumeration SizeVisualVariableAxis](CIMRenderers.md#enumeration-sizevisualvariableaxis) | Size visual variable axis. 
| target | string | Size visual variable target which specifies the portion of the symbol targeted for sizing. 
| normalizationField | string | The normalization field. 
| normalizationType | [enumeration DataNormalizationMethod](CIMRenderers.md#enumeration-datanormalizationmethod) | The data normalization method. 
| sizeValues | [double] | The size values that correspond to data values. 
| dataValues | [double] | The data values. 
| valueExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns value as a number. 





### Enumeration: SizeVisualVariableAxis
#### Size visual variable axis. 

|Property | Value | Description | 
|---------|--------|--------|
| HeightAxis| 0| Height axis: interpreted as Z for 3D markers, Y for billboarded 
| WidthAxis| 1| Width axis. 
| DepthAxis| 2| Depth axis. 
| WidthAndDepthAxes| 3| Width and depth axes. 
| AllAxes| 4| All axes. 



### Enumeration: SizeVisualVariableType
#### Size visual variable type. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| None. 
| Expression| 1| Expression. 
| Random| 2| Random. 
| Proportional| 3| Proportional. 
| Graduated| 4| Graduated. 




## CIMStringMap
#### Represents a string map of key value pairs. 


### CIMStringMap 

|Property | Type | Description | 
|---------|--------|--------|
| key | string | The key. 
| value | string | The value. 






## CIMSymbolReference
#### Represents a symbol reference. Symbol references currently store the symbol in-line in the symbol property. Overrides here are used primarily by renderers to pass overrides through the drawing pipeline. 


### CIMSymbolReference 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveOverrides | [[CIMPrimitiveOverride]](CIMRenderers.md#cimprimitiveoverride) | The primitive overrides. Typically set by renderers at draw time. 
| stylePath | string | The style path. Reserved for future use. 
| symbol | [Symbol](Types.md#symbol) | The symbol. 
| symbolName | string | The symbol name. 
| minScale | double | The minimum scale range the symbol reference should be displayed at. 
| maxScale | double | The maximum scale range the symbol reference should be displayed at. 
| scaleDependentSizeVariation | [[CIMScaleDependentSizeVariation]](CIMRenderers.md#cimscaledependentsizevariation) | An array of scale dependent sizes. 
| minDistance | double | The minimum distance at which symbols are visible. Objects closer than this don't get rendered. 
| maxDistance | double | The maximum distance at which symbols are visible. Objects beyond this point don't get rendered. 





### Enumeration: SymbolRotationType
#### Symbol rotation types. 

|Property | Value | Description | 
|---------|--------|--------|
| Geographic| 0| Geographic. 
| Arithmetic| 1| Arithmetic. 



### Enumeration: SymbolShapes
#### Symbol shapes. 

|Property | Value | Description | 
|---------|--------|--------|
| Unknown| 0| Unknown shape. 
| Circle| 1| Circle shape. 
| Square| 2| Square shape. 




## CIMTransparencyVisualVariable
#### Represents a transparency visual variable. 


### CIMVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMRenderers.md#cimvisualvariableauthoringinfo) | The authoring info. 


### CIMTransparencyVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| field | string | The field to base the transparency on. 
| transparencyValues | [double] | The transparency values that correspond to data values. 
| dataValues | [double] | The data values. 
| normalizationField | string | The normalization field. 
| normalizationTotal | double | The normalization total. 
| normalizationType | [enumeration DataNormalizationMethod](CIMRenderers.md#enumeration-datanormalizationmethod) | The normalization method. 
| valueExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns value as a number. 






## CIMUniqueValue
#### Represents a unique value. 


### CIMUniqueValue 

|Property | Type | Description | 
|---------|--------|--------|
| fieldValues | [string] | The field values. 






## CIMUniqueValueClass
#### Represents a unique value class. 


### CIMUniqueValueClass 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| editable | boolean | A value indicating whether this class is editable. 
| label | string | The label. 
| patch | [enumeration PatchShape](CIMRenderers.md#enumeration-patchshape) | The patch. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 
| values | [[CIMUniqueValue]](CIMRenderers.md#cimuniquevalue) | The values this class corresponds to. 
| visible | boolean | A value indicating whether this class is visible. 
| alternateSymbols | [[CIMSymbolReference]](CIMRenderers.md#cimsymbolreference) | An array of symbol references that are intended to be used at specific scale ranges. 
| customPatch | [LegendPatch](Types.md#legendpatch) | The custom patch. 






## CIMUniqueValueGroup
#### Represents a unique value group. 


### CIMUniqueValueGroup 

|Property | Type | Description | 
|---------|--------|--------|
| classes | [[CIMUniqueValueClass]](CIMRenderers.md#cimuniquevalueclass) | The classes belonging to the group. 
| heading | string | The heading. 






## CIMUniqueValueRenderer
#### Represents a unique value renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDataSampling 

|Property | Type | Description | 
|---------|--------|--------|
| sampleSize | long | The maximum number of records to sample. 


### CIMVisualVariableRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariables | [[CIMVisualVariable]](Types.md#visualvariable) | The visual variables. 


### CIMUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| defaultDescription | string | The default description. 
| defaultLabel | string | The default label. 
| defaultSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The default symbol. 
| defaultSymbolPatch | [enumeration PatchShape](CIMRenderers.md#enumeration-patchshape) | The patch shape for the default symbol. 
| fields | [string] | The fields used by this renderer. 
| groups | [[CIMUniqueValueGroup]](CIMRenderers.md#cimuniquevaluegroup) | The unique value groups. 
| useDefaultSymbol | boolean | A value indicating whether or not to use the default symbol. 
| isDefaultSymbolVisible | boolean | A value indicating whether or not the default symbol is visible. 
| styleGallery | string | The style item name for the color ramp. 
| valueExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns value as a string. When both Fields and ValueExpressionInfo are present ValueExpressionInfo is used. 
| polygonSymbolColorTarget | [enumeration PolygonSymbolColorTarget](CIMRenderers.md#enumeration-polygonsymbolcolortarget) | The property that controls how the color ramp is applied to polygon symbols. 
| authoringInfo | [CIMUniqueValueRendererAuthoringInfo](CIMRenderers.md#cimuniquevaluerendererauthoringinfo) | The property that controls how the color ramp is applied to polygon symbols. 
| defaultSymbolCustomPatch | [LegendPatch](Types.md#legendpatch) | The custom patch for the default symbol. 
| showClassVisibility | boolean | A value indicating whether the class visibility is shown in the contents pane. 






## CIMUnitSymbolization
#### Represents unit symbolization. 


### CIMUnitSymbolization 

|Property | Type | Description | 
|---------|--------|--------|
| valueRepresentation | [enumeration ValueRepresentations](CIMRenderers.md#enumeration-valuerepresentations) | The value representation. 
| valueUnit | [LinearUnit](ExternalReferences.md#linearunit) | The value unit. 
| symbolShape | [enumeration SymbolShapes](CIMRenderers.md#enumeration-symbolshapes) | The symbol shape. 





### Enumeration: ValueRepresentations
#### Represents value representations. 

|Property | Value | Description | 
|---------|--------|--------|
| Radius| 0| Radius. 
| Area| 1| Area. 
| Distance| 2| Distance. 
| Width| 3| Width. 




## CIMVisualVariableAuthoringInfo
#### Represents visual variable metadata used for authoring. 


### CIMVisualVariableAuthoringInfo 

|Property | Type | Description | 
|---------|--------|--------|
| minSliderValue | double | The minimum value. 
| maxSliderValue | double | The maximum value. 
| theme | string | A theme as an array of strings. 
| showLegend | boolean | A value indicating whether or not to show legends. 
| heading | string | The legend heading. 
| numberOfHistogramBins | long | The number of bins displayed in the histogram. 






## CIMVisualVariableInfo
#### Represents visual variable info. 


### CIMVisualVariableInfo 

|Property | Type | Description | 
|---------|--------|--------|
| expression | string | The expression. This property is used for Python or VBScript expressions. Arcade expressions will use the ValueExpressionInfo property. 
| randomMax | double | The random max. 
| randomMin | double | The random min. 
| visualVariableInfoType | [enumeration VisualVariableInfoType](CIMRenderers.md#enumeration-visualvariableinfotype) | The visual variable info type. 
| valueExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns value as a number. 





### Enumeration: VisualVariableInfoType
#### Visual variable info types. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| None. 
| Expression| 1| Expression 
| Random| 2| Random. 




## CIMVisualVariableLevel
#### Represents a level-of-detail for a multilevel visual variable. 


### CIMVisualVariableLevel 

|Property | Type | Description | 
|---------|--------|--------|
| ID | long | The identifier of this level. 
| minValue | double | The minimum value. 
| maxValue | double | The maximum value. 
| mean | double | The cached mean of the data at this level. Used to rapidly compute new minimum and maximum values. 
| standardDeviation | double | The cached standard deviation of the data at this level. Used to rapidly compute new minimum and maximum values. 



