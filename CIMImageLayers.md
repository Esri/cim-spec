


## CIMAuxiliaryRasterProperties
Represents auxiliary raster properties.


### CIMAuxiliaryRasterProperties

|Property | Type | Description |
|---------|--------|--------|
| bandIndexes | [long]|A long array of the band indexes.
| extent | [Envelope](ExternalReferences.md#envelope)|The extent.
| height | number //int32|The height.
| width | number //int32|The width.





### Enumeration: ColorBalanceMethod
A list of color balance methods.

|Property | Value | Description |
|---------|--------|--------|
| Dodging| 0| Dodging.
| Histogram| 1| Histogram.
| StdDev| 2| Standard deviation.
| None| 3| None.



### Enumeration: ColorCorrectionStretchType
A list of color correction stretch types.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| None.
| Adaptive| 1| Adaptive.
| MinMax| 2| Min and max.
| StdDev| 3| Standard deviation.



### Enumeration: ColorMatchingMethod
A list of color matching methods.

|Property | Value | Description |
|---------|--------|--------|
| Statistics| 0| Statistics.
| Histogram| 1| Histogram.
| LinearCorrelation| 2| Linear correlation.
| None| 3| None.




## CIMFeatureMosaicSubLayer
Represents mosiac feature sub layer.


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


### CIMMosaicSubLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| mosaicSubLayerType | [enumeration MosaicSubLayerType](CIMImageLayers.md#enumeration-mosaicsublayertype)|The mosaic sublayer type.





### Enumeration: FlowRepresentationType
A list of flow representation types.

|Property | Value | Description |
|---------|--------|--------|
| From| 0| Flow from.
| To| 1| Flow to.




## CIMImageMosaicSubLayer
Represents an image mosaic sublayer.


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


### CIMRasterLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|The data connection for the raster this layer is based on.
| colorizer | [CIMRasterColorizer](CIMImageLayers.md#cimrastercolorizer)|The raster colorizer.
| attributeTable | [CIMRasterTable](CIMVectorLayers.md#cimrastertable)|The raster table definition.
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|The time display definition.
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition)|The time dimension fields.
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|The time definition.
| auxiliaryRasterProperties | [CIMAuxiliaryRasterProperties](CIMImageLayers.md#cimauxiliaryrasterproperties)|The auxiliary raster properties.
| autoComputeStatsHistogram | boolean|A boolean parameter indicating whether or not to automatically compute the statistics histogram.
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |The range definitions.
| activeRangeName | string|The name of the active range.
| activeVariables | [string,]|The active variables.


### CIMImageServiceLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| compression | string|The compression as a string.
| compressionQuality | number //int32|The compression quality.
| drawFootprints | boolean|A boolean option indicating whether or not to draw footprints.
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable)|The feature table.
| footprintDrawMode | [enumeration RasterFootprintDrawMode](CIMImageLayers.md#enumeration-rasterfootprintdrawmode)|The footprint draw mode.
| footprintSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The footprint symbol.
| mosaicRule | [CIMMosaicRule](CIMImageLayers.md#cimmosaicrule)|The mosaic rule.
| renderingRule | [CIMRenderingRule](CIMImageLayers.md#cimrenderingrule)|The rendering rule.
| selectable | boolean|A boolean option indicating whether or not the layer is selectable.
| selectionColor | [Color](Types.md#color)|The selection color.
| selectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The selection symbol.
| useSelectionSymbol | boolean|A boolean option indicating whether or not to use the selection symbol.
| ignoreRenderingRuleOnIdentify | boolean|A boolean option indicating whether or not to ignore the rendering rule on identify.
| useServiceCache | boolean|A boolean option indicating whether or not to use the service cache.


### CIMMosaicSubLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| mosaicSubLayerType | [enumeration MosaicSubLayerType](CIMImageLayers.md#enumeration-mosaicsublayertype)|The mosaic sublayer type.






## CIMImageServiceLayer
Represents an image service layer corresponding to an ArcGIS Server image service.


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


### CIMRasterLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|The data connection for the raster this layer is based on.
| colorizer | [CIMRasterColorizer](CIMImageLayers.md#cimrastercolorizer)|The raster colorizer.
| attributeTable | [CIMRasterTable](CIMVectorLayers.md#cimrastertable)|The raster table definition.
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|The time display definition.
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition)|The time dimension fields.
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|The time definition.
| auxiliaryRasterProperties | [CIMAuxiliaryRasterProperties](CIMImageLayers.md#cimauxiliaryrasterproperties)|The auxiliary raster properties.
| autoComputeStatsHistogram | boolean|A boolean parameter indicating whether or not to automatically compute the statistics histogram.
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |The range definitions.
| activeRangeName | string|The name of the active range.
| activeVariables | [string,]|The active variables.


### CIMImageServiceLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| compression | string|The compression as a string.
| compressionQuality | number //int32|The compression quality.
| drawFootprints | boolean|A boolean option indicating whether or not to draw footprints.
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable)|The feature table.
| footprintDrawMode | [enumeration RasterFootprintDrawMode](CIMImageLayers.md#enumeration-rasterfootprintdrawmode)|The footprint draw mode.
| footprintSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The footprint symbol.
| mosaicRule | [CIMMosaicRule](CIMImageLayers.md#cimmosaicrule)|The mosaic rule.
| renderingRule | [CIMRenderingRule](CIMImageLayers.md#cimrenderingrule)|The rendering rule.
| selectable | boolean|A boolean option indicating whether or not the layer is selectable.
| selectionColor | [Color](Types.md#color)|The selection color.
| selectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The selection symbol.
| useSelectionSymbol | boolean|A boolean option indicating whether or not to use the selection symbol.
| ignoreRenderingRuleOnIdentify | boolean|A boolean option indicating whether or not to ignore the rendering rule on identify.
| useServiceCache | boolean|A boolean option indicating whether or not to use the service cache.






## CIMMosaicLayer
Represents a mosaic layer corresponding to a mosaic dataset.


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


### CIMMosaicLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| boundaryLayer | string|The boundary layer.
| footprintLayer | string|The footprint layer.
| imageLayer | string|The image layer.
| seamlineLayer | string|The seamline layer.
| mosaicDatasetConnection | [DataConnection](Types.md#dataconnection)|The data connection of the mosaic dataset.
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|The time definition.
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|The time display definition.
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition)|The time fields.
| definitionExpression | string|The definition expression.
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |The data connection of the mosaic dataset.
| activeRangeName | string|The name of the active range.
| activeVariables | [string,]|An array of the active variables.






## CIMMosaicRule
Represents a mosaic rule.


### CIMMosaicRule

|Property | Type | Description |
|---------|--------|--------|
| ascending | boolean|A boolean option indicating ascending order.
| FIDs | [number], //[int64],|An array of IDs.
| lockRasterID | string|The ID of the lock raster.
| mosaicMethod | [enumeration RasterMosaicMethod](CIMImageLayers.md#enumeration-rastermosaicmethod)|The mosaic method.
| mosaicOperatorType | [enumeration RasterMosaicOperatorType](CIMImageLayers.md#enumeration-rastermosaicoperatortype)|The mosaic operator type.
| orderByBaseValue | VARIANT|The order by base value.
| orderByFieldName | string|The order by field name.
| timeValue | [TimeValue](ExternalReferences.md#timevalue)|The time value.
| viewpoint | [Point](ExternalReferences.md#point)|The viewpoint as a point.
| whereClause | string|The where clause as a string.





### Enumeration: MosaicSubLayerType
Types of mosaic sublayers.

|Property | Value | Description |
|---------|--------|--------|
| Boundary| 0| Boundary
| Footprint| 1| Footprint
| Image| 2| Image
| Seamline| 3| Seamline




## CIMPansharpeningFilter
Represents a pansharpening filter.


### CIMPansharpeningFilter

|Property | Type | Description |
|---------|--------|--------|
| panImage | [DataConnection](Types.md#dataconnection)|The data connection of the optional panchromatic image.
| pansharpeningType | [enumeration PansharpeningType](CIMImageLayers.md#enumeration-pansharpeningtype)|The data connection of the current pansharpening type.
| infraredImage | [DataConnection](Types.md#dataconnection)|The data connection of the optional infrared image.
| RWeight | number //double|The red weight.
| GWeight | number //double|The green weight.
| BWeight | number //double|The blue weight.
| IWeight | number //double|The infrared weight.





### Enumeration: PansharpeningType
Types of pansharpening.

|Property | Value | Description |
|---------|--------|--------|
| IHS| 0| IHS.
| Brovey| 1| Brovey.
| ESRI| 2| Esri.
| Mean| 3| Mean.




## CIMRasterBandDataConnection
Represents a raster band data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMRasterBandDataConnection

|Property | Type | Description |
|---------|--------|--------|
| rasterBandName | string|The raster band name.


### CIMStandardDataConnection

|Property | Type | Description |
|---------|--------|--------|
| workspaceConnectionString | string|The workspace connection string.
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|The workspace factory.
| customWorkspaceFactoryCLSID | string|The classID of the custom workspace factory.
| dataset | string|The dataset name.
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|The dataset type.






## CIMRasterCMYKColorizer
Represents a raster CMYK colorizer.


### CIMOrthoRectification

|Property | Type | Description |
|---------|--------|--------|
| constantZ | number //double|The constant Z value in meters.
| ZFactor | number //double|The conversion factor from DEM Z unit to meters.
| ZOffset | number //double|The Z offset in meters applied to DEM.
| geoid | boolean|The a boolean option indicating if Geoid correction is needed.
| DEM | [DataConnection](Types.md#dataconnection)|The data connection of the DEM used for orthorectification.


### CIMRasterColorizer

|Property | Type | Description |
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|The raster resampling type.
| contrast | number //int32|The contrast value.
| brightness | number //int32|The brightness value.
| noDataColor | [Color](Types.md#color)|The no data color.


### CIMRasterCMYKColorizer

|Property | Type | Description |
|---------|--------|--------|
| backgroundColor | [Color](Types.md#color)|The background color.
| backgroundValueBlack | number //double|The background value for black.
| backgroundValueCyan | number //double|The background value for cyan.
| backgroundValueMagenta | number //double|The background value for magenta.
| backgroundValueYellow | number //double|The background value for yellow.
| blackBandIndex | number //int32|The band index for black.
| cyanBandIndex | number //int32|The band index for cyan.
| displayBackgroundValue | boolean|The boolean option indicating whether or not to display the background value.
| invert | boolean|The boolean option indicating whether or not the stretch is inverted.
| magentaBandIndex | number //int32|The band index for magenta.
| specificationHistogramBlack | [StatsHistogram](ExternalReferences.md#statshistogram)|The specification histogram for black.
| specificationHistogramCyan | [StatsHistogram](ExternalReferences.md#statshistogram)|The specification histogram for cyan.
| specificationHistogramMagenta | [StatsHistogram](ExternalReferences.md#statshistogram)|The specification histogram for magenta.
| specificationHistogramYellow | [StatsHistogram](ExternalReferences.md#statshistogram)|The specification histogram for yellow.
| standardDeviationParam | number //double|The standard deviation parameter for the stretch renderer.
| stretchStatsBlack | [StatsHistogram](ExternalReferences.md#statshistogram)|The stretch histogram for black.
| stretchStatsCyan | [StatsHistogram](ExternalReferences.md#statshistogram)|The stretch histogram for cyan.
| stretchStatsMagenta | [StatsHistogram](ExternalReferences.md#statshistogram)|The stretch histogram for magenta.
| stretchStatsType | [enumeration RasterStretchStatsType](CIMEnumerations.md#enumeration-rasterstretchstatstype)|The stretch statistics type.
| stretchStatsYellow | [StatsHistogram](ExternalReferences.md#statshistogram)|The stretch histogram for yellow.
| stretchType | [enumeration RasterStretchType](CIMEnumerations.md#enumeration-rasterstretchtype)|The stretch type.
| useBlackMapping | boolean|The boolean option indicating whether or not to use black mapping.
| useCyanMapping | boolean|The boolean option indicating whether or not to use cyan mapping.
| useDefaultMapping | boolean|The boolean option indicating whether or not to use default mapping.
| useMagentaMapping | boolean|The boolean option indicating whether or not to use magenta mapping.
| useYellowMapping | boolean|The boolean option indicating whether or not to use yellow mapping.
| yellowBandIndex | number //int32|The band index for yellow.






## CIMRasterCatalogLayer
Represents a raster catalog layer.


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


### CIMRasterCatalogLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| displayRastersThreshold | number //int32|The threshold for displaying wire frames.
| drawRastersOnly | boolean|A boolean option indicating whether or not to draw only rasters.
| fixedLabelPositions | boolean|A boolean option indicating whether or not to draw labels in fixed positions relative to the tile boundaries, and does not use the label placement engine.
| colorizerMapping | [CIMRasterColorizerMapping](CIMImageLayers.md#cimrastercolorizermapping) |The colorizer mapping.
| colorizers | [CIMRasterColorizer](CIMImageLayers.md#cimrastercolorizer) |The colorizer.
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|The resampling type.
| transitionScale | number //double|The transition scale.
| useColorCorrection | boolean|A boolean option indicating whether or not to use color correction.
| useScale | boolean|A boolean option indicating whether or not to use scale.
| wireFrameSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The wire frame symbol.
| sortFieldAscending | boolean|A boolean option indicating whether or not the sort is ascending.
| sortField | string|The sort field.
| colorCorrection | [CIMRasterColorCorrection](CIMImageLayers.md#cimrastercolorcorrection)|The color correction.






## CIMRasterClassBreak
Represents a raster class break.


### CIMRasterClassBreak

|Property | Type | Description |
|---------|--------|--------|
| upperBound | number //double|The upper bound for the raster class break.
| label | string|The label for the raster class break.
| description | string|The description for the raster class break.
| color | [Color](Types.md#color)|The color for the raster class break.






## CIMRasterClassifyColorizer
Represents a raster classify colorizer.


### CIMOrthoRectification

|Property | Type | Description |
|---------|--------|--------|
| constantZ | number //double|The constant Z value in meters.
| ZFactor | number //double|The conversion factor from DEM Z unit to meters.
| ZOffset | number //double|The Z offset in meters applied to DEM.
| geoid | boolean|The a boolean option indicating if Geoid correction is needed.
| DEM | [DataConnection](Types.md#dataconnection)|The data connection of the DEM used for orthorectification.


### CIMRasterColorizer

|Property | Type | Description |
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|The raster resampling type.
| contrast | number //int32|The contrast value.
| brightness | number //int32|The brightness value.
| noDataColor | [Color](Types.md#color)|The no data color.


### CIMRasterClassifyColorizer

|Property | Type | Description |
|---------|--------|--------|
| classBreaks | [CIMRasterClassBreak](CIMImageLayers.md#cimrasterclassbreak) |The class breaks of the renderer.
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|The classification method.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
| exclusionColor | [Color](Types.md#color)|The exclusion color.
| exclusionDescription | string|The exclusion description.
| exclusionLabel | string|The exclusion label.
| exclusionRanges | [number], //[double],|The exclusion ranges as an array of doubles.
| exclusionValues | [number], //[double],|The exclusion values as an array of doubles.
| field | string|The renderer field.
| hillshadeZFactor | number //double|The Z factor of the hillshade.
| minimumBreak | number //double|The minimum break of the classification.
| showClassGaps | boolean|A boolean option indicating whether or not to show class gaps.
| showInAscendingOrder | boolean|A boolean option indicating whether or not to show classes in ascending order.
| useExclusionColor | boolean|A boolean option indicating whether or not to use the exclusion color.
| useHillshade | boolean|A boolean option indicating whether or not to use the hillshade.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format applied to values.


### CIMDataNormalization

|Property | Type | Description |
|---------|--------|--------|
| normalizationField | string|The normalization field.
| normalizationTotal | number //double|The normalization total.
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|The normalization type.






## CIMRasterColorCorrection
Represents a raster color correction configuration.


### CIMRasterColorCorrection

|Property | Type | Description |
|---------|--------|--------|
| preStretchType | [enumeration ColorCorrectionStretchType](CIMImageLayers.md#enumeration-colorcorrectionstretchtype)|The pre-stretch type of color correction.
| colorBalanceMethod | [enumeration ColorBalanceMethod](CIMImageLayers.md#enumeration-colorbalancemethod)|The color balance method.
| colorMatchingMethod | [enumeration ColorMatchingMethod](CIMImageLayers.md#enumeration-colormatchingmethod)|The color matching method.
| needContrastAdjustment | boolean|A boolean option indicating whether or not contrast adjustment is needed.
| targetColorSurfaceType | [enumeration TargetColorSurfaceType](CIMImageLayers.md#enumeration-targetcolorsurfacetype)|The target color surface type.
| targetColorRaster | [DataConnection](Types.md#dataconnection)|The target color raster.
| userDefinedReference | boolean|A boolean option indicating whether or not this is a user defined reference.
| referenceOID | number //int32|The reference OID.






## CIMRasterColorMapColorizer
Represents a raster color map colorizer.


### CIMOrthoRectification

|Property | Type | Description |
|---------|--------|--------|
| constantZ | number //double|The constant Z value in meters.
| ZFactor | number //double|The conversion factor from DEM Z unit to meters.
| ZOffset | number //double|The Z offset in meters applied to DEM.
| geoid | boolean|The a boolean option indicating if Geoid correction is needed.
| DEM | [DataConnection](Types.md#dataconnection)|The data connection of the DEM used for orthorectification.


### CIMRasterColorizer

|Property | Type | Description |
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|The raster resampling type.
| contrast | number //int32|The contrast value.
| brightness | number //int32|The brightness value.
| noDataColor | [Color](Types.md#color)|The no data color.


### CIMRasterColorMapColorizer

|Property | Type | Description |
|---------|--------|--------|
| colors | [CIMColor](Types.md#cimcolor) |An array of colors.
| bandID | number //int32|The band ID.
| labels | [string,]|The color labels as a string array.
| min | number //int32|The min value.
| max | number //int32|Max value.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format.
| values | [long]|The array of values.






## CIMRasterColorizerMapping
Represents a raster colorizer mapping.


### CIMRasterColorizerMapping

|Property | Type | Description |
|---------|--------|--------|
| rasterOID | number //int32|The Object ID of the raster in the raster catalog.
| colorizerIndex | number //int32|The index of the colorizer.






## CIMRasterDiscreteColorColorizer
Represents a raster discrete color colorizer.


### CIMOrthoRectification

|Property | Type | Description |
|---------|--------|--------|
| constantZ | number //double|The constant Z value in meters.
| ZFactor | number //double|The conversion factor from DEM Z unit to meters.
| ZOffset | number //double|The Z offset in meters applied to DEM.
| geoid | boolean|The a boolean option indicating if Geoid correction is needed.
| DEM | [DataConnection](Types.md#dataconnection)|The data connection of the DEM used for orthorectification.


### CIMRasterColorizer

|Property | Type | Description |
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|The raster resampling type.
| contrast | number //int32|The contrast value.
| brightness | number //int32|The brightness value.
| noDataColor | [Color](Types.md#color)|The no data color.


### CIMRasterDiscreteColorColorizer

|Property | Type | Description |
|---------|--------|--------|
| numColors | number //int32|The number of colors.
| colormap | [RasterColormap](ExternalReferences.md#rastercolormap)|The colormap.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.





### Enumeration: RasterFootprintDrawMode
Raster footprint draw modes.

|Property | Value | Description |
|---------|--------|--------|
| All| 0| Draw all footprints.
| OnlyPrimary| 1| Draw only primary footprints.




## CIMRasterLayer
Represents a raster layer which displays raster imagery stored in a raster dataset.


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


### CIMRasterLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|The data connection for the raster this layer is based on.
| colorizer | [CIMRasterColorizer](CIMImageLayers.md#cimrastercolorizer)|The raster colorizer.
| attributeTable | [CIMRasterTable](CIMVectorLayers.md#cimrastertable)|The raster table definition.
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|The time display definition.
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition)|The time dimension fields.
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|The time definition.
| auxiliaryRasterProperties | [CIMAuxiliaryRasterProperties](CIMImageLayers.md#cimauxiliaryrasterproperties)|The auxiliary raster properties.
| autoComputeStatsHistogram | boolean|A boolean parameter indicating whether or not to automatically compute the statistics histogram.
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |The range definitions.
| activeRangeName | string|The name of the active range.
| activeVariables | [string,]|The active variables.





### Enumeration: RasterMosaicMethod
Raster mosaic methods.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| None.
| Center| 1| Center.
| Nadir| 2| Nadir.
| Viewpoint| 3| Viewpoint.
| Attribute| 4| Attribute.
| LockRaster| 5| Lock raster.
| Northwest| 6| Northwest.
| Seamline| 7| Seamline.



### Enumeration: RasterMosaicOperatorType
Raster mosaic operator type.

|Property | Value | Description |
|---------|--------|--------|
| First| 0| First.
| Last| 1| Last.
| Min| 2| Min.
| Max| 3| Max.
| Mean| 4| Mean.
| Blend| 5| Blend.
| Sum| 6| Sum.




## CIMRasterRGBColorizer
Represents a raster RGB colorizer.


### CIMOrthoRectification

|Property | Type | Description |
|---------|--------|--------|
| constantZ | number //double|The constant Z value in meters.
| ZFactor | number //double|The conversion factor from DEM Z unit to meters.
| ZOffset | number //double|The Z offset in meters applied to DEM.
| geoid | boolean|The a boolean option indicating if Geoid correction is needed.
| DEM | [DataConnection](Types.md#dataconnection)|The data connection of the DEM used for orthorectification.


### CIMRasterColorizer

|Property | Type | Description |
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|The raster resampling type.
| contrast | number //int32|The contrast value.
| brightness | number //int32|The brightness value.
| noDataColor | [Color](Types.md#color)|The no data color.


### CIMRasterRGBColorizer

|Property | Type | Description |
|---------|--------|--------|
| alphaBandIndex | number //int32|The band to be represented in alpha.
| backgroundColor | [Color](Types.md#color)|The background display color.
| backgroundValueBlue | number //double|The background blue value.
| backgroundValueGreen | number //double|The background green value.
| backgroundValueRed | number //double|The background red value.
| blueBandIndex | number //int32|The band to be represented in blue.
| blueLookup | [long]|The blue lookup values.
| displayBackgroundValue | boolean|A boolean option on whether or not to display the background value.
| ESRIStretchContrastB | number //double|The Esri stretch contrast value for blue.
| ESRIStretchContrastG | number //double|The Esri stretch contrast value for green.
| ESRIStretchContrastR | number //double|The Esri stretch contrast value for red.
| ESRIStretchMeanB | number //double|The Esri stretch mean value for blue.
| ESRIStretchMeanG | number //double|The Esri stretch mean value for green.
| ESRIStretchMeanR | number //double|The Esri stretch mean value for red.
| gammaB | number //double|The gamma value for blue.
| gammaG | number //double|The gamma value for green.
| gammaR | number //double|The gamma value for red.
| greenBandIndex | number //int32|The band to be represented in green.
| greenLookup | [long]|The green lookup values.
| invert | boolean|The boolean option indicating whether or not the stretch is inverted.
| lumLookup | [long]|The lum lookup values.
| maxPercent | number //double|The max percent.
| minPercent | number //double|The min percent.
| pansharpeningFilter | [CIMPansharpeningFilter](CIMImageLayers.md#cimpansharpeningfilter)|The pansharpening filter.
| redBandIndex | number //int32|The band to be represented in red.
| redLookup | [long]|The red lookup values.
| specificationHistogramBlue | [StatsHistogram](ExternalReferences.md#statshistogram)|The specification histogram for blue.
| specificationHistogramGreen | [StatsHistogram](ExternalReferences.md#statshistogram)|The specification histogram for green.
| specificationHistogramRed | [StatsHistogram](ExternalReferences.md#statshistogram)|The specification histogram for red.
| standardDeviationsParam | number //double|The standard deviations parameter.
| stretchStatsBlue | [StatsHistogram](ExternalReferences.md#statshistogram)|The stretch statistics for blue.
| stretchStatsGreen | [StatsHistogram](ExternalReferences.md#statshistogram)|The stretch statistics for green.
| stretchStatsRed | [StatsHistogram](ExternalReferences.md#statshistogram)|The stretch statistics for red.
| stretchStatsType | [enumeration RasterStretchStatsType](CIMEnumerations.md#enumeration-rasterstretchstatstype)|The stretch statistics type.
| stretchType | [enumeration RasterStretchType](CIMEnumerations.md#enumeration-rasterstretchtype)|The stretch type.
| useAlphaBand | boolean|A boolean option on whether or not to use the alpha band.
| useBlueBand | boolean|A boolean option on whether or not to use the blue band.
| useDefaultMapping | boolean|A boolean option on whether or not to use default mapping.
| useGammaStretch | boolean|A boolean option on whether or not to use gamma stretch.
| useGreenBand | boolean|A boolean option on whether or not to use the green band.
| useRedBand | boolean|A boolean option on whether or not to use the red band.






## CIMRasterStretchClass
Represents a raster stretch class.


### CIMRasterStretchClass

|Property | Type | Description |
|---------|--------|--------|
| label | string|The raster stretch class label.
| value | number //double|The raster stretch class value.






## CIMRasterStretchColorizer
Represents a raster stretch colorizer.


### CIMOrthoRectification

|Property | Type | Description |
|---------|--------|--------|
| constantZ | number //double|The constant Z value in meters.
| ZFactor | number //double|The conversion factor from DEM Z unit to meters.
| ZOffset | number //double|The Z offset in meters applied to DEM.
| geoid | boolean|The a boolean option indicating if Geoid correction is needed.
| DEM | [DataConnection](Types.md#dataconnection)|The data connection of the DEM used for orthorectification.


### CIMRasterColorizer

|Property | Type | Description |
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|The raster resampling type.
| contrast | number //int32|The contrast value.
| brightness | number //int32|The brightness value.
| noDataColor | [Color](Types.md#color)|The no data color.


### CIMRasterStretchColorizer

|Property | Type | Description |
|---------|--------|--------|
| backgroundColor | [Color](Types.md#color)|The background color.
| backgroundValue | number //double|The background value.
| bandIndex | number //int32|The band index of the band being stretched.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
| colorScheme | string|The color ramp scheme name.
| customStretchMax | number //double|The color stretch custom max.
| customStretchMin | number //double|The color stretch custom min.
| displayBackgroundValue | boolean|A boolean indicating whether or not to display the background.
| ESRIStretchContrast | number //double|The Esri stretch contrast parameter.
| ESRIStretchMean | number //double|The Esri stretch mean parameter.
| gammaValue | number //double|The gamma value.
| hillshadeZFactor | number //double|The hillshade Z factor.
| invert | boolean|A boolean value indicating whether or not to invert the stretch.
| lookup | [long]|A long array of lookup values.
| maxPercent | number //double|The max percent.
| minPercent | number //double|The min percent.
| standardDeviationParam | number //double|The standard deviation parameter value.
| statsHistogram | [StatsHistogram](ExternalReferences.md#statshistogram)|The statistics histogram.
| statsType | [enumeration RasterStretchStatsType](CIMEnumerations.md#enumeration-rasterstretchstatstype)|The type of raster stretch statistics.
| stretchClasses | [CIMRasterStretchClass](CIMImageLayers.md#cimrasterstretchclass) |The raster stretch classes.
| stretchStats | [StatsHistogram](ExternalReferences.md#statshistogram)|The raster stretch statistics.
| stretchType | [enumeration RasterStretchType](CIMEnumerations.md#enumeration-rasterstretchtype)|The raster stretch type.
| useCustomMinMax | boolean|A boolean value indicating whether or not to use custom min and max.
| useCustomStretchMinMax | boolean|A boolean value indicating whether or not to use custom stretch min and max.
| useGammaStretch | boolean|A boolean value indicating whether or not to use gamma stretch.
| useHillshade | boolean|A boolean value indicating whether or not to hillshade.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format applied to the display of values.






## CIMRasterUniqueValueClass
Represents a raster unique value class.


### CIMRasterUniqueValueClass

|Property | Type | Description |
|---------|--------|--------|
| values | [string,]|The class values as a string array.
| label | string|The class label.
| description | string|The class description.
| color | [Color](Types.md#color)|The class color.
| editable | boolean|A boolean indicating whether or not this class is editable.
| visible | boolean|A boolean indicating whether or not this class is visible.






## CIMRasterUniqueValueColorizer
Represents a raster unique value colorizer.


### CIMOrthoRectification

|Property | Type | Description |
|---------|--------|--------|
| constantZ | number //double|The constant Z value in meters.
| ZFactor | number //double|The conversion factor from DEM Z unit to meters.
| ZOffset | number //double|The Z offset in meters applied to DEM.
| geoid | boolean|The a boolean option indicating if Geoid correction is needed.
| DEM | [DataConnection](Types.md#dataconnection)|The data connection of the DEM used for orthorectification.


### CIMRasterColorizer

|Property | Type | Description |
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|The raster resampling type.
| contrast | number //int32|The contrast value.
| brightness | number //int32|The brightness value.
| noDataColor | [Color](Types.md#color)|The no data color.


### CIMRasterUniqueValueColorizer

|Property | Type | Description |
|---------|--------|--------|
| defaultColor | [Color](Types.md#color)|The default color.
| useDefaultColor | boolean|A boolean value indicating whether or not to use the default color.
| fieldName | string|The field name to render.
| groups | [CIMRasterUniqueValueGroup](CIMImageLayers.md#cimrasteruniquevaluegroup) |The unique value groups.
| colorRamp | [ColorRamp](Types.md#colorramp)|The color ramp.
| defaultLabel | string|The default label.
| defaultDescription | string|The default description.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format applied to values for display.






## CIMRasterUniqueValueGroup
Represents a raster unique value group.


### CIMRasterUniqueValueGroup

|Property | Type | Description |
|---------|--------|--------|
| classes | [CIMRasterUniqueValueClass](CIMImageLayers.md#cimrasteruniquevalueclass) |An array of classes making up the group.
| heading | string|The group heading.






## CIMRasterVectorFieldColorizer
Represents a raster vector field colorizer.


### CIMOrthoRectification

|Property | Type | Description |
|---------|--------|--------|
| constantZ | number //double|The constant Z value in meters.
| ZFactor | number //double|The conversion factor from DEM Z unit to meters.
| ZOffset | number //double|The Z offset in meters applied to DEM.
| geoid | boolean|The a boolean option indicating if Geoid correction is needed.
| DEM | [DataConnection](Types.md#dataconnection)|The data connection of the DEM used for orthorectification.


### CIMRasterColorizer

|Property | Type | Description |
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|The raster resampling type.
| contrast | number //int32|The contrast value.
| brightness | number //int32|The brightness value.
| noDataColor | [Color](Types.md#color)|The no data color.


### CIMRasterVectorFieldColorizer

|Property | Type | Description |
|---------|--------|--------|
| magnitudeBandIndex | number //int32|The magnitude band index.
| directionBandIndex | number //int32|The direction band index.
| isUVComponents | boolean|A boolean indicating whether flow is composed from U and V components.
| referenceSystem | [enumeration SymbolRotationType](CIMSymbolizers.md#enumeration-symbolrotationtype)|The reference system for symbol rotation.
| flowRepresentation | [enumeration FlowRepresentationType](CIMImageLayers.md#enumeration-flowrepresentationtype)|The flow representation type.
| symbolTileSize | number //double|The symbol tile size.
| symbolTileSizeUnits | [enumeration SymbolTileUnitType](CIMImageLayers.md#enumeration-symboltileunittype)|The symbol tile size units.
| symbolizationType | [enumeration SymbolizationType](CIMImageLayers.md#enumeration-symbolizationtype)|The symbolization type.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol.
| classBreaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |The class breaks.
| minimumClassBreak | number //double|The minimum class break.
| minimumMagnitude | number //double|The minimum magnitude.
| maximumMagnitude | number //double|The maximum magnitude.
| minimumSymbolSize | number //double|The minimum symbol size.
| maximumSymbolSize | number //double|The maximum symbol size.
| fromUnit | [enumeration SpeedUnitType](CIMImageLayers.md#enumeration-speedunittype)|The from unit.
| toUnit | [enumeration SpeedUnitType](CIMImageLayers.md#enumeration-speedunittype)|The to unit.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format used for format values for display.






## CIMRenderingRule
Represents a raster rendering rule.


### CIMRenderingRule

|Property | Type | Description |
|---------|--------|--------|
| description | string|The rendering rule description
| name | string|The rendering rule name.
| variableName | string|The rendering rule variable name.
| arguments | Object|The rendering rule arguments as a property set.
| definition | string|The rendering rule definition.





### Enumeration: SpeedUnitType
Speed unit types.

|Property | Value | Description |
|---------|--------|--------|
| Unknown| 0| Unknown speed.
| MetersPerSecond| 1| Meters per second.
| KilometersPerHour| 2| Kilometers per hour.
| Knots| 3| Knots.
| FeetPerSecond| 4| Feed per second.
| MilesPerHour| 5| Miles per hour.




## CIMStandaloneVideo
Represents a standalone video.


### CIMDefinition

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| URI | string|The URI of the definition. Typically set by the system and used as an identifier.
| sourceURI | string|The source URI of the item. Set if sourced from an external item such as an item on a portal.
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|The time the definition was last modfied.
| metadataURI | string|The metadata URI.
| useSourceMetadata | boolean|A boolean indicating if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project.


### CIMStandaloneVideoDefinition

|Property | Type | Description |
|---------|--------|--------|
| dataConnection | [CIMVideoDataConnection](CIMImageLayers.md#cimvideodataconnection)|The data connection for the video.
| footprintColor | [Color](Types.md#color)|The footprint color.
| elapsedTime | number //double|Elapsed time in seconds.





### Enumeration: StretchType
Stretch types.

|Property | Value | Description |
|---------|--------|--------|
| Gamma| 0| Gamma stretch.
| MinMax| 1| Min max stretch.
| StdDev| 2| Standard deviation stretch.
| None| 3| No stretch.



### Enumeration: SymbolTileUnitType
Symbol tile unit type.

|Property | Value | Description |
|---------|--------|--------|
| Unknown| 0| Unknown.
| Feet| 1| Feet.
| Miles| 2| Miles.
| NauticalMiles| 3| Nautical miles.
| Meters| 4| Meters.
| Kilometers| 5| Kilometers.
| DecimalDegrees| 6| Decimal degrees.
| Pixels| 100| Pixels.



### Enumeration: SymbolizationType
Symbolization type.

|Property | Value | Description |
|---------|--------|--------|
| Scalar| 0| Scalar.
| SingleArrow| 1| Single Arrow.
| WindBarbs| 2| Wind barbs.
| BeaufortWindKnots| 3| Beaufort wind knots.
| BeaufortWindMetersPerSecond| 4| Beaufort wind meters per second.
| OceanCurrentKnots| 5| Ocean current knots.
| OceanCurrentMetersPerSecond| 6| Ocean current meters per second.
| BeaufortWindMilesPerHour| 7| Beaufort wind miles per hour.
| BeaufortWindKilometersPerHour| 8| Beaufort wind kilometers per hour.
| Custom| 100| Custom.



### Enumeration: TargetColorSurfaceType
Target color surface type.

|Property | Value | Description |
|---------|--------|--------|
| SingleColorPoint| 0| Single color point.
| ColorGrid| 1| Color grid.
| FirstOrderSurface| 2| First order surface.
| SecondOrderSurface| 3| Second order surface.
| ThirdOrderSurface| 4| Third order surface.




## CIMVideoDataConnection
Represents a video data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMVideoDataConnection

|Property | Type | Description |
|---------|--------|--------|
| URI | string|The URI of the video files.
