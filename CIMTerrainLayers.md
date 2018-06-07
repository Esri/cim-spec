


## CIMColorClassBreak
#### Represents a color class break. 


### CIMColorClassBreak 

|Property | Type | Description | 
|---------|--------|--------|
| upperBound | double|Gets and sets the upper bound for the color class break. 
| label | string|Gets and sets the label for the color class break. 
| description | string|Gets and sets the description for the color class break. 
| color | [Color](Types.md#color)|Gets and sets the color for the color class break. 






## CIMColorModulationInfo
#### Indicates whether modulation should be used to render the point. Low modulation values will darken the point color. 


### CIMColorModulationInfo 

|Property | Type | Description | 
|---------|--------|--------|
| field | string|The attribute to use as a source for the color modulation. 
| minValue | double|Minimum value to compute modulation on linear scale based on field value. 
| maxValue | double|Maximum value to compute modulation on linear scale based on field value. 






## CIMColorUniqueValue
#### Represents a color unique value. 


### CIMColorUniqueValue 

|Property | Type | Description | 
|---------|--------|--------|
| value | string|Gets and sets the class value as a string. 
| label | string|Gets and sets the class label. 
| description | string|Gets and sets the class description. 
| color | [Color](Types.md#color)|Gets and sets the class color. 






## CIMLASDatasetLayer
#### Represents a LAS dataset layer. 


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


### CIMLASDatasetLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| analysisToolsResolution | double|Gets and sets the analysis tool resolution. 
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection to the LAS dataset. 
| displayField | string|Gets and sets the display field. 
| fileExtentSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the file extent symbol. 
| fileNameSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the file name symbol. 
| fullResolutionScale | double|Gets and sets the full resolution scale. 
| isFlattened | boolean|Gets and sets a boolean value indicating if this layer is flattened. 
| LASDatasetFilter | [LasFilter](ExternalReferences.md#lasfilter)|Gets and sets the LAS dataset filter. 
| maintainCurrentSurface | boolean|Gets and sets a boolean value indicating if the current surface should be maintained. 
| pointBudget | long|Gets and sets the point budget. 
| pointCountPerCentimeter | long|Gets and sets the point count per centimeter. 
| renderers | [CIMTinRenderer](Types.md#cimtinrenderer) |Gets and sets the renderers. 
| scaleSymbols | bool|Gets and sets a boolean value indicating whether to scale symbols. 
| showFileExtent | boolean|Gets and sets a boolean value indicating whether to show the file extent. 
| showFileName | boolean|Gets and sets a boolean value indicating whether to show the file name. 
| showResolution | boolean|Gets and sets a boolean value indicating whether to show the resolution. 
| useFullResolutionScale | boolean|Gets and sets a boolean value indicating whether to use the full resolution scale. 
| selectable | boolean|Gets and sets a boolean option indicating whether the layer is selectable. 






## CIMLASPointElevationRenderer
#### Represents a LAS point elevation renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string|Gets and sets an attribute field name. 
| embeddedDataSources | [long]|Gets and sets embedded data sources. 


### CIMTinColorRampRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |Gets and sets the class breaks. 
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|Gets and sets the classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype)|Gets and sets the cursor type. 
| description | string|Gets and sets the description. 
| label | string|Gets and sets the label. 
| minimumBreak | double|Gets and sets the minimum break. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format. 
| showClassGaps | boolean|Gets and sets a boolean value indicating if class gaps should be shown. 
| sortClassesAscending | boolean|Gets and sets a boolean value indicating if class are ascending. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the base symbol. 


### CIMLASPointElevationRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| modulateIntensity | boolean|Gets and sets a boolean value indicating whether to modulate intensity. 
| pointSplatter | [CIMLASPointSplatter](CIMTerrainLayers.md#cimlaspointsplatter)|Gets and sets the point splatter properties. 
| useSplat | boolean|Gets and sets a boolean value indicating whether to use the splat technique. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo)|Gets and sets color modulation. 






## CIMLASPointSplatter
#### Represents a LAS point splatter. 


### CIMLASPointSplatter 

|Property | Type | Description | 
|---------|--------|--------|
| splatMinimumSize | double|Gets and sets splat minimum size. 
| splatScale | double|Gets and sets splat scale. 
| useSplatHighlight | boolean|Gets and sets a boolean value indicating whether to use splat highlighting. 





### Enumeration: LASStretchAttribute
#### LAS stretch attributes. 

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
#### Represents a LAS stretch class. 


### CIMLASStretchClass 

|Property | Type | Description | 
|---------|--------|--------|
| label | string|Gets and sets the class label. 
| value | double|Gets and sets the class value. 





### Enumeration: LASStretchDrawingType
#### LAS stretch drawing type. 

|Property | Value | Description | 
|---------|--------|--------|
| Symbol| 0| Symbol. 
| Splat| 1| Splat. 
| SymbolTint| 2| Symbol tint. 




## CIMLASStretchInput
#### Represents LAS stretch input. 


### CIMLASStretchInput 

|Property | Type | Description | 
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp), *(Flags: [Display2D_Only])*|Gets and sets the color ramp. 
| stretchMax | double|Gets and sets the stretch max. 
| stretchMin | double, *(Flags: [Display2D_Only])*|Gets and sets the stretch min. 
| gammaValue | double, *(Flags: [Display2D_Only])*|Gets and sets the gamma value. 
| invert | boolean|Gets and sets a boolean value indicating whether to invert the stretch. 
| lookup | [long]|Gets and sets the lookup values. 
| maxPercent | double, *(Flags: [Display2D_Only])*|Gets and sets the max percent. 
| minPercent | double, *(Flags: [Display2D_Only])*|Gets and sets the min percent. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format. 
| standardDeviationParam | double, *(Flags: [Display2D_Only])*|Gets and sets the standard deviation parameter. 
| statsType | [enumeration LASStretchStatsType](CIMTerrainLayers.md#enumeration-lasstretchstatstype)|Gets and sets the LAS stats type. 
| stretchAttribute | [enumeration LASStretchAttribute](CIMTerrainLayers.md#enumeration-lasstretchattribute)|Gets and sets the LAS stretch attribute. 
| stretchClasses | [CIMLASStretchClass](CIMTerrainLayers.md#cimlasstretchclass) |Gets and sets the stretch classes. 
| stretchStats | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the stretch statistics. 
| stretchType | [enumeration LASStretchType](CIMTerrainLayers.md#enumeration-lasstretchtype)|Gets and sets the stretch type. 
| useCustomStretchMinMax | boolean|Gets and sets a boolean value indicating whether to use custom stretch min max. 
| useGammaStretch | boolean, *(Flags: [Display2D_Only])*|Gets and sets a boolean value indicating whether to use gamma stretch. 






## CIMLASStretchRenderer
#### Represents a LAS stretch renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string|Gets and sets an attribute field name. 
| embeddedDataSources | [long]|Gets and sets embedded data sources. 


### CIMLASStretchRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| modulationInput | [CIMLASStretchInput](CIMTerrainLayers.md#cimlasstretchinput)|Gets and sets the modulation input. 
| modulationWeight | double|Gets and sets the modulation weight. 
| pointSplatter | [CIMLASPointSplatter](CIMTerrainLayers.md#cimlaspointsplatter), *(Flags: [Display2D_Only])*|Gets and sets the point splatter. 
| stretchDrawingType | [enumeration LASStretchDrawingType](CIMTerrainLayers.md#enumeration-lasstretchdrawingtype), *(Flags: [Display2D_Only])*|Gets and sets the stretch drawing type. 
| stretchSourceInput | [CIMLASStretchInput](CIMTerrainLayers.md#cimlasstretchinput), *(Flags: [Display2D_Only])*|Gets and sets the stretch source input. 
| tintSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the tint symbol. 
| useModulation | boolean|Gets and sets a boolean value indicating whether to use modulation. 
| useSplat | boolean, *(Flags: [Display2D_Only])*|Gets and sets a boolean value indicating whether to use the splat technique. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo)|Gets and sets color modulation. 





### Enumeration: LASStretchStatsType
#### LAS stretch statistic types. 

|Property | Value | Description | 
|---------|--------|--------|
| AreaOfView| 0| Area of view. 
| Dataset| 1| Entire dataset. 
| GlobalStats| 2| Global statistics. 



### Enumeration: LASStretchType
#### LAS stretch types. 

|Property | Value | Description | 
|---------|--------|--------|
| DefaultFromSource| 0| Default from source. 
| Custom| 1| Custom. 
| MinimumMaximum| 2| Minimum Maximum. 
| StandardDeviations| 3| Standard deviations. 
| Histogram| 4| Histogram. 
| PercentMinMax| 5| Percent min max. 




## CIMLASUniqueValueRenderer
#### Represents a LAS unique value renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string|Gets and sets an attribute field name. 
| embeddedDataSources | [long]|Gets and sets embedded data sources. 


### CIMTinUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorScheme | string|Gets and sets the color ramp name. 
| description | string|Gets and sets the description. 
| groups | [CIMUniqueValueGroup](CIMSymbolizers.md#cimuniquevaluegroup) |Gets and sets the unique value groups. 
| heading | string|Gets and sets the heading. 
| label | string|Gets and sets the label. 
| lookupStyleset | string|Gets and sets the lookup styleset. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 
| useDefaultSymbol | boolean|Gets and sets a boolean value indicating whether or not to use the default symbol. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 


### CIMLASUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attribute | long|Gets and sets the attribute index. 
| modulateIntensity | boolean|Gets and sets a boolean indicating whether or not to modulate intensity. 
| pointSplatter | [CIMLASPointSplatter](CIMTerrainLayers.md#cimlaspointsplatter), *(Flags: [Display2D_Only])*|Gets and sets point splatter properties. 
| useSplat | boolean, *(Flags: [Display2D_Only])*|Gets and sets a boolean indicating whether or not to use the splat technique. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo), *(Flags: [Display2D_Only])*|Gets and sets color modulation. 






## CIMPointCloudBitFieldFilter
#### Represents a point cloud bit field filter. Filters based on the bit-wise representation of the provided field. For a point to be retained, its attribute field bits must match BitsToSet and BitsToClear. Bits which are not explicitly clear nor set, are ignored. 


### CIMPointCloudFilter 

|Property | Type | Description | 
|---------|--------|--------|
| field | string|Gets and sets the field used for the filter. 


### CIMPointCloudBitFieldFilter 

|Property | Type | Description | 
|---------|--------|--------|
| requiredSetBits | [long]|Array of bit numbers set. Bit 0 is the least significant bit. 
| requiredClearBits | [long]|Array of bit numbers cleared. Bit 0 is the least significant bit. 






## CIMPointCloudClassBreaksRenderer
#### Represents a point cloud class breaks renderer. 


### CIMPointCloudRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| pointShape | [enumeration PointCloudShapeType](CIMTerrainLayers.md#enumeration-pointcloudshapetype)|Gets and sets the symbol type. 
| pointSizeAlgorithm | [CIMPointCloudAlgorithm](CIMTerrainLayers.md#cimpointcloudalgorithm)|Gets and sets the algorithm used to determine the symbol size. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo)|Gets and sets the filter used to filter the points being drawn. 
| fieldTransformType | [enumeration PointCloudFieldTransformType](CIMTerrainLayers.md#enumeration-pointcloudfieldtransformtype)|Gets and sets the field transform type. 
| field | string|Gets and sets the field used to render the points. 


### CIMPointCloudClassBreaksRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [CIMColorClassBreak](CIMTerrainLayers.md#cimcolorclassbreak) |Gets and sets the color class breaks of the renderer. 





### Enumeration: PointCloudFieldTransformType
#### Point cloud field transform types. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Do not transform field values. 
| LowFourBit| 1| Apply 0xF mask to field values. 
| HighFourBit| 2| Bitwise shift field values to the right by 4. 
| AbsoluteValue| 3| Apply abs() to field values. 
| ModuloTen| 4| Modulate field values by 10. 




## CIMPointCloudFixedSizeAlgorithm
#### Represents a point cloud fixed size algorithm. 


### CIMPointCloudSizeAlgorithm 

|Property | Type | Description | 
|---------|--------|--------|


### CIMPointCloudFixedSizeAlgorithm 

|Property | Type | Description | 
|---------|--------|--------|
| useRealWorldSymbolSizes | boolean|Gets and sets a boolean option indicating whether to use real world symbols sizes (meters) vs. points. 
| size | double|Gets and sets the size of the symbols. 






## CIMPointCloudLayer
#### Represents a point cloud layer. 


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


### CIMPointCloudLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| renderer | [PointCloudRenderer](Types.md#pointcloudrenderer)|Gets and sets the symbol renderer. 
| dataConnection | [CIMSceneDataConnection](CIMTerrainLayers.md#cimscenedataconnection)|Gets and sets the data connection. 
| pointsPerInch | double|Gets and sets the double value that determins the number of points to draw per display inch. 
| pointsBudget | long|Gets and sets the double value to determine the upper limit on the number of points drawn. 
| filters | [CIMPointCloudFilter](Types.md#cimpointcloudfilter) |Gets and sets the filter used to filter the points being drawn. 
| snappable | boolean|Gets and sets a boolean option indicating whether this layer participates in snapping in the editor. 






## CIMPointCloudRGBRenderer
#### Represents a point cloud RGB renderer. 


### CIMPointCloudRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| pointShape | [enumeration PointCloudShapeType](CIMTerrainLayers.md#enumeration-pointcloudshapetype)|Gets and sets the symbol type. 
| pointSizeAlgorithm | [CIMPointCloudAlgorithm](CIMTerrainLayers.md#cimpointcloudalgorithm)|Gets and sets the algorithm used to determine the symbol size. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo)|Gets and sets the filter used to filter the points being drawn. 
| fieldTransformType | [enumeration PointCloudFieldTransformType](CIMTerrainLayers.md#enumeration-pointcloudfieldtransformtype)|Gets and sets the field transform type. 
| field | string|Gets and sets the field used to render the points. 


### CIMPointCloudRGBRenderer 

|Property | Type | Description | 
|---------|--------|--------|






## CIMPointCloudReturnFilter
#### Represents a point cloud return filter. 


### CIMPointCloudFilter 

|Property | Type | Description | 
|---------|--------|--------|
| field | string|Gets and sets the field used for the filter. 


### CIMPointCloudReturnFilter 

|Property | Type | Description | 
|---------|--------|--------|
| includedReturnsBitmask | long|Gets and sets the binary combination of PointCouldReturnType enum flags. 





### Enumeration: PointCloudReturnType
#### Point cloud return types. 

|Property | Value | Description | 
|---------|--------|--------|
| Last| 1| Show last return only. 
| FirstOfMany| 2| Show first return of multi-return only. 
| LastOfMany| 4| Show last return of multi-return only. 
| Single| 8| Show single return only. 
| All| -1| No return filtering. 



### Enumeration: PointCloudShapeType
#### Point cloud shape types. 

|Property | Value | Description | 
|---------|--------|--------|
| DiskFlat| 0| Disk shaped symbol with no shading. 
| DiskShaded| 1| Disk shaped symbol with shading. 




## CIMPointCloudSplatAlgorithm
#### Represents a point cloud splat algorithm. 


### CIMPointCloudSizeAlgorithm 

|Property | Type | Description | 
|---------|--------|--------|


### CIMPointCloudSplatAlgorithm 

|Property | Type | Description | 
|---------|--------|--------|
| scaleFactor | double|Gets and sets the scale factor used to compute the point size. 
| minSize | double|Gets and sets the miniumum point size. 






## CIMPointCloudStretchRenderer
#### Represents a point cloud stretch renderer. 


### CIMPointCloudRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| pointShape | [enumeration PointCloudShapeType](CIMTerrainLayers.md#enumeration-pointcloudshapetype)|Gets and sets the symbol type. 
| pointSizeAlgorithm | [CIMPointCloudAlgorithm](CIMTerrainLayers.md#cimpointcloudalgorithm)|Gets and sets the algorithm used to determine the symbol size. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo)|Gets and sets the filter used to filter the points being drawn. 
| fieldTransformType | [enumeration PointCloudFieldTransformType](CIMTerrainLayers.md#enumeration-pointcloudfieldtransformtype)|Gets and sets the field transform type. 
| field | string|Gets and sets the field used to render the points. 


### CIMPointCloudStretchRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| rangeMin | double|Gets and sets the minimum value used to compute the linear mapping of the renderer. 
| rangeMax | double|Gets and sets the maximum value used to compute the linear mapping of the renderer. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp of the renderer. 






## CIMPointCloudUniqueValueRenderer
#### Represents a point cloud unique value renderer. 


### CIMPointCloudRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| pointShape | [enumeration PointCloudShapeType](CIMTerrainLayers.md#enumeration-pointcloudshapetype)|Gets and sets the symbol type. 
| pointSizeAlgorithm | [CIMPointCloudAlgorithm](CIMTerrainLayers.md#cimpointcloudalgorithm)|Gets and sets the algorithm used to determine the symbol size. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo)|Gets and sets the filter used to filter the points being drawn. 
| fieldTransformType | [enumeration PointCloudFieldTransformType](CIMTerrainLayers.md#enumeration-pointcloudfieldtransformtype)|Gets and sets the field transform type. 
| field | string|Gets and sets the field used to render the points. 


### CIMPointCloudUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| classes | [CIMColorUniqueValue](CIMTerrainLayers.md#cimcoloruniquevalue) |Gets and sets the unique color classes of the renderer. 






## CIMPointCloudValueFilter
#### Represents a point cloud value filter. Filter points based on the value of an specified attribute. 


### CIMPointCloudFilter 

|Property | Type | Description | 
|---------|--------|--------|
| field | string|Gets and sets the field used for the filter. 


### CIMPointCloudValueFilter 

|Property | Type | Description | 
|---------|--------|--------|
| values | [double]|Gets and sets the values used as exclude or include list. 
| mode | [enumeration PointCloudValueFilterMode](CIMTerrainLayers.md#enumeration-pointcloudvaluefiltermode)|Gets and sets the mode that determines if the ValueList is an include list or an exclude list. 





### Enumeration: PointCloudValueFilterMode
#### Point cloud value filter modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Exclude| 0| List of values in the exclude list 
| Include| 1| List of values in the include list 




## CIMSceneDataConnection
#### Represents a scene data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMSceneDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string|Gets and sets the URI. 






## CIMTerrainDirtyAreaRenderer
#### Represents a terrain dirty area renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTinSimpleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| label | string|Gets and sets the label. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 





### Enumeration: TerrainDrawCursorType
#### Terrain draw cursor types. 

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
#### Represents a terrain layer. A terrain layer draws a terrain dataset. A terrain dataset is a specialized data structure in the geodatabase that represents terrain surfaces based on vector measurements. 


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


### CIMTerrainLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| analysisToolsResolution | double|Gets and sets the resolution use by analysis tools. 
| autoLOR | boolean|Gets and sets a boolean value indicating whether or not LOR should be updated when scale changes. 
| currentResolution | double|Gets and sets the current resolution. 
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection. 
| displayField | string|Gets and sets the display field. 
| lockCurrentSurface | boolean|Gets and sets a boolean value indicating if current surface should be updated based on scale change. 
| pointBudget | long|Gets and sets the point budget. 
| pyramidHonored | boolean|Gets and sets a boolean value indicating if current surface resolution honors the scale/resolution relationship in the pyramin definition. 
| scaleSymbols | boolean|Gets and sets a boolean value indicating if symbols should be scaled. 
| showResolution | boolean|Gets and sets a boolean value indicating if the resolution should be shown in the contents pane. 
| renderers | [CIMTinRenderer](Types.md#cimtinrenderer) |Gets and sets the renderers. 
| targetResolution | double|Gets and sets the target resolution. 
| useOverviewTerrain | boolean|Gets and sets a boolean value indicating if the terrain overview should be used. 
| usePointBudget | boolean|Gets and sets a boolean value indicating if the point budget should be used. 






## CIMTerrainPointAttributeGraduatedRenderer
#### Represents a terrain point attribute graduated renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string|Gets and sets an attribute field name. 
| embeddedDataSources | [long]|Gets and sets embedded data sources. 


### CIMTinColorRampRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |Gets and sets the class breaks. 
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|Gets and sets the classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype)|Gets and sets the cursor type. 
| description | string|Gets and sets the description. 
| label | string|Gets and sets the label. 
| minimumBreak | double|Gets and sets the minimum break. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format. 
| showClassGaps | boolean|Gets and sets a boolean value indicating if class gaps should be shown. 
| sortClassesAscending | boolean|Gets and sets a boolean value indicating if class are ascending. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the base symbol. 






## CIMTerrainPointAttributeUniqueRenderer
#### Represents a terrain point attribute unique renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string|Gets and sets an attribute field name. 
| embeddedDataSources | [long]|Gets and sets embedded data sources. 


### CIMTinUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorScheme | string|Gets and sets the color ramp name. 
| description | string|Gets and sets the description. 
| groups | [CIMUniqueValueGroup](CIMSymbolizers.md#cimuniquevaluegroup) |Gets and sets the unique value groups. 
| heading | string|Gets and sets the heading. 
| label | string|Gets and sets the label. 
| lookupStyleset | string|Gets and sets the lookup styleset. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 
| useDefaultSymbol | boolean|Gets and sets a boolean value indicating whether or not to use the default symbol. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 






## CIMTerrainPointElevationRenderer
#### Represents a terrain point elevation renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string|Gets and sets an attribute field name. 
| embeddedDataSources | [long]|Gets and sets embedded data sources. 


### CIMTinColorRampRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |Gets and sets the class breaks. 
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|Gets and sets the classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype)|Gets and sets the cursor type. 
| description | string|Gets and sets the description. 
| label | string|Gets and sets the label. 
| minimumBreak | double|Gets and sets the minimum break. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format. 
| showClassGaps | boolean|Gets and sets a boolean value indicating if class gaps should be shown. 
| sortClassesAscending | boolean|Gets and sets a boolean value indicating if class are ascending. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the base symbol. 






## CIMTinBreaklineRenderer
#### Represents a TIN breakline renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string|Gets and sets an attribute field name. 
| embeddedDataSources | [long]|Gets and sets embedded data sources. 


### CIMTinUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorScheme | string|Gets and sets the color ramp name. 
| description | string|Gets and sets the description. 
| groups | [CIMUniqueValueGroup](CIMSymbolizers.md#cimuniquevaluegroup) |Gets and sets the unique value groups. 
| heading | string|Gets and sets the heading. 
| label | string|Gets and sets the label. 
| lookupStyleset | string|Gets and sets the lookup styleset. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 
| useDefaultSymbol | boolean|Gets and sets a boolean value indicating whether or not to use the default symbol. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 






## CIMTinContourRenderer
#### Represents a TIN contour renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTinContourRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| contourDescription | string|Gets and sets the contour description. 
| contourInterval | double|Gets and sets the contour interval. 
| contourLabel | string|Gets and sets the contour label. 
| contourSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the contour symbol. 
| indexContourDescription | string|Gets and sets the index contour description. 
| indexContourFactor | long|Gets and sets the index contour factor. 
| indexContourLabel | string|Gets and sets the index contour label. 
| indexContourSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the index contour symbol. 
| referenceContourHeight | double|Gets and sets the reference contour height. 






## CIMTinEdgeRenderer
#### Represents a TIN edge renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTinSimpleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| label | string|Gets and sets the label. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 






## CIMTinFaceClassBreaksRenderer
#### Represents a TIN face class breaks renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string|Gets and sets an attribute field name. 
| embeddedDataSources | [long]|Gets and sets embedded data sources. 


### CIMTinColorRampRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |Gets and sets the class breaks. 
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|Gets and sets the classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype)|Gets and sets the cursor type. 
| description | string|Gets and sets the description. 
| label | string|Gets and sets the label. 
| minimumBreak | double|Gets and sets the minimum break. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format. 
| showClassGaps | boolean|Gets and sets a boolean value indicating if class gaps should be shown. 
| sortClassesAscending | boolean|Gets and sets a boolean value indicating if class are ascending. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the base symbol. 






## CIMTinFaceRenderer
#### Represents a TIN face renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTinSimpleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| label | string|Gets and sets the label. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 






## CIMTinFaceValueRenderer
#### Represents a TIN face value renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string|Gets and sets an attribute field name. 
| embeddedDataSources | [long]|Gets and sets embedded data sources. 


### CIMTinUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorScheme | string|Gets and sets the color ramp name. 
| description | string|Gets and sets the description. 
| groups | [CIMUniqueValueGroup](CIMSymbolizers.md#cimuniquevaluegroup) |Gets and sets the unique value groups. 
| heading | string|Gets and sets the heading. 
| label | string|Gets and sets the label. 
| lookupStyleset | string|Gets and sets the lookup styleset. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 
| useDefaultSymbol | boolean|Gets and sets a boolean value indicating whether or not to use the default symbol. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 






## CIMTinLayer
#### Represents a TIN layer which displays TIN data sources, a data structure that represents terrain data as a triangulated irregular network. 


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


### CIMTinLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection. 
| displayField | string|Gets and sets the display field. 
| renderers | [CIMTinRenderer](Types.md#cimtinrenderer) |Gets and sets the renderers. 
| scaleSymbols | boolean|Gets and sets a boolean value indicating whether or not to scale symbols. 






## CIMTinNodeElevationRenderer
#### Represents a TIN node elevation renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string|Gets and sets an attribute field name. 
| embeddedDataSources | [long]|Gets and sets embedded data sources. 


### CIMTinColorRampRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |Gets and sets the class breaks. 
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|Gets and sets the classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype)|Gets and sets the cursor type. 
| description | string|Gets and sets the description. 
| label | string|Gets and sets the label. 
| minimumBreak | double|Gets and sets the minimum break. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format. 
| showClassGaps | boolean|Gets and sets a boolean value indicating if class gaps should be shown. 
| sortClassesAscending | boolean|Gets and sets a boolean value indicating if class are ascending. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the base symbol. 






## CIMTinNodeRenderer
#### Represents a TIN node renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTinSimpleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| label | string|Gets and sets the label. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 






## CIMTinNodeValueRenderer
#### Represents a TIN node value renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | bool|Gets and sets a boolean value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string|Gets and sets an attribute field name. 
| embeddedDataSources | [long]|Gets and sets embedded data sources. 


### CIMTinUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorScheme | string|Gets and sets the color ramp name. 
| description | string|Gets and sets the description. 
| groups | [CIMUniqueValueGroup](CIMSymbolizers.md#cimuniquevaluegroup) |Gets and sets the unique value groups. 
| heading | string|Gets and sets the heading. 
| label | string|Gets and sets the label. 
| lookupStyleset | string|Gets and sets the lookup styleset. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 
| useDefaultSymbol | boolean|Gets and sets a boolean value indicating whether or not to use the default symbol. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 



