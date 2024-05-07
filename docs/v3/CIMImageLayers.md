


## CIMAuxiliaryRasterProperties
#### Represents auxiliary raster properties. 


### CIMAuxiliaryRasterProperties 

|Property | Type | Description | 
|---------|--------|--------|
| bandIndexes | [long] | A long array of the band indexes. 
| extent | [Envelope](ExternalReferences.md#envelope) | The extent. 
| height | long | The height. 
| width | long | The width. 





### Enumeration: ColorBalanceMethod
#### A list of color balance methods. 

|Property | Value | Description | 
|---------|--------|--------|
| Dodging| 0| Dodging. 
| Histogram| 1| Histogram. 
| StdDev| 2| Standard deviation. 
| None| 3| None. 



### Enumeration: ColorCorrectionStretchType
#### A list of color correction stretch types. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| None. 
| Adaptive| 1| Adaptive. 
| MinMax| 2| Minimum and maximum. 
| StdDev| 3| Standard deviation. 



### Enumeration: ColorMatchingMethod
#### A list of color matching methods. 

|Property | Value | Description | 
|---------|--------|--------|
| Statistics| 0| Statistics. 
| Histogram| 1| Histogram. 
| LinearCorrelation| 2| Linear correlation. 
| None| 3| None. 



### Enumeration: ColorizerHillshadeType
#### A list of hillshade types for colorizer. 

|Property | Value | Description | 
|---------|--------|--------|
| Traditional| 0| Calculates hillshade from a single illumination direction. You can set the Azimuth and Altitude options to control the location of the light source. 
| Multidirectional| 1| Combines light from multiple sources to represent an enhanced visualization of the terrain. 



### Enumeration: ColorizerScalingType
#### A list of scaling types for colorizer. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No scaling is applied. This is ideal for a single raster dataset covering a local area. 
| Adjusted| 1| A nonlinear adjustment is applied using the default Pixel Size Power and Pixel Size Factor values, which accommodate a wide variety of altitude changes (scale) as the viewer zooms in and out. 




## CIMFeatureMosaicSubLayer
#### Represents mosaic feature sub layer. 


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


### CIMFeatureLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| autoGenerateFeatureTemplates | boolean | A value indicating whether to automatically generate feature templates from the renderer. 
| extrusion | [CIMFeatureExtrusion](CIMVectorLayers.md#cimfeatureextrusion) | The feature extrusion. 
| featureElevationExpression | string | The feature elevation expression. 
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable) | The feature table. 
| featureTemplates | [[CIMEditingTemplate]](Types.md#editingtemplate) | The feature templates. 
| htmlPopupEnabled | boolean | A value indicating whether HTML pop-ups are enabled. 
| htmlPopupFormat | [CIMHtmlPopupFormat](CIMVectorLayers.md#cimhtmlpopupformat) | The HTML pop-ups format. 
| isFlattened | boolean | A value indicating whether the layer is flattened. 
| selectable | boolean | A value indicating whether the layer is selectable. 
| selectionColor | [Color](Types.md#color) | The selection color. For polygons, this is used as the outline color. 
| polygonSelectionFillColor | [Color](Types.md#color) | The selection fill color. Only used for polygons. 
| selectionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The selection symbol. 
| useSelectionSymbol | boolean | A value indicating whether to use the selection symbol. 
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition) | The page definition which allows for using current map series page to filter features. 
| featureCacheType | [enumeration FeatureCacheType](CIMVectorLayers.md#enumeration-featurecachetype) | The feature cache type. 
| enableDisplayFilters | boolean | A value indicating whether the current set of display filters are honored during drawing. 
| displayFilters | [[CIMDisplayFilter]](CIMVectorLayers.md#cimdisplayfilter) | The current set of scale based display filters. 
| displayFiltersType | [enumeration DisplayFilterType](CIMVectorLayers.md#enumeration-displayfiltertype) | DisplayFiltersType value. 
| displayFilterName | string | The active display filter. 
| displayFilterChoices | [[CIMDisplayFilter]](CIMVectorLayers.md#cimdisplayfilter) | The current set of display filters. 
| featureElevationExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The expression for setting the feature elevation. 
| featureBlendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The per-feature blending mode which allows features in a layer to blend against other features in the same layer that have already drawn. 
| featureSortInfos | [[CIMFeatureSortInfo]](CIMVectorLayers.md#cimfeaturesortinfo) | The collection of field names and sort directions used to sort features during draw. 
| layerEffectsMode | [enumeration LayerEffectsMode](CIMLayer.md#enumeration-layereffectsmode) | The layer effects mode. 
| featureEffects | [CIMFeatureLayerEffect](CIMLayer.md#cimfeaturelayereffect) | The collection of layer effects that apply to subset of features. 


### CIMGeoFeatureLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| actions | [[CIMLayerAction]](CIMVectorLayers.md#cimlayeraction) | The layer actions. 
| exclusionSet | [long long] | The set of excluded features. 
| featureMasks | [[CIMDataConnection]](Types.md#dataconnection) | The data connection of the masking data. 
| labelClasses | [[CIMLabelClass]](CIMLabelPlacement.md#cimlabelclass) | The collection of label class definitions. 
| labelVisibility | boolean | A value indicating whether to display labels for this layer's label classes. 
| maskedSymbolLayers | [[CIMSymbolLayerMasking]](CIMVectorLayers.md#cimsymbollayermasking) | The masked symbol layers. Each SymbolLayerMasking gives the symbol layers that are masked by that masking layer. 
| renderer | [Renderer](Types.md#renderer) | The primary symbol renderer. 
| scaleSymbols | boolean | A value indicating whether to scale the symbols in this layer based on the map's reference scale. 
| snappable | boolean | A value indicating whether this layer participates in snapping in the editor. 
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing) | The symbol layer drawing properties. 
| trackLinesRenderer | [Renderer](Types.md#renderer) | The track renderer when displaying tracks. 
| previousObservationsRenderer | [Renderer](Types.md#renderer) | The previous observations renderer. 
| previousObservationsCount | long | The previous observation count. 
| useRealWorldSymbolSizes | boolean | A value indicating whether to use real world symbols sizes (meters) vs. points. This value should always be in sync with the UseRealWorldSymbolSizes property at the symbol level. 
| showPreviousObservations | boolean | A value indicating whether previous observations are being drawn. 
| featureReduction | [FeatureReduction](Types.md#featurereduction) | The feature reduction technique in use by this layer. 
| showTracks | boolean | A value indicating whether track lines are being drawn. 


### CIMMosaicSubLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| mosaicSubLayerType | [enumeration MosaicSubLayerType](CIMImageLayers.md#enumeration-mosaicsublayertype) | The mosaic sublayer type. 





### Enumeration: FlowRepresentationType
#### A list of flow representation types. 

|Property | Value | Description | 
|---------|--------|--------|
| From| 0| Flow from. 
| To| 1| Flow to. 




## CIMImageMosaicSubLayer
#### Represents an image mosaic sublayer. 


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


### CIMRasterLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection for the raster this layer is based on. 
| colorizer | [RasterColorizer](Types.md#rastercolorizer) | The raster colorizer. 
| attributeTable | [CIMRasterTable](CIMVectorLayers.md#cimrastertable) | The raster table definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition) | The time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition) | The time dimension fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition) | The time definition. 
| auxiliaryRasterProperties | [CIMAuxiliaryRasterProperties](CIMImageLayers.md#cimauxiliaryrasterproperties) | The auxiliary raster properties. 
| autoComputeStatsHistogram | boolean | A value indicating whether or not to automatically compute the statistics histogram. 
| rangeDefinitions | [[CIMRangeDefinition]](CIMVectorLayers.md#cimrangedefinition) | The range definitions. 
| activeRangeName | string | The name of the active range. 
| activeVariables | [string] | The active variables. 
| multidimensionalExtent | [CIMRasterMultidimensionalExtentDefinition](CIMImageLayers.md#cimrastermultidimensionalextentdefinition) | A multidimensional extent definition describing the data cube(s) used for analysis. 
| activeSlice | [CIMRasterMultidimensionalDisplayDefinition](CIMImageLayers.md#cimrastermultidimensionaldisplaydefinition) | A multidimensional display definition describing the current display slice. 
| renderingRule | [CIMRenderingRule](CIMImageLayers.md#cimrenderingrule) | The rendering rule. 
| activeCustomColorizer | string | The active custom colorizer. 
| customColorizers | [[CIMRasterColorizer]](Types.md#rastercolorizer) | The custom colorizers. 


### CIMImageServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| compression | string | The compression as a string. 
| compressionQuality | long | The compression quality. 
| drawFootprints | boolean | A value indicating whether or not to draw footprints. 
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable) | The feature table. 
| footprintDrawMode | [enumeration RasterFootprintDrawMode](CIMImageLayers.md#enumeration-rasterfootprintdrawmode) | The footprint draw mode. 
| footprintSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The footprint symbol. 
| mosaicRule | [CIMMosaicRule](CIMImageLayers.md#cimmosaicrule) | The mosaic rule. 
| selectable | boolean | A value indicating whether or not the layer is selectable. 
| selectionColor | [Color](Types.md#color) | The selection color. 
| selectionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The selection symbol. 
| useSelectionSymbol | boolean | A value indicating whether or not to use the selection symbol. 
| ignoreRenderingRuleOnIdentify | boolean | A value indicating whether or not to ignore the rendering rule on identify. 
| useServiceCache | boolean | A value indicating whether or not to use the service cache. 
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition) | The page definition which allows for using current map series page to filter features. 


### CIMMosaicSubLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| mosaicSubLayerType | [enumeration MosaicSubLayerType](CIMImageLayers.md#enumeration-mosaicsublayertype) | The mosaic sublayer type. 






## CIMImageServiceLayer
#### Represents an image service layer corresponding to an ArcGIS Server image service. 


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


### CIMRasterLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection for the raster this layer is based on. 
| colorizer | [RasterColorizer](Types.md#rastercolorizer) | The raster colorizer. 
| attributeTable | [CIMRasterTable](CIMVectorLayers.md#cimrastertable) | The raster table definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition) | The time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition) | The time dimension fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition) | The time definition. 
| auxiliaryRasterProperties | [CIMAuxiliaryRasterProperties](CIMImageLayers.md#cimauxiliaryrasterproperties) | The auxiliary raster properties. 
| autoComputeStatsHistogram | boolean | A value indicating whether or not to automatically compute the statistics histogram. 
| rangeDefinitions | [[CIMRangeDefinition]](CIMVectorLayers.md#cimrangedefinition) | The range definitions. 
| activeRangeName | string | The name of the active range. 
| activeVariables | [string] | The active variables. 
| multidimensionalExtent | [CIMRasterMultidimensionalExtentDefinition](CIMImageLayers.md#cimrastermultidimensionalextentdefinition) | A multidimensional extent definition describing the data cube(s) used for analysis. 
| activeSlice | [CIMRasterMultidimensionalDisplayDefinition](CIMImageLayers.md#cimrastermultidimensionaldisplaydefinition) | A multidimensional display definition describing the current display slice. 
| renderingRule | [CIMRenderingRule](CIMImageLayers.md#cimrenderingrule) | The rendering rule. 
| activeCustomColorizer | string | The active custom colorizer. 
| customColorizers | [[CIMRasterColorizer]](Types.md#rastercolorizer) | The custom colorizers. 


### CIMImageServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| compression | string | The compression as a string. 
| compressionQuality | long | The compression quality. 
| drawFootprints | boolean | A value indicating whether or not to draw footprints. 
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable) | The feature table. 
| footprintDrawMode | [enumeration RasterFootprintDrawMode](CIMImageLayers.md#enumeration-rasterfootprintdrawmode) | The footprint draw mode. 
| footprintSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The footprint symbol. 
| mosaicRule | [CIMMosaicRule](CIMImageLayers.md#cimmosaicrule) | The mosaic rule. 
| selectable | boolean | A value indicating whether or not the layer is selectable. 
| selectionColor | [Color](Types.md#color) | The selection color. 
| selectionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The selection symbol. 
| useSelectionSymbol | boolean | A value indicating whether or not to use the selection symbol. 
| ignoreRenderingRuleOnIdentify | boolean | A value indicating whether or not to ignore the rendering rule on identify. 
| useServiceCache | boolean | A value indicating whether or not to use the service cache. 
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition) | The page definition which allows for using current map series page to filter features. 






## CIMMosaicLayer
#### Represents a mosaic layer corresponding to a mosaic dataset. 


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


### CIMMosaicLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| boundaryLayer | string | The boundary layer. 
| footprintLayer | string | The footprint layer. 
| imageLayer | string | The image layer. 
| seamlineLayer | string | The seamline layer. 
| mosaicDatasetConnection | [DataConnection](Types.md#dataconnection) | The data connection of the mosaic dataset. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition) | The time definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition) | The time display definition. 
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition) | The time fields. 
| definitionExpression | string | The definition expression. 
| definitionExpressionName | string | The Name of definition expression. 
| definitionFilterChoices | [[CIMDefinitionFilter]](CIMLayer.md#cimdefinitionfilter) | The definition filter choices. 
| rangeDefinitions | [[CIMRangeDefinition]](CIMVectorLayers.md#cimrangedefinition) | The range definitions of the mosaic dataset. 
| activeRangeName | string | The name of the active range. 
| activeVariables | [string] | An array of the active variables. 
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition) | The page definition which allows for using current map series page to filter features. 






## CIMMosaicRule
#### Represents a mosaic rule. 


### CIMMosaicRule 

|Property | Type | Description | 
|---------|--------|--------|
| ascending | boolean | A value indicating whether the mosaic rule uses ascending order. 
| FIDs | [long long] | An array of IDs. 
| lockRasterID | string | The ID of the lock raster. 
| mosaicMethod | [enumeration RasterMosaicMethod](CIMImageLayers.md#enumeration-rastermosaicmethod) | The mosaic method. 
| mosaicOperatorType | [enumeration RasterMosaicOperatorType](CIMImageLayers.md#enumeration-rastermosaicoperatortype) | The mosaic operator type. 
| orderByBaseValue | any | The order by base value. 
| orderByFieldName | string | The order by field name. 
| timeValue | [TimeValue](ExternalReferences.md#timevalue) | The time value. 
| viewpoint | [Point](ExternalReferences.md#point) | The viewpoint as a point. 
| whereClause | string | The where clause as a string. 





### Enumeration: MosaicSubLayerType
#### Types of mosaic sublayers. 

|Property | Value | Description | 
|---------|--------|--------|
| Boundary| 0| Boundary 
| Footprint| 1| Footprint 
| Image| 2| Image 
| Seamline| 3| Seamline 




## CIMNITFDataConnection
#### Represents a NITF data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMNITFDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string | The URI of the NITF files. 






## CIMNitfFeatureSubLayer
#### Represents NITF feature sub layer. 


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


### CIMFeatureLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| autoGenerateFeatureTemplates | boolean | A value indicating whether to automatically generate feature templates from the renderer. 
| extrusion | [CIMFeatureExtrusion](CIMVectorLayers.md#cimfeatureextrusion) | The feature extrusion. 
| featureElevationExpression | string | The feature elevation expression. 
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable) | The feature table. 
| featureTemplates | [[CIMEditingTemplate]](Types.md#editingtemplate) | The feature templates. 
| htmlPopupEnabled | boolean | A value indicating whether HTML pop-ups are enabled. 
| htmlPopupFormat | [CIMHtmlPopupFormat](CIMVectorLayers.md#cimhtmlpopupformat) | The HTML pop-ups format. 
| isFlattened | boolean | A value indicating whether the layer is flattened. 
| selectable | boolean | A value indicating whether the layer is selectable. 
| selectionColor | [Color](Types.md#color) | The selection color. For polygons, this is used as the outline color. 
| polygonSelectionFillColor | [Color](Types.md#color) | The selection fill color. Only used for polygons. 
| selectionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The selection symbol. 
| useSelectionSymbol | boolean | A value indicating whether to use the selection symbol. 
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition) | The page definition which allows for using current map series page to filter features. 
| featureCacheType | [enumeration FeatureCacheType](CIMVectorLayers.md#enumeration-featurecachetype) | The feature cache type. 
| enableDisplayFilters | boolean | A value indicating whether the current set of display filters are honored during drawing. 
| displayFilters | [[CIMDisplayFilter]](CIMVectorLayers.md#cimdisplayfilter) | The current set of scale based display filters. 
| displayFiltersType | [enumeration DisplayFilterType](CIMVectorLayers.md#enumeration-displayfiltertype) | DisplayFiltersType value. 
| displayFilterName | string | The active display filter. 
| displayFilterChoices | [[CIMDisplayFilter]](CIMVectorLayers.md#cimdisplayfilter) | The current set of display filters. 
| featureElevationExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The expression for setting the feature elevation. 
| featureBlendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The per-feature blending mode which allows features in a layer to blend against other features in the same layer that have already drawn. 
| featureSortInfos | [[CIMFeatureSortInfo]](CIMVectorLayers.md#cimfeaturesortinfo) | The collection of field names and sort directions used to sort features during draw. 
| layerEffectsMode | [enumeration LayerEffectsMode](CIMLayer.md#enumeration-layereffectsmode) | The layer effects mode. 
| featureEffects | [CIMFeatureLayerEffect](CIMLayer.md#cimfeaturelayereffect) | The collection of layer effects that apply to subset of features. 


### CIMGeoFeatureLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| actions | [[CIMLayerAction]](CIMVectorLayers.md#cimlayeraction) | The layer actions. 
| exclusionSet | [long long] | The set of excluded features. 
| featureMasks | [[CIMDataConnection]](Types.md#dataconnection) | The data connection of the masking data. 
| labelClasses | [[CIMLabelClass]](CIMLabelPlacement.md#cimlabelclass) | The collection of label class definitions. 
| labelVisibility | boolean | A value indicating whether to display labels for this layer's label classes. 
| maskedSymbolLayers | [[CIMSymbolLayerMasking]](CIMVectorLayers.md#cimsymbollayermasking) | The masked symbol layers. Each SymbolLayerMasking gives the symbol layers that are masked by that masking layer. 
| renderer | [Renderer](Types.md#renderer) | The primary symbol renderer. 
| scaleSymbols | boolean | A value indicating whether to scale the symbols in this layer based on the map's reference scale. 
| snappable | boolean | A value indicating whether this layer participates in snapping in the editor. 
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing) | The symbol layer drawing properties. 
| trackLinesRenderer | [Renderer](Types.md#renderer) | The track renderer when displaying tracks. 
| previousObservationsRenderer | [Renderer](Types.md#renderer) | The previous observations renderer. 
| previousObservationsCount | long | The previous observation count. 
| useRealWorldSymbolSizes | boolean | A value indicating whether to use real world symbols sizes (meters) vs. points. This value should always be in sync with the UseRealWorldSymbolSizes property at the symbol level. 
| showPreviousObservations | boolean | A value indicating whether previous observations are being drawn. 
| featureReduction | [FeatureReduction](Types.md#featurereduction) | The feature reduction technique in use by this layer. 
| showTracks | boolean | A value indicating whether track lines are being drawn. 


### CIMNitfSubLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|






## CIMNitfImageSubLayer
#### Represents NITF image sub layer. 


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


### CIMRasterLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection for the raster this layer is based on. 
| colorizer | [RasterColorizer](Types.md#rastercolorizer) | The raster colorizer. 
| attributeTable | [CIMRasterTable](CIMVectorLayers.md#cimrastertable) | The raster table definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition) | The time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition) | The time dimension fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition) | The time definition. 
| auxiliaryRasterProperties | [CIMAuxiliaryRasterProperties](CIMImageLayers.md#cimauxiliaryrasterproperties) | The auxiliary raster properties. 
| autoComputeStatsHistogram | boolean | A value indicating whether or not to automatically compute the statistics histogram. 
| rangeDefinitions | [[CIMRangeDefinition]](CIMVectorLayers.md#cimrangedefinition) | The range definitions. 
| activeRangeName | string | The name of the active range. 
| activeVariables | [string] | The active variables. 
| multidimensionalExtent | [CIMRasterMultidimensionalExtentDefinition](CIMImageLayers.md#cimrastermultidimensionalextentdefinition) | A multidimensional extent definition describing the data cube(s) used for analysis. 
| activeSlice | [CIMRasterMultidimensionalDisplayDefinition](CIMImageLayers.md#cimrastermultidimensionaldisplaydefinition) | A multidimensional display definition describing the current display slice. 
| renderingRule | [CIMRenderingRule](CIMImageLayers.md#cimrenderingrule) | The rendering rule. 
| activeCustomColorizer | string | The active custom colorizer. 
| customColorizers | [[CIMRasterColorizer]](Types.md#rastercolorizer) | The custom colorizers. 


### CIMNitfSubLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|






## CIMNitfLayer
#### Represents a NITF composite layer. 


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


### CIMStandaloneTableContainer 

|Property | Type | Description | 
|---------|--------|--------|
| standaloneTables | [string] | The standalone tables as an array of table repository paths. 


### CIMNitfLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection for the raster this layer is based on. 
| layers | [string] | The layer URIs of the layers in the NITF layer. 
| extraItems | [string] | The names of the layers (and tables) not visible by default. 






## CIMPansharpeningFilter
#### Represents a pansharpening filter. 


### CIMPansharpeningFilter 

|Property | Type | Description | 
|---------|--------|--------|
| panImage | [DataConnection](Types.md#dataconnection) | The data connection of the optional panchromatic image. 
| pansharpeningType | [enumeration PansharpeningType](CIMImageLayers.md#enumeration-pansharpeningtype) | The data connection of the current pansharpening type. 
| infraredImage | [DataConnection](Types.md#dataconnection) | The data connection of the optional infrared image. 
| RWeight | double | The red weight. 
| GWeight | double | The green weight. 
| BWeight | double | The blue weight. 
| IWeight | double | The infrared weight. 





### Enumeration: PansharpeningType
#### Types of pansharpening. 

|Property | Value | Description | 
|---------|--------|--------|
| IHS| 0| IHS. 
| Brovey| 1| Brovey. 
| ESRI| 2| Esri. 
| Mean| 3| Mean. 




## CIMRangeDimensionValue
#### Represents a range dimension name and value pair used to define the multidimensional display definition for the current display slice. 


### CIMRangeDimensionValue 

|Property | Type | Description | 
|---------|--------|--------|
| rangeDimensionName | string | The name of the dimension. 
| rangeDimensionValue | [CIMRange](CIMVectorLayers.md#cimrange) | The range dimension value. 






## CIMRasterBandDataConnection
#### Represents a raster band data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string | The workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory) | The workspace factory. 
| customWorkspaceFactoryCLSID | string | The classID of the custom workspace factory. 
| dataset | string | The dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype) | The dataset type. 


### CIMRasterBandDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| rasterBandName | string | The raster band name. 






## CIMRasterCMYKColorizer
#### Represents a raster CMYK colorizer. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype) | The raster resampling type. 
| contrast | long | The contrast value. 
| brightness | long | The brightness value. 
| noDataColor | [Color](Types.md#color) | The no data color. 
| name | string | The name. 


### CIMRasterCMYKColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundColor | [Color](Types.md#color) | The background color. 
| backgroundValueBlack | double | The background value for black. 
| backgroundValueCyan | double | The background value for cyan. 
| backgroundValueMagenta | double | The background value for magenta. 
| backgroundValueYellow | double | The background value for yellow. 
| blackBandIndex | long | The band index for black. 
| cyanBandIndex | long | The band index for cyan. 
| displayBackgroundValue | boolean | A value indicating whether or not to display the background value. 
| invert | boolean | A value indicating whether or not the stretch is inverted. 
| magentaBandIndex | long | The band index for magenta. 
| specificationHistogramBlack | [StatsHistogram](ExternalReferences.md#statshistogram) | The specification histogram for black. 
| specificationHistogramCyan | [StatsHistogram](ExternalReferences.md#statshistogram) | The specification histogram for cyan. 
| specificationHistogramMagenta | [StatsHistogram](ExternalReferences.md#statshistogram) | The specification histogram for magenta. 
| specificationHistogramYellow | [StatsHistogram](ExternalReferences.md#statshistogram) | The specification histogram for yellow. 
| standardDeviationParam | double | The standard deviation parameter for the stretch renderer. 
| stretchStatsBlack | [StatsHistogram](ExternalReferences.md#statshistogram) | The stretch histogram for black. 
| stretchStatsCyan | [StatsHistogram](ExternalReferences.md#statshistogram) | The stretch histogram for cyan. 
| stretchStatsMagenta | [StatsHistogram](ExternalReferences.md#statshistogram) | The stretch histogram for magenta. 
| stretchStatsType | [enumeration RasterStretchStatsType](CIMEnumerations.md#enumeration-rasterstretchstatstype) | The stretch statistics type. 
| stretchStatsYellow | [StatsHistogram](ExternalReferences.md#statshistogram) | The stretch histogram for yellow. 
| stretchType | [enumeration RasterStretchType](CIMEnumerations.md#enumeration-rasterstretchtype) | The stretch type. 
| useBlackMapping | boolean | A value indicating whether or not to use black mapping. 
| useCyanMapping | boolean | A value indicating whether or not to use cyan mapping. 
| useDefaultMapping | boolean | A value indicating whether or not to use default mapping. 
| useMagentaMapping | boolean | A value indicating whether or not to use magenta mapping. 
| useYellowMapping | boolean | A value indicating whether or not to use yellow mapping. 
| yellowBandIndex | long | The band index for yellow. 






## CIMRasterClassBreak
#### Represents a raster class break. 


### CIMRasterClassBreak 

|Property | Type | Description | 
|---------|--------|--------|
| upperBound | double | The upper bound for the raster class break. 
| label | string | The label for the raster class break. 
| description | string | The description for the raster class break. 
| color | [Color](Types.md#color) | The color for the raster class break. 






## CIMRasterClassifyColorizer
#### Represents a raster classify colorizer. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype) | The raster resampling type. 
| contrast | long | The contrast value. 
| brightness | long | The brightness value. 
| noDataColor | [Color](Types.md#color) | The no data color. 
| name | string | The name. 


### CIMDataNormalization 

|Property | Type | Description | 
|---------|--------|--------|
| normalizationField | string | The normalization field. 
| normalizationTotal | double | The normalization total. 
| normalizationType | [enumeration DataNormalizationMethod](CIMRenderers.md#enumeration-datanormalizationmethod) | The normalization type. 


### CIMRasterClassifyColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| classBreaks | [[CIMRasterClassBreak]](CIMImageLayers.md#cimrasterclassbreak) | The class breaks of the renderer. 
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| exclusionColor | [Color](Types.md#color) | The exclusion color. 
| exclusionDescription | string | The exclusion description. 
| exclusionLabel | string | The exclusion label. 
| exclusionRanges | [double] | The exclusion ranges as an array of doubles. 
| exclusionValues | [double] | The exclusion values as an array of doubles. 
| field | string | The renderer field. 
| minimumBreak | double | The minimum break of the classification. 
| showClassGaps | boolean | A value indicating whether or not to show class gaps. 
| showInAscendingOrder | boolean | A value indicating whether or not to show classes in ascending order. 
| useExclusionColor | boolean | A value indicating whether or not to use the exclusion color. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format applied to values. 
| heading | string | The legend heading. 






## CIMRasterColorCorrection
#### Represents a raster color correction configuration. 


### CIMRasterColorCorrection 

|Property | Type | Description | 
|---------|--------|--------|
| preStretchType | [enumeration ColorCorrectionStretchType](CIMImageLayers.md#enumeration-colorcorrectionstretchtype) | The pre-stretch type of color correction. 
| colorBalanceMethod | [enumeration ColorBalanceMethod](CIMImageLayers.md#enumeration-colorbalancemethod) | The color balance method. 
| colorMatchingMethod | [enumeration ColorMatchingMethod](CIMImageLayers.md#enumeration-colormatchingmethod) | The color matching method. 
| needContrastAdjustment | boolean | A value indicating whether or not contrast adjustment is needed. 
| targetColorSurfaceType | [enumeration TargetColorSurfaceType](CIMImageLayers.md#enumeration-targetcolorsurfacetype) | The target color surface type. 
| targetColorRaster | [DataConnection](Types.md#dataconnection) | The target color raster. 
| userDefinedReference | boolean | A value indicating whether or not this is a user defined reference. 
| referenceOID | long | The reference OID. 






## CIMRasterColorMapColorizer
#### Represents a raster color map colorizer. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype) | The raster resampling type. 
| contrast | long | The contrast value. 
| brightness | long | The brightness value. 
| noDataColor | [Color](Types.md#color) | The no data color. 
| name | string | The name. 


### CIMRasterColorMapColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| colors | [[CIMColor]](Types.md#color) | Array of colors. 
| bandID | long | The band ID. 
| labels | [string] | The color labels as a string array. 
| min | long | Minimum value. 
| max | long | Maximum value. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| values | [long] | The array of values. 






## CIMRasterColorizerMapping
#### Represents a raster colorizer mapping. 


### CIMRasterColorizerMapping 

|Property | Type | Description | 
|---------|--------|--------|
| rasterOID | long | The Object ID of the raster in the raster catalog. 
| colorizerIndex | long | The index of the colorizer. 






## CIMRasterDimensionalDefinition
#### Represents a set of criteria used to define the multidimensional extent of a raster layer. 


### CIMRasterDimensionalDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| variableName | string | The name of the variable. 
| dimensionName | string | The name of the dimension. 
| minimumValues | [double] | The minimum dimension values. 
| maximumValues | [double] | The maximum dimension values. 






## CIMRasterDiscreteColorColorizer
#### Represents a raster discrete color colorizer. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype) | The raster resampling type. 
| contrast | long | The contrast value. 
| brightness | long | The brightness value. 
| noDataColor | [Color](Types.md#color) | The no data color. 
| name | string | The name. 


### CIMRasterDiscreteColorColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| numColors | long | The number of colors. 
| colormap | [RasterColormap](ExternalReferences.md#rastercolormap) | The colormap. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 





### Enumeration: RasterFootprintDrawMode
#### Raster footprint draw modes. 

|Property | Value | Description | 
|---------|--------|--------|
| All| 0| Draw all footprints. 
| OnlyPrimary| 1| Draw only primary footprints. 




## CIMRasterHistogramEditInfo
#### Represents raster histogram custom stretch edit info. 


### CIMRasterHistogramEditInfo 

|Property | Type | Description | 
|---------|--------|--------|
| breakPointsX | [long] | The X coordinate or input value at each breakpoint. 
| breakPointsY | [long] | The Y coordinate or input value at each breakpoint. 
| editType | [enumeration RasterHistogramEditType](CIMImageLayers.md#enumeration-rasterhistogramedittype) | The histogram edit type. 





### Enumeration: RasterHistogramEditType
#### Raster histogram edit types. 

|Property | Value | Description | 
|---------|--------|--------|
| Lines| 0| The breakpoints represent lines defining a piecewise linear stretch. 
| Splines| 1| The breakpoints represent splines defining a piecewise non-linear stretch. 
| Points| 2| The breakpoints represent specific pixels to stretch. 




## CIMRasterLayer
#### Represents a raster layer which displays raster imagery stored in a raster dataset. 


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


### CIMRasterLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection for the raster this layer is based on. 
| colorizer | [RasterColorizer](Types.md#rastercolorizer) | The raster colorizer. 
| attributeTable | [CIMRasterTable](CIMVectorLayers.md#cimrastertable) | The raster table definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition) | The time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition) | The time dimension fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition) | The time definition. 
| auxiliaryRasterProperties | [CIMAuxiliaryRasterProperties](CIMImageLayers.md#cimauxiliaryrasterproperties) | The auxiliary raster properties. 
| autoComputeStatsHistogram | boolean | A value indicating whether or not to automatically compute the statistics histogram. 
| rangeDefinitions | [[CIMRangeDefinition]](CIMVectorLayers.md#cimrangedefinition) | The range definitions. 
| activeRangeName | string | The name of the active range. 
| activeVariables | [string] | The active variables. 
| multidimensionalExtent | [CIMRasterMultidimensionalExtentDefinition](CIMImageLayers.md#cimrastermultidimensionalextentdefinition) | A multidimensional extent definition describing the data cube(s) used for analysis. 
| activeSlice | [CIMRasterMultidimensionalDisplayDefinition](CIMImageLayers.md#cimrastermultidimensionaldisplaydefinition) | A multidimensional display definition describing the current display slice. 
| renderingRule | [CIMRenderingRule](CIMImageLayers.md#cimrenderingrule) | The rendering rule. 
| activeCustomColorizer | string | The active custom colorizer. 
| customColorizers | [[CIMRasterColorizer]](Types.md#rastercolorizer) | The custom colorizers. 





### Enumeration: RasterMosaicMethod
#### Raster mosaic methods. 

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
#### Raster mosaic operator type. 

|Property | Value | Description | 
|---------|--------|--------|
| First| 0| First. 
| Last| 1| Last. 
| Min| 2| Minimum. 
| Max| 3| Maximum. 
| Mean| 4| Mean. 
| Blend| 5| Blend. 
| Sum| 6| Sum. 




## CIMRasterMultidimensionalDisplayDefinition
#### Represents a multidimensional display definition for the current display slice. 


### CIMRasterMultidimensionalDisplayDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| variableName | string | The name of the variable. 
| timeValue | [TimeExtent](ExternalReferences.md#timeextent) | The time value for the current display slice. 
| hasRangeDimension | boolean | A value indicating whether the active variable has a range dimension. 
| rangeDimensionName | string | The name of the selected range dimension. 
| rangeDimensionValue | [CIMRange](CIMVectorLayers.md#cimrange) | The selected range dimension value for the current display slice. 
| additionalDimensionValues | [[CIMRangeDimensionValue]](CIMImageLayers.md#cimrangedimensionvalue) | The additional range dimension values for the current display slice. 






## CIMRasterMultidimensionalExtentDefinition
#### Represents a multidimensional extent applicable to a raster layer. 


### CIMRasterMultidimensionalExtentDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| subsetDefinitions | [[CIMRasterDimensionalDefinition]](CIMImageLayers.md#cimrasterdimensionaldefinition) | The dimensional definitions that define a multidimensional subset. 
| areaOfInterest | [Geometry](ExternalReferences.md#geometry) | The area of interest for the multidimensional extent. 






## CIMRasterRGBColorizer
#### Represents a raster RGB colorizer. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype) | The raster resampling type. 
| contrast | long | The contrast value. 
| brightness | long | The brightness value. 
| noDataColor | [Color](Types.md#color) | The no data color. 
| name | string | The name. 


### CIMRasterRGBColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| alphaBandIndex | long | The band to be represented in alpha. 
| backgroundColor | [Color](Types.md#color) | The background display color. 
| backgroundValueBlue | double | The background blue value. 
| backgroundValueGreen | double | The background green value. 
| backgroundValueRed | double | The background red value. 
| blueBandIndex | long | The band to be represented in blue. 
| blueLookup | [long] | The blue lookup values. 
| displayBackgroundValue | boolean | A value indicating whether or not to display the background value. 
| ESRIStretchContrastB | double | The Esri stretch contrast value for blue. 
| ESRIStretchContrastG | double | The Esri stretch contrast value for green. 
| ESRIStretchContrastR | double | The Esri stretch contrast value for red. 
| ESRIStretchMeanB | double | The Esri stretch mean value for blue. 
| ESRIStretchMeanG | double | The Esri stretch mean value for green. 
| ESRIStretchMeanR | double | The Esri stretch mean value for red. 
| gammaB | double | The gamma value for blue. 
| gammaG | double | The gamma value for green. 
| gammaR | double | The gamma value for red. 
| greenBandIndex | long | The band to be represented in green. 
| greenLookup | [long] | The green lookup values. 
| invert | boolean | A value indicating whether or not the stretch is inverted. 
| lumLookup | [long] | The lum lookup values. 
| maxPercent | double | The maximum percent. 
| minPercent | double | The minimum percent. 
| pansharpeningFilter | [CIMPansharpeningFilter](CIMImageLayers.md#cimpansharpeningfilter) | The pansharpening filter. 
| redBandIndex | long | The band to be represented in red. 
| redLookup | [long] | The red lookup values. 
| specificationHistogramBlue | [StatsHistogram](ExternalReferences.md#statshistogram) | The specification histogram for blue. 
| specificationHistogramGreen | [StatsHistogram](ExternalReferences.md#statshistogram) | The specification histogram for green. 
| specificationHistogramRed | [StatsHistogram](ExternalReferences.md#statshistogram) | The specification histogram for red. 
| standardDeviationsParam | double | The standard deviations parameter. 
| stretchStatsBlue | [StatsHistogram](ExternalReferences.md#statshistogram) | The stretch statistics for blue. 
| stretchStatsGreen | [StatsHistogram](ExternalReferences.md#statshistogram) | The stretch statistics for green. 
| stretchStatsRed | [StatsHistogram](ExternalReferences.md#statshistogram) | The stretch statistics for red. 
| stretchStatsType | [enumeration RasterStretchStatsType](CIMEnumerations.md#enumeration-rasterstretchstatstype) | The stretch statistics type. 
| stretchType | [enumeration RasterStretchType](CIMEnumerations.md#enumeration-rasterstretchtype) | The stretch type. 
| useAlphaBand | boolean | A value indicating whether or not to use the alpha band. 
| useBlueBand | boolean | A value indicating whether or not to use the blue band. 
| useDefaultMapping | boolean | A value indicating whether or not to use default mapping. 
| useGammaStretch | boolean | A value indicating whether or not to use gamma stretch. 
| useGreenBand | boolean | A value indicating whether or not to use the green band. 
| useRedBand | boolean | A value indicating whether or not to use the red band. 
| heading | string | The legend heading. 
| useCustomStretchMinMax | boolean | A value indicating whether or not to use custom stretch minimum and maximum. 
| customStretchMinRed | double | The color stretch custom minimum value for red. 
| customStretchMinGreen | double | The color stretch custom minimum value for green. 
| customStretchMinBlue | double | The color stretch custom minimum value for blue. 
| customStretchMaxRed | double | The color stretch custom maximum value for red. 
| customStretchMaxGreen | double | The color stretch custom maximum value for green. 
| customStretchMaxBlue | double | The color stretch custom maximum value for blue. 
| histogramEditInfoRed | [CIMRasterHistogramEditInfo](CIMImageLayers.md#cimrasterhistogrameditinfo) | The edit info defining the histogram customization for red. 
| histogramEditInfoGreen | [CIMRasterHistogramEditInfo](CIMImageLayers.md#cimrasterhistogrameditinfo) | The edit info defining the histogram customization for green. 
| histogramEditInfoBlue | [CIMRasterHistogramEditInfo](CIMImageLayers.md#cimrasterhistogrameditinfo) | The edit info defining the histogram customization for blue. 






## CIMRasterShadedReliefColorizer
#### Represents a raster shaded relief colorizer. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype) | The raster resampling type. 
| contrast | long | The contrast value. 
| brightness | long | The brightness value. 
| noDataColor | [Color](Types.md#color) | The no data color. 
| name | string | The name. 


### CIMRasterShadedReliefColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| hillShadeType | [enumeration ColorizerHillshadeType](CIMImageLayers.md#enumeration-colorizerhillshadetype) | The hillshade type. 
| scalingType | [enumeration ColorizerScalingType](CIMImageLayers.md#enumeration-colorizerscalingtype) | The scaling type. 
| pixelSizePower | double | The pixel size power. 
| pixelSizeFactor | double | The pixel size factor. 
| azimuth | double | The azimuth. The value will be ignored if UseMapIlluminationProperties is set to true. 
| altitude | double | The Altitude. The value will be ignored if UseMapIlluminationProperties is set to true. 
| removeEdgeEffect | boolean | A value indicating whether or not to remove edge effect. 
| useMapIlluminationProperties | boolean | A value indicating whether or not to use map level illumination properties of altitude and azimuth. 
| ZFactor | double | A scaling factor used to convert the elevation values. 






## CIMRasterStretchClass
#### Represents a raster stretch class. 


### CIMRasterStretchClass 

|Property | Type | Description | 
|---------|--------|--------|
| label | string | The raster stretch class label. 
| value | double | The raster stretch class value. 






## CIMRasterStretchColorizer
#### Represents a raster stretch colorizer. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype) | The raster resampling type. 
| contrast | long | The contrast value. 
| brightness | long | The brightness value. 
| noDataColor | [Color](Types.md#color) | The no data color. 
| name | string | The name. 


### CIMRasterStretchColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundColor | [Color](Types.md#color) | The background color. 
| backgroundValue | double | The background value. 
| bandIndex | long | The band index of the band being stretched. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| colorScheme | string | The color ramp scheme name. 
| customStretchMax | double | The color stretch custom max. 
| customStretchMin | double | The color stretch custom min. 
| displayBackgroundValue | boolean | A value indicating whether or not to display the background. 
| ESRIStretchContrast | double | The Esri stretch contrast parameter. 
| ESRIStretchMean | double | The Esri stretch mean parameter. 
| gammaValue | double | The gamma value. 
| invert | boolean | A value indicating whether or not to invert the stretch. 
| lookup | [long] | A long array of lookup values. 
| maxPercent | double | The maximum percent. 
| minPercent | double | The minimum percent. 
| standardDeviationParam | double | The standard deviation parameter value. 
| statsType | [enumeration RasterStretchStatsType](CIMEnumerations.md#enumeration-rasterstretchstatstype) | The type of raster stretch statistics. 
| stretchClasses | [[CIMRasterStretchClass]](CIMImageLayers.md#cimrasterstretchclass) | The raster stretch classes. 
| stretchStats | [StatsHistogram](ExternalReferences.md#statshistogram) | The raster stretch statistics. 
| stretchType | [enumeration RasterStretchType](CIMEnumerations.md#enumeration-rasterstretchtype) | The raster stretch type. 
| useCustomStretchMinMax | boolean | A value indicating whether or not to use custom stretch minimum and maximum. 
| useGammaStretch | boolean | A value indicating whether or not to use gamma stretch. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format applied to the display of values. 
| heading | string | The legend heading. 
| specificationHistogram | [StatsHistogram](ExternalReferences.md#statshistogram) | The statistics for histogram specification stretch. 
| histogramEditInfo | [CIMRasterHistogramEditInfo](CIMImageLayers.md#cimrasterhistogrameditinfo) | The edit info defining the raster histogram customization. 
| useAdvancedLabeling | boolean | A value indicating whether or not to use advanced labeling. 






## CIMRasterUniqueValueClass
#### Represents a raster unique value class. 


### CIMRasterUniqueValueClass 

|Property | Type | Description | 
|---------|--------|--------|
| values | [string] | The class values as a string array. 
| label | string | The class label. 
| description | string | The class description. 
| color | [Color](Types.md#color) | The class color. 
| editable | boolean | A value indicating whether or not this class is editable. 
| visible | boolean | A value indicating whether or not this class is visible. 






## CIMRasterUniqueValueColorizer
#### Represents a raster unique value colorizer. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype) | The raster resampling type. 
| contrast | long | The contrast value. 
| brightness | long | The brightness value. 
| noDataColor | [Color](Types.md#color) | The no data color. 
| name | string | The name. 


### CIMRasterUniqueValueColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| defaultColor | [Color](Types.md#color) | The default color. 
| useDefaultColor | boolean | A value indicating whether or not to use the default color. 
| fieldName | string | The field name to render. 
| groups | [[CIMRasterUniqueValueGroup]](CIMImageLayers.md#cimrasteruniquevaluegroup) | The unique value groups. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| defaultLabel | string | The default label. 
| defaultDescription | string | The default description. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format applied to values for display. 






## CIMRasterUniqueValueGroup
#### Represents a raster unique value group. 


### CIMRasterUniqueValueGroup 

|Property | Type | Description | 
|---------|--------|--------|
| classes | [[CIMRasterUniqueValueClass]](CIMImageLayers.md#cimrasteruniquevalueclass) | An array of classes making up the group. 
| heading | string | The group heading. 






## CIMRasterVectorFieldColorizer
#### Represents a raster vector field colorizer. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype) | The raster resampling type. 
| contrast | long | The contrast value. 
| brightness | long | The brightness value. 
| noDataColor | [Color](Types.md#color) | The no data color. 
| name | string | The name. 


### CIMRasterVectorFieldColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| magnitudeBandIndex | long | The magnitude band index. 
| directionBandIndex | long | The direction band index. 
| isUVComponents | boolean | A value indicating whether flow is composed from U and V components. 
| referenceSystem | [enumeration SymbolRotationType](CIMRenderers.md#enumeration-symbolrotationtype) | The reference system for symbol rotation. 
| flowRepresentation | [enumeration FlowRepresentationType](CIMImageLayers.md#enumeration-flowrepresentationtype) | The flow representation type. 
| symbolTileSize | double | The symbol tile size. 
| symbolTileSizeUnits | [enumeration SymbolTileUnitType](CIMImageLayers.md#enumeration-symboltileunittype) | The symbol tile size units. 
| symbolizationType | [enumeration SymbolizationType](CIMImageLayers.md#enumeration-symbolizationtype) | The symbolization type. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | Symbol. 
| classBreaks | [[CIMClassBreak]](CIMRenderers.md#cimclassbreak) | The class breaks. 
| minimumClassBreak | double | The minimum class break. 
| minimumMagnitude | double | The minimum magnitude. 
| maximumMagnitude | double | The maximum magnitude. 
| minimumSymbolSize | double | The minimum symbol size. 
| maximumSymbolSize | double | The maximum symbol size. 
| fromUnit | [enumeration SpeedUnitType](CIMImageLayers.md#enumeration-speedunittype) | The from unit. 
| toUnit | [enumeration SpeedUnitType](CIMImageLayers.md#enumeration-speedunittype) | The to unit. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format used for format values for display. 






## CIMRenderingRule
#### Represents a raster rendering rule. 


### CIMRenderingRule 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The rendering rule description. 
| name | string | The rendering rule name. 
| variableName | string | The rendering rule variable name. 
| arguments | {JSON_object}| The rendering rule arguments as a property set. 
| definition | string | The rendering rule definition. 





### Enumeration: SpeedUnitType
#### Speed unit types. 

|Property | Value | Description | 
|---------|--------|--------|
| Unknown| 0| Unknown speed. 
| MetersPerSecond| 1| Meters per second. 
| KilometersPerHour| 2| Kilometers per hour. 
| Knots| 3| Knots. 
| FeetPerSecond| 4| Feed per second. 
| MilesPerHour| 5| Miles per hour. 




## CIMStandaloneVideo
#### Represents a standalone video. 


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


### CIMStandaloneVideoDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [CIMVideoDataConnection](CIMImageLayers.md#cimvideodataconnection) | The data connection for the video. 
| footprintColor | [Color](Types.md#color) | The footprint color. 
| elapsedTime | double | The elapsed time in seconds. 
| visibility | boolean | A value indicating whether the standalone video graphics is visible. 
| expanded | boolean | A value indicating whether the standalone video is expanded in the contents pane. 
| frameCenterGraphic | [CIMVideoGraphicElement](CIMImageLayers.md#cimvideographicelement) | The graphic element representing the frame center. 
| frameOutlineGraphic | [CIMVideoGraphicElement](CIMImageLayers.md#cimvideographicelement) | The graphic element representing the frame outline. 
| platformTrailGraphic | [CIMVideoGraphicElement](CIMImageLayers.md#cimvideographicelement) | The graphic element representing the platform trail. 
| platformPositionGraphic | [CIMVideoGraphicElement](CIMImageLayers.md#cimvideographicelement) | The graphic element representing the platform position. 
| bookmarkIndicators | [[CIMVideoTimelineEventIndicator]](CIMImageLayers.md#cimvideotimelineeventindicator) | The collection of event indicators for Bookmark. 
| exportFrameIndicators | [[CIMVideoTimelineEventIndicator]](CIMImageLayers.md#cimvideotimelineeventindicator) | The collection of event indicators for ExportFrame. 
| exportToPPTIndicators | [[CIMVideoTimelineEventIndicator]](CIMImageLayers.md#cimvideotimelineeventindicator) | The collection of event indicators for ExportToPPT. 
| exportFramesIndicators | [[CIMVideoTimelineRangeIndicator]](CIMImageLayers.md#cimvideotimelinerangeindicator) | The collection of range indicators for ExportFrames. 
| metadataToCSVIndicators | [[CIMVideoTimelineRangeIndicator]](CIMImageLayers.md#cimvideotimelinerangeindicator) | The collection of range indicators for MetadataToCSV. 
| recordVideoIndicators | [[CIMVideoTimelineRangeIndicator]](CIMImageLayers.md#cimvideotimelinerangeindicator) | The collection of range indicators for RecordVideo. 
| exportSegmentIndicators | [[CIMVideoTimelineRangeIndicator]](CIMImageLayers.md#cimvideotimelinerangeindicator) | The collection of range indicators for ExportSegment. 
| recordSegmentsIndicators | [[CIMVideoTimelineRangeIndicator]](CIMImageLayers.md#cimvideotimelinerangeindicator) | The collection of range indicators for RecordSegments. 
| selectedKLVChannels | [long] | The collection of selected Key-Length-Value (KLV) channels. 





### Enumeration: StretchType
#### Stretch types. 

|Property | Value | Description | 
|---------|--------|--------|
| Gamma| 0| Gamma stretch. 
| MinMax| 1| Minimum maximum stretch. 
| StdDev| 2| Standard deviation stretch. 
| None| 3| No stretch. 



### Enumeration: SymbolTileUnitType
#### Symbol tile unit type. 

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
#### Symbolization type. 

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
| ClassifiedArrow| 9| Classified arrow. 
| Custom| 100| Custom. 



### Enumeration: TargetColorSurfaceType
#### Target color surface type. 

|Property | Value | Description | 
|---------|--------|--------|
| SingleColorPoint| 0| Single color point. 
| ColorGrid| 1| Color grid. 
| FirstOrderSurface| 2| First order surface. 
| SecondOrderSurface| 3| Second order surface. 
| ThirdOrderSurface| 4| Third order surface. 




## CIMVideoDataConnection
#### Represents a video data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMVideoDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string | The URI of the video files. 






## CIMVideoGraphicElement
#### Represents video-related graphic being displayed on the map. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMGraphicElement 

|Property | Type | Description | 
|---------|--------|--------|
| graphic | [Graphic](Types.md#graphic) | The CIMGraphic for an element on a page layout. 


### CIMVideoGraphicElement 

|Property | Type | Description | 
|---------|--------|--------|






## CIMVideoTimelineEventIndicator
#### Represents an event indicator on a video timeline. 


### CIMVideoTimelineIndicator 

|Property | Type | Description | 
|---------|--------|--------|
| label | string | The indicator label. 


### CIMVideoTimelineEventIndicator 

|Property | Type | Description | 
|---------|--------|--------|
| time | long long | The elapsed time from the beginning of the video in ticks for the event. 






## CIMVideoTimelineRangeIndicator
#### Represents a range indicator on a video timeline. 


### CIMVideoTimelineIndicator 

|Property | Type | Description | 
|---------|--------|--------|
| label | string | The indicator label. 


### CIMVideoTimelineRangeIndicator 

|Property | Type | Description | 
|---------|--------|--------|
| minimum | long long | The elapsed time from the beginning of the video in ticks for the minimum time in the range. 
| maximum | long long | The elapsed time from the beginning of the video in ticks for the maximum time in the range. 



