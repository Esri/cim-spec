


## CIMColorClassBreak
#### Represents a color class break. 


### CIMColorClassBreak 

|Property | Type | Description | 
|---------|--------|--------|
| upperBound | double | The upper bound for the color class break. 
| label | string | The label for the color class break. 
| description | string | The description for the color class break. 
| color | [Color](Types.md#color) | The color for the color class break. 






## CIMColorModulationInfo
#### Indicates whether modulation should be used to render the point. Low modulation values will darken the point color. 


### CIMColorModulationInfo 

|Property | Type | Description | 
|---------|--------|--------|
| field | string | The attribute to use as a source for the color modulation. 
| minValue | double | The minimum value to compute modulation on linear scale based on field value. 
| maxValue | double | The maximum value to compute modulation on linear scale based on field value. 






## CIMColorUniqueValue
#### Represents a color unique value. 


### CIMColorUniqueValue 

|Property | Type | Description | 
|---------|--------|--------|
| value | string | The class value as a string. 
| label | string | The class label. 
| description | string | The class description. 
| color | [Color](Types.md#color) | The class color. 
| visible | boolean | A value indicating whether this class is visible. 






## CIMLASDatasetLayer
#### Represents a LAS dataset layer. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the source was last modified, as of the last sync. Used to detect when another sync is needed. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 
| sourcePortalUrl | string | The source portal URI of the item. Set if sourced from an external item such as an item on a portal. 


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The URIs of the layers used as masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| layerScaleVisibilityOptions | [CIMLayerScaleVisibilityOptions](CIMLayer.md#cimlayerscalevisibilityoptions) | The layer's scale visibility options. 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 
| enableLayerEffects | boolean | A value indicating whether to enable any type of effects on the layer. 
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. 


### CIMLASDatasetLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| analysisToolsResolution | double | The analysis tool resolution. 
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection to the LAS dataset. 
| displayField | string | The display field. 
| fileExtentSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The file extent symbol. 
| fileNameSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The file name symbol. 
| fullResolutionScale | double | The full resolution scale. 
| isFlattened | boolean | A value indicating whether this layer is flattened. 
| LASDatasetFilter | [LasFilter](ExternalReferences.md#lasfilter) | The LAS dataset filter. 
| maintainCurrentSurface | boolean | A value indicating whether the current surface should be maintained. 
| pointBudget | long | The point budget. 
| pointCountPerCentimeter | long | The point count per centimeter. 
| renderers | [[CIMTinRenderer]](Types.md#tinrenderer) | The renderers. 
| scaleSymbols | boolean | A value indicating whether to scale symbols. 
| showFileExtent | boolean | A value indicating whether to show the file extent. 
| showFileName | boolean | A value indicating whether to show the file name. 
| showResolution | boolean | A value indicating whether to show the resolution. 
| useFullResolutionScale | boolean | A value indicating whether to use the full resolution scale. 
| selectable | boolean | A value indicating whether the layer is selectable. 
| eyeDomeLighting | [CIMEyeDomeLighting](CIMLayer.md#cimeyedomelighting) | Eye-dome lighting properties. 
| useDynamicLOD | boolean | A value indicating whether to use dynamic level-of-detail. 






## CIMLASPointElevationRenderer
#### Represents a LAS point elevation renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string | An attribute field name. 
| embeddedDataSources | [long] | Embedded data sources. 


### CIMTinColorRampRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [[CIMClassBreak]](CIMRenderers.md#cimclassbreak) | The class breaks. 
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype) | The cursor type. 
| description | string | The description. 
| label | string | The label. 
| minimumBreak | double | The minimum break. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| showClassGaps | boolean | A value indicating whether or not to show class gaps. 
| sortClassesAscending | boolean | A value indicating whether classes are ascending. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The base symbol. 


### CIMLASPointElevationRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| modulateIntensity | boolean | A value indicating whether to modulate intensity. 
| pointSplatter | [CIMLASPointSplatter](CIMTerrainLayers.md#cimlaspointsplatter) | The point splatter properties. 
| useSplat | boolean | A value indicating whether to use the splat technique. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo) | Color modulation. 






## CIMLASPointSplatter
#### Represents a LAS point splatter. 


### CIMLASPointSplatter 

|Property | Type | Description | 
|---------|--------|--------|
| splatMinimumSize | double | Splat minimum size. 
| splatScale | double | Splat scale. 
| useSplatHighlight | boolean | A value indicating whether to use splat highlighting. 





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
| label | string | The class label. 
| value | double | The class value. 





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
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| stretchMax | double | The stretch max. 
| stretchMin | double | The stretch min. 
| gammaValue | double | The gamma value. 
| invert | boolean | A value indicating whether to invert the stretch. 
| lookup | [long] | The lookup values. 
| maxPercent | double | The maximum percent. 
| minPercent | double | The minimum percent. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| standardDeviationParam | double | The standard deviation parameter. 
| statsType | [enumeration LASStretchStatsType](CIMTerrainLayers.md#enumeration-lasstretchstatstype) | The LAS stats type. 
| stretchAttribute | [enumeration LASStretchAttribute](CIMTerrainLayers.md#enumeration-lasstretchattribute) | The LAS stretch attribute. 
| stretchClasses | [[CIMLASStretchClass]](CIMTerrainLayers.md#cimlasstretchclass) | The stretch classes. 
| stretchStats | [StatsHistogram](ExternalReferences.md#statshistogram) | The stretch statistics. 
| stretchType | [enumeration LASStretchType](CIMTerrainLayers.md#enumeration-lasstretchtype) | The stretch type. 
| useCustomStretchMinMax | boolean | A value indicating whether to use custom stretch minimum maximum. 
| useGammaStretch | boolean | A value indicating whether to use gamma stretch. 






## CIMLASStretchRenderer
#### Represents a LAS stretch renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string | An attribute field name. 
| embeddedDataSources | [long] | Embedded data sources. 


### CIMLASStretchRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| modulationInput | [CIMLASStretchInput](CIMTerrainLayers.md#cimlasstretchinput) | The modulation input. 
| modulationWeight | double | The modulation weight. 
| pointSplatter | [CIMLASPointSplatter](CIMTerrainLayers.md#cimlaspointsplatter) | The point splatter. 
| stretchDrawingType | [enumeration LASStretchDrawingType](CIMTerrainLayers.md#enumeration-lasstretchdrawingtype) | The stretch drawing type. 
| stretchSourceInput | [CIMLASStretchInput](CIMTerrainLayers.md#cimlasstretchinput) | The stretch source input. 
| tintSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The tint symbol. 
| useModulation | boolean | A value indicating whether to use modulation. 
| useSplat | boolean | A value indicating whether to use the splat technique. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo) | Color modulation. 





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
| PercentMinMax| 5| Percent minimum maximum. 




## CIMLASUniqueValueRenderer
#### Represents a LAS unique value renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string | An attribute field name. 
| embeddedDataSources | [long] | Embedded data sources. 


### CIMTinUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorScheme | string | The color ramp name. 
| description | string | The description. 
| groups | [[CIMUniqueValueGroup]](CIMRenderers.md#cimuniquevaluegroup) | The unique value groups. 
| heading | string | The heading. 
| label | string | The label. 
| lookupStyleset | string | The lookup styleset. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 
| useDefaultSymbol | boolean | A value indicating whether or not to use the default symbol. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 


### CIMLASUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attribute | long | The attribute index. 
| modulateIntensity | boolean | A value indicating whether or not to modulate intensity. 
| pointSplatter | [CIMLASPointSplatter](CIMTerrainLayers.md#cimlaspointsplatter) | Point splatter properties. 
| useSplat | boolean | A value indicating whether or not to use the splat technique. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo) | Color modulation. 






## CIMPointCloudBitFieldFilter
#### Represents a point cloud bit field filter. Filters based on the bit-wise representation of the provided field. For a point to be retained, its attribute field bits must match BitsToSet and BitsToClear. Bits which are not explicitly clear nor set, are ignored. 


### CIMPointCloudFilter 

|Property | Type | Description | 
|---------|--------|--------|
| field | string | The field used for the filter. 


### CIMPointCloudBitFieldFilter 

|Property | Type | Description | 
|---------|--------|--------|
| requiredSetBits | [long] | An array of bit numbers set. Bit 0 is the least significant bit. 
| requiredClearBits | [long] | An array of bit numbers cleared. Bit 0 is the least significant bit. 






## CIMPointCloudClassBreaksRenderer
#### Represents a point cloud class breaks renderer. 


### CIMPointCloudRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| pointShape | [enumeration PointCloudShapeType](CIMTerrainLayers.md#enumeration-pointcloudshapetype) | The symbol type. 
| pointSizeAlgorithm | [CIMPointCloudAlgorithm](CIMTerrainLayers.md#cimpointcloudalgorithm) | The algorithm used to determine the symbol size. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo) | The filter used to filter the points being drawn. 
| fieldTransformType | [enumeration PointCloudFieldTransformType](CIMTerrainLayers.md#enumeration-pointcloudfieldtransformtype) | The field transform type. 
| field | string | The field used to render the points. 


### CIMPointCloudClassBreaksRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [[CIMColorClassBreak]](CIMTerrainLayers.md#cimcolorclassbreak) | The color class breaks of the renderer. 





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
| useRealWorldSymbolSizes | boolean | A value indicating whether to use real world symbols sizes (meters) vs. points. This value should always be in sync with the UseRealWorldSymbolSizes property at the symbol level. 
| size | double | The size of the symbols. 






## CIMPointCloudLayer
#### Represents a point cloud layer. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the source was last modified, as of the last sync. Used to detect when another sync is needed. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 
| sourcePortalUrl | string | The source portal URI of the item. Set if sourced from an external item such as an item on a portal. 


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The URIs of the layers used as masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| layerScaleVisibilityOptions | [CIMLayerScaleVisibilityOptions](CIMLayer.md#cimlayerscalevisibilityoptions) | The layer's scale visibility options. 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 
| enableLayerEffects | boolean | A value indicating whether to enable any type of effects on the layer. 
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. 


### CIMPointCloudLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| renderer | [PointCloudRenderer](Types.md#pointcloudrenderer) | The symbol renderer. 
| dataConnection | [CIMSceneDataConnection](CIMTerrainLayers.md#cimscenedataconnection) | The data connection. 
| pointsPerInch | double | The double value that determines the number of points to draw per display inch. 
| pointsBudget | long | The double value to determine the upper limit on the number of points drawn. 
| filters | [[CIMPointCloudFilter]](Types.md#pointcloudfilter) | The filter used to filter the points being drawn. 
| snappable | boolean | A value indicating whether this layer participates in snapping in the editor. 
| eyeDomeLighting | [CIMEyeDomeLighting](CIMLayer.md#cimeyedomelighting) | Eye-dome lighting properties. 






## CIMPointCloudRGBRenderer
#### Represents a point cloud RGB renderer. 


### CIMPointCloudRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| pointShape | [enumeration PointCloudShapeType](CIMTerrainLayers.md#enumeration-pointcloudshapetype) | The symbol type. 
| pointSizeAlgorithm | [CIMPointCloudAlgorithm](CIMTerrainLayers.md#cimpointcloudalgorithm) | The algorithm used to determine the symbol size. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo) | The filter used to filter the points being drawn. 
| fieldTransformType | [enumeration PointCloudFieldTransformType](CIMTerrainLayers.md#enumeration-pointcloudfieldtransformtype) | The field transform type. 
| field | string | The field used to render the points. 


### CIMPointCloudRGBRenderer 

|Property | Type | Description | 
|---------|--------|--------|






## CIMPointCloudReturnFilter
#### Represents a point cloud return filter. 


### CIMPointCloudFilter 

|Property | Type | Description | 
|---------|--------|--------|
| field | string | The field used for the filter. 


### CIMPointCloudReturnFilter 

|Property | Type | Description | 
|---------|--------|--------|
| includedReturnsBitmask | long | The binary combination of PointCouldReturnType enumeration flags. 





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
| scaleFactor | double | The scale factor used to compute the point size. 
| minSize | double | The minimum point size. 






## CIMPointCloudStretchRenderer
#### Represents a point cloud stretch renderer. 


### CIMPointCloudRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| pointShape | [enumeration PointCloudShapeType](CIMTerrainLayers.md#enumeration-pointcloudshapetype) | The symbol type. 
| pointSizeAlgorithm | [CIMPointCloudAlgorithm](CIMTerrainLayers.md#cimpointcloudalgorithm) | The algorithm used to determine the symbol size. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo) | The filter used to filter the points being drawn. 
| fieldTransformType | [enumeration PointCloudFieldTransformType](CIMTerrainLayers.md#enumeration-pointcloudfieldtransformtype) | The field transform type. 
| field | string | The field used to render the points. 


### CIMPointCloudStretchRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| rangeMin | double | The minimum value used to compute the linear mapping of the renderer. 
| rangeMax | double | The maximum value used to compute the linear mapping of the renderer. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp of the renderer. 






## CIMPointCloudUniqueValueRenderer
#### Represents a point cloud unique value renderer. 


### CIMPointCloudRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| pointShape | [enumeration PointCloudShapeType](CIMTerrainLayers.md#enumeration-pointcloudshapetype) | The symbol type. 
| pointSizeAlgorithm | [CIMPointCloudAlgorithm](CIMTerrainLayers.md#cimpointcloudalgorithm) | The algorithm used to determine the symbol size. 
| colorModulation | [CIMColorModulationInfo](CIMTerrainLayers.md#cimcolormodulationinfo) | The filter used to filter the points being drawn. 
| fieldTransformType | [enumeration PointCloudFieldTransformType](CIMTerrainLayers.md#enumeration-pointcloudfieldtransformtype) | The field transform type. 
| field | string | The field used to render the points. 


### CIMPointCloudUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| classes | [[CIMColorUniqueValue]](CIMTerrainLayers.md#cimcoloruniquevalue) | The unique color classes of the renderer. 






## CIMPointCloudValueFilter
#### Represents a point cloud value filter. Filter points based on the value of an specified attribute. 


### CIMPointCloudFilter 

|Property | Type | Description | 
|---------|--------|--------|
| field | string | The field used for the filter. 


### CIMPointCloudValueFilter 

|Property | Type | Description | 
|---------|--------|--------|
| values | [double] | The values used as exclude or include list. 
| mode | [enumeration PointCloudValueFilterMode](CIMTerrainLayers.md#enumeration-pointcloudvaluefiltermode) | The mode that determines if the ValueList is an include list or an exclude list. 





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


### CIMServiceDataConnectionProperties 

|Property | Type | Description | 
|---------|--------|--------|
| customParameters | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | Vendor specific parameters. 


### CIMSceneDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string | The URI. 






## CIMTerrainDirtyAreaRenderer
#### Represents a terrain dirty area renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTinSimpleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| label | string | The label. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 





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
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the source was last modified, as of the last sync. Used to detect when another sync is needed. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 
| sourcePortalUrl | string | The source portal URI of the item. Set if sourced from an external item such as an item on a portal. 


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The URIs of the layers used as masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| layerScaleVisibilityOptions | [CIMLayerScaleVisibilityOptions](CIMLayer.md#cimlayerscalevisibilityoptions) | The layer's scale visibility options. 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 
| enableLayerEffects | boolean | A value indicating whether to enable any type of effects on the layer. 
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. 


### CIMTerrainLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| analysisToolsResolution | double | The resolution use by analysis tools. 
| autoLOR | boolean | A value indicating whether or not LOR should be updated when scale changes. 
| currentResolution | double | The current resolution. 
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| displayField | string | The display field. 
| lockCurrentSurface | boolean | A value indicating whether the current surface should be updated based on scale change. 
| pointBudget | long | The point budget. 
| pyramidHonored | boolean | A value indicating whether the current surface resolution honors the scale/resolution relationship in the pyramid definition. 
| scaleSymbols | boolean | A value indicating whether symbols should be scaled. 
| showResolution | boolean | A value indicating whether the resolution should be shown in the contents pane. 
| renderers | [[CIMTinRenderer]](Types.md#tinrenderer) | The renderers. 
| targetResolution | double | The target resolution. 
| useOverviewTerrain | boolean | A value indicating whether the terrain overview should be used. 
| usePointBudget | boolean | A value indicating whether the point budget should be used. 






## CIMTerrainPointAttributeGraduatedRenderer
#### Represents a terrain point attribute graduated renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string | An attribute field name. 
| embeddedDataSources | [long] | Embedded data sources. 


### CIMTinColorRampRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [[CIMClassBreak]](CIMRenderers.md#cimclassbreak) | The class breaks. 
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype) | The cursor type. 
| description | string | The description. 
| label | string | The label. 
| minimumBreak | double | The minimum break. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| showClassGaps | boolean | A value indicating whether or not to show class gaps. 
| sortClassesAscending | boolean | A value indicating whether classes are ascending. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The base symbol. 






## CIMTerrainPointAttributeUniqueRenderer
#### Represents a terrain point attribute unique renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string | An attribute field name. 
| embeddedDataSources | [long] | Embedded data sources. 


### CIMTinUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorScheme | string | The color ramp name. 
| description | string | The description. 
| groups | [[CIMUniqueValueGroup]](CIMRenderers.md#cimuniquevaluegroup) | The unique value groups. 
| heading | string | The heading. 
| label | string | The label. 
| lookupStyleset | string | The lookup styleset. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 
| useDefaultSymbol | boolean | A value indicating whether or not to use the default symbol. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 






## CIMTerrainPointElevationRenderer
#### Represents a terrain point elevation renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string | An attribute field name. 
| embeddedDataSources | [long] | Embedded data sources. 


### CIMTinColorRampRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [[CIMClassBreak]](CIMRenderers.md#cimclassbreak) | The class breaks. 
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype) | The cursor type. 
| description | string | The description. 
| label | string | The label. 
| minimumBreak | double | The minimum break. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| showClassGaps | boolean | A value indicating whether or not to show class gaps. 
| sortClassesAscending | boolean | A value indicating whether classes are ascending. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The base symbol. 






## CIMTinBreaklineRenderer
#### Represents a TIN breakline renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string | An attribute field name. 
| embeddedDataSources | [long] | Embedded data sources. 


### CIMTinUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorScheme | string | The color ramp name. 
| description | string | The description. 
| groups | [[CIMUniqueValueGroup]](CIMRenderers.md#cimuniquevaluegroup) | The unique value groups. 
| heading | string | The heading. 
| label | string | The label. 
| lookupStyleset | string | The lookup styleset. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 
| useDefaultSymbol | boolean | A value indicating whether or not to use the default symbol. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 






## CIMTinContourRenderer
#### Represents a TIN contour renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTinContourRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| contourDescription | string | The contour description. 
| contourInterval | double | The contour interval. 
| contourLabel | string | The contour label. 
| contourSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The contour symbol. 
| indexContourDescription | string | The index contour description. 
| indexContourFactor | long | The index contour factor. 
| indexContourLabel | string | The index contour label. 
| indexContourSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The index contour symbol. 
| referenceContourHeight | double | The reference contour height. 






## CIMTinEdgeRenderer
#### Represents a TIN edge renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTinSimpleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| label | string | The label. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 






## CIMTinFaceClassBreaksRenderer
#### Represents a TIN face class breaks renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string | An attribute field name. 
| embeddedDataSources | [long] | Embedded data sources. 


### CIMTinColorRampRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [[CIMClassBreak]](CIMRenderers.md#cimclassbreak) | The class breaks. 
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype) | The cursor type. 
| description | string | The description. 
| label | string | The label. 
| minimumBreak | double | The minimum break. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| showClassGaps | boolean | A value indicating whether or not to show class gaps. 
| sortClassesAscending | boolean | A value indicating whether classes are ascending. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The base symbol. 






## CIMTinFaceRenderer
#### Represents a TIN face renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTinSimpleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| label | string | The label. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 






## CIMTinFaceValueRenderer
#### Represents a TIN face value renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string | An attribute field name. 
| embeddedDataSources | [long] | Embedded data sources. 


### CIMTinUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorScheme | string | The color ramp name. 
| description | string | The description. 
| groups | [[CIMUniqueValueGroup]](CIMRenderers.md#cimuniquevaluegroup) | The unique value groups. 
| heading | string | The heading. 
| label | string | The label. 
| lookupStyleset | string | The lookup styleset. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 
| useDefaultSymbol | boolean | A value indicating whether or not to use the default symbol. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 






## CIMTinLayer
#### Represents a TIN layer which displays TIN data sources, a data structure that represents terrain data as a triangulated irregular network. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the source was last modified, as of the last sync. Used to detect when another sync is needed. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 
| sourcePortalUrl | string | The source portal URI of the item. Set if sourced from an external item such as an item on a portal. 


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The URIs of the layers used as masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| layerScaleVisibilityOptions | [CIMLayerScaleVisibilityOptions](CIMLayer.md#cimlayerscalevisibilityoptions) | The layer's scale visibility options. 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 
| enableLayerEffects | boolean | A value indicating whether to enable any type of effects on the layer. 
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. 


### CIMTinLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| displayField | string | The display field. 
| renderers | [[CIMTinRenderer]](Types.md#tinrenderer) | The renderers. 
| scaleSymbols | boolean | A value indicating whether or not to scale symbols. 






## CIMTinNodeElevationRenderer
#### Represents a TIN node elevation renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string | An attribute field name. 
| embeddedDataSources | [long] | Embedded data sources. 


### CIMTinColorRampRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [[CIMClassBreak]](CIMRenderers.md#cimclassbreak) | The class breaks. 
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| cursorType | [enumeration TerrainDrawCursorType](CIMTerrainLayers.md#enumeration-terraindrawcursortype) | The cursor type. 
| description | string | The description. 
| label | string | The label. 
| minimumBreak | double | The minimum break. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| showClassGaps | boolean | A value indicating whether or not to show class gaps. 
| sortClassesAscending | boolean | A value indicating whether classes are ascending. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The base symbol. 






## CIMTinNodeRenderer
#### Represents a TIN node renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTinSimpleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| label | string | The label. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 






## CIMTinNodeValueRenderer
#### Represents a TIN node value renderer. 


### CIMTinRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| illuminate | boolean | A value indicating whether or not to illuminate. 


### CIMTerrainAttributeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| attributeFieldName | string | An attribute field name. 
| embeddedDataSources | [long] | Embedded data sources. 


### CIMTinUniqueValueRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| colorScheme | string | The color ramp name. 
| description | string | The description. 
| groups | [[CIMUniqueValueGroup]](CIMRenderers.md#cimuniquevaluegroup) | The unique value groups. 
| heading | string | The heading. 
| label | string | The label. 
| lookupStyleset | string | The lookup styleset. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 
| useDefaultSymbol | boolean | A value indicating whether or not to use the default symbol. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 



