


## CIMChartRenderer
#### Represents chart renderer which contains properties common to all symbolizers that depict some feature value as a chart drawn on top of the feature itself. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMChartRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight)|Gets and sets the barrier weight for chart label collision. 
| baseSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the base symbol features are drawn with. 
| chartSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the chart symbol. 
| fieldNames | IStringArray|Gets and sets field names used to populate the chart. 
| fieldTotals | [double]|Gets and sets the field totals. 
| label | string|Gets and sets the renderer label. 
| maxValue | double|Gets and sets max value. 
| preventChartOverlap | boolean|Gets and sets a boolean option indicating whether or not to prevent chart overlap. 
| proportionalPieSizeOptions | [CIMProportionalPieSizeOptions](CIMSymbolizers.md#cimproportionalpiesizeoptions)|Gets and sets the proportional pie size options. 


### CIMDataExclusion 

|Property | Type | Description | 
|---------|--------|--------|
| exclusionClause | string|Gets and sets the exclusion clause. 
| exclusionDescription | string|Gets and sets the exclusion description. 
| exclusionLabel | string|Gets and sets the exclusion label. 
| exclusionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the exclusion symbol. 
| useExclusionSymbol | boolean|Gets and sets a boolean value indicating whether or not to use the exclusion symbol. 


### CIMDataNormalization 

|Property | Type | Description | 
|---------|--------|--------|
| normalizationField | string|Gets and sets the normalization field. 
| normalizationTotal | double|Gets and sets the normalization total. 
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|Gets and sets the normalization type. 






## CIMClassBreak
#### Represents a class break. 


### CIMClassBreak 

|Property | Type | Description | 
|---------|--------|--------|
| criticalBreak | boolean|Gets and sets a boolean value indicating whether or not this is a critical break. 
| description | string|Gets and sets the description. 
| label | string|Gets and sets the label. 
| patch | [enumeration PatchShape](CIMSymbolizers.md#enumeration-patchshape)|Gets and sets the patch shape for this class. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol for the class. 
| upperBound | double|Gets and sets the upper bound of the class. 
| alternateSymbols | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference) |Gets and sets an array of symbol references that are intended to be used at specific scale ranges. 





### Enumeration: ClassBreakType
#### Class break types. 

|Property | Value | Description | 
|---------|--------|--------|
| GraduatedColor| 0| Graduated color. 
| GraduatedSymbol| 1| Graduated symbol. 
| UnclassedColor| 2| Unclassed color. Applies only to Polygons and Multi Patches. 




## CIMClassBreaksRenderer
#### Represents a class break renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMClassBreaksRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the background symbol used for graduated symbols. 
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight)|Gets and sets the barrier weight used for graduate symbols to avoid labels. 
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |Gets and sets the class breaks. 
| classBreakType | [enumeration ClassBreakType](CIMSymbolizers.md#enumeration-classbreaktype)|Gets and sets the class break type. 
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|Gets and sets the classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| field | string|Gets and sets the field for rendering. 
| minimumBreak | double|Gets and sets the minimum break for the renderer. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format. 
| showClassGaps | boolean|Gets and sets a boolean value indicating whether or not to show class gaps. 
| showInAscendingOrder | boolean|Gets and sets a boolean value indicating whether or not to show classes in ascending order. 
| heading | string|Gets and sets the heading. 
| sampleSize | long|Gets and sets the sample size used for creating the classification. 
| useDefaultSymbol | boolean|Gets and sets a boolean value indicating whether or not to use the default symbol. 
| defaultSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the default symbol. 
| minimumLabel | string|Gets and sets the minimum label. 
| defaultLabel | string|Gets and sets the default label. 
| defaultDescription | string|Gets and sets the default description. 
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets ExpressionInfo that contains the Arcade expression that returns value as a number. When both Fields and ValueExpressionInfo are present ValueExpressionInfo is used. 


### CIMDataExclusion 

|Property | Type | Description | 
|---------|--------|--------|
| exclusionClause | string|Gets and sets the exclusion clause. 
| exclusionDescription | string|Gets and sets the exclusion description. 
| exclusionLabel | string|Gets and sets the exclusion label. 
| exclusionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the exclusion symbol. 
| useExclusionSymbol | boolean|Gets and sets a boolean value indicating whether or not to use the exclusion symbol. 


### CIMDataNormalization 

|Property | Type | Description | 
|---------|--------|--------|
| normalizationField | string|Gets and sets the normalization field. 
| normalizationTotal | double|Gets and sets the normalization total. 
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|Gets and sets the normalization type. 


### CIMVisualVariableRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariables | [CIMVisualVariable](Types.md#cimvisualvariable) |Gets and sets the visual variables. 





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




## CIMColorVisualVariable
#### Represents a color visual variable. 


### CIMVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMSymbolizers.md#cimvisualvariableauthoringinfo)|Gets and sets the authoring info. 


### CIMColorVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| expression | string|Gets and sets expression. 
| minValue | double|Gets and sets the min value. 
| maxValue | double|Gets and sets the max value. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| normalizationField | string|Gets and sets the normalization field. 
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|Gets and sets the data normalization method. 
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets ExpressionInfo that contains the Arcade expression that returns value as a number 





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
| dictionaryName | string|Gets and sets the dictionary name. 
| fieldMap | [CIMStringMap](CIMSymbolizers.md#cimstringmap) |Gets and sets the field map between expected fields and actual fields. 






## CIMDotDensityRenderer
#### Represents a dot density renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDotDensityRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| dotDensitySymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the dot density symbol. 
| dotSize | double|Gets and sets the dot size. 
| dotValue | double|Gets and sets the dot value. 
| excludeDotsFromMaskedArea | boolean|Gets and sets a boolean value indicating whether or not the exclude dots from masked areas. 
| fieldNames | IStringArray|Gets and sets the field names dot data comes from. 
| fieldLabels | IStringArray|Gets and sets the label for each selected field name. 
| fixedPlacement | boolean|Gets and sets a boolean value indicating whether or not placement is fixed. 
| maintainDensity | boolean|Gets and sets a boolean value indicating whether or not to maintain density. 
| maskingLayer | string|Gets and sets a path to the layer that supplies masks. 
| randomSeed | long|Gets and sets a random seed. 
| referenceScale | double|Gets and sets the reference scale. If specified, dots are calibrated from this scale. 
| useMasking | boolean|Gets and sets a boolean value indicating whether or not to use masking. 


### CIMDataExclusion 

|Property | Type | Description | 
|---------|--------|--------|
| exclusionClause | string|Gets and sets the exclusion clause. 
| exclusionDescription | string|Gets and sets the exclusion description. 
| exclusionLabel | string|Gets and sets the exclusion label. 
| exclusionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the exclusion symbol. 
| useExclusionSymbol | boolean|Gets and sets a boolean value indicating whether or not to use the exclusion symbol. 


### CIMVisualVariableRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariables | [CIMVisualVariable](Types.md#cimvisualvariable) |Gets and sets the visual variables. 






## CIMExpressionInfo
#### Represents the properties required for authoring an Arcade expression 


### CIMExpressionInfo 

|Property | Type | Description | 
|---------|--------|--------|
| title | string|Gets or sets the human readable text that describes the expression. 
| expression | string|Gets or sets the Arcade expression used to evaluate and return the value that a property expects. 
| name | string|Gets and sets the Name of the expression. 
| returnType | [enumeration ExpressionReturnType](CIMSymbolizers.md#enumeration-expressionreturntype)|Gets and sets the ReturnType of the expression. 





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
| colorScheme | [ColorRamp](Types.md#colorramp)|Controls how smooth the color gradient appears. Controls the color scheme of the heat map. Must be either a continuous or multipart color ramp. If no color scheme is specified, a default color ramp will be used. 
| field | string|Name of the field denoting weighting values for each feature. The field's value is the count or quantity to be spread across the landscape to create a continuous surface. Values in the field may be integer or floating point. The options for the field are listed below. Specify the name of a numeric field in the feature table Use "" if no item or special value will be used and each feature will be counted once. Use Shape if input features contains Z. 
| radius | long|Controls how far the heat spreads away from the points. Specified and stored in Points and translates to Pixels at draw time. 
| rendererQuality | long|Controls the pixilation of the raster. This is an arbitrary range that goes from Best (10) to Fastest (0). 
| heading | string|Gets and sets the legend heading. 
| minLabel | string|Gets and sets the legend label for the minimum density value. 
| maxLabel | string|Gets and sets the legend label for the maximum density value. 





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




## CIMPrimitiveOverride
#### Represents a primative override. 


### CIMPrimitiveOverride 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string|Gets and sets the primitive name this override applies to. 
| propertyName | string|Gets and sets the property name in the primative this override applies to. 
| expression | string|Gets and sets the expression. 
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets ExpressionInfo that contains the Arcade expression that returns value as a number or a string depending on the PropertyName. 






## CIMProportionalPieSizeOptions
#### Represents proportional pie size options. 


### CIMProportionalPieSizeOptions 

|Property | Type | Description | 
|---------|--------|--------|
| flanneryCompensation | boolean|Gets and sets a boolean value indicating whether or not to use Flannery compensation. 
| minimumSize | double|Gets and sets the minimum size. 
| minimumValue | double|Gets and sets the minimum value. 
| proportionalBySum | boolean|Gets and sets a boolean value indicating whether proportion by sum. 
| proportionalFieldName | string|Gets and sets the proportional field name. 






## CIMProportionalRenderer
#### Represents a proportional renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMProportionalRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets background symbol features are drawn with underneath the proportional symbols. 
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight)|Gets and sets the barrier weight used for graduate symbols to avoid labels. 
| field | string|Gets and sets the field the renderer is using. 
| flanneryCompensation | boolean|Gets and sets a boolean value indicating whether or not to use Flannery compensation. 
| legendSymbolCount | long|Gets and sets the legend symbol count. 
| maxDataValue | double|Gets and sets the max data value. 
| minDataValue | double|Gets and sets the min data value. 
| minSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the min symbol. 
| unitSymbolization | [CIMUnitSymbolization](CIMSymbolizers.md#cimunitsymbolization)|Gets and sets the unit symbolization. 
| heading | string|Gets and sets the heading. 
| useDefaultSymbol | boolean|Gets and sets a Boolean value indicating whether or not to use the default symbol. 
| defaultSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the default symbol. 
| defaultLabel | string|Gets and sets the default label. 
| defaultDescription | string|Gets and sets the default description. 
| showInAscendingOrder | boolean|Gets and sets a boolean value indicating whether or not to show classes in ascending order. 
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets ExpressionInfo that contains the Arcade expression that returns value as a number. When both Fields and ValueExpressionInfo are present ValueExpressionInfo is used. 


### CIMDataExclusion 

|Property | Type | Description | 
|---------|--------|--------|
| exclusionClause | string|Gets and sets the exclusion clause. 
| exclusionDescription | string|Gets and sets the exclusion description. 
| exclusionLabel | string|Gets and sets the exclusion label. 
| exclusionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the exclusion symbol. 
| useExclusionSymbol | boolean|Gets and sets a boolean value indicating whether or not to use the exclusion symbol. 


### CIMDataNormalization 

|Property | Type | Description | 
|---------|--------|--------|
| normalizationField | string|Gets and sets the normalization field. 
| normalizationTotal | double|Gets and sets the normalization total. 
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|Gets and sets the normalization type. 


### CIMVisualVariableRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariables | [CIMVisualVariable](Types.md#cimvisualvariable) |Gets and sets the visual variables. 






## CIMRepresentationRenderer
#### Represents a representation renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMRepresentationRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| drawInvalidRule | boolean|Gets and sets a boolean value indicating whether or not the draw invalid rules. 
| drawInvisibleRepresentation | boolean|Gets and sets a boolean value indicating whether or not the draw invisible representations. 
| invalidRuleColor | [Color](Types.md#color)|Gets and sets the invalid rule color. 
| invisibleRepresentationColor | [Color](Types.md#color)|Gets and sets the invisible representation color. 
| representationClassName | string|Gets and sets the representation class name. 
| ruleLegendVisibility | [long]|Gets and sets the rule legend visibilty. 
| symbolLayerNameMapping | [CIMRuleSymbolLayerNames](CIMSymbolizers.md#cimrulesymbollayernames) |Gets and sets the symbol layer name mapping. 






## CIMRotationVisualVariable
#### Represents a rotation visual variable. 


### CIMVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMSymbolizers.md#cimvisualvariableauthoringinfo)|Gets and sets the authoring info. 


### CIMRotationVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariableInfoX | [CIMVisualVariableInfo](CIMSymbolizers.md#cimvisualvariableinfo)|Gets and sets the visual variable info for the X dimension. 
| visualVariableInfoY | [CIMVisualVariableInfo](CIMSymbolizers.md#cimvisualvariableinfo)|Gets and sets the visual variable info for the Y dimension. 
| visualVariableInfoZ | [CIMVisualVariableInfo](CIMSymbolizers.md#cimvisualvariableinfo)|Gets and sets the visual variable info for the Z dimension. 
| rotationTypeZ | [enumeration SymbolRotationType](CIMSymbolizers.md#enumeration-symbolrotationtype)|Gets and sets the Z rotation type. 
| normalToSurface | boolean|Gets and sets a boolean value indicating the normal to surface value which applies to 3D views. If true, rotation is applied after marker is rotated normal to the 3D surface. If false, all rotations are applied starting from zeroed X, Y, Z rotation. 






## CIMRuleRenderer
#### Represents a rule renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMRuleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| rules | [CIMSymbolizationRule](CIMSymbolizers.md#cimsymbolizationrule) |Gets and sets symbolization rules. 


### CIMVisualVariableRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariables | [CIMVisualVariable](Types.md#cimvisualvariable) |Gets and sets the visual variables. 






## CIMRuleSymbolLayerNames
#### Represents rule symbol layer names. 


### CIMRuleSymbolLayerNames 

|Property | Type | Description | 
|---------|--------|--------|
| ruleID | long|Gets and sets the rule ID. 
| symbolLayerNames | IStringArray|Gets and sets the symbol layer names. 






## CIMScaleDependentSizeVariation
#### Represents the scale dependent size variations for a symbol reference. Applies to point symbols, line symbols and the outline of polygon symbols. When the symbol reference is rendered at an intermediate scale a linearly scaled size is used. 


### CIMScaleDependentSizeVariation 

|Property | Type | Description | 
|---------|--------|--------|
| scale | double|Gets and sets the scale the size is associated with. 
| size | double|Gets and sets the size for the associated scale. 






## CIMSimpleRenderer
#### Represents a simple renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMSimpleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| label | string|Gets and sets the legend label. 
| patch | [enumeration PatchShape](CIMSymbolizers.md#enumeration-patchshape)|Gets and sets the patch. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 
| alternateSymbols | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference) |Gets and sets an array of symbol references that are intended to be used at specific scale ranges. 


### CIMVisualVariableRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariables | [CIMVisualVariable](Types.md#cimvisualvariable) |Gets and sets the visual variables. 






## CIMSizeVisualVariable
#### Represents a size visual variable. VariableType = Graduated use expression, Min/Max size, Min/Max value VariableType = Proportional, unit defined use Expression, ValueUnit, ValueShape, ValueRepresentation VariableType = Proportional, unit NOT defined use Expression, MinSize, MinValue, could use MaxSize 


### CIMVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMSymbolizers.md#cimvisualvariableauthoringinfo)|Gets and sets the authoring info. 


### CIMSizeVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| expression | string|Gets and sets the expression. 
| randomMin | double|Gets and sets the random min. 
| randomMax | double|Gets and sets the random max. 
| minSize | double|Gets and sets the min size. 
| maxSize | double|Gets and sets the max size. 
| minValue | double|Gets and sets the min value. 
| maxValue | double|Gets and sets the max value. 
| valueUnits | [LinearUnit](ExternalReferences.md#linearunit)|Gets and sets the size visual variable type. 
| valueRepresentation | [enumeration ValueRepresentations](CIMSymbolizers.md#enumeration-valuerepresentations)|Gets and sets the value representations. 
| variableType | [enumeration SizeVisualVariableType](CIMSymbolizers.md#enumeration-sizevisualvariabletype)|Gets and sets size visual variable type. 
| valueShape | [enumeration SymbolShapes](CIMSymbolizers.md#enumeration-symbolshapes)|Gets and sets the value shape. 
| axis | [enumeration SizeVisualVariableAxis](CIMSymbolizers.md#enumeration-sizevisualvariableaxis)|Gets and sets size visual variable axis. 
| target | string|Gets and sets size visual variable target which specifies the portion of the symbol targeted for sizing. 
| normalizationField | string|Gets and sets the normalization field. 
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|Gets and sets the data normalization method. 
| sizeValues | [double]|Gets and sets the size values that correspond to data values. 
| dataValues | [double]|Gets and sets the data values. 
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets ExpressionInfo that contains the Arcade expression that returns value as a number 





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
| key | string|Gets and sets the key. 
| value | string|Gets and sets the value. 






## CIMSymbolReference
#### Represents a symbol reference. Symbol references currently store the symbol inline in the symbol property. Overrides here are used primarily by renderers to pass overrides through the drawing pipeline. 


### CIMSymbolReference 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveOverrides | [CIMPrimitiveOverride](CIMSymbolizers.md#cimprimitiveoverride) |Gets and sets the primative overrides. Typically set by renderers at draw time. 
| stylePath | string|Gets and sets the style path. Reserved for future use. 
| symbol | [Symbol](Types.md#symbol)|Gets and sets the symbol. 
| symbolName | string|Gets and sets the symbol name. 
| minScale | double|Gets and sets the minimum scale range the symbol refererence should be displayed at. 
| maxScale | double|Gets and sets the maximum scale range the symbol refererence should be displayed at. 
| scaleDependentSizeVariation | [CIMScaleDependentSizeVariation](CIMSymbolizers.md#cimscaledependentsizevariation) |Gets and sets an array of scale dependent sizes. 
| minDistance | double|Gets and sets the minimum distance at which symbols are visible. Objects closer than this don't get rendered. 
| maxDistance | double|Gets and sets the maximum distance at which symbols are visible. Objects beyond this point don't get rendered. 





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




## CIMSymbolizationRule
#### Represents a symbolization rule. 


### CIMSymbolizationRule 

|Property | Type | Description | 
|---------|--------|--------|
| minScale | double|Gets and sets the min scale. 
| maxScale | double|Gets and sets the max scale. 
| filter | [QueryFilter](ExternalReferences.md#queryfilter)|Gets and sets the query filter. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 
| label | string|Gets and sets rule label. 
| description | string|Gets and sets the description. 






## CIMTransparencyVisualVariable
#### Represents a transparency visual variable. 


### CIMVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMSymbolizers.md#cimvisualvariableauthoringinfo)|Gets and sets the authoring info. 


### CIMTransparencyVisualVariable 

|Property | Type | Description | 
|---------|--------|--------|
| field | string|Gets and sets the field to base the transparency on. 
| transparencyValues | [double]|Gets and sets the transparency values that correspond to data values. 
| dataValues | [double]|Gets and sets the data values. 
| normalizationField | string|Gets and sets the normalization field. 
| normalizationTotal | double|Gets and sets the normalization total. 
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|Gets and sets the normalization method. 
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets ExpressionInfo that contains the Arcade expression that returns value as a number 






## CIMUniqueValue
#### Represents a unique value. 


### CIMUniqueValue 

|Property | Type | Description | 
|---------|--------|--------|
| fieldValues | IStringArray|Gets and sets the field values. 






## CIMUniqueValueClass
#### Represents a unique value class. 


### CIMUniqueValueClass 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| editable | boolean|Gets and sets a boolean value indicating if this class is editable. 
| label | string|Gets and sets the label. 
| patch | [enumeration PatchShape](CIMSymbolizers.md#enumeration-patchshape)|Gets and sets the patch. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 
| values | [CIMUniqueValue](CIMSymbolizers.md#cimuniquevalue) |Gets and sets the values this class corresponds to. 
| visible | boolean|Gets and sets a boolean value indicating if this class is visible. 
| alternateSymbols | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference) |Gets and sets an array of symbol references that are intended to be used at specific scale ranges. 






## CIMUniqueValueGroup
#### Represents a unique value group. 


### CIMUniqueValueGroup 

|Property | Type | Description | 
|---------|--------|--------|
| classes | [CIMUniqueValueClass](CIMSymbolizers.md#cimuniquevalueclass) |Gets and sets the classes belonging to the group. 
| heading | string|Gets and sets the heading. 






## CIMUniqueValueRenderer
#### Represents a unique value renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| defaultDescription | string|Gets and sets the default description. 
| defaultLabel | string|Gets and sets the default label. 
| defaultSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the default symbol. 
| fields | IStringArray|Gets and sets the fields used by this renderer. 
| groups | [CIMUniqueValueGroup](CIMSymbolizers.md#cimuniquevaluegroup) |Gets and sets the unique value groups. 
| useDefaultSymbol | boolean|Gets and sets a boolean option indicating whether of not to use the default symbol. 
| styleGallery | string|Gets and sets the style item name for the color ramp. 
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets ExpressionInfo that contains the Arcade expression that returns value as a string. When both Fields and ValueExpressionInfo are present ValueExpressionInfo is used. 


### CIMVisualVariableRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| visualVariables | [CIMVisualVariable](Types.md#cimvisualvariable) |Gets and sets the visual variables. 






## CIMUnitSymbolization
#### Represents unit symbolization. 


### CIMUnitSymbolization 

|Property | Type | Description | 
|---------|--------|--------|
| valueRepresentation | [enumeration ValueRepresentations](CIMSymbolizers.md#enumeration-valuerepresentations)|Gets and sets the value representation. 
| valueUnit | [LinearUnit](ExternalReferences.md#linearunit)|Gets and sets the value unit. 
| symbolShape | [enumeration SymbolShapes](CIMSymbolizers.md#enumeration-symbolshapes)|Gets and sets the symbol shape. 





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
| minSliderValue | double|Gets and sets the min value. 
| maxSliderValue | double|Gets and sets the max value. 
| theme | string|Gets and sets a theme as an array of strings. 
| showLegend | boolean|Gets and sets a boolean indicating whether or not to show legends. 
| heading | string|Gets or sets the legend heading. 






## CIMVisualVariableInfo
#### Represents visual variable info. 


### CIMVisualVariableInfo 

|Property | Type | Description | 
|---------|--------|--------|
| expression | string|Gets and sets the expression. 
| randomMax | double|Gets and sets the random max. 
| randomMin | double|Gets and sets the random min. 
| visualVariableInfoType | [enumeration VisualVariableInfoType](CIMSymbolizers.md#enumeration-visualvariableinfotype)|Gets and sets the visual variable info type. 
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets ExpressionInfo that contains the Arcade expression that returns value as a number 





### Enumeration: VisualVariableInfoType
#### Visual variable info types. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| None. 
| Expression| 1| Expression 
| Random| 2| Random. 

