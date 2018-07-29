


## CIMChartRenderer
Represents chart renderer which contains properties common to all symbolizers that depict some feature value as a chart drawn on top of the feature itself.


### CIMRenderer

|Property | Type | Description |
|---------|--------|--------|


### CIMChartRenderer

|Property | Type | Description |
|---------|--------|--------|
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight)|The barrier weight for chart label collision.
| baseSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The base symbol features are drawn with.
| chartSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The chart symbol.
| fieldNames | [string,]|The field names used to populate the chart.
| fieldTotals | [number], //[double],|The field totals.
| label | string|The renderer label.
| maxValue | number //double|Max value.
| preventChartOverlap | boolean|A boolean option indicating whether or not to prevent chart overlap.
| proportionalPieSizeOptions | [CIMProportionalPieSizeOptions](CIMSymbolizers.md#cimproportionalpiesizeoptions)|The proportional pie size options.


### CIMDataExclusion

|Property | Type | Description |
|---------|--------|--------|
| exclusionClause | string|The exclusion clause.
| exclusionDescription | string|The exclusion description.
| exclusionLabel | string|The exclusion label.
| exclusionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The exclusion symbol.
| useExclusionSymbol | boolean|A boolean value indicating whether or not to use the exclusion symbol.


### CIMDataNormalization

|Property | Type | Description |
|---------|--------|--------|
| normalizationField | string|The normalization field.
| normalizationTotal | number //double|The normalization total.
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|The normalization type.






## CIMClassBreak
Represents a class break.


### CIMClassBreak

|Property | Type | Description |
|---------|--------|--------|
| criticalBreak | boolean|A boolean value indicating whether or not this is a critical break.
| description | string|The description.
| label | string|The label.
| patch | [enumeration PatchShape](CIMSymbolizers.md#enumeration-patchshape)|The patch shape for this class.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the class.
| upperBound | number //double|The upper bound of the class.
| alternateSymbols | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference) |An array of symbol references that are intended to be used at specific scale ranges.





### Enumeration: ClassBreakType
Class break types.

|Property | Value | Description |
|---------|--------|--------|
| GraduatedColor| 0| Graduated color.
| GraduatedSymbol| 1| Graduated symbol.
| UnclassedColor| 2| Unclassed color. Applies only to Polygons and Multi Patches.




## CIMClassBreaksRenderer
Represents a class break renderer.


### CIMRenderer

|Property | Type | Description |
|---------|--------|--------|


### CIMClassBreaksRenderer

|Property | Type | Description |
|---------|--------|--------|
| backgroundSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The background symbol used for graduated symbols.
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight)|The barrier weight used for graduate symbols to avoid labels.
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |The class breaks.
| classBreakType | [enumeration ClassBreakType](CIMSymbolizers.md#enumeration-classbreaktype)|The class break type.
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|The classification method.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
| field | string|The field for rendering.
| minimumBreak | number //double|The minimum break for the renderer.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format.
| showClassGaps | boolean|A boolean value indicating whether or not to show class gaps.
| showInAscendingOrder | boolean|A boolean value indicating whether or not to show classes in ascending order.
| heading | string|The heading.
| sampleSize | number //int32|The sample size used for creating the classification.
| useDefaultSymbol | boolean|A boolean value indicating whether or not to use the default symbol.
| defaultSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The default symbol.
| minimumLabel | string|The minimum label.
| defaultLabel | string|The default label.
| defaultDescription | string|The default description.
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The ExpressionInfo that contains the Arcade expression that returns value as a number. When both Fields and ValueExpressionInfo are present ValueExpressionInfo is used.


### CIMDataExclusion

|Property | Type | Description |
|---------|--------|--------|
| exclusionClause | string|The exclusion clause.
| exclusionDescription | string|The exclusion description.
| exclusionLabel | string|The exclusion label.
| exclusionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The exclusion symbol.
| useExclusionSymbol | boolean|A boolean value indicating whether or not to use the exclusion symbol.


### CIMDataNormalization

|Property | Type | Description |
|---------|--------|--------|
| normalizationField | string|The normalization field.
| normalizationTotal | number //double|The normalization total.
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|The normalization type.


### CIMVisualVariableRenderer

|Property | Type | Description |
|---------|--------|--------|
| visualVariables | [CIMVisualVariable](Types.md#cimvisualvariable) |The visual variables.





### Enumeration: ClassificationMethod
Classification methods.

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
Represents a color visual variable.


### CIMVisualVariable

|Property | Type | Description |
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMSymbolizers.md#cimvisualvariableauthoringinfo)|The authoring info.


### CIMColorVisualVariable

|Property | Type | Description |
|---------|--------|--------|
| expression | string|The expression.
| minValue | number //double|The min value.
| maxValue | number //double|The max value.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
| normalizationField | string|The normalization field.
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|The data normalization method.
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The ExpressionInfo that contains the Arcade expression that returns value as a number





### Enumeration: DataNormalizationMethod
Data normalization methods.

|Property | Value | Description |
|---------|--------|--------|
| Field| 0| Normalize by field.
| Log| 1| Log normalization.
| PercentOfTotal| 2| Percent of total.
| Nothing| 3| None.




## CIMDictionaryRenderer
Represents a dictionary renderer where symbols are drawn from a symbol dictionary.


### CIMRenderer

|Property | Type | Description |
|---------|--------|--------|


### CIMDictionaryRenderer

|Property | Type | Description |
|---------|--------|--------|
| dictionaryName | string|The dictionary name.
| fieldMap | [CIMStringMap](CIMSymbolizers.md#cimstringmap) |The field map between expected fields and actual fields.






## CIMDotDensityRenderer
Represents a dot density renderer.


### CIMRenderer

|Property | Type | Description |
|---------|--------|--------|


### CIMDotDensityRenderer

|Property | Type | Description |
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
| dotDensitySymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The dot density symbol.
| dotSize | number //double|The dot size.
| dotValue | number //double|The dot value.
| excludeDotsFromMaskedArea | boolean|A boolean value indicating whether or not the exclude dots from masked areas.
| fieldNames | [string,]|The field names dot data comes from.
| fieldLabels | [string,]|The label for each selected field name.
| fixedPlacement | boolean|A boolean value indicating whether or not placement is fixed.
| maintainDensity | boolean|A boolean value indicating whether or not to maintain density.
| maskingLayer | string|A path to the layer that supplies masks.
| randomSeed | number //int32|A random seed.
| referenceScale | number //double|The reference scale. If specified, dots are calibrated from this scale.
| useMasking | boolean|A boolean value indicating whether or not to use masking.


### CIMDataExclusion

|Property | Type | Description |
|---------|--------|--------|
| exclusionClause | string|The exclusion clause.
| exclusionDescription | string|The exclusion description.
| exclusionLabel | string|The exclusion label.
| exclusionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The exclusion symbol.
| useExclusionSymbol | boolean|A boolean value indicating whether or not to use the exclusion symbol.


### CIMVisualVariableRenderer

|Property | Type | Description |
|---------|--------|--------|
| visualVariables | [CIMVisualVariable](Types.md#cimvisualvariable) |The visual variables.






## CIMExpressionInfo
Represents the properties required for authoring an Arcade expression


### CIMExpressionInfo

|Property | Type | Description |
|---------|--------|--------|
| title | string|The human readable text that describes the expression.
| expression | string|The Arcade expression used to evaluate and return the value that a property expects.
| name | string|The Name of the expression.
| returnType | [enumeration ExpressionReturnType](CIMSymbolizers.md#enumeration-expressionreturntype)|The ReturnType of the expression.





### Enumeration: ExpressionReturnType
Visual variable info types.

|Property | Value | Description |
|---------|--------|--------|
| Default| 0| The return type of the expression is determined by the consumer using the expression.
| String| 1| The return type of the expression is treated as a string by all consumers.
| Numeric| 2| The return type of the expression is treated as a numeric value by all consumers.




## CIMHeatMapRenderer
Represents a heat map renderer. The Heat Map Renderer draws point features as a continuous color gradient representing the density of the points. The resulting density surface represents the physical proximity between points, optionally weighted by a specified attribute value. The displayed raster surface is dynamic and morphs according to the zoom level and updates if the source point features are edited.


### CIMRenderer

|Property | Type | Description |
|---------|--------|--------|


### CIMHeatMapRenderer

|Property | Type | Description |
|---------|--------|--------|
| colorScheme | [ColorRamp](Types.md#colorramp)|Controls how smooth the color gradient appears. Controls the color scheme of the heat map. Must be either a continuous or multipart color ramp. If no color scheme is specified, a default color ramp will be used.
| field | string|Name of the field denoting weighting values for each feature. The field's value is the count or quantity to be spread across the landscape to create a continuous surface. Values in the field may be integer or number //floating point. The options for the field are listed below. Specify the name of a numeric field in the feature table Use "" if no item or special value will be used and each feature will be counted once. Use Shape if input features contains Z.
| radius | number //int32|Controls how far the heat spreads away from the points. Specified and stored in Points and translates to Pixels at draw time.
| rendererQuality | number //int32|Controls the pixilation of the raster. This is an arbitrary range that goes from Best (10) to Fastest (0).
| heading | string|The legend heading.
| minLabel | string|The legend label for the minimum density value.
| maxLabel | string|The legend label for the maximum density value.





### Enumeration: PatchShape
Patch shapes.

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
Represents a primative override.


### CIMPrimitiveOverride

|Property | Type | Description |
|---------|--------|--------|
| primitiveName | string|The primitive name this override applies to.
| propertyName | string|The property name in the primative this override applies to.
| expression | string|The expression.
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The ExpressionInfo that contains the Arcade expression that returns value as a number or a string depending on the PropertyName.






## CIMProportionalPieSizeOptions
Represents proportional pie size options.


### CIMProportionalPieSizeOptions

|Property | Type | Description |
|---------|--------|--------|
| flanneryCompensation | boolean|A boolean value indicating whether or not to use Flannery compensation.
| minimumSize | number //double|The minimum size.
| minimumValue | number //double|The minimum value.
| proportionalBySum | boolean|A boolean value indicating whether proportion by sum.
| proportionalFieldName | string|The proportional field name.






## CIMProportionalRenderer
Represents a proportional renderer.


### CIMRenderer

|Property | Type | Description |
|---------|--------|--------|


### CIMProportionalRenderer

|Property | Type | Description |
|---------|--------|--------|
| backgroundSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The background symbol features are drawn with underneath the proportional symbols.
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight)|The barrier weight used for graduate symbols to avoid labels.
| field | string|The field the renderer is using.
| flanneryCompensation | boolean|A boolean value indicating whether or not to use Flannery compensation.
| legendSymbolCount | number //int32|The legend symbol count.
| maxDataValue | number //double|The max data value.
| minDataValue | number //double|The min data value.
| minSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The min symbol.
| unitSymbolization | [CIMUnitSymbolization](CIMSymbolizers.md#cimunitsymbolization)|The unit symbolization.
| heading | string|The heading.
| useDefaultSymbol | boolean|A Boolean value indicating whether or not to use the default symbol.
| defaultSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The default symbol.
| defaultLabel | string|The default label.
| defaultDescription | string|The default description.
| showInAscendingOrder | boolean|A boolean value indicating whether or not to show classes in ascending order.
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The ExpressionInfo that contains the Arcade expression that returns value as a number. When both Fields and ValueExpressionInfo are present ValueExpressionInfo is used.


### CIMDataExclusion

|Property | Type | Description |
|---------|--------|--------|
| exclusionClause | string|The exclusion clause.
| exclusionDescription | string|The exclusion description.
| exclusionLabel | string|The exclusion label.
| exclusionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The exclusion symbol.
| useExclusionSymbol | boolean|A boolean value indicating whether or not to use the exclusion symbol.


### CIMDataNormalization

|Property | Type | Description |
|---------|--------|--------|
| normalizationField | string|The normalization field.
| normalizationTotal | number //double|The normalization total.
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|The normalization type.


### CIMVisualVariableRenderer

|Property | Type | Description |
|---------|--------|--------|
| visualVariables | [CIMVisualVariable](Types.md#cimvisualvariable) |The visual variables.






## CIMRepresentationRenderer
Represents a representation renderer.


### CIMRenderer

|Property | Type | Description |
|---------|--------|--------|


### CIMRepresentationRenderer

|Property | Type | Description |
|---------|--------|--------|
| drawInvalidRule | boolean|A boolean value indicating whether or not the draw invalid rules.
| drawInvisibleRepresentation | boolean|A boolean value indicating whether or not the draw invisible representations.
| invalidRuleColor | [Color](Types.md#color)|The invalid rule color.
| invisibleRepresentationColor | [Color](Types.md#color)|The invisible representation color.
| representationClassName | string|The representation class name.
| ruleLegendVisibility | [long]|The rule legend visibilty.
| symbolLayerNameMapping | [CIMRuleSymbolLayerNames](CIMSymbolizers.md#cimrulesymbollayernames) |The symbol layer name mapping.






## CIMRotationVisualVariable
Represents a rotation visual variable.


### CIMVisualVariable

|Property | Type | Description |
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMSymbolizers.md#cimvisualvariableauthoringinfo)|The authoring info.


### CIMRotationVisualVariable

|Property | Type | Description |
|---------|--------|--------|
| visualVariableInfoX | [CIMVisualVariableInfo](CIMSymbolizers.md#cimvisualvariableinfo)|The visual variable info for the X dimension.
| visualVariableInfoY | [CIMVisualVariableInfo](CIMSymbolizers.md#cimvisualvariableinfo)|The visual variable info for the Y dimension.
| visualVariableInfoZ | [CIMVisualVariableInfo](CIMSymbolizers.md#cimvisualvariableinfo)|The visual variable info for the Z dimension.
| rotationTypeZ | [enumeration SymbolRotationType](CIMSymbolizers.md#enumeration-symbolrotationtype)|The Z rotation type.
| normalToSurface | boolean|A boolean value indicating the normal to surface value which applies to 3D views. If true, rotation is applied after marker is rotated normal to the 3D surface. If false, all rotations are applied starting from zeroed X, Y, Z rotation.






## CIMRuleRenderer
Represents a rule renderer.


### CIMRenderer

|Property | Type | Description |
|---------|--------|--------|


### CIMRuleRenderer

|Property | Type | Description |
|---------|--------|--------|
| rules | [CIMSymbolizationRule](CIMSymbolizers.md#cimsymbolizationrule) |The symbolization rules.


### CIMVisualVariableRenderer

|Property | Type | Description |
|---------|--------|--------|
| visualVariables | [CIMVisualVariable](Types.md#cimvisualvariable) |The visual variables.






## CIMRuleSymbolLayerNames
Represents rule symbol layer names.


### CIMRuleSymbolLayerNames

|Property | Type | Description |
|---------|--------|--------|
| ruleID | number //int32|The rule ID.
| symbolLayerNames | [string,]|The symbol layer names.






## CIMScaleDependentSizeVariation
Represents the scale dependent size variations for a symbol reference. Applies to point symbols, line symbols and the outline of polygon symbols. When the symbol reference is rendered at an intermediate scale a linearly scaled size is used.


### CIMScaleDependentSizeVariation

|Property | Type | Description |
|---------|--------|--------|
| scale | number //double|The scale the size is associated with.
| size | number //double|The size for the associated scale.






## CIMSimpleRenderer
Represents a simple renderer.


### CIMRenderer

|Property | Type | Description |
|---------|--------|--------|


### CIMSimpleRenderer

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| label | string|The legend label.
| patch | [enumeration PatchShape](CIMSymbolizers.md#enumeration-patchshape)|The patch.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.
| alternateSymbols | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference) |An array of symbol references that are intended to be used at specific scale ranges.


### CIMVisualVariableRenderer

|Property | Type | Description |
|---------|--------|--------|
| visualVariables | [CIMVisualVariable](Types.md#cimvisualvariable) |The visual variables.






## CIMSizeVisualVariable
Represents a size visual variable. VariableType = Graduated use expression, Min/Max size, Min/Max value VariableType = Proportional, unit defined use Expression, ValueUnit, ValueShape, ValueRepresentation VariableType = Proportional, unit NOT defined use Expression, MinSize, MinValue, could use MaxSize


### CIMVisualVariable

|Property | Type | Description |
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMSymbolizers.md#cimvisualvariableauthoringinfo)|The authoring info.


### CIMSizeVisualVariable

|Property | Type | Description |
|---------|--------|--------|
| expression | string|The expression.
| randomMin | number //double|The random min.
| randomMax | number //double|The random max.
| minSize | number //double|The min size.
| maxSize | number //double|The max size.
| minValue | number //double|The min value.
| maxValue | number //double|The max value.
| valueUnits | [LinearUnit](ExternalReferences.md#linearunit)|The size visual variable type.
| valueRepresentation | [enumeration ValueRepresentations](CIMSymbolizers.md#enumeration-valuerepresentations)|The value representations.
| variableType | [enumeration SizeVisualVariableType](CIMSymbolizers.md#enumeration-sizevisualvariabletype)|The size visual variable type.
| valueShape | [enumeration SymbolShapes](CIMSymbolizers.md#enumeration-symbolshapes)|The value shape.
| axis | [enumeration SizeVisualVariableAxis](CIMSymbolizers.md#enumeration-sizevisualvariableaxis)|The size visual variable axis.
| target | string|The size visual variable target which specifies the portion of the symbol targeted for sizing.
| normalizationField | string|The normalization field.
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|The data normalization method.
| sizeValues | [number], //[double],|The size values that correspond to data values.
| dataValues | [number], //[double],|The data values.
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The ExpressionInfo that contains the Arcade expression that returns value as a number





### Enumeration: SizeVisualVariableAxis
Size visual variable axis.

|Property | Value | Description |
|---------|--------|--------|
| HeightAxis| 0| Height axis: interpreted as Z for 3D markers, Y for billboarded
| WidthAxis| 1| Width axis.
| DepthAxis| 2| Depth axis.
| WidthAndDepthAxes| 3| Width and depth axes.
| AllAxes| 4| All axes.



### Enumeration: SizeVisualVariableType
Size visual variable type.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| None.
| Expression| 1| Expression.
| Random| 2| Random.
| Proportional| 3| Proportional.
| Graduated| 4| Graduated.




## CIMStringMap
Represents a string map of key value pairs.


### CIMStringMap

|Property | Type | Description |
|---------|--------|--------|
| key | string|The key.
| value | string|The value.






## CIMSymbolReference
Represents a symbol reference. Symbol references currently store the symbol inline in the symbol property. Overrides here are used primarily by renderers to pass overrides through the drawing pipeline.


### CIMSymbolReference

|Property | Type | Description |
|---------|--------|--------|
| primitiveOverrides | [CIMPrimitiveOverride](CIMSymbolizers.md#cimprimitiveoverride) |The primative overrides. Typically set by renderers at draw time.
| stylePath | string|The style path. Reserved for future use.
| symbol | [Symbol](Types.md#symbol)|The symbol.
| symbolName | string|The symbol name.
| minScale | number //double|The minimum scale range the symbol refererence should be displayed at.
| maxScale | number //double|The maximum scale range the symbol refererence should be displayed at.
| scaleDependentSizeVariation | [CIMScaleDependentSizeVariation](CIMSymbolizers.md#cimscaledependentsizevariation) |An array of scale dependent sizes.
| minDistance | number //double|The minimum distance at which symbols are visible. Objects closer than this don't get rendered.
| maxDistance | number //double|The maximum distance at which symbols are visible. Objects beyond this point don't get rendered.





### Enumeration: SymbolRotationType
Symbol rotation types.

|Property | Value | Description |
|---------|--------|--------|
| Geographic| 0| Geographic.
| Arithmetic| 1| Arithmetic.



### Enumeration: SymbolShapes
Symbol shapes.

|Property | Value | Description |
|---------|--------|--------|
| Unknown| 0| Unknown shape.
| Circle| 1| Circle shape.
| Square| 2| Square shape.




## CIMSymbolizationRule
Represents a symbolization rule.


### CIMSymbolizationRule

|Property | Type | Description |
|---------|--------|--------|
| minScale | number //double|The min scale.
| maxScale | number //double|The max scale.
| filter | [QueryFilter](ExternalReferences.md#queryfilter)|The query filter.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.
| label | string|The rule label.
| description | string|The description.






## CIMTransparencyVisualVariable
Represents a transparency visual variable.


### CIMVisualVariable

|Property | Type | Description |
|---------|--------|--------|
| authoringInfo | [CIMVisualVariableAuthoringInfo](CIMSymbolizers.md#cimvisualvariableauthoringinfo)|The authoring info.


### CIMTransparencyVisualVariable

|Property | Type | Description |
|---------|--------|--------|
| field | string|The field to base the transparency on.
| transparencyValues | [number], //[double],|The transparency values that correspond to data values.
| dataValues | [number], //[double],|The data values.
| normalizationField | string|The normalization field.
| normalizationTotal | number //double|The normalization total.
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|The normalization method.
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The ExpressionInfo that contains the Arcade expression that returns value as a number






## CIMUniqueValue
Represents a unique value.


### CIMUniqueValue

|Property | Type | Description |
|---------|--------|--------|
| fieldValues | [string,]|The field values.






## CIMUniqueValueClass
Represents a unique value class.


### CIMUniqueValueClass

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| editable | boolean|A boolean value indicating if this class is editable.
| label | string|The label.
| patch | [enumeration PatchShape](CIMSymbolizers.md#enumeration-patchshape)|The patch.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.
| values | [CIMUniqueValue](CIMSymbolizers.md#cimuniquevalue) |The values this class corresponds to.
| visible | boolean|A boolean value indicating if this class is visible.
| alternateSymbols | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference) |An array of symbol references that are intended to be used at specific scale ranges.






## CIMUniqueValueGroup
Represents a unique value group.


### CIMUniqueValueGroup

|Property | Type | Description |
|---------|--------|--------|
| classes | [CIMUniqueValueClass](CIMSymbolizers.md#cimuniquevalueclass) |The classes belonging to the group.
| heading | string|The heading.






## CIMUniqueValueRenderer
Represents a unique value renderer.


### CIMRenderer

|Property | Type | Description |
|---------|--------|--------|


### CIMUniqueValueRenderer

|Property | Type | Description |
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
| defaultDescription | string|The default description.
| defaultLabel | string|The default label.
| defaultSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The default symbol.
| fields | [string,]|The fields used by this renderer.
| groups | [CIMUniqueValueGroup](CIMSymbolizers.md#cimuniquevaluegroup) |The unique value groups.
| useDefaultSymbol | boolean|A boolean option indicating whether of not to use the default symbol.
| styleGallery | string|The style item name for the color ramp.
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The ExpressionInfo that contains the Arcade expression that returns value as a string. When both Fields and ValueExpressionInfo are present ValueExpressionInfo is used.


### CIMVisualVariableRenderer

|Property | Type | Description |
|---------|--------|--------|
| visualVariables | [CIMVisualVariable](Types.md#cimvisualvariable) |The visual variables.






## CIMUnitSymbolization
Represents unit symbolization.


### CIMUnitSymbolization

|Property | Type | Description |
|---------|--------|--------|
| valueRepresentation | [enumeration ValueRepresentations](CIMSymbolizers.md#enumeration-valuerepresentations)|The value representation.
| valueUnit | [LinearUnit](ExternalReferences.md#linearunit)|The value unit.
| symbolShape | [enumeration SymbolShapes](CIMSymbolizers.md#enumeration-symbolshapes)|The symbol shape.





### Enumeration: ValueRepresentations
Represents value representations.

|Property | Value | Description |
|---------|--------|--------|
| Radius| 0| Radius.
| Area| 1| Area.
| Distance| 2| Distance.
| Width| 3| Width.




## CIMVisualVariableAuthoringInfo
Represents visual variable metadata used for authoring.


### CIMVisualVariableAuthoringInfo

|Property | Type | Description |
|---------|--------|--------|
| minSliderValue | number //double|The min value.
| maxSliderValue | number //double|The max value.
| theme | string|A theme as an array of strings.
| showLegend | boolean|A boolean indicating whether or not to show legends.
| heading | string|The legend heading.






## CIMVisualVariableInfo
Represents visual variable info.


### CIMVisualVariableInfo

|Property | Type | Description |
|---------|--------|--------|
| expression | string|The expression.
| randomMax | number //double|The random max.
| randomMin | number //double|The random min.
| visualVariableInfoType | [enumeration VisualVariableInfoType](CIMSymbolizers.md#enumeration-visualvariableinfotype)|The visual variable info type.
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|The ExpressionInfo that contains the Arcade expression that returns value as a number





### Enumeration: VisualVariableInfoType
Visual variable info types.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| None.
| Expression| 1| Expression
| Random| 2| Random.
