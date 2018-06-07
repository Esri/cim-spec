


## CIMAuxiliaryRasterProperties
#### Represents auxiliary raster properties. 


### CIMAuxiliaryRasterProperties 

|Property | Type | Description | 
|---------|--------|--------|
| bandIndexes | [long]|Gets and sets a long array of the band indexes. 
| extent | [Envelope](ExternalReferences.md#envelope)|Gets and sets the extent. 
| height | long|Gets and sets the height. 
| width | long|Gets and sets the width. 





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
| MinMax| 2| Min and max. 
| StdDev| 3| Standard deviation. 



### Enumeration: ColorMatchingMethod
#### A list of color matching methods. 

|Property | Value | Description | 
|---------|--------|--------|
| Statistics| 0| Statistics. 
| Histogram| 1| Histogram. 
| LinearCorrelation| 2| Linear correlation. 
| None| 3| None. 




## CIMFeatureMosaicSubLayer
#### Represents mosiac feature sub layer. 


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


### CIMMosaicSubLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| mosaicSubLayerType | [enumeration MosaicSubLayerType](CIMImageLayers.md#enumeration-mosaicsublayertype)|Gets and sets the mosaic sublayer type. 





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


### CIMRasterLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection for the raster this layer is based on. 
| colorizer | [CIMRasterColorizer](CIMImageLayers.md#cimrastercolorizer)|Gets and sets the raster colorizer. 
| attributeTable | [CIMRasterTable](CIMVectorLayers.md#cimrastertable)|Gets and sets the raster table definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|Gets and sets the time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition)|Gets and sets the time dimension fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|Gets and sets the time definition. 
| auxiliaryRasterProperties | [CIMAuxiliaryRasterProperties](CIMImageLayers.md#cimauxiliaryrasterproperties)|Gets and sets the auxiliary raster properties. 
| autoComputeStatsHistogram | boolean|Gets and sets a boolean parameter indicating whether or not to automatically compute the statistics histogram. 
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |Gets and sets the range definitions. 
| activeRangeName | string|Gets and sets the name of the active range. 
| activeVariables | IStringArray|Gets and sets the active variables. 


### CIMImageServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| compression | string|Gets and sets the compression as a string. 
| compressionQuality | long|Gets and sets the compression quality. 
| drawFootprints | boolean|Gets and sets a boolean option indicating whether or not to draw footprints. 
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable)|Gets and sets the feature table. 
| footprintDrawMode | [enumeration RasterFootprintDrawMode](CIMImageLayers.md#enumeration-rasterfootprintdrawmode)|Gets and sets the footprint draw mode. 
| footprintSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the footprint symbol. 
| mosaicRule | [CIMMosaicRule](CIMImageLayers.md#cimmosaicrule)|Gets and sets the mosaic rule. 
| renderingRule | [CIMRenderingRule](CIMImageLayers.md#cimrenderingrule)|Gets and sets the rendering rule. 
| selectable | boolean|Gets and sets a boolean option indicating whether or not the layer is selectable. 
| selectionColor | [Color](Types.md#color)|Gets and sets the selection color. 
| selectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the selection symbol. 
| useSelectionSymbol | boolean|Gets and sets a boolean option indicating whether or not to use the selection symbol. 
| ignoreRenderingRuleOnIdentify | boolean|Gets and sets a boolean option indicating whether or not to ignore the rendering rule on identify. 
| useServiceCache | boolean|Gets and sets a boolean option indicating whether or not to use the service cache. 


### CIMMosaicSubLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| mosaicSubLayerType | [enumeration MosaicSubLayerType](CIMImageLayers.md#enumeration-mosaicsublayertype)|Gets and sets the mosaic sublayer type. 






## CIMImageServiceLayer
#### Represents an image service layer corresponding to an ArcGIS Server image service. 


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


### CIMRasterLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection for the raster this layer is based on. 
| colorizer | [CIMRasterColorizer](CIMImageLayers.md#cimrastercolorizer)|Gets and sets the raster colorizer. 
| attributeTable | [CIMRasterTable](CIMVectorLayers.md#cimrastertable)|Gets and sets the raster table definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|Gets and sets the time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition)|Gets and sets the time dimension fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|Gets and sets the time definition. 
| auxiliaryRasterProperties | [CIMAuxiliaryRasterProperties](CIMImageLayers.md#cimauxiliaryrasterproperties)|Gets and sets the auxiliary raster properties. 
| autoComputeStatsHistogram | boolean|Gets and sets a boolean parameter indicating whether or not to automatically compute the statistics histogram. 
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |Gets and sets the range definitions. 
| activeRangeName | string|Gets and sets the name of the active range. 
| activeVariables | IStringArray|Gets and sets the active variables. 


### CIMImageServiceLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| compression | string|Gets and sets the compression as a string. 
| compressionQuality | long|Gets and sets the compression quality. 
| drawFootprints | boolean|Gets and sets a boolean option indicating whether or not to draw footprints. 
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable)|Gets and sets the feature table. 
| footprintDrawMode | [enumeration RasterFootprintDrawMode](CIMImageLayers.md#enumeration-rasterfootprintdrawmode)|Gets and sets the footprint draw mode. 
| footprintSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the footprint symbol. 
| mosaicRule | [CIMMosaicRule](CIMImageLayers.md#cimmosaicrule)|Gets and sets the mosaic rule. 
| renderingRule | [CIMRenderingRule](CIMImageLayers.md#cimrenderingrule)|Gets and sets the rendering rule. 
| selectable | boolean|Gets and sets a boolean option indicating whether or not the layer is selectable. 
| selectionColor | [Color](Types.md#color)|Gets and sets the selection color. 
| selectionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the selection symbol. 
| useSelectionSymbol | boolean|Gets and sets a boolean option indicating whether or not to use the selection symbol. 
| ignoreRenderingRuleOnIdentify | boolean|Gets and sets a boolean option indicating whether or not to ignore the rendering rule on identify. 
| useServiceCache | boolean|Gets and sets a boolean option indicating whether or not to use the service cache. 






## CIMMosaicLayer
#### Represents a mosaic layer corresponding to a mosaic dataset. 


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


### CIMMosaicLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| boundaryLayer | string|Gets and sets the boundary layer. 
| footprintLayer | string|Gets and sets the footprint layer. 
| imageLayer | string|Gets and sets the image layer. 
| seamlineLayer | string|Gets and sets the seamline layer. 
| mosaicDatasetConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection of the mosaic dataset. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|Gets and sets the time definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|Gets and sets the time display definition. 
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition)|Gets and sets the time fields. 
| definitionExpression | string|Gets and sets the definition expression. 
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |Gets and sets the data connection of the mosaic dataset. 
| activeRangeName | string|Gets and sets the name of the active range. 
| activeVariables | IStringArray|Gets and sets an array of the active variables. 






## CIMMosaicRule
#### Represents a mosaic rule. 


### CIMMosaicRule 

|Property | Type | Description | 
|---------|--------|--------|
| ascending | boolean|Gets and sets a boolean option indicating ascending order. 
| FIDs | [LongLongArray](ExternalReferences.md#longlongarray)|Gets and sets an array of IDs. 
| lockRasterID | string|Gets and sets the ID of the lock raster. 
| mosaicMethod | [enumeration RasterMosaicMethod](CIMImageLayers.md#enumeration-rastermosaicmethod)|Gets and sets the mosaic method. 
| mosaicOperatorType | [enumeration RasterMosaicOperatorType](CIMImageLayers.md#enumeration-rastermosaicoperatortype)|Gets and sets the mosaic operator type. 
| orderByBaseValue | VARIANT|Gets and sets the order by base value. 
| orderByFieldName | string|Gets and sets the order by field name. 
| timeValue | [TimeValue](ExternalReferences.md#timevalue)|Gets and sets the time value. 
| viewpoint | [Point](ExternalReferences.md#point)|Gets and sets the viewpoint as a point. 
| whereClause | string|Gets and sets the where clause as a string. 





### Enumeration: MosaicSubLayerType
#### Types of mosaic sublayers. 

|Property | Value | Description | 
|---------|--------|--------|
| Boundary| 0| Boundary 
| Footprint| 1| Footprint 
| Image| 2| Image 
| Seamline| 3| Seamline 




## CIMPansharpeningFilter
#### Represents a pansharpening filter. 


### CIMPansharpeningFilter 

|Property | Type | Description | 
|---------|--------|--------|
| panImage | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection of the optional panchromatic image. 
| pansharpeningType | [enumeration PansharpeningType](CIMImageLayers.md#enumeration-pansharpeningtype)|Gets and sets the data connection of the current pansharpening type. 
| infraredImage | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection of the optional infrared image. 
| RWeight | double|Gets and sets the red weight. 
| GWeight | double|Gets and sets the green weight. 
| BWeight | double|Gets and sets the blue weight. 
| IWeight | double|Gets and sets the infrared weight. 





### Enumeration: PansharpeningType
#### Types of pansharpening. 

|Property | Value | Description | 
|---------|--------|--------|
| IHS| 0| IHS. 
| Brovey| 1| Brovey. 
| ESRI| 2| Esri. 
| Mean| 3| Mean. 




## CIMRasterBandDataConnection
#### Represents a raster band data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMRasterBandDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| rasterBandName | string|Gets and sets the raster band name. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string|Gets and sets the workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory)|Gets and sets the workspace factory. 
| customWorkspaceFactoryCLSID | string|Gets and sets the classID of the custom workspace factory. 
| dataset | string|Gets and sets the dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype)|Gets and sets the dataset type. 






## CIMRasterCMYKColorizer
#### Represents a raster CMYK colorizer. 


### CIMOrthoRectification 

|Property | Type | Description | 
|---------|--------|--------|
| constantZ | double|Gets and sets the constant Z value in meters. 
| ZFactor | double|Gets and sets the conversion factor from DEM Z unit to meters. 
| ZOffset | double|Gets and sets the Z offset in meters applied to DEM. 
| geoid | bool|Gets and sets the a boolean option indicating if Geoid correction is needed. 
| DEM | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection of the DEM used for orthorectification. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|Gets and sets the raster resampling type. 
| contrast | long|Gets and sets the contrast value. 
| brightness | long|Gets and sets the brightness value. 
| noDataColor | [Color](Types.md#color)|Gets and sets the no data color. 


### CIMRasterCMYKColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundColor | [Color](Types.md#color)|Gets and sets the background color. 
| backgroundValueBlack | double|Gets and sets the background value for black. 
| backgroundValueCyan | double|Gets and sets the background value for cyan. 
| backgroundValueMagenta | double|Gets and sets the background value for magenta. 
| backgroundValueYellow | double|Gets and sets the background value for yellow. 
| blackBandIndex | long|Gets and sets the band index for black. 
| cyanBandIndex | long|Gets and sets the band index for cyan. 
| displayBackgroundValue | boolean|Gets and sets the boolean option indicating whether or not to display the background value. 
| invert | boolean|Gets and sets the boolean option indicating whether or not the stretch is inverted. 
| magentaBandIndex | long|Gets and sets the band index for magenta. 
| specificationHistogramBlack | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the specification histogram for black. 
| specificationHistogramCyan | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the specification histogram for cyan. 
| specificationHistogramMagenta | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the specification histogram for magenta. 
| specificationHistogramYellow | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the specification histogram for yellow. 
| standardDeviationParam | double|Gets and sets the standard deviation parameter for the stretch renderer. 
| stretchStatsBlack | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the stretch histogram for black. 
| stretchStatsCyan | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the stretch histogram for cyan. 
| stretchStatsMagenta | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the stretch histogram for magenta. 
| stretchStatsType | [enumeration RasterStretchStatsType](CIMEnumerations.md#enumeration-rasterstretchstatstype)|Gets and sets the stretch statistics type. 
| stretchStatsYellow | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the stretch histogram for yellow. 
| stretchType | [enumeration RasterStretchType](CIMEnumerations.md#enumeration-rasterstretchtype)|Gets and sets the stretch type. 
| useBlackMapping | boolean|Gets and sets the boolean option indicating whether or not to use black mapping. 
| useCyanMapping | boolean|Gets and sets the boolean option indicating whether or not to use cyan mapping. 
| useDefaultMapping | boolean|Gets and sets the boolean option indicating whether or not to use default mapping. 
| useMagentaMapping | boolean|Gets and sets the boolean option indicating whether or not to use magenta mapping. 
| useYellowMapping | boolean|Gets and sets the boolean option indicating whether or not to use yellow mapping. 
| yellowBandIndex | long|Gets and sets the band index for yellow. 






## CIMRasterCatalogLayer
#### Represents a raster catalog layer. 


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


### CIMRasterCatalogLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| displayRastersThreshold | long|Gets and sets threshold for displaying wire frames. 
| drawRastersOnly | boolean|Gets and sets a boolean option indicating whether or not to draw only rasters. 
| fixedLabelPositions | boolean|Gets and sets a boolean option indicating whether or not to draw labels in fixed positions relative to the tile boundaries, and does not use the label placement engine. 
| colorizerMapping | [CIMRasterColorizerMapping](CIMImageLayers.md#cimrastercolorizermapping) |Gets and sets the colorizer mapping. 
| colorizers | [CIMRasterColorizer](CIMImageLayers.md#cimrastercolorizer) |Gets and sets the colorizer. 
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|Gets and sets the resampling type. 
| transitionScale | double|Gets and sets the transition scale. 
| useColorCorrection | boolean|Gets and sets a boolean option indicating whether or not to use color correction. 
| useScale | boolean|Gets and sets a boolean option indicating whether or not to use scale. 
| wireFrameSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the wire frame symbol. 
| sortFieldAscending | boolean|Gets and sets a boolean option indicating whether or not the sort is ascending. 
| sortField | string|Gets and sets the sort field. 
| colorCorrection | [CIMRasterColorCorrection](CIMImageLayers.md#cimrastercolorcorrection)|Gets and sets the color correction. 






## CIMRasterClassBreak
#### Represents a raster class break. 


### CIMRasterClassBreak 

|Property | Type | Description | 
|---------|--------|--------|
| upperBound | double|Gets and sets the upper bound for the raster class break. 
| label | string|Gets and sets the label for the raster class break. 
| description | string|Gets and sets the description for the raster class break. 
| color | [Color](Types.md#color)|Gets and sets the color for the raster class break. 






## CIMRasterClassifyColorizer
#### Represents a raster classify colorizer. 


### CIMOrthoRectification 

|Property | Type | Description | 
|---------|--------|--------|
| constantZ | double|Gets and sets the constant Z value in meters. 
| ZFactor | double|Gets and sets the conversion factor from DEM Z unit to meters. 
| ZOffset | double|Gets and sets the Z offset in meters applied to DEM. 
| geoid | bool|Gets and sets the a boolean option indicating if Geoid correction is needed. 
| DEM | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection of the DEM used for orthorectification. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|Gets and sets the raster resampling type. 
| contrast | long|Gets and sets the contrast value. 
| brightness | long|Gets and sets the brightness value. 
| noDataColor | [Color](Types.md#color)|Gets and sets the no data color. 


### CIMRasterClassifyColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| classBreaks | [CIMRasterClassBreak](CIMImageLayers.md#cimrasterclassbreak) |Gets and sets the class breaks of the renderer. 
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|Gets and sets the classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| exclusionColor | [Color](Types.md#color)|Gets and sets the exclusion color. 
| exclusionDescription | string|Gets and sets the exclusion description. 
| exclusionLabel | string|Gets and sets the exclusion label. 
| exclusionRanges | [double]|Gets and sets the exclusion ranges as an array of doubles. 
| exclusionValues | [double]|Gets and sets the exclusion values as an array of doubles. 
| field | string|Gets and sets the renderer field. 
| hillshadeZFactor | double|Gets and sets the Z factor of the hillshade. 
| minimumBreak | double|Gets and sets the minimum break of the classification. 
| showClassGaps | boolean|Gets and sets a boolean option indicating whether or not to show class gaps. 
| showInAscendingOrder | boolean|Gets and sets a boolean option indicating whether or not to show classes in ascending order. 
| useExclusionColor | boolean|Gets and sets a boolean option indicating whether or not to use the exclusion color. 
| useHillshade | bool|Gets and sets a boolean option indicating whether or not to use the hillshade. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format applied to values. 


### CIMDataNormalization 

|Property | Type | Description | 
|---------|--------|--------|
| normalizationField | string|Gets and sets the normalization field. 
| normalizationTotal | double|Gets and sets the normalization total. 
| normalizationType | [enumeration DataNormalizationMethod](CIMSymbolizers.md#enumeration-datanormalizationmethod)|Gets and sets the normalization type. 






## CIMRasterColorCorrection
#### Represents a raster color correction configuration. 


### CIMRasterColorCorrection 

|Property | Type | Description | 
|---------|--------|--------|
| preStretchType | [enumeration ColorCorrectionStretchType](CIMImageLayers.md#enumeration-colorcorrectionstretchtype)|Gets and sets the pre-stretch type of color correction. 
| colorBalanceMethod | [enumeration ColorBalanceMethod](CIMImageLayers.md#enumeration-colorbalancemethod)|Gets and sets the color balance method. 
| colorMatchingMethod | [enumeration ColorMatchingMethod](CIMImageLayers.md#enumeration-colormatchingmethod)|Gets and sets the color matching method. 
| needContrastAdjustment | boolean|Gets and sets a boolean option indicating whether or not contrast adjustment is needed. 
| targetColorSurfaceType | [enumeration TargetColorSurfaceType](CIMImageLayers.md#enumeration-targetcolorsurfacetype)|Gets and sets the target color surface type. 
| targetColorRaster | [DataConnection](Types.md#dataconnection)|Gets and sets the target color raster. 
| userDefinedReference | boolean|Gets and sets a boolean option indicating whether or not this is a user defined reference. 
| referenceOID | long|Gets and sets the reference OID. 






## CIMRasterColorMapColorizer
#### Represents a raster color map colorizer. 


### CIMOrthoRectification 

|Property | Type | Description | 
|---------|--------|--------|
| constantZ | double|Gets and sets the constant Z value in meters. 
| ZFactor | double|Gets and sets the conversion factor from DEM Z unit to meters. 
| ZOffset | double|Gets and sets the Z offset in meters applied to DEM. 
| geoid | bool|Gets and sets the a boolean option indicating if Geoid correction is needed. 
| DEM | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection of the DEM used for orthorectification. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|Gets and sets the raster resampling type. 
| contrast | long|Gets and sets the contrast value. 
| brightness | long|Gets and sets the brightness value. 
| noDataColor | [Color](Types.md#color)|Gets and sets the no data color. 


### CIMRasterColorMapColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| colors | [CIMColor](Types.md#cimcolor) |Gets and sets array of colors. 
| bandID | long|Gets and sets the band ID. 
| labels | IStringArray|Gets and sets the color labels as a string array. 
| min | long|Gets and sets min value. 
| max | long|Gets and sets max value. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format. 
| values | [long]|Gets and sets the array of values. 






## CIMRasterColorizerMapping
#### Represents a raster colorizer mapping. 


### CIMRasterColorizerMapping 

|Property | Type | Description | 
|---------|--------|--------|
| rasterOID | long|Gets and sets the Object ID of the raster in the raster catalog. 
| colorizerIndex | long|Gets and sets the index of the colorizer. 






## CIMRasterDiscreteColorColorizer
#### Represents a raster discrete color colorizer. 


### CIMOrthoRectification 

|Property | Type | Description | 
|---------|--------|--------|
| constantZ | double|Gets and sets the constant Z value in meters. 
| ZFactor | double|Gets and sets the conversion factor from DEM Z unit to meters. 
| ZOffset | double|Gets and sets the Z offset in meters applied to DEM. 
| geoid | bool|Gets and sets the a boolean option indicating if Geoid correction is needed. 
| DEM | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection of the DEM used for orthorectification. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|Gets and sets the raster resampling type. 
| contrast | long|Gets and sets the contrast value. 
| brightness | long|Gets and sets the brightness value. 
| noDataColor | [Color](Types.md#color)|Gets and sets the no data color. 


### CIMRasterDiscreteColorColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| numColors | long|Gets and sets the number of colors. 
| colormap | [RasterColormap](ExternalReferences.md#rastercolormap)|Gets and sets the colormap. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 





### Enumeration: RasterFootprintDrawMode
#### Raster footprint draw modes. 

|Property | Value | Description | 
|---------|--------|--------|
| All| 0| Draw all footprints. 
| OnlyPrimary| 1| Draw only primary footprints. 




## CIMRasterLayer
#### Represents a raster layer which displays raster imagery stored in a raster dataset. 


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


### CIMRasterLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection for the raster this layer is based on. 
| colorizer | [CIMRasterColorizer](CIMImageLayers.md#cimrastercolorizer)|Gets and sets the raster colorizer. 
| attributeTable | [CIMRasterTable](CIMVectorLayers.md#cimrastertable)|Gets and sets the raster table definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition)|Gets and sets the time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition)|Gets and sets the time dimension fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition)|Gets and sets the time definition. 
| auxiliaryRasterProperties | [CIMAuxiliaryRasterProperties](CIMImageLayers.md#cimauxiliaryrasterproperties)|Gets and sets the auxiliary raster properties. 
| autoComputeStatsHistogram | boolean|Gets and sets a boolean parameter indicating whether or not to automatically compute the statistics histogram. 
| rangeDefinitions | [CIMRangeDefinition](CIMVectorLayers.md#cimrangedefinition) |Gets and sets the range definitions. 
| activeRangeName | string|Gets and sets the name of the active range. 
| activeVariables | IStringArray|Gets and sets the active variables. 





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
| Min| 2| Min. 
| Max| 3| Max. 
| Mean| 4| Mean. 
| Blend| 5| Blend. 
| Sum| 6| Sum. 




## CIMRasterRGBColorizer
#### Represents a raster RGB colorizer. 


### CIMOrthoRectification 

|Property | Type | Description | 
|---------|--------|--------|
| constantZ | double|Gets and sets the constant Z value in meters. 
| ZFactor | double|Gets and sets the conversion factor from DEM Z unit to meters. 
| ZOffset | double|Gets and sets the Z offset in meters applied to DEM. 
| geoid | bool|Gets and sets the a boolean option indicating if Geoid correction is needed. 
| DEM | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection of the DEM used for orthorectification. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|Gets and sets the raster resampling type. 
| contrast | long|Gets and sets the contrast value. 
| brightness | long|Gets and sets the brightness value. 
| noDataColor | [Color](Types.md#color)|Gets and sets the no data color. 


### CIMRasterRGBColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| alphaBandIndex | long|Gets and sets the band to be represented in alpha. 
| backgroundColor | [Color](Types.md#color)|Gets and sets the background display color. 
| backgroundValueBlue | double|Gets and sets the background blue value. 
| backgroundValueGreen | double|Gets and sets the background green value. 
| backgroundValueRed | double|Gets and sets the background red value. 
| blueBandIndex | long|Gets and sets the band to be represented in blue. 
| blueLookup | [long]|Gets and sets the blue lookup values. 
| displayBackgroundValue | boolean|Gets and sets a boolean option on whether or not to display the background value. 
| ESRIStretchContrastB | double|Gets and sets the Esri stretch contrast value for blue. 
| ESRIStretchContrastG | double|Gets and sets the Esri stretch contrast value for green. 
| ESRIStretchContrastR | double|Gets and sets the Esri stretch contrast value for red. 
| ESRIStretchMeanB | double|Gets and sets the Esri stretch mean value for blue. 
| ESRIStretchMeanG | double|Gets and sets the Esri stretch mean value for green. 
| ESRIStretchMeanR | double|Gets and sets the Esri stretch mean value for red. 
| gammaB | double|Gets and sets the gamma value for blue. 
| gammaG | double|Gets and sets the gamma value for green. 
| gammaR | double|Gets and sets the gamma value for red. 
| greenBandIndex | long|Gets and sets the band to be represented in green. 
| greenLookup | [long]|Gets and sets the green lookup values. 
| invert | boolean|Gets and sets the boolean option indicating whether or not the stretch is inverted. 
| lumLookup | [long]|Gets and sets the lum lookup values. 
| maxPercent | double|Gets and sets the max percent. 
| minPercent | double|Gets and sets the min percent. 
| pansharpeningFilter | [CIMPansharpeningFilter](CIMImageLayers.md#cimpansharpeningfilter)|Gets and sets the pansharpening filter. 
| redBandIndex | long|Gets and sets the band to be represented in red. 
| redLookup | [long]|Gets and sets the red lookup values. 
| specificationHistogramBlue | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the specification histogram for blue. 
| specificationHistogramGreen | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the specification histogram for green. 
| specificationHistogramRed | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the specification histogram for red. 
| standardDeviationsParam | double|Gets and sets the standard deviations parameter. 
| stretchStatsBlue | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the stretch statistics for blue. 
| stretchStatsGreen | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the stretch statistics for green. 
| stretchStatsRed | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the stretch statistics for red. 
| stretchStatsType | [enumeration RasterStretchStatsType](CIMEnumerations.md#enumeration-rasterstretchstatstype)|Gets and sets the stretch statistics type. 
| stretchType | [enumeration RasterStretchType](CIMEnumerations.md#enumeration-rasterstretchtype)|Gets and sets the stretch type. 
| useAlphaBand | boolean|Gets and sets a boolean option on whether or not to use the alpha band. 
| useBlueBand | boolean|Gets and sets a boolean option on whether or not to use the blue band. 
| useDefaultMapping | boolean|Gets and sets a boolean option on whether or not to use default mapping. 
| useGammaStretch | boolean|Gets and sets a boolean option on whether or not to use gamma stretch. 
| useGreenBand | boolean|Gets and sets a boolean option on whether or not to use the green band. 
| useRedBand | boolean|Gets and sets a boolean option on whether or not to use the red band. 






## CIMRasterStretchClass
#### Represents a raster stretch class. 


### CIMRasterStretchClass 

|Property | Type | Description | 
|---------|--------|--------|
| label | string|Gets and sets the raster stretch class label. 
| value | double|Gets and sets the raster stretch class value. 






## CIMRasterStretchColorizer
#### Represents a raster stretch colorizer. 


### CIMOrthoRectification 

|Property | Type | Description | 
|---------|--------|--------|
| constantZ | double|Gets and sets the constant Z value in meters. 
| ZFactor | double|Gets and sets the conversion factor from DEM Z unit to meters. 
| ZOffset | double|Gets and sets the Z offset in meters applied to DEM. 
| geoid | bool|Gets and sets the a boolean option indicating if Geoid correction is needed. 
| DEM | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection of the DEM used for orthorectification. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|Gets and sets the raster resampling type. 
| contrast | long|Gets and sets the contrast value. 
| brightness | long|Gets and sets the brightness value. 
| noDataColor | [Color](Types.md#color)|Gets and sets the no data color. 


### CIMRasterStretchColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundColor | [Color](Types.md#color)|Gets and sets the background color. 
| backgroundValue | double|Gets and sets the background value. 
| bandIndex | long|Gets and sets the band index of the band being stretched. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| colorScheme | string|Gets and sets the color ramp scheme name. 
| customStretchMax | double|Gets and sets the color stretch custom max. 
| customStretchMin | double|Gets and sets the color stretch custom min. 
| displayBackgroundValue | boolean|Gets and sets a boolean indicating whether or not to display the background. 
| ESRIStretchContrast | double|Gets and sets the Esri stretch contrast parameter. 
| ESRIStretchMean | double|Gets and sets the Esri stretch mean parameter. 
| gammaValue | double|Gets and sets the gamma value. 
| hillshadeZFactor | double|Gets and sets the hillshade Z factor. 
| invert | boolean|Gets and sets a boolean value indicating whether or not to invert the stretch. 
| lookup | [long]|Gets and sets a long array of lookup values. 
| maxPercent | double|Gets and sets the max percent. 
| minPercent | double|Gets and sets the min percent. 
| standardDeviationParam | double|Gets and sets the standard deviation parameter value. 
| statsHistogram | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the statistics histogram. 
| statsType | [enumeration RasterStretchStatsType](CIMEnumerations.md#enumeration-rasterstretchstatstype)|Gets and sets the type of raster stretch statistics. 
| stretchClasses | [CIMRasterStretchClass](CIMImageLayers.md#cimrasterstretchclass) |Gets and sets the raster stretch classes. 
| stretchStats | [StatsHistogram](ExternalReferences.md#statshistogram)|Gets and sets the raster stretch statistics. 
| stretchType | [enumeration RasterStretchType](CIMEnumerations.md#enumeration-rasterstretchtype)|Gets and sets the raster stretch type. 
| useCustomMinMax | boolean|Gets and sets a boolean value indicating whether or not to use custom min and max. 
| useCustomStretchMinMax | bool|Gets and sets a boolean value indicating whether or not to use custom stretch min and max. 
| useGammaStretch | boolean|Gets and sets a boolean value indicating whether or not to use gamma stretch. 
| useHillshade | bool|Gets and sets a boolean value indicating whether or not to hillshade. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format applied to the display of values. 






## CIMRasterUniqueValueClass
#### Represents a raster unique value class. 


### CIMRasterUniqueValueClass 

|Property | Type | Description | 
|---------|--------|--------|
| values | IStringArray|Gets and sets the class values as a string array. 
| label | string|Gets and sets the class label. 
| description | string|Gets and sets the class description. 
| color | [Color](Types.md#color)|Gets and sets the class color. 
| editable | boolean|Gets and sets a boolean indicating whether or not this class is editable. 
| visible | boolean|Gets and sets a boolean indicating whether or not this class is visible. 






## CIMRasterUniqueValueColorizer
#### Represents a raster unique value colorizer. 


### CIMOrthoRectification 

|Property | Type | Description | 
|---------|--------|--------|
| constantZ | double|Gets and sets the constant Z value in meters. 
| ZFactor | double|Gets and sets the conversion factor from DEM Z unit to meters. 
| ZOffset | double|Gets and sets the Z offset in meters applied to DEM. 
| geoid | bool|Gets and sets the a boolean option indicating if Geoid correction is needed. 
| DEM | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection of the DEM used for orthorectification. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|Gets and sets the raster resampling type. 
| contrast | long|Gets and sets the contrast value. 
| brightness | long|Gets and sets the brightness value. 
| noDataColor | [Color](Types.md#color)|Gets and sets the no data color. 


### CIMRasterUniqueValueColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| defaultColor | [Color](Types.md#color)|Gets and sets the default color. 
| useDefaultColor | boolean|Gets and sets a boolean value indicating whether or not to use the default color. 
| fieldName | string|Gets and sets the field name to render. 
| groups | [CIMRasterUniqueValueGroup](CIMImageLayers.md#cimrasteruniquevaluegroup) |Gets and sets the unique value groups. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| defaultLabel | string|Gets and sets the default label. 
| defaultDescription | string|Gets and sets the default description. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format applied to values for display. 






## CIMRasterUniqueValueGroup
#### Represents a raster unique value group. 


### CIMRasterUniqueValueGroup 

|Property | Type | Description | 
|---------|--------|--------|
| classes | [CIMRasterUniqueValueClass](CIMImageLayers.md#cimrasteruniquevalueclass) |Gets and sets an array of classes making up the group. 
| heading | string|Gets and sets the group heading. 






## CIMRasterVectorFieldColorizer
#### Represents a raster vector field colorizer. 


### CIMOrthoRectification 

|Property | Type | Description | 
|---------|--------|--------|
| constantZ | double|Gets and sets the constant Z value in meters. 
| ZFactor | double|Gets and sets the conversion factor from DEM Z unit to meters. 
| ZOffset | double|Gets and sets the Z offset in meters applied to DEM. 
| geoid | bool|Gets and sets the a boolean option indicating if Geoid correction is needed. 
| DEM | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection of the DEM used for orthorectification. 


### CIMRasterColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| resamplingType | [enumeration RasterResamplingType](CIMEnumerations.md#enumeration-rasterresamplingtype)|Gets and sets the raster resampling type. 
| contrast | long|Gets and sets the contrast value. 
| brightness | long|Gets and sets the brightness value. 
| noDataColor | [Color](Types.md#color)|Gets and sets the no data color. 


### CIMRasterVectorFieldColorizer 

|Property | Type | Description | 
|---------|--------|--------|
| magnitudeBandIndex | long|Gets and sets the magnitude band index. 
| directionBandIndex | long|Gets and sets the direction band index. 
| isUVComponents | boolean|Gets and sets a boolean indicating whether flow is composed from U and V components. 
| referenceSystem | [enumeration SymbolRotationType](CIMSymbolizers.md#enumeration-symbolrotationtype)|Gets and sets the reference system for symbol rotation. 
| flowRepresentation | [enumeration FlowRepresentationType](CIMImageLayers.md#enumeration-flowrepresentationtype)|Gets and sets the flow representation type. 
| symbolTileSize | double|Gets and sets the symbol tile size. 
| symbolTileSizeUnits | [enumeration SymbolTileUnitType](CIMImageLayers.md#enumeration-symboltileunittype)|Gets and sets the symbol tile size units. 
| symbolizationType | [enumeration SymbolizationType](CIMImageLayers.md#enumeration-symbolizationtype)|Gets and sets the symbolization type. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets symbol. 
| classBreaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |Gets and sets the class breaks. 
| minimumClassBreak | double|Gets and sets the minimum class break. 
| minimumMagnitude | double|Gets and sets the minimum magnitude. 
| maximumMagnitude | double|Gets and sets the maximum magnitude. 
| minimumSymbolSize | double|Gets and sets the minimum symbol size. 
| maximumSymbolSize | double|Gets and sets the maximum symbol size. 
| fromUnit | [enumeration SpeedUnitType](CIMImageLayers.md#enumeration-speedunittype)|Gets and sets the from unit. 
| toUnit | [enumeration SpeedUnitType](CIMImageLayers.md#enumeration-speedunittype)|Gets and sets the to unit. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format used for format values for display. 






## CIMRenderingRule
#### Represents a raster rendering rule. 


### CIMRenderingRule 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the rendering rule description 
| name | string|Gets and sets the rendering rule name. 
| variableName | string|Gets and sets the rendering rule variable name. 
| arguments | {JSON_object}|Gets and sets the rendering rule arguments as a property set. 
| definition | string|Gets and sets the rendering rule definition. 





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
| name | string|Gets and sets the name. 
| URI | string|Gets and sets the URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string|Gets and sets the source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|Gets and sets the time the definition was last modfied. 
| metadataURI | string|Gets and sets the metadata URI. 
| useSourceMetadata | bool|Gets and sets if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


### CIMStandaloneVideoDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [CIMVideoDataConnection](CIMImageLayers.md#cimvideodataconnection)|Gets and sets the data connection for the video. 
| footprintColor | [Color](Types.md#color)|Gets and sets the footprint color. 
| elapsedTime | double|Elapsed time in seconds. 





### Enumeration: StretchType
#### Stretch types. 

|Property | Value | Description | 
|---------|--------|--------|
| Gamma| 0| Gamma stretch. 
| MinMax| 1| Min max stretch. 
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
| URI | string|Gets and sets the URI of the video files. 



