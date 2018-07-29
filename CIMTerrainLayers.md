


## CIMColorClassBreak
Represents a color class break.


### CIMColorClassBreak

|Property | Type | Description |
|---------|--------|--------|
| upperBound | number //double|The upper bound for the color class break.
| label | string|The label for the color class break.
| description | string|The description for the color class break.
| color | [Color](Types.md#color)|The color for the color class break.






## CIMColorModulationInfo
Indicates whether modulation should be used to render the point. Low modulation values will darken the point color.


### CIMColorModulationInfo

|Property | Type | Description |
|---------|--------|--------|
| field | string|The attribute to use as a source for the color modulation.
| minValue | number //double|Minimum value to compute modulation on linear scale based on field value.
| maxValue | number //double|Maximum value to compute modulation on linear scale based on field value.






## CIMColorUniqueValue
Represents a color unique value.


### CIMColorUniqueValue

|Property | Type | Description |
|---------|--------|--------|
| value | string|The class value as a string.
| label | string|The class label.
| description | string|The class description.
| color | [Color](Types.md#color)|The class color.






## CIMLASDatasetLayer
Represents a LAS dataset layer.


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


### CIMLASDatasetLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| analysisToolsResolution | number //double|The analysis tool resolution.
| dataConnection | [DataConnection](Types.md#dataconnection)|The data connection to the LAS dataset.
| displayField | string|The display field.
| fileExtentSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The file extent symbol.
| fileNameSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The file name symbol.
| fullResolutionScale | number //double|The full resolution scale.
| isFlattened | boolean|A boolean value indicating if this layer is flattened.
| LASDatasetFilter | [LasFilter](ExternalReferences.md#lasfilter)|The LAS dataset filter.
| maintainCurrentSurface | boolean|A boolean value indicating if the current surface should be maintained.
| pointBudget | number //int32|The point budget.
| pointCountPerCentimeter | number //int32|The point count per centimeter.
| renderers | [CIMTinRenderer](Types.md#cimtinrenderer) |The renderers.
| scaleSymbols | boolean|A boolean value indicating whether to scale symbols.
| showFileExtent | boolean|A boolean value indicating whether to show the file extent.
| showFileName | boolean|A boolean value indicating whether to show the file name.
| showResolution | boolean|A boolean value indicating whether to show the resolution.
| useFullResolutionScale | boolean|A boolean value indicating whether to use the full resolution scale.
| selectable | boolean|A boolean option indicating whether the layer is selectable.






## CIMLASPointElevationRenderer
Represents a LAS point elevation renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTerrainAttributeRenderer

|Property | Type | Description |
|---------|--------|--------|
| attributeFieldName | string|An attribute field name.
| embeddedDataSources | [long]|The embedded data sources.


### CIMTinColorRampRenderer

|Property | Type | Description |
|---------|--------|--------|
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |The class breaks.
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|The classification method.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype)|The cursor type.
| description | string|The description.
| label | string|The label.
| minimumBreak | number //double|The minimum break.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format.
| showClassGaps | boolean|A boolean value indicating if class gaps should be shown.
| sortClassesAscending | boolean|A boolean value indicating if class are ascending.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The base symbol.


### CIMLASPointElevationRenderer

|Property | Type | Description |
|---------|--------|--------|
| modulateIntensity | boolean|A boolean value indicating whether to modulate intensity.
| pointSplatter | [CIMLASPointSplatter](CIMTerrainLayers.md#cimlaspointsplatter)|The point splatter properties.
| useSplat | boolean|A boolean value indicating whether to use the splat technique.
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo)|Color modulation.






## CIMLASPointSplatter
Represents a LAS point splatter.


### CIMLASPointSplatter

|Property | Type | Description |
|---------|--------|--------|
| splatMinimumSize | number //double|The splat minimum size.
| splatScale | number //double|The splat scale.
| useSplatHighlight | boolean|A boolean value indicating whether to use splat highlighting.





### Enumeration: LASStretchAttribute
LAS stretch attributes.

|Property | Value | Description |
|---------|--------|--------|
| Elevation| 0| Elevation.
| RGB| 1| RGB.
| Red| 2| Red.
| Green| 3| Green.
| Blue| 4| Blue.
| NearInfrared| 5| Near infrared.
| Intensity| 6| Intensity.
| ScanAngle| 7| Scan angle.
| GPSTime| 8| GPS time.
| None| 9| None.




## CIMLASStretchClass
Represents a LAS stretch class.


### CIMLASStretchClass

|Property | Type | Description |
|---------|--------|--------|
| label | string|The class label.
| value | number //double|The class value.





### Enumeration: LASStretchDrawingType
LAS stretch drawing type.

|Property | Value | Description |
|---------|--------|--------|
| Symbol| 0| Symbol.
| Splat| 1| Splat.
| SymbolTint| 2| Symbol tint.




## CIMLASStretchInput
Represents LAS stretch input.


### CIMLASStretchInput

|Property | Type | Description |
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp), *(Flags: [Display2D_Only])*|The color ramp.
| stretchMax | number //double|The stretch max.
| stretchMin | double, *(Flags: [Display2D_Only])*|The stretch min.
| gammaValue | double, *(Flags: [Display2D_Only])*|The gamma value.
| invert | boolean|A boolean value indicating whether to invert the stretch.
| lookup | [long]|The lookup values.
| maxPercent | double, *(Flags: [Display2D_Only])*|The max percent.
| minPercent | double, *(Flags: [Display2D_Only])*|The min percent.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format.
| standardDeviationParam | double, *(Flags: [Display2D_Only])*|The standard deviation parameter.
| statsType | [enumeration LASStretchStatsType](CIMTerrainLayers.md#enumeration-lasstretchstatstype)|The LAS stats type.
| stretchAttribute | [enumeration LASStretchAttribute](CIMTerrainLayers.md#enumeration-lasstretchattribute)|The LAS stretch attribute.
| stretchClasses | [CIMLASStretchClass](CIMTerrainLayers.md#cimlasstretchclass) |The stretch classes.
| stretchStats | [StatsHistogram](ExternalReferences.md#statshistogram)|The stretch statistics.
| stretchType | [enumeration LASStretchType](CIMTerrainLayers.md#enumeration-lasstretchtype)|The stretch type.
| useCustomStretchMinMax | boolean|A boolean value indicating whether to use custom stretch min max.
| useGammaStretch | boolean, *(Flags: [Display2D_Only])*|A boolean value indicating whether to use gamma stretch.






## CIMLASStretchRenderer
Represents a LAS stretch renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTerrainAttributeRenderer

|Property | Type | Description |
|---------|--------|--------|
| attributeFieldName | string|An attribute field name.
| embeddedDataSources | [long]|The embedded data sources.


### CIMLASStretchRenderer

|Property | Type | Description |
|---------|--------|--------|
| modulationInput | [CIMLASStretchInput](CIMTerrainLayers.md#cimlasstretchinput)|The modulation input.
| modulationWeight | number //double|The modulation weight.
| pointSplatter | [CIMLASPointSplatter](CIMTerrainLayers.md#cimlaspointsplatter), *(Flags: [Display2D_Only])*|The point splatter.
| stretchDrawingType | [enumeration LASStretchDrawingType](CIMTerrainLayers.md#enumeration-lasstretchdrawingtype), *(Flags: [Display2D_Only])*|The stretch drawing type.
| stretchSourceInput | [CIMLASStretchInput](CIMTerrainLayers.md#cimlasstretchinput), *(Flags: [Display2D_Only])*|The stretch source input.
| tintSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The tint symbol.
| useModulation | boolean|A boolean value indicating whether to use modulation.
| useSplat | boolean, *(Flags: [Display2D_Only])*|A boolean value indicating whether to use the splat technique.
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo)|Color modulation.





### Enumeration: LASStretchStatsType
LAS stretch statistic types.

|Property | Value | Description |
|---------|--------|--------|
| AreaOfView| 0| Area of view.
| Dataset| 1| Entire dataset.
| GlobalStats| 2| Global statistics.



### Enumeration: LASStretchType
LAS stretch types.

|Property | Value | Description |
|---------|--------|--------|
| DefaultFromSource| 0| Default from source.
| Custom| 1| Custom.
| MinimumMaximum| 2| Minimum Maximum.
| StandardDeviations| 3| Standard deviations.
| Histogram| 4| Histogram.
| PercentMinMax| 5| Percent min max.




## CIMLASUniqueValueRenderer
Represents a LAS unique value renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTerrainAttributeRenderer

|Property | Type | Description |
|---------|--------|--------|
| attributeFieldName | string|An attribute field name.
| embeddedDataSources | [long]|The embedded data sources.


### CIMTinUniqueValueRenderer

|Property | Type | Description |
|---------|--------|--------|
| colorScheme | string|The color ramp name.
| description | string|The description.
| groups | [CIMUniqueValueGroup](CIMSymbolizers.md#cimuniquevaluegroup) |The unique value groups.
| heading | string|The heading.
| label | string|The label.
| lookupStyleset | string|The lookup styleset.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.
| useDefaultSymbol | boolean|A boolean value indicating whether or not to use the default symbol.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.


### CIMLASUniqueValueRenderer

|Property | Type | Description |
|---------|--------|--------|
| attribute | number //int32|The attribute index.
| modulateIntensity | boolean|A boolean indicating whether or not to modulate intensity.
| pointSplatter | [CIMLASPointSplatter](CIMTerrainLayers.md#cimlaspointsplatter), *(Flags: [Display2D_Only])*|The point splatter properties.
| useSplat | boolean, *(Flags: [Display2D_Only])*|A boolean indicating whether or not to use the splat technique.
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo), *(Flags: [Display2D_Only])*|Color modulation.






## CIMPointCloudBitFieldFilter
Represents a point cloud bit field filter. Filters based on the bit-wise representation of the provided field. For a point to be retained, its attribute field bits must match BitsToSet and BitsToClear. Bits which are not explicitly clear nor set, are ignored.


### CIMPointCloudFilter

|Property | Type | Description |
|---------|--------|--------|
| field | string|The field used for the filter.


### CIMPointCloudBitFieldFilter

|Property | Type | Description |
|---------|--------|--------|
| requiredSetBits | [long]|Array of bit numbers set. Bit 0 is the least significant bit.
| requiredClearBits | [long]|Array of bit numbers cleared. Bit 0 is the least significant bit.






## CIMPointCloudClassBreaksRenderer
Represents a point cloud class breaks renderer.


### CIMPointCloudRenderer

|Property | Type | Description |
|---------|--------|--------|
| pointShape | [enumeration PointCloudShapeType](CIMTerrainLayers.md#enumeration-pointcloudshapetype)|The symbol type.
| pointSizeAlgorithm | [CIMPointCloudAlgorithm](CIMTerrainLayers.md#cimpointcloudalgorithm)|The algorithm used to determine the symbol size.
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo)|The filter used to filter the points being drawn.
| fieldTransformType | [enumeration PointCloudFieldTransformType](CIMTerrainLayers.md#enumeration-pointcloudfieldtransformtype)|The field transform type.
| field | string|The field used to render the points.


### CIMPointCloudClassBreaksRenderer

|Property | Type | Description |
|---------|--------|--------|
| breaks | [CIMColorClassBreak](CIMTerrainLayers.md#cimcolorclassbreak) |The color class breaks of the renderer.





### Enumeration: PointCloudFieldTransformType
Point cloud field transform types.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| Do not transform field values.
| LowFourBit| 1| Apply 0xF mask to field values.
| HighFourBit| 2| Bitwise shift field values to the right by 4.
| AbsoluteValue| 3| Apply abs() to field values.
| ModuloTen| 4| Modulate field values by 10.




## CIMPointCloudFixedSizeAlgorithm
Represents a point cloud fixed size algorithm.


### CIMPointCloudSizeAlgorithm

|Property | Type | Description |
|---------|--------|--------|


### CIMPointCloudFixedSizeAlgorithm

|Property | Type | Description |
|---------|--------|--------|
| useRealWorldSymbolSizes | boolean|A boolean option indicating whether to use real world symbols sizes (meters) vs. points.
| size | number //double|The size of the symbols.






## CIMPointCloudLayer
Represents a point cloud layer.


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


### CIMPointCloudLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| renderer | [PointCloudRenderer](Types.md#pointcloudrenderer)|The symbol renderer.
| dataConnection | [CIMSceneDataConnection](CIMTerrainLayers.md#cimscenedataconnection)|The data connection.
| pointsPerInch | number //double|The double value that determins the number of points to draw per display inch.
| pointsBudget | number //int32|The double value to determine the upper limit on the number of points drawn.
| filters | [CIMPointCloudFilter](Types.md#cimpointcloudfilter) |The filter used to filter the points being drawn.
| snappable | boolean|A boolean option indicating whether this layer participates in snapping in the editor.






## CIMPointCloudRGBRenderer
Represents a point cloud RGB renderer.


### CIMPointCloudRenderer

|Property | Type | Description |
|---------|--------|--------|
| pointShape | [enumeration PointCloudShapeType](CIMTerrainLayers.md#enumeration-pointcloudshapetype)|The symbol type.
| pointSizeAlgorithm | [CIMPointCloudAlgorithm](CIMTerrainLayers.md#cimpointcloudalgorithm)|The algorithm used to determine the symbol size.
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo)|The filter used to filter the points being drawn.
| fieldTransformType | [enumeration PointCloudFieldTransformType](CIMTerrainLayers.md#enumeration-pointcloudfieldtransformtype)|The field transform type.
| field | string|The field used to render the points.


### CIMPointCloudRGBRenderer

|Property | Type | Description |
|---------|--------|--------|






## CIMPointCloudReturnFilter
Represents a point cloud return filter.


### CIMPointCloudFilter

|Property | Type | Description |
|---------|--------|--------|
| field | string|The field used for the filter.


### CIMPointCloudReturnFilter

|Property | Type | Description |
|---------|--------|--------|
| includedReturnsBitmask | number //int32|The binary combination of PointCouldReturnType enum flags.





### Enumeration: PointCloudReturnType
Point cloud return types.

|Property | Value | Description |
|---------|--------|--------|
| Last| 1| Show last return only.
| FirstOfMany| 2| Show first return of multi-return only.
| LastOfMany| 4| Show last return of multi-return only.
| Single| 8| Show single return only.
| All| -1| No return filtering.



### Enumeration: PointCloudShapeType
Point cloud shape types.

|Property | Value | Description |
|---------|--------|--------|
| DiskFlat| 0| Disk shaped symbol with no shading.
| DiskShaded| 1| Disk shaped symbol with shading.




## CIMPointCloudSplatAlgorithm
Represents a point cloud splat algorithm.


### CIMPointCloudSizeAlgorithm

|Property | Type | Description |
|---------|--------|--------|


### CIMPointCloudSplatAlgorithm

|Property | Type | Description |
|---------|--------|--------|
| scaleFactor | number //double|The scale factor used to compute the point size.
| minSize | number //double|The miniumum point size.






## CIMPointCloudStretchRenderer
Represents a point cloud stretch renderer.


### CIMPointCloudRenderer

|Property | Type | Description |
|---------|--------|--------|
| pointShape | [enumeration PointCloudShapeType](CIMTerrainLayers.md#enumeration-pointcloudshapetype)|The symbol type.
| pointSizeAlgorithm | [CIMPointCloudAlgorithm](CIMTerrainLayers.md#cimpointcloudalgorithm)|The algorithm used to determine the symbol size.
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo)|The filter used to filter the points being drawn.
| fieldTransformType | [enumeration PointCloudFieldTransformType](CIMTerrainLayers.md#enumeration-pointcloudfieldtransformtype)|The field transform type.
| field | string|The field used to render the points.


### CIMPointCloudStretchRenderer

|Property | Type | Description |
|---------|--------|--------|
| rangeMin | number //double|The minimum value used to compute the linear mapping of the renderer.
| rangeMax | number //double|The maximum value used to compute the linear mapping of the renderer.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp of the renderer.






## CIMPointCloudUniqueValueRenderer
Represents a point cloud unique value renderer.


### CIMPointCloudRenderer

|Property | Type | Description |
|---------|--------|--------|
| pointShape | [enumeration PointCloudShapeType](CIMTerrainLayers.md#enumeration-pointcloudshapetype)|The symbol type.
| pointSizeAlgorithm | [CIMPointCloudAlgorithm](CIMTerrainLayers.md#cimpointcloudalgorithm)|The algorithm used to determine the symbol size.
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo)|The filter used to filter the points being drawn.
| fieldTransformType | [enumeration PointCloudFieldTransformType](CIMTerrainLayers.md#enumeration-pointcloudfieldtransformtype)|The field transform type.
| field | string|The field used to render the points.


### CIMPointCloudUniqueValueRenderer

|Property | Type | Description |
|---------|--------|--------|
| classes | [CIMColorUniqueValue](CIMTerrainLayers.md#cimcoloruniquevalue) |The unique color classes of the renderer.






## CIMPointCloudValueFilter
Represents a point cloud value filter. Filter points based on the value of an specified attribute.


### CIMPointCloudFilter

|Property | Type | Description |
|---------|--------|--------|
| field | string|The field used for the filter.


### CIMPointCloudValueFilter

|Property | Type | Description |
|---------|--------|--------|
| values | [number], //[double],|The values used as exclude or include list.
| mode | [enumeration PointCloudValueFilterMode](CIMTerrainLayers.md#enumeration-pointcloudvaluefiltermode)|The mode that determines if the ValueList is an include list or an exclude list.





### Enumeration: PointCloudValueFilterMode
Point cloud value filter modes.

|Property | Value | Description |
|---------|--------|--------|
| Exclude| 0| List of values in the exclude list
| Include| 1| List of values in the include list




## CIMSceneDataConnection
Represents a scene data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMSceneDataConnection

|Property | Type | Description |
|---------|--------|--------|
| URI | string|The URI.






## CIMTerrainDirtyAreaRenderer
Represents a terrain dirty area renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTinSimpleRenderer

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| label | string|The label.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.





### Enumeration: TerrainDrawCursorType
Terrain draw cursor types.

|Property | Value | Description |
|---------|--------|--------|
| Composite| 0| Composite.
| NodeSimple| 1| Simple node.
| NodeValue| 2| Value node.
| NodeElevation| 3| Elevation node.
| EdgeSimple| 4| Simple edge.
| EdgeType| 5| Edge type.
| FaceSimple| 6| Simple face.
| FaceElevation| 7| Elevation face.
| FaceSlope| 8| Slope face.
| FaceAspect| 9| Aspect face.
| FaceValue| 10| Value face.
| TerrainPointElevation| 11| Terrain point elevation.
| TerrainPointAttributeGraduated| 12| Terrain point graduated attribute.
| TerrainPointAttributeUnique| 13| Terrain point unique attribute.
| TerrainDirtyArea| 14| Terrain dirty area.




## CIMTerrainLayer
Represents a terrain layer. A terrain layer draws a terrain dataset. A terrain dataset is a specialized data structure in the geodatabase that represents terrain surfaces based on vector measurements.


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


### CIMTerrainLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| analysisToolsResolution | number //double|The resolution use by analysis tools.
| autoLOR | boolean|A boolean value indicating whether or not LOR should be updated when scale changes.
| currentResolution | number //double|The current resolution.
| dataConnection | [DataConnection](Types.md#dataconnection)|The data connection.
| displayField | string|The display field.
| lockCurrentSurface | boolean|A boolean value indicating if current surface should be updated based on scale change.
| pointBudget | number //int32|The point budget.
| pyramidHonored | boolean|A boolean value indicating if current surface resolution honors the scale/resolution relationship in the pyramin definition.
| scaleSymbols | boolean|A boolean value indicating if symbols should be scaled.
| showResolution | boolean|A boolean value indicating if the resolution should be shown in the contents pane.
| renderers | [CIMTinRenderer](Types.md#cimtinrenderer) |The renderers.
| targetResolution | number //double|The target resolution.
| useOverviewTerrain | boolean|A boolean value indicating if the terrain overview should be used.
| usePointBudget | boolean|A boolean value indicating if the point budget should be used.






## CIMTerrainPointAttributeGraduatedRenderer
Represents a terrain point attribute graduated renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTerrainAttributeRenderer

|Property | Type | Description |
|---------|--------|--------|
| attributeFieldName | string|An attribute field name.
| embeddedDataSources | [long]|The embedded data sources.


### CIMTinColorRampRenderer

|Property | Type | Description |
|---------|--------|--------|
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |The class breaks.
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|The classification method.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype)|The cursor type.
| description | string|The description.
| label | string|The label.
| minimumBreak | number //double|The minimum break.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format.
| showClassGaps | boolean|A boolean value indicating if class gaps should be shown.
| sortClassesAscending | boolean|A boolean value indicating if class are ascending.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The base symbol.






## CIMTerrainPointAttributeUniqueRenderer
Represents a terrain point attribute unique renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTerrainAttributeRenderer

|Property | Type | Description |
|---------|--------|--------|
| attributeFieldName | string|An attribute field name.
| embeddedDataSources | [long]|The embedded data sources.


### CIMTinUniqueValueRenderer

|Property | Type | Description |
|---------|--------|--------|
| colorScheme | string|The color ramp name.
| description | string|The description.
| groups | [CIMUniqueValueGroup](CIMSymbolizers.md#cimuniquevaluegroup) |The unique value groups.
| heading | string|The heading.
| label | string|The label.
| lookupStyleset | string|The lookup styleset.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.
| useDefaultSymbol | boolean|A boolean value indicating whether or not to use the default symbol.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.






## CIMTerrainPointElevationRenderer
Represents a terrain point elevation renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTerrainAttributeRenderer

|Property | Type | Description |
|---------|--------|--------|
| attributeFieldName | string|An attribute field name.
| embeddedDataSources | [long]|The embedded data sources.


### CIMTinColorRampRenderer

|Property | Type | Description |
|---------|--------|--------|
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |The class breaks.
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|The classification method.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype)|The cursor type.
| description | string|The description.
| label | string|The label.
| minimumBreak | number //double|The minimum break.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format.
| showClassGaps | boolean|A boolean value indicating if class gaps should be shown.
| sortClassesAscending | boolean|A boolean value indicating if class are ascending.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The base symbol.






## CIMTinBreaklineRenderer
Represents a TIN breakline renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTerrainAttributeRenderer

|Property | Type | Description |
|---------|--------|--------|
| attributeFieldName | string|An attribute field name.
| embeddedDataSources | [long]|The embedded data sources.


### CIMTinUniqueValueRenderer

|Property | Type | Description |
|---------|--------|--------|
| colorScheme | string|The color ramp name.
| description | string|The description.
| groups | [CIMUniqueValueGroup](CIMSymbolizers.md#cimuniquevaluegroup) |The unique value groups.
| heading | string|The heading.
| label | string|The label.
| lookupStyleset | string|The lookup styleset.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.
| useDefaultSymbol | boolean|A boolean value indicating whether or not to use the default symbol.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.






## CIMTinContourRenderer
Represents a TIN contour renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTinContourRenderer

|Property | Type | Description |
|---------|--------|--------|
| contourDescription | string|The contour description.
| contourInterval | number //double|The contour interval.
| contourLabel | string|The contour label.
| contourSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The contour symbol.
| indexContourDescription | string|The index contour description.
| indexContourFactor | number //int32|The index contour factor.
| indexContourLabel | string|The index contour label.
| indexContourSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The index contour symbol.
| referenceContourHeight | number //double|The reference contour height.






## CIMTinEdgeRenderer
Represents a TIN edge renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTinSimpleRenderer

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| label | string|The label.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.






## CIMTinFaceClassBreaksRenderer
Represents a TIN face class breaks renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTerrainAttributeRenderer

|Property | Type | Description |
|---------|--------|--------|
| attributeFieldName | string|An attribute field name.
| embeddedDataSources | [long]|The embedded data sources.


### CIMTinColorRampRenderer

|Property | Type | Description |
|---------|--------|--------|
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |The class breaks.
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|The classification method.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype)|The cursor type.
| description | string|The description.
| label | string|The label.
| minimumBreak | number //double|The minimum break.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format.
| showClassGaps | boolean|A boolean value indicating if class gaps should be shown.
| sortClassesAscending | boolean|A boolean value indicating if class are ascending.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The base symbol.






## CIMTinFaceRenderer
Represents a TIN face renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTinSimpleRenderer

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| label | string|The label.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.






## CIMTinFaceValueRenderer
Represents a TIN face value renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTerrainAttributeRenderer

|Property | Type | Description |
|---------|--------|--------|
| attributeFieldName | string|An attribute field name.
| embeddedDataSources | [long]|The embedded data sources.


### CIMTinUniqueValueRenderer

|Property | Type | Description |
|---------|--------|--------|
| colorScheme | string|The color ramp name.
| description | string|The description.
| groups | [CIMUniqueValueGroup](CIMSymbolizers.md#cimuniquevaluegroup) |The unique value groups.
| heading | string|The heading.
| label | string|The label.
| lookupStyleset | string|The lookup styleset.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.
| useDefaultSymbol | boolean|A boolean value indicating whether or not to use the default symbol.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.






## CIMTinLayer
Represents a TIN layer which displays TIN data sources, a data structure that represents terrain data as a triangulated irregular network.


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


### CIMTinLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|The data connection.
| displayField | string|The display field.
| renderers | [CIMTinRenderer](Types.md#cimtinrenderer) |The renderers.
| scaleSymbols | boolean|A boolean value indicating whether or not to scale symbols.






## CIMTinNodeElevationRenderer
Represents a TIN node elevation renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTerrainAttributeRenderer

|Property | Type | Description |
|---------|--------|--------|
| attributeFieldName | string|An attribute field name.
| embeddedDataSources | [long]|The embedded data sources.


### CIMTinColorRampRenderer

|Property | Type | Description |
|---------|--------|--------|
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |The class breaks.
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|The classification method.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype)|The cursor type.
| description | string|The description.
| label | string|The label.
| minimumBreak | number //double|The minimum break.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format.
| showClassGaps | boolean|A boolean value indicating if class gaps should be shown.
| sortClassesAscending | boolean|A boolean value indicating if class are ascending.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The base symbol.






## CIMTinNodeRenderer
Represents a TIN node renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTinSimpleRenderer

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| label | string|The label.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.






## CIMTinNodeValueRenderer
Represents a TIN node value renderer.


### CIMTinRenderer

|Property | Type | Description |
|---------|--------|--------|
| illuminate | boolean|A boolean value indicating whether or not to illuminate.


### CIMTerrainAttributeRenderer

|Property | Type | Description |
|---------|--------|--------|
| attributeFieldName | string|An attribute field name.
| embeddedDataSources | [long]|The embedded data sources.


### CIMTinUniqueValueRenderer

|Property | Type | Description |
|---------|--------|--------|
| colorScheme | string|The color ramp name.
| description | string|The description.
| groups | [CIMUniqueValueGroup](CIMSymbolizers.md#cimuniquevaluegroup) |The unique value groups.
| heading | string|The heading.
| label | string|The label.
| lookupStyleset | string|The lookup styleset.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.
| useDefaultSymbol | boolean|A boolean value indicating whether or not to use the default symbol.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
