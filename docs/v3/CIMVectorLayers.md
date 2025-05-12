


## CIMAggregateField
#### A field holding the result of an aggregation of multiple field values. 


### CIMFieldDescription 

|Property | Type | Description | 
|---------|--------|--------|
| alias | string | The field alias. 
| fieldName | string | The field name. 
| highlight | boolean | A value indicating whether the field is highlighted. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| readOnly | boolean | A value indicating whether the field is read only. 
| visible | boolean | A value indicating whether the field is visible. 
| valueAsRatio | boolean | A value indicating whether the field value is a ratio (used only by geoprocessing). 
| searchable | boolean | A value indicating whether the values from this field should be included in the search. 
| searchMode | [enumeration DataSearchMode](CIMVectorLayers.md#enumeration-datasearchmode) | Search mode to use when searching for values in this field. 


### CIMAggregateField 

|Property | Type | Description | 
|---------|--------|--------|
| aggregatedFieldName | string | The field name on which the aggregation was done. 
| statisticType | [enumeration esriDataStatType](ExternalReferences.md#enumeration-esridatastattype) | The type of statistic used to aggregate data. 






## CIMAggregateVisualization
#### Describes the appearance of aggregated features. 


### CIMAggregateVisualization 

|Property | Type | Description | 
|---------|--------|--------|
| renderer | [Renderer](Types.md#renderer) | The renderer used by the aggregated features. 
| labelClass | [CIMLabelClass](CIMLabelPlacement.md#cimlabelclass) | The label class used by the aggregated features. 
| showLabels | boolean | A value indicating whether or not to show labels for the aggregated features. 






## CIMAnnotationLayer
#### Represents an annotation layer used to draw annotation feature classes. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


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


### CIMAnnotationLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight) | The weight of features in this layer when considered as barriers to labeling. 
| drawGeometry | boolean | A value indicating whether the geometry of the text graphics should be drawn. 
| drawUnplacedAnnotation | boolean | A value indicating whether unplaced annotation should be drawn. 
| drawGeometryLineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol used to draw text graphic line geometries when the DrawGeometry option is true. 
| drawGeometryPointSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The point symbol used to draw text graphic line geometries when the DrawGeometry option is true. 
| unplacedAnnotationColor | [Color](Types.md#color) | The color that unplaced text graphics will be drawn with when Unplaced Annotation is drawn. 
| symbolSubstitutionType | [enumeration SymbolSubstitutionType](CIMVectorLayers.md#enumeration-symbolsubstitutiontype) | The type of symbol substitution this layer uses. 
| massColorSubstitute | [Color](Types.md#color) | The mass color substitute. When using the SymbolSubstitutionColor substitution type this is the color that all text graphics will be overridden with. 
| inlineColor | [Color](Types.md#color) | The in-line color. When using the SymbolSubstitutionIndividualSubordinate or SymbolSubstitutionIndividualDominant substitution types this is the color that all text graphics that are stored in-line (bloated) will be overridden with. 
| substitutionSymbolCollection | [[CIMSymbolIdentifier]](CIMVectorLayers.md#cimsymbolidentifier) | A symbol substitution collection. When using the SymbolSubstitutionIndividualSubordinate or SymbolSubstitutionIndividualDominant substitution types this collection defines which symbols in the symbol collection are substituted and what their substitute values are. The symbol substitution properties allow the users to swap out symbols/colors of annotation stored in the geodatabase at the layer level. This allows annotation to be re-purposed in maps without duplicating the annotation. The classic case for this behavior is when a user wishes to utilize black text generated for standard parcel maps on top of a map with raster imagery. By substituting the color or symbol collection of the annotation the user is allowed to change the appearance for this one map without a large performance or data management overhead. One complex aspect of symbol substitution is how overrides are treated when it is enabled. When this feature was originally added some wanted overrides to be respected and others did not, so options were added for this (dominant and subordinate substitution types). When the dominant type is chosen overrides are ignored. When the subordinate type is chosen overrides are applied on top of the new symbols. 
| subLayers | [[CIMAnnotationSubLayer]](CIMVectorLayers.md#cimannotationsublayer) | A collection of AnnotationSubLayers, corresponding to the annotation subclasses defined by the annotation feature class. 






## CIMAnnotationSubLayer
#### Represents an annotation sublayer used to draw annotation feature classes subclasses. 


### CIMSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| name | string | The name. 
| showLegends | boolean | A value indicating whether or not to show legends. 
| subLayerID | string | The sublayer ID. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 


### CIMAnnotationSubLayer 

|Property | Type | Description | 
|---------|--------|--------|






## CIMAttributeCondition
#### Represents an attribute condition. 


### CIMCondition 

|Property | Type | Description | 
|---------|--------|--------|


### CIMAttributeCondition 

|Property | Type | Description | 
|---------|--------|--------|
| whereClause | string | The where clause. 





### Enumeration: BarrierWeight
#### Barrier weights. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No weight. 
| Low| 1| Low weight. 
| Medium| 2| Medium weight. 
| High| 3| High weight. 



### Enumeration: BindVariableType
#### Bind variable types. 

|Property | Value | Description | 
|---------|--------|--------|
| String| 0| String variable type. 
| Integer| 1| Integer variable type. 
| Double| 2| Double variable type. 
| Date| 3| Date variable type. 
| Geometry| 4| Geometry variable type. 




## CIMBinningFeatureReduction
#### Represents a technique for reducing features by aggregating them into polygon bins. 


### CIMFeatureReduction 

|Property | Type | Description | 
|---------|--------|--------|
| enabled | boolean | A value indicating whether feature reduction is enabled in the feature layer. 


### CIMAggregationFeatureReduction 

|Property | Type | Description | 
|---------|--------|--------|
| fields | [[CIMAggregateField]](CIMVectorLayers.md#cimaggregatefield) | The fields that should be shown with the aggregated features. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The popup info for the aggregated features. 


### CIMBinningFeatureReduction 

|Property | Type | Description | 
|---------|--------|--------|
| thresholdType | [enumeration BinsToPointsThresholdType](CIMVectorLayers.md#enumeration-binstopointsthresholdtype) | The threshold at which points are shown. 
| maximumScale | double | The maximum scale to use when . 
| featureCount | long | The number of features to use when . 
| minimumBinSize | double | The minimum size (in points) to maintain as the bins are drawn at different scales. 
| visualization | [CIMBinningVisualization](CIMVectorLayers.md#cimbinningvisualization) | The visualization used by the bins. 
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference in which features are aggregated. A dataset may be aggregated in one or more spatial references. These may differ from the spatial reference of the dataset itself (the Geohash scheme always uses WGS84, for example). This property is the user's choice from among those spatial references. 
| fixedLevel | long | The bin level at which bins will be drawn. If -1, the bin level will be automatically chosen based on the minimum bin size. 
| binType | [enumeration esriFeatureBinType](ExternalReferences.md#enumeration-esrifeaturebintype) | The bin type in which features are aggregated. A dataset may be aggregated using one or more binning types. This property is the user's choice from among those binning types. 
| clientSideBinning | boolean | A value indicating whether binning should be performed on the client side, even when the data source has binning capabilities. 






## CIMBinningVisualization
#### Describes the appearance and application behavior of polygon aggregation bins. 


### CIMAggregateVisualization 

|Property | Type | Description | 
|---------|--------|--------|
| renderer | [Renderer](Types.md#renderer) | The renderer used by the aggregated features. 
| labelClass | [CIMLabelClass](CIMLabelPlacement.md#cimlabelclass) | The label class used by the aggregated features. 
| showLabels | boolean | A value indicating whether or not to show labels for the aggregated features. 


### CIMBinningVisualization 

|Property | Type | Description | 
|---------|--------|--------|
| standardDeviationMultiplier | [enumeration StandardDeviationMultiplier](CIMVectorLayers.md#enumeration-standarddeviationmultiplier) | The standard deviation multiplier used to define the data min, max values for visualization. 





### Enumeration: BinsToPointsThresholdType
#### A threshold for determining when binned features should be shown as points. 

|Property | Value | Description | 
|---------|--------|--------|
| MaxScale| 0| Points will be shown when the map is zoomed in beyond the largest scale of the bin levels. 
| FeatureCount| 1| Points will be shown when the number of features in a given map view falls below a certain number. 




## CIMBuildingDisciplineLayer
#### Represents a building discipline layer. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


### CIMBuildingDisciplineLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| disciplineType | [enumeration DisciplineType](CIMVectorLayers.md#enumeration-disciplinetype) | The discipline type of this layer. 
| categoryLayers | [string] | The category layers for this discipline in the project. 






## CIMBuildingLayer
#### Represents a building composite layer. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


### CIMObject3DRenderingFilters 

|Property | Type | Description | 
|---------|--------|--------|
| filters | [[CIMObject3DRenderingFilter]](CIMServiceLayers.md#cimobject3drenderingfilter) | The 3D object rendering filters. 
| activeFilterID | string | The ID of the filter currently used for rendering. 


### CIMBuildingLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| buildingDisciplineLayers | [string] | The building discipline composite layers in the project. 
| exteriorLayer | string | The exterior shell feature layer in the project. 
| buildingID | string | The building ID to filter by building. 
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection to the workspace. 
| summaryStatisticsURI | string | The URI of the binary reference containing the summary statistics. 






## CIMCatalogDynamicGroupLayer
#### Composite layer to hold all the dynamic content of a Catalog layer. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


### CIMCatalogDynamicGroupLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|






## CIMCatalogLayer
#### Represents a layer which dynamically loads its sublayers according to scale and extent constraints. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


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


### CIMCatalogLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| footprintLayer | string | The path of the footprint feature layer. 
| catalogDynamicGroupLayer | string | The path of the composite layer that contains all the currently-visible layers. The layers inside the composite layer are updated as the extent of the active view changes. 
| maximumVisibleSublayers | long | Upper bound for number of layers in view. 






## CIMClusteringFeatureReduction
#### Represents a technique for reducing features by aggregating them into point clusters. 


### CIMFeatureReduction 

|Property | Type | Description | 
|---------|--------|--------|
| enabled | boolean | A value indicating whether feature reduction is enabled in the feature layer. 


### CIMAggregationFeatureReduction 

|Property | Type | Description | 
|---------|--------|--------|
| fields | [[CIMAggregateField]](CIMVectorLayers.md#cimaggregatefield) | The fields that should be shown with the aggregated features. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The popup info for the aggregated features. 


### CIMClusteringFeatureReduction 

|Property | Type | Description | 
|---------|--------|--------|
| maximumScale | double | The maximum scale. Beyond this scale, unclustered points will be shown. 
| clusterRadius | double | The radius within which points are clustered. Units are points. 
| visualization | [AggregateVisualization](Types.md#aggregatevisualization) | The visualization used by the clusters. 





### Enumeration: DataSearchMode
#### Field search modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Contains| 0| Search for values that contain the search text. 
| Exact| 1| Search for values that are the exact match with the search text. 
| StartsWith| 2| Search for values that start with the search text. 
| FullTextSearchStartsWith| 3| Search for values that start with the search text using full text index. 
| FullTextSearchExact| 4| Search for values that are the exact match with the search text using full text index. 




## CIMDatabaseRelateInfo
#### Represents database relationship info that is used to represent layer or table level overrides. 


### CIMDatabaseRelateInfo 

|Property | Type | Description | 
|---------|--------|--------|
| relationshipClassName | string | The relationship class Name. 
| serviceRelateID | long | A integer indicating the relate ID when published in a map service. 
| relatedMapMemberURI | string | The related layer/table URI. This value is used to disambiguate cases where the same data connection is used by multiple layers or tables in a map. 






## CIMDimensionLayer
#### Represents an dimension layer used to draw dimension feature classes. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


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


### CIMDimensionLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight) | The weight of features in this layer when considered as barriers to labeling. 
| snappable | boolean | A value indicating whether or not geometries are snappable. 





### Enumeration: DimensionMarkerFit
#### Dimension marker fit options. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Do not fit markers with text. 
| Tolerance| 1| Fit markers with text using the length of the dimension line. 
| Text| 2| Fit markers when overlapping the text. 



### Enumeration: DimensionPartOptions
#### Dimension part options. 

|Property | Value | Description | 
|---------|--------|--------|
| Begin| 1| Only display the beginning dimension part. 
| End| 2| Only display the end dimension part. 
| None| 3| Do not display any dimension parts. 
| Both| 0| Display both dimension parts. 




## CIMDimensionShape
#### Represents a dimension shape as used by a dimension feature. 


### CIMDimensionShape 

|Property | Type | Description | 
|---------|--------|--------|
| beginDimensionPoint | [Point](ExternalReferences.md#point) | The begin dimension point. 
| endDimensionPoint | [Point](ExternalReferences.md#point) | The end dimension point. 
| dimensionLinePoint | [Point](ExternalReferences.md#point) | The point which describes the height of the dimension line. 
| textPoint | [Point](ExternalReferences.md#point) | The point for the text placement. 
| extensionLineAngle | double | The angle of the extension lines in radians. 
| textAngle | double | The angle of the text in radians. 






## CIMDimensionStyle
#### Represents an dimension style which defines dimension appearance. 


### CIMDimensionStyle 

|Property | Type | Description | 
|---------|--------|--------|
| align | boolean | A value indicating whether the text should be aligned with the dimension line. 
| baselineHeight | double | The height of the construction for creating baseline dimensions with this style. 
| beginMarkerSymbol | [CIMPointSymbol](CIMSymbols.md#cimpointsymbol) | The symbol used for the begin arrow. 
| convertUnits | boolean | A value indicating whether the length of the dimension needs to be converted for display. 
| dimensionLineOption | [enumeration DimensionPartOptions](CIMVectorLayers.md#enumeration-dimensionpartoptions) | The dimension line display of the style. 
| dimensionLineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol) | The symbol used for the dimension line. 
| displayPrecision | long | The precision for the value displayed by the dimension text. 
| displayUnits | [Unit](ExternalReferences.md#unit) | The units the length of the dimension text is displayed in. 
| drawLineOnFit | boolean | A value indicating whether a dimension line should be drawn between the extension lines for an inward dimension. 
| endMarkerSymbol | [CIMPointSymbol](CIMSymbols.md#cimpointsymbol) | The symbol used for the end arrow. 
| expression | string | The text expression for the style. 
| expressionParserName | string | The text expression parser for the text expression for the style. 
| expressionTitle | string | The human readable text title that describes the dimension expression. 
| extendLineOnFit | boolean | A value indicating whether the dimension line will be extended to underline the text on inward dimensions. 
| extensionLineOffset | double | The length of the extension line offset. 
| extensionLineOption | [enumeration DimensionPartOptions](CIMVectorLayers.md#enumeration-dimensionpartoptions) | The extension line display options of the style. 
| extensionLineOvershot | double | The length of the extension line overshot. 
| extensionLineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol) | The symbol used for extension lines. 
| ID | long | The ID of the style. 
| markerFit | [enumeration DimensionMarkerFit](CIMVectorLayers.md#enumeration-dimensionmarkerfit) | The arrow fit policy of the style. 
| markerFitTolerance | double | The arrow fit tolerance of the style. 
| markerOption | [enumeration DimensionPartOptions](CIMVectorLayers.md#enumeration-dimensionpartoptions) | The arrow display properties of the style. 
| name | string | The name of the style. 
| prefix | string | The prefix for the text expression for the style. 
| suffix | string | The suffix for the text expression for the style. 
| textFit | [enumeration DimensionTextFit](CIMVectorLayers.md#enumeration-dimensiontextfit) | The text fit policy for the style. 
| textOption | [enumeration DimensionTextOption](CIMVectorLayers.md#enumeration-dimensiontextoption) | The text display option for the style. 
| textSymbol | [CIMTextSymbol](CIMSymbols.md#cimtextsymbol) | The text symbol used for the text. 





### Enumeration: DimensionTextFit
#### Dimension text fit options. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Do not fit the text. 
| MoveBegin| 1| Move the text outside the begin extension line. 
| MoveEnd| 2| Move the text outside the end extension line. 



### Enumeration: DimensionTextOption
#### Dimension text options. 

|Property | Value | Description | 
|---------|--------|--------|
| Only| 0| Only display the value of the dimension length. 
| Suffix| 1| Display the value of the dimension length with a prefix and suffix. 
| Expression| 2| Display a text string derived from a custom expression. 
| None| 3| Do not display any text. 



### Enumeration: DimensionType
#### Dimension types supported by dimension features. 

|Property | Value | Description | 
|---------|--------|--------|
| Aligned| 0| An aligned dimension that displays the distance between the measure points. 
| Linear| 1| A linear dimension that displays the distance between the extension lines. 



### Enumeration: DisciplineType
#### Represents the discipline type of a building layer. 

|Property | Value | Description | 
|---------|--------|--------|
| Architectural| 0| Architectural. 
| Electrical| 1| Electrical. 
| Mechanical| 2| Mechanical. 
| Piping| 3| Piping. 
| Structural| 4| Structural. 
| Infrastructure| 5| Infrastructure. 




## CIMDiscreteVariable
#### Represents a single bind variable. 


### CIMBindVariable 

|Property | Type | Description | 
|---------|--------|--------|
| variableName | string | The name of the variable. The name must be unique among all variables. 
| alias | string | The alias of the variable. 
| dataType | [enumeration BindVariableType](CIMVectorLayers.md#enumeration-bindvariabletype) | The type of the variable. 


### CIMDiscreteVariable 

|Property | Type | Description | 
|---------|--------|--------|
| defaultValue | [[any]]| The variable's required default value. The array can have multiple values only if AllowMultiple is true. 
| boundValue | [[any]]| The variable's currently-bound value. The array can have multiple values only if AllowMultiple is true. 
| allowMultiple | boolean | A value indicating whether the variable will accept an array of values. 






## CIMDisplayFilter
#### Represents a display filter used to restrict the display of features across scale ranges. 


### CIMDisplayFilter 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the display filter. 
| whereClause | string | The where clause that filters features for a given scale range. 
| minScale | double | The minimum scale for this display filter. 
| maxScale | double | The maximum scale for this display filter. 





### Enumeration: DisplayFilterType
#### DisplayFilterType. 

|Property | Value | Description | 
|---------|--------|--------|
| ByChoice| 0| DisplayFilter independent of scale. 
| ByScale| 1| Scale based DisplayFilter. 




## CIMENCDataConnection
#### Represents an ENC layer data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceDataConnectionProperties 

|Property | Type | Description | 
|---------|--------|--------|
| customParameters | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | Vendor specific parameters. 


### CIMENCDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string | The URI of the ENC files or resources. 






## CIMENCLayer
#### Represents an Electronic Navigational Charts (ENC) layer. ENC layers allow to visualize nautical charts from S-57 cells using S-52 symbology. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


### CIMENCLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [CIMENCDataConnection](CIMVectorLayers.md#cimencdataconnection) | The data connection to the ENC resource. 
| displaySettings | [CIMENCDisplaySettings](CIMVectorLayers.md#cimencdisplaysettings) | The display settings of the ENC layer. 
| subLayers | [[CIMENCSubLayer]](CIMVectorLayers.md#cimencsublayer) | A collection of ENCSubLayers, used to access features by type. 
| subTables | [[CIMENCSubTable]](CIMVectorLayers.md#cimencsubtable) | A collection of ENCSubTables. 
| selectionSetURI | string | The URI of the selection set for the layer. 
| selectable | boolean | A value indicating whether the layer is selectable. 






## CIMENCSubLayer
#### Represents an ENC sublayer used to access features by type. 


### CIMSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| name | string | The name. 
| showLegends | boolean | A value indicating whether or not to show legends. 
| subLayerID | string | The sublayer ID. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 


### CIMENCSubLayer 

|Property | Type | Description | 
|---------|--------|--------|






## CIMENCSubTable
#### Represents an ENC subtable. 


### CIMENCSubTable 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| subTableID | string | The sub table ID. 






## CIMEditingTemplateRelationship
#### Represents an editing template relationship. 


### CIMEditingTemplateRelationship 

|Property | Type | Description | 
|---------|--------|--------|
| tableURI | string | The table URI of the table the relationship corresponds to. 
| name | string | The name. 
| relationshipID | long | The relationship ID. 






## CIMEditingTemplateToolOptions
#### Represents editing template tool options. 


### CIMEditingTemplateToolOptions 

|Property | Type | Description | 
|---------|--------|--------|
| toolProgID | string | The tool ProgID. 
| options | {JSON_object}| The options for the specified creation tool. 





### Enumeration: FeatureCacheType
#### Feature cache type options. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No cache. 
| Session| 1| Cache is maintained in session. 




## CIMFeatureDatasetDataConnection
#### Represents a feature dataset data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFeatureDatasetDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| featureDataset | string | Feature dataset. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string | The workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory) | The workspace factory. 
| customWorkspaceFactoryCLSID | string | The classID of the custom workspace factory. 
| dataset | string | The dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype) | The dataset type. 


### CIMServiceDataConnectionProperties 

|Property | Type | Description | 
|---------|--------|--------|
| customParameters | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | Vendor specific parameters. 





### Enumeration: FeatureExpirationMethod
#### Stream service feature expiration method. 

|Property | Value | Description | 
|---------|--------|--------|
| MaximumFeatureCount| 0| The oldest features will expire after a threshold number of features has been reached. 
| MaximumFeatureAge| 1| Features will expire after the specified time since the beginning of their lifetime. 




## CIMFeatureExtrusion
#### Represents feature extrusion. 


### CIMFeatureExtrusion 

|Property | Type | Description | 
|---------|--------|--------|
| extrusionType | [enumeration ExtrusionType](CIMEnumerations.md#enumeration-extrusiontype) | The extrusion type. 
| extrusionExpression | string | The extrusion expression. 
| extrusionUnit | [LinearUnit](ExternalReferences.md#linearunit) | The feature layer's extrusion unit. 
| extrusionExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The ExpressionInfo that contains Arcade expression that returns a numeric value. 






## CIMFeatureLayer
#### Represents feature layer used to draw data from feature classes. A feature layer displays a set of geographic features. A geographic feature represents a real-world object on the earth. It has a spatially- referenced location, stored as a point, line, or polygon, and a set of attributes that describe the feature. Its position is accurate and relevant within a particular scale range. Geographic features are the core spatial data holdings of an organization. They can serve as official records, are used in spatial analysis, and are used as source data for cartography. Feature layers draw their features by using a feature renderer to transform the geographic feature into one or more graphic entities. Feature renderers read the feature's geometry and attribute values to generate graphic entities that graphically depict the feature on a map. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


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






## CIMFeatureSortInfo
#### Contains information about the field name and sort order used to draw features. 


### CIMFeatureSortInfo 

|Property | Type | Description | 
|---------|--------|--------|
| fieldName | string | The name of the Field. 
| sortDirection | [enumeration SortOrderType](CIMLayer.md#enumeration-sortordertype) | A value indicating the sort direction. 






## CIMFeatureTable
#### Represents a feature table. 


### CIMDisplayTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| definitionExpression | string | The definition expression that can subset the rows in the virtual table. 
| definitionExpressionName | string | The Name of definition expression. 
| definitionFilterChoices | [[CIMDefinitionFilter]](CIMLayer.md#cimdefinitionfilter) | The definition filter choices. 
| displayField | string | The name of the attribute field that will be used as a label that represents each row in the table. The display field must be able to be represented as a string (string or numeric). 
| editable | boolean | A value indicating whether or not the table can be edited. 
| relates | [[CIMRelateInfoBase]](CIMVectorLayers.md#cimrelateinfobase) | The relates. 
| fieldDescriptions | [[CIMFieldDescription]](Types.md#fielddescription) | The field descriptions. Field descriptions for fields may only be written if values are overridden from defaults. 
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition) | The time fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition) | The time definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition) | The time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition) | The time definition fields. 
| rangeDefinitions | [[CIMRangeDefinition]](CIMVectorLayers.md#cimrangedefinition) | The range definitions. 
| activeRangeName | string | The active range name. 
| selectRelatedData | boolean | A value indicating whether related data should be selected when creating a new selection. 
| bindVariables | [[CIMBindVariable]](Types.md#bindvariable) | The bind variables. 
| subtypeValue | long | The subtype value that should be used in the feature layer definition. This property is honored only when feature layer is a member of SubtypeLayer. 
| useSubtypeValue | boolean | A value indicating whether or not the SubtypeValue should be used. 
| displayExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The expression information used for coming up with a string that represents a row or a feature. 
| selectionSetURI | string | The URI of the selection set for the table. 
| floorAwareTableProperties | [CIMFloorAwareTableProperties](CIMVectorLayers.md#cimfloorawaretableproperties) | Floor-aware properties for the layer/table used in floor filtering. 
| routeIDFieldName | string | The route identifier field of a route feature class. This property will only be set for route feature classes, namely line and polyline feature classes that are m-aware. 
| databaseRelates | [[CIMDatabaseRelateInfo]](CIMVectorLayers.md#cimdatabaserelateinfo) | Overrides for database relationships as relationship info. By default this property is null. This will contain relationship info elements for those database relationships that have overrides. 


### CIMFeatureTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| studyArea | [Area](ExternalReferences.md#area) | An area that can be used to subset the rows in the virtual table. 
| studyAreaSpatialRel | [enumeration esriSpatialRelEnum](ExternalReferences.md#enumeration-esrispatialrelenum) | The study area spatial relationship. 
| searchOrder | [enumeration esriSearchOrder](ExternalReferences.md#enumeration-esrisearchorder) | The search order option. 
| isLicensedDataSource | boolean | A value indicating whether the data source is licensed. 
| definitionSetURI | string | The DefinitionSet for the table. 






## CIMFeatureTrajectorySubLayer
#### Represents the trajectory feature sublayer. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


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


### CIMTrajectorySubLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| trajectorySubLayerType | [enumeration TrajectorySubLayerType](CIMVectorLayers.md#enumeration-trajectorysublayertype) | The trajectory sublayer type. 






## CIMFieldDescription
#### Represents a field description. 


### CIMFieldDescription 

|Property | Type | Description | 
|---------|--------|--------|
| alias | string | The field alias. 
| fieldName | string | The field name. 
| highlight | boolean | A value indicating whether the field is highlighted. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| readOnly | boolean | A value indicating whether the field is read only. 
| visible | boolean | A value indicating whether the field is visible. 
| valueAsRatio | boolean | A value indicating whether the field value is a ratio (used only by geoprocessing). 
| searchable | boolean | A value indicating whether the values from this field should be included in the search. 
| searchMode | [enumeration DataSearchMode](CIMVectorLayers.md#enumeration-datasearchmode) | Search mode to use when searching for values in this field. 






## CIMFloorAwareTableProperties
#### Represents floor-aware properties for the layer/table used in floor filtering. 


### CIMFloorAwareTableProperties 

|Property | Type | Description | 
|---------|--------|--------|
| floorFilterRank | [enumeration FloorFilterRank](CIMVectorLayers.md#enumeration-floorfilterrank) | Rank or "level" at which the layer/table participates in filtering for Indoors or floor-aware layers/tables. 
| floorField | string | The name of the field that carries the floor value used for floor filtering. 





### Enumeration: FloorFilterRank
#### Represents the rank or "level" at which the layer participates in filtering for Indoors or floor-aware layers. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Does not participate in floor filtering. 
| Site| 1| Layer is an Indoors Site layer and will be filtered according to the selected site. 
| Facility| 2| Layer is an Indoors Facility layer and will be filtered according to the selected facility or facilities within the selected site. 
| Level| 3| Layer is a "floor-aware" layer and will be filtered according to the selected level or levels within the selected site. 




## CIMFolderConnection
#### Represents a folder connection. 


### CIMFolderConnection 

|Property | Type | Description | 
|---------|--------|--------|
| folderConnectionString | string | The folder connection string. 
| alias | string | The connection alias. 






## CIMGeometryLocationCondition
#### Represents geometry location condition. 


### CIMCondition 

|Property | Type | Description | 
|---------|--------|--------|


### CIMLocationCondition 

|Property | Type | Description | 
|---------|--------|--------|
| conditionType | [enumeration LocationConditionType](CIMVectorLayers.md#enumeration-locationconditiontype) | The location condition type. 


### CIMGeometryLocationCondition 

|Property | Type | Description | 
|---------|--------|--------|
| geometries | [GeometryArray](ExternalReferences.md#geometryarray) | The geometries. 






## CIMGroupEditingTemplate
#### Represents a group editing template. 


### CIMEditingTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| name | string | The name. 
| tags | string | The tags. 
| defaultToolGUID | string | The default tool GUID. 
| excludedToolGUIDs | [string] | The excluded tool GUIDs. 
| toolOptions | [[CIMEditingTemplateToolOptions]](CIMVectorLayers.md#cimeditingtemplatetooloptions) | The per-tool options. 


### CIMGroupEditingTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| baseName | string | The base name. 
| basePart | [CIMGroupEditingTemplatePart](CIMVectorLayers.md#cimgroupeditingtemplatepart) | The base part. 
| parts | [[CIMGroupEditingTemplatePart]](CIMVectorLayers.md#cimgroupeditingtemplatepart) | The parts. 
| createUtilityNetworkAssociations | boolean | A value indicating whether this template will attempt to create associations between features being created. This property is only used with group templates in layers participating in a utility network. 






## CIMGroupEditingTemplatePart
#### Represents a group editing template part. 


### CIMGroupEditingTemplatePart 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string | The URI of the layer this template is defined for. 
| name | string | The name. 
| transformationID | string | The transformation ID. 
| options | {JSON_object}| The options. 






## CIMHighlightActivity
#### Represents a highlight activity. 


### CIMActivity 

|Property | Type | Description | 
|---------|--------|--------|


### CIMHighlightActivity 

|Property | Type | Description | 
|---------|--------|--------|
| highlightSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The highlight symbol. 






## CIMHtmlPopupFormat
#### Represents an HTML pop-up format. 


### CIMHtmlPopupFormat 

|Property | Type | Description | 
|---------|--------|--------|
| htmlRedirectField | string | The redirect field. 
| htmlRedirectFieldPrefix | string | The redirect field prefix. 
| htmlRedirectFieldSuffix | string | The redirect field suffix. 
| htmlXSLStyleSheet | string | The XSL style sheet. 
| htmlHideFieldNameColumn | boolean | A value indicating whether of not to hide the field name column. 
| htmlUseCodedDomainValues | boolean | A value indicating whether of not to use coded domain values. 
| htmlPresentationStyle | [enumeration HtmlPopupStyle](CIMVectorLayers.md#enumeration-htmlpopupstyle) | The presentation style. 





### Enumeration: HtmlPopupStyle
#### HTML pop-up styles. 

|Property | Value | Description | 
|---------|--------|--------|
| TwoColumnTable| 0| A two column table. 
| RedirectedHTML| 1| Redirected HTML. 
| XSLStyleSheet| 2| An XSL style sheet. 




## CIMLayerAction
#### Represents a layer action. 


### CIMLayerAction 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| activities | [[CIMActivity]](Types.md#activity) | Activities. 
| conditions | [[CIMCondition]](Types.md#condition) | Conditions. 






## CIMLayerRange
#### Represents a layer range. 


### CIMLayerRange 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string | The URI of the layer this range is defined for. 
| rangeName | string | The range name. 
| currentRange | [CIMRange](CIMVectorLayers.md#cimrange) | The current range. 
| currentRangeRelation | [enumeration RangeRelation](CIMEnumerations.md#enumeration-rangerelation) | The current range relation. 
| isExclusion | boolean | A value indicating whether or not this is an exclusion range. 





### Enumeration: LocationConditionType
#### Location condition types. 

|Property | Value | Description | 
|---------|--------|--------|
| In| 0| In. 
| Depart| 1| Depart. 
| Out| 2| Out. 
| Arrive| 3| Arrive. 
| Cross| 4| Cross. 
| Crossover| 5| Crossover. 



### Enumeration: MappedOIDFieldType
#### A list of mapped OID field types. 

|Property | Value | Description | 
|---------|--------|--------|
| OID32Bit| 4| Mapped OID field type is 32 bit. 
| OID64Bit| 8| Mapped OID field type is 64 bit. 




## CIMMaterializedViewProperties
#### Properties relevant to query layers based on materialized views. 


### CIMMaterializedViewProperties 

|Property | Type | Description | 
|---------|--------|--------|
| materializedViewQuery | string | The original definition of the materialized view. 
| materializedViewExpiration | long | The number of days after creating a materialized view that it is set to expire. 






## CIMMultipatchFeatureTemplate
#### Represents a multipatch feature template. 


### CIMEditingTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| name | string | The name. 
| tags | string | The tags. 
| defaultToolGUID | string | The default tool GUID. 
| excludedToolGUIDs | [string] | The excluded tool GUIDs. 
| toolOptions | [[CIMEditingTemplateToolOptions]](CIMVectorLayers.md#cimeditingtemplatetooloptions) | The per-tool options. 


### CIMBasicRowTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| defaultValues | {JSON_object}| The default values. 
| requiredFields | [string] | The required fields. 
| hiddenFields | [string] | The hidden fields. 
| relationships | [[CIMEditingTemplateRelationship]](CIMVectorLayers.md#cimeditingtemplaterelationship) | The template relationships. 


### CIMMultipatchFeatureTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| galleryMode | boolean | A value indicating whether or not this is gallery mode. 
| models | [[CIMMultipatchFeatureTemplateModel]](CIMVectorLayers.md#cimmultipatchfeaturetemplatemodel) | The models. 






## CIMMultipatchFeatureTemplateModel
#### Represents a multipatch feature template model. 


### CIMMultipatchTemplateModel 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether or not this is active. 
| modelURI | string | The URI of the binary reference containing the model. 
| modelSourceURI | string | The file path to the original model source. 
| thumbnailURI | string | The URI of the binary reference containing the thumbnail. 
| camera | [CIMViewCamera](CIMMap.md#cimviewcamera) | The camera. 






## CIMNetCDFRasterDataConnection
#### Represents a NetCDF raster data connection. 


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


### CIMNetCDFRasterDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| bandDimension | string | The band dimension. 
| extent | [Envelope](ExternalReferences.md#envelope) | The extent. 
| invertRows | boolean | A value indicating whether or not to invert rows. 
| selectedDimensionIndexes | [long] | The selected dimension indexes. 
| selectedDimensions | [string] | The selected dimensions. 
| selectedDimensionValues | [[any]]| The selected dimension values. 
| variable | string | The variable. 
| verticalDimension | string | The vertical dimension. 
| verticalDimensionUnit | string | The vertical dimension unit. 
| XDimension | string | The X dimension. 
| YDimension | string | The Y dimension. 






## CIMNetCDFStandardDataConnection
#### Represents a NetCDF standard data connection. 


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


### CIMNetCDFStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| variableList | [string] | The variable list. 
| rowDimensionList | [string] | The row dimension list. 
| XDimension | string | The X dimension. 
| YDimension | string | The Y dimension. 
| ZDimension | string | The Z dimension. 
| MDimension | string | The M dimension. 
| selectedDimensions | [string] | The selected dimensions. 
| selectedDimensionIndexes | [long] | The selected dimension indexes. 
| selectedDimensionValues | [[any]]| The selected dimension values. 
| shapeFieldName | string | The shape field name. 
| verticalDimension | string | The vertical dimension. 
| verticalDimensionUnit | string | The vertical dimension unit. 
| selectedVolume | string | The selected volume in a multi-volume dataset. 






## CIMOrientedImageryLayer
#### Represents an oriented imagery layer. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


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


### CIMOrientedImageryLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| orientedImageryPropertyOverrides | {JSON_object}| The overrides for editable properties of the oriented imagery dataset on the layer. 






## CIMPageDefinition
#### Represents page definition. 


### CIMPageDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| pageFieldName | string | The page field name. Show features where the value of this field either matches or doesn't match the current map series page name. Match versus don't match is controlled by ExcludePages. 
| excludePages | boolean | A value indicating whether to exclude pages. Specify false to show features that match or true to show features that don't match. 






## CIMParcelFabricActiveRecord
#### Defines the parcel fabric active record properties needed for record-driven parcel workflows. 


### CIMParcelFabricActiveRecord 

|Property | Type | Description | 
|---------|--------|--------|
| activeRecord | string | The active record GlobalID. 
| enabled | boolean | A value indicating whether or not there is an active record. 
| showActiveRecordOnly | boolean | A value indicating whether to show only the features associated with the active record in the map. 






## CIMParcelFabricLayer
#### Represents a parcel fabric layer. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


### CIMParcelFabricLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| accuracyTable | string | The path of the accuracy table. 
| allLayers | [string] | The paths of the layers in the parcel fabric layer. 
| adjustmentsTable | string | The path of the adjustments table. 
| cadastralFabricConnection | [DataConnection](Types.md#dataconnection) | The data connection to the fabric. 
| controlPointLayer | string | The path of the control point layer. 
| controlPointSelectionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The control point selection symbol. 
| jobsTable | string | The path to the jobs table. 
| lineLayer | string | The path to the line layer. 
| linePointLayer | string | The path to the line point layer. 
| parcelLayer | string | The path to the parcel layer. 
| plansTable | string | The path to the plans table. 
| pointLayer | string | The path to the point layer. 






## CIMParcelLayer
#### Represents a parcel fabric layer. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


### CIMParcelLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| recordsLayer | string | The path to the parcel polygon records layer. The records layer links parcel polygons and lines to the legal record that created / retired it as well as integration point to business systems. 
| parcelConnection | [DataConnection](Types.md#dataconnection) | The data connection to the Parcel Fabric. A Parcel Fabric controls simple feature classes and uses topology rules and parcel rules. Parcel geometry is edited using feature services The Parcel Layer provides additional services to control the fabric classes such as validate. 
| parcelFabricActiveRecord | [CIMParcelFabricActiveRecord](CIMVectorLayers.md#cimparcelfabricactiverecord) | The Parcel Fabric Active Record properties. 






## CIMRange
#### Represents a range. 


### CIMRange 

|Property | Type | Description | 
|---------|--------|--------|
| min | double | The minimum. 
| max | double | The maximum. 






## CIMRangeDefinition
#### Represents a range definition. 


### CIMRangeDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| fieldName | string | The field name. Used as the start field name when an end field name is set. 
| endFieldName | string | The end field name. 
| uniqueValues | [double] | A cached set of unique range values. 
| currentRange | [CIMRange](CIMVectorLayers.md#cimrange) | The current range. 
| currentRangeRelation | [enumeration RangeRelation](CIMEnumerations.md#enumeration-rangerelation) | The current range relation. 
| customFullExtent | [CIMRange](CIMVectorLayers.md#cimrange) | The custom full extent. 
| isExclusion | boolean | A value indicating whether or not range is exclusion. 
| aliasExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns a string representing range alias value. 






## CIMRangeVariable
#### Represents a range variable. 


### CIMBindVariable 

|Property | Type | Description | 
|---------|--------|--------|
| variableName | string | The name of the variable. The name must be unique among all variables. 
| alias | string | The alias of the variable. 
| dataType | [enumeration BindVariableType](CIMVectorLayers.md#enumeration-bindvariabletype) | The type of the variable. 


### CIMRangeVariable 

|Property | Type | Description | 
|---------|--------|--------|
| fieldExpression | string | The field for which the value range will be specified. 
| optional | boolean | A value indicating whether this variable is optional. If not, default values must be provided. 
| defaultMin | any | The default minimum value. 
| defaultMax | any | The default maximum value. 
| tableName | string | The name of the table to which the field in FieldExpression belongs. 
| valueIfMissing | boolean | A value indicating whether the resulting expression should take if the variable is optional and no value is passed. 






## CIMRasterTable
#### Represents a raster table. 


### CIMDisplayTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| definitionExpression | string | The definition expression that can subset the rows in the virtual table. 
| definitionExpressionName | string | The Name of definition expression. 
| definitionFilterChoices | [[CIMDefinitionFilter]](CIMLayer.md#cimdefinitionfilter) | The definition filter choices. 
| displayField | string | The name of the attribute field that will be used as a label that represents each row in the table. The display field must be able to be represented as a string (string or numeric). 
| editable | boolean | A value indicating whether or not the table can be edited. 
| relates | [[CIMRelateInfoBase]](CIMVectorLayers.md#cimrelateinfobase) | The relates. 
| fieldDescriptions | [[CIMFieldDescription]](Types.md#fielddescription) | The field descriptions. Field descriptions for fields may only be written if values are overridden from defaults. 
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition) | The time fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition) | The time definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition) | The time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition) | The time definition fields. 
| rangeDefinitions | [[CIMRangeDefinition]](CIMVectorLayers.md#cimrangedefinition) | The range definitions. 
| activeRangeName | string | The active range name. 
| selectRelatedData | boolean | A value indicating whether related data should be selected when creating a new selection. 
| bindVariables | [[CIMBindVariable]](Types.md#bindvariable) | The bind variables. 
| subtypeValue | long | The subtype value that should be used in the feature layer definition. This property is honored only when feature layer is a member of SubtypeLayer. 
| useSubtypeValue | boolean | A value indicating whether or not the SubtypeValue should be used. 
| displayExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The expression information used for coming up with a string that represents a row or a feature. 
| selectionSetURI | string | The URI of the selection set for the table. 
| floorAwareTableProperties | [CIMFloorAwareTableProperties](CIMVectorLayers.md#cimfloorawaretableproperties) | Floor-aware properties for the layer/table used in floor filtering. 
| routeIDFieldName | string | The route identifier field of a route feature class. This property will only be set for route feature classes, namely line and polyline feature classes that are m-aware. 
| databaseRelates | [[CIMDatabaseRelateInfo]](CIMVectorLayers.md#cimdatabaserelateinfo) | Overrides for database relationships as relationship info. By default this property is null. This will contain relationship info elements for those database relationships that have overrides. 


### CIMRasterTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| joins | [DataConnection](Types.md#dataconnection) | The joins as a data connection. 






## CIMRelQueryTableDataConnection
#### Represents a RelQuery table data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMRelQueryTableDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| sourceTable | [DataConnection](Types.md#dataconnection) | The source table data connection. 
| destinationTable | [DataConnection](Types.md#dataconnection) | The destination table. 
| primaryKey | string | The primary key. 
| foreignKey | string | The foreign key. 
| name | string | The name. 
| cardinality | [enumeration esriRelCardinality](ExternalReferences.md#enumeration-esrirelcardinality) | The join cardinality. 
| joinType | [enumeration esriJoinType](ExternalReferences.md#enumeration-esrijointype) | The join type. 
| joinForward | boolean | A value indicating whether or not this is a forward join. 
| oneToFirst | boolean | A value indicating whether or not the join will be one-to-first. 






## CIMRelateInfo
#### Represents relate info. 


### CIMRelateInfo 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The relate data connection. 
| foreignKey | string | The foreign key. 
| primaryKey | string | The primary key. 
| cardinality | [enumeration esriRelCardinality](ExternalReferences.md#enumeration-esrirelcardinality) | The relate cardinality. 
| name | string | The name. 
| serviceRelateID | long | A integer indicating the relate ID when published in a map service. 
| relatedMapMemberURI | string | The related layer/table URI. This value is used to disambiguate cases where the same data connection is used by multiple layers or tables in a map. 






## CIMRouteEventDataConnection
#### Represents a route event data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMRouteEventDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| routeFeatureClass | [DataConnection](Types.md#dataconnection) | The data connection for the route feature class. 
| routeIDFieldName | string | The route identifier field of the route feature class. 
| routeWhereClause | string | The where clause that limits the routes that events can be located on. 
| routeMeasureUnit | [Unit](ExternalReferences.md#unit) | The route measure units. 
| eventMeasureUnit | [Unit](ExternalReferences.md#unit) | The units of the event measure(s). 
| eventRouteIDFieldName | string | The route identifier field name. 
| isLineEvent | boolean | A value indicating whether or not this is a line event. 
| lateralOffsetFieldName | string | The lateral offset field name. 
| MDirectionOffsetting | boolean | A value indicating whether the offset should based on the M direction or the digitized direction. 
| errorFieldName | string | The error field name. 
| addErrorField | boolean | A value indicating whether an error field should be added to the field set. 
| fromMeasureFieldName | string | The from measure field name. 
| toMeasureFieldName | string | The to measure field name. 
| addAngleField | boolean | A value indicating whether an angle field should be added to the field set. 
| angleFieldName | string | The angle field name. 
| asPointFeature | boolean | A value indicating whether the point event shape should be output as a multipoint or a point. 
| complementAngle | boolean | A value indicating whether 180 degrees should be added to the angle field value. 
| normalAngle | boolean | A value indicating whether the angle field should be the normal or the tangent angles. 
| eventTable | [DataConnection](Types.md#dataconnection) | The data connection for the route events. 






## CIMRowTemplate
#### Represents a row template. 


### CIMEditingTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The description. 
| name | string | The name. 
| tags | string | The tags. 
| defaultToolGUID | string | The default tool GUID. 
| excludedToolGUIDs | [string] | The excluded tool GUIDs. 
| toolOptions | [[CIMEditingTemplateToolOptions]](CIMVectorLayers.md#cimeditingtemplatetooloptions) | The per-tool options. 


### CIMBasicRowTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| defaultValues | {JSON_object}| The default values. 
| requiredFields | [string] | The required fields. 
| hiddenFields | [string] | The hidden fields. 
| relationships | [[CIMEditingTemplateRelationship]](CIMVectorLayers.md#cimeditingtemplaterelationship) | The template relationships. 


### CIMRowTemplate 

|Property | Type | Description | 
|---------|--------|--------|





### Enumeration: S52AreaSymbolizationType
#### ENC area symbolization type. This is used to specify whether areas should be symbolized with plain or traditional symbols. 

|Property | Value | Description | 
|---------|--------|--------|
| Plain| 0| Use plain symbols. 
| Symbolized| 1| Use traditional symbols. 



### Enumeration: S52ColorScheme
#### ENC Color Schemes. 

|Property | Value | Description | 
|---------|--------|--------|
| Day| 0| Day. 
| Dusk| 1| Dusk. 
| Night| 2| Night. 



### Enumeration: S52DepthDisplayUnits
#### ENC Depth Display Units. 

|Property | Value | Description | 
|---------|--------|--------|
| Meters| 0| Meters. 
| Feet| 1| Feet. 
| Fathoms| 2| Fathoms. 




## CIMS52DisplaySettings
#### Represents S-52 display settings. 


### CIMENCDisplaySettings 

|Property | Type | Description | 
|---------|--------|--------|


### CIMS52DisplaySettings 

|Property | Type | Description | 
|---------|--------|--------|
| marinerSettings | [CIMS52MarinerSettings](CIMVectorLayers.md#cims52marinersettings) | The S-52 display properties for the layer. 
| textGroupVisibilitySettings | [CIMS52TextGroupVisibilitySettings](CIMVectorLayers.md#cims52textgroupvisibilitysettings) | The S-52 text group properties for the layer. 
| viewingGroupSettings | [CIMS52ViewingGroupSettings](CIMVectorLayers.md#cims52viewinggroupsettings) | The S-52 view group properties for the layer. 






## CIMS52MarinerSettings
#### Represents S-52 mariner settings object for controlling the drawing of ENC layers. 


### CIMS52MarinerSettings 

|Property | Type | Description | 
|---------|--------|--------|
| areaSymbolizationType | [enumeration S52AreaSymbolizationType](CIMVectorLayers.md#enumeration-s52areasymbolizationtype) | The area symbolization type. This controls the line symbol style for area boundaries. 
| colorScheme | [enumeration S52ColorScheme](CIMVectorLayers.md#enumeration-s52colorscheme) | The color scheme. 
| showDataQuality | boolean | A value indicating whether to display data quality (M_QUAL) for S-57 features. 
| deepContour | double | The deep water contour depth in meters. This must be greater than or equal to the safety contour value. When four(rather than two) depth shades are used, this controls the boundary between safe and deep areas. 
| showDisplayBase | boolean | A value indicating whether the S-52 "displaybase" display category is enabled. 
| showOtherDisplay | boolean | A value indicating whether the S-52 "other" display category is enabled. 
| showStandardDisplay | boolean | A value indicating whether the S-52 "standard" display category is enabled. 
| depthDisplayUnits | [enumeration S52DepthDisplayUnits](CIMVectorLayers.md#enumeration-s52depthdisplayunits) | The depth units (meters/feet/fathoms) for display. 
| showNOBJNM | boolean | A value indicating whether to display the national name attribute on S-57 features. This is text group 31 per IHO S-52 Annex A. 
| honorSCAMIN | boolean | A value indicating whether the 'SCAMIN' (scale min) S-57 feature attribute will be used. If disabled, all ENC features will be rendered regardless of scale. 
| showIsolatedDangers | boolean | A value indicating whether to display isolated dangers in shallow water. This is viewing group 24020, 24050 per IHO 2-52 Annex A. 
| labelContours | boolean | A value indicating whether to display the depth contour labels, including safety contour labels. This is viewing group 33021, 33022 per IHO S-52 Annex A. 
| labelSafetyContours | boolean | A value indicating whether to display the safety contour labels. 
| showLowAccuracy | boolean | A value indicating whether to use low accuracy symbols (CATZOC). This is viewing group 31010 per IHO S-52 Annex A. When low accuracy is set to false, low accuracy data will be visually indistinguishable from other data. 
| pointSymbolizationType | [enumeration S52PointSymbolizationType](CIMVectorLayers.md#enumeration-s52pointsymbolizationtype) | The S-52 point feature symbolization type (simplified/paperchart). Paperchart symbolization is based on traditional paper charts. Simplified symbols are more compact and visible. 
| safetyContour | double | The depth of the safety contour in meters. 
| shallowContour | double | The depth of the shallow contour in meters. This must be less than or equal to the safety contour value. When four(rather than two) depth shades are used, this value controls the separation between shallow and unsafe areas. 
| showShallowDepthPattern | boolean | A value indicating whether the shallow depth pattern will be symbolized. 
| showTwoDepthShades | boolean | A value indicating whether two or four depth shades will be used; two is the default. 





### Enumeration: S52PointSymbolizationType
#### ENC point symbolization options. This is used to specify whether point features should be symbolized with simplified or paperchart symbols. 

|Property | Value | Description | 
|---------|--------|--------|
| PaperChart| 0| Paper chart symbols which are based on traditional paper charts. 
| Simplified| 1| Simplified symbols which are more compact and visible. 




## CIMS52TextGroupVisibilitySettings
#### Represents S-52 text group settings. 


### CIMS52TextGroupVisibilitySettings 

|Property | Type | Description | 
|---------|--------|--------|
| showBerthNumber | boolean | A value indicating whether the "berth number" text group should be visible. Per IHO S-52 Annex A, controls text group 29, which includes OBJNAM from BERTHS and ACHBRT. 
| showCurrentVelocity | boolean | A value indicating whether the "current velocity" text group should be visible. Per IHO S-52 Annex A, controls text group 30, which includes CURVEL. 
| showGeographicNames | boolean | A value indicating whether the "geographic names" text group should be visible. Per IHO S-52 Annex A, controls text group 26, which includes OBJNAM from ACHARE, BRIDGE, BUAARE, BUISGL, DOCARE, FAIRWY, LNDARE, LNDMARK, LNDRGN, SEAARE, TIDEWY, and PILBOP. 
| showHeightOfIsletOrLandFeature | boolean | A value indicating whether the "height of islet or land feature" text group should be visible. Per IHO S-52 Annex A, controls text group 28, which includes HEIGHT of LNDARE. 
| showImportantText | boolean | A value indicating whether the "important text" text group should be visible. Per IHO S-52 Annex A, controls text groups 10 and 11. 
| showLightDescription | boolean | A value indicating whether the "light descriptions" text group should be visible. Per IHO S-52 Annex A, controls text group 23. 
| showMagneticVariationAndSweptDepth | boolean | A value indicating whether the "magnetic variation and swept depth" text group should be visible. Per IHO S-52 Annex A, controls text group 27, which includes MAGVAR, VALMAG, SWPARE, and DRVAL1. 
| showNamesForPositionReporting | boolean | A value indicating whether the "names for position reporting" text group should be visible. Per IHO S-52 Annex A, controls text group 21. 
| showNatureOfSeabed | boolean | A value indicating whether the "nature of seabed" text group should be visible. Per IHO S-52 Annex A, controls text group 25, which includes SBDARE and NATSUR. 
| showNoteOnChartData | boolean | A value indicating whether the "note on chart data" text group should be visible. Per IHO S-52 Annex A, controls text group 24. 






## CIMS52ViewingGroupSettings
#### Represents S-52 viewing group properties object. 


### CIMS52ViewingGroupSettings 

|Property | Type | Description | 
|---------|--------|--------|
| showAllIsolatedDangers | boolean | // Viewing Group settings a value indicating whether the "all isolated dangers" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 13, which includes viewing groups 34050 and 34051. 
| showArchipelagicSeaLanes | boolean | A value indicating whether the "archipelagic sea lanes" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 9, which includes viewing group 26260. 
| showBoundariesAndLimits | boolean | A value indicating whether the "boundaries and limits" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 4, which includes viewing groups 23030, 26050, 26220, 26240, and 26250. 
| showBuoysBeaconsAidsToNavigation | boolean | A value indicating whether the "buoys, beacons, aids to navigation" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 3, which includes viewing groups 21020, 22200 ? 22240, 27000, 27010, 27011, 27020, 27025, 27040, 27050, 27070, 27080, 27200, 27210, 27230, 27030, and 27060. 
| showBuoysBeaconsStructures | boolean | A value indicating whether the "buoys, beacons, structures" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 3.1, which includes viewing groups 21010, 21020, 22200 - 22240, 27000-27050, 27080, 27200 ? 27230, 27030, and 27060. 
| showChartScaleBoundaries | boolean | A value indicating whether the "chart scale boundaries" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 6, which includes viewing group 21030. 
| showDepthContours | boolean | A value indicating whether the "depth contours" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 15, which includes viewing group 33020. 
| showDryingLine | boolean | A value indicating whether the "drying line" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 2, which includes viewing group 22010. 
| showLights | boolean | A value indicating whether the "lights" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 3.2, which includes viewing group 27070. 
| showMagneticVariation | boolean | A value indicating whether the "magnetic variation" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 14, which includes viewing group 31080. 
| showOtherMiscellaneous | boolean | A value indicating whether the "other miscellaneous" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 18, which includes viewing group 30000-39999. 
| showProhibitedAndRestrictedAreas | boolean | A value indicating whether the "prohibited and restricted areas" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 5, which includes viewing groups 2600, 26010, and 26040. 
| showSeabed | boolean | A value indicating whether the "seabed" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 16, which includes viewing groups 34010, 34020, and 33040. 
| showShipsRoutingSystemsAndFerryRoutes | boolean | A value indicating whether the "ships' routing systems and ferry routes" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 8, which includes viewing groups 25010-25060. 
| showSpotSoundings | boolean | A value indicating whether the "spot soundings" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 11, which includes viewing group 33010. 
| showStandardMiscellaneous | boolean | A value indicating whether the "standard miscellaneous" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 10 under the "standard display" viewing group, which includes all objects not covered by viewing groups 20000-29999. 
| showSubmarineCablesAndPipelines | boolean | A value indicating whether the "submarine cables and pipelines" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 12, which includes viewing groups 34030 and 34070. 
| showTidal | boolean | A value indicating whether the "tidal" viewing group is enabled. Per IHO S-52 Annex A, controls viewing group layer 17, which includes viewing groups 33050 and 33060. 






## CIMSqlQueryDataConnection
#### Represents a SQL query data connection. 


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


### CIMSqlQueryDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| sqlQuery | string | The SQL query. 
| srid | string | The SRID of the spatial reference. 
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference. 
| OIDFields | string | The OID fields. 
| geometryType | [enumeration esriGeometryType](ExternalReferences.md#enumeration-esrigeometrytype) | The geometry type. 
| extent | [Envelope](ExternalReferences.md#envelope) | The extent. 
| queryFields | Fields | 
| spatialStorageType | long | The spatial storage type. 
| sridType | long | The SRID type. Only used for query layers based on Oracle Spatial (SDO) storage. This property is managed by the system as an optimization. 
| spatialIndexDimension | long | The spatial index dimension. Only used for query layers based on Oracle Spatial (SDO) storage. This property is managed by the system as an optimization. 
| isTableBased | boolean | A value indicating whether the query is "table based" (retrieves all the columns from the table and has no where clause or postfix clause). This property is used as an optimization and is typically set by the system. 
| materializedViewProperties | [CIMMaterializedViewProperties](CIMVectorLayers.md#cimmaterializedviewproperties) | The properties relevant to materialized view-based query layers. 
| mappedOIDFieldLength | [enumeration MappedOIDFieldType](CIMVectorLayers.md#enumeration-mappedoidfieldtype) | A value indicating whether the auto generated Esri OID field will be 32-bit or 64-bit. 






## CIMStandaloneTable
#### Represents a standalone table. 


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


### CIMDisplayTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| definitionExpression | string | The definition expression that can subset the rows in the virtual table. 
| definitionExpressionName | string | The Name of definition expression. 
| definitionFilterChoices | [[CIMDefinitionFilter]](CIMLayer.md#cimdefinitionfilter) | The definition filter choices. 
| displayField | string | The name of the attribute field that will be used as a label that represents each row in the table. The display field must be able to be represented as a string (string or numeric). 
| editable | boolean | A value indicating whether or not the table can be edited. 
| relates | [[CIMRelateInfoBase]](CIMVectorLayers.md#cimrelateinfobase) | The relates. 
| fieldDescriptions | [[CIMFieldDescription]](Types.md#fielddescription) | The field descriptions. Field descriptions for fields may only be written if values are overridden from defaults. 
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition) | The time fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition) | The time definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition) | The time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition) | The time definition fields. 
| rangeDefinitions | [[CIMRangeDefinition]](CIMVectorLayers.md#cimrangedefinition) | The range definitions. 
| activeRangeName | string | The active range name. 
| selectRelatedData | boolean | A value indicating whether related data should be selected when creating a new selection. 
| bindVariables | [[CIMBindVariable]](Types.md#bindvariable) | The bind variables. 
| subtypeValue | long | The subtype value that should be used in the feature layer definition. This property is honored only when feature layer is a member of SubtypeLayer. 
| useSubtypeValue | boolean | A value indicating whether or not the SubtypeValue should be used. 
| displayExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The expression information used for coming up with a string that represents a row or a feature. 
| selectionSetURI | string | The URI of the selection set for the table. 
| floorAwareTableProperties | [CIMFloorAwareTableProperties](CIMVectorLayers.md#cimfloorawaretableproperties) | Floor-aware properties for the layer/table used in floor filtering. 
| routeIDFieldName | string | The route identifier field of a route feature class. This property will only be set for route feature classes, namely line and polyline feature classes that are m-aware. 
| databaseRelates | [[CIMDatabaseRelateInfo]](CIMVectorLayers.md#cimdatabaserelateinfo) | Overrides for database relationships as relationship info. By default this property is null. This will contain relationship info elements for those database relationships that have overrides. 


### CIMStandaloneTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection for the table. 
| description | string | The description. 
| autoGenerateRowTemplates | boolean | A value indicating whether to automatically generate row templates from the renderer. 
| rowTemplates | [[CIMEditingTemplate]](Types.md#editingtemplate) | The row templates. 
| serviceTableID | long | Identifier that will be used to identify the layer in server. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | The table's charts. 
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition) | The page definition which allows for using current map series page to filter rows. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the standalone table. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapTableID | string | An identifier that will be used to identify the standalone table in a web map. This value is present if the standalone table originated in a web map and facilitates matching the standalone table back to its origin when updating the web map. 
| searchable | boolean | A value indicating whether or not this table should be included in the search. This property is honored only by tables that support search. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the table to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 






## CIMStandardDataConnection
#### Represents a standard data connection, the most common data connection type. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceDataConnectionProperties 

|Property | Type | Description | 
|---------|--------|--------|
| customParameters | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | Vendor specific parameters. 


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string | The workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory) | The workspace factory. 
| customWorkspaceFactoryCLSID | string | The classID of the custom workspace factory. 
| dataset | string | The dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype) | The dataset type. 





### Enumeration: StandardDeviationMultiplier
#### Standard deviation multiplier to define min and max data values from the mean for binning levels. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No multiplier, use full data range. 
| OneFourth| 1| Use one fourth of the standard deviation to define data range. 
| OneThird| 2| Use one third of the standard deviation to define data range. 
| OneHalf| 3| Use one half of the standard deviation to define data range. 
| One| 4| Use one standard deviation to define data range. 
| Two| 5| Use two standard deviations to define data range. 
| Custom| 6| Allow users to define custom data range. 




## CIMStreamServiceDataConnection
#### Represents a stream service data connection. 


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


### CIMStreamServiceDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| featureExpirationMethod | [enumeration FeatureExpirationMethod](CIMVectorLayers.md#enumeration-featureexpirationmethod) | Feature expiration method used at dataset level. 
| maximumFeatureCount | long long | The maximum number of features that are held in memory before features are discarded. 
| maximumFeatureAge | long long | The maximum age for each feature before the feature is discarded. 






## CIMSubtypeGroupLayer
#### Represents a subtype group layer that works with feature classes enabled with subtypes. A subtype layer is a group layer that contains feature layers, each of which represents a subtype in a feature class. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


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


### CIMSubtypeGroupLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| subtypeLayers | [string] | The layer URI corresponding to each subtype value. 






## CIMSubtypeGroupTable
#### Represents a subtype group table that works with tables enabled with subtypes. 


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


### CIMStandaloneTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection for the table. 
| description | string | The description. 
| autoGenerateRowTemplates | boolean | A value indicating whether to automatically generate row templates from the renderer. 
| rowTemplates | [[CIMEditingTemplate]](Types.md#editingtemplate) | The row templates. 
| serviceTableID | long | Identifier that will be used to identify the layer in server. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | The table's charts. 
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition) | The page definition which allows for using current map series page to filter rows. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the standalone table. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapTableID | string | An identifier that will be used to identify the standalone table in a web map. This value is present if the standalone table originated in a web map and facilitates matching the standalone table back to its origin when updating the web map. 
| searchable | boolean | A value indicating whether or not this table should be included in the search. This property is honored only by tables that support search. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the table to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 


### CIMDisplayTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| definitionExpression | string | The definition expression that can subset the rows in the virtual table. 
| definitionExpressionName | string | The Name of definition expression. 
| definitionFilterChoices | [[CIMDefinitionFilter]](CIMLayer.md#cimdefinitionfilter) | The definition filter choices. 
| displayField | string | The name of the attribute field that will be used as a label that represents each row in the table. The display field must be able to be represented as a string (string or numeric). 
| editable | boolean | A value indicating whether or not the table can be edited. 
| relates | [[CIMRelateInfoBase]](CIMVectorLayers.md#cimrelateinfobase) | The relates. 
| fieldDescriptions | [[CIMFieldDescription]](Types.md#fielddescription) | The field descriptions. Field descriptions for fields may only be written if values are overridden from defaults. 
| timeFields | [CIMTimeTableDefinition](CIMVectorLayers.md#cimtimetabledefinition) | The time fields. 
| timeDefinition | [CIMTimeDataDefinition](CIMVectorLayers.md#cimtimedatadefinition) | The time definition. 
| timeDisplayDefinition | [CIMTimeDisplayDefinition](CIMVectorLayers.md#cimtimedisplaydefinition) | The time display definition. 
| timeDimensionFields | [CIMTimeDimensionDefinition](CIMVectorLayers.md#cimtimedimensiondefinition) | The time definition fields. 
| rangeDefinitions | [[CIMRangeDefinition]](CIMVectorLayers.md#cimrangedefinition) | The range definitions. 
| activeRangeName | string | The active range name. 
| selectRelatedData | boolean | A value indicating whether related data should be selected when creating a new selection. 
| bindVariables | [[CIMBindVariable]](Types.md#bindvariable) | The bind variables. 
| subtypeValue | long | The subtype value that should be used in the feature layer definition. This property is honored only when feature layer is a member of SubtypeLayer. 
| useSubtypeValue | boolean | A value indicating whether or not the SubtypeValue should be used. 
| displayExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The expression information used for coming up with a string that represents a row or a feature. 
| selectionSetURI | string | The URI of the selection set for the table. 
| floorAwareTableProperties | [CIMFloorAwareTableProperties](CIMVectorLayers.md#cimfloorawaretableproperties) | Floor-aware properties for the layer/table used in floor filtering. 
| routeIDFieldName | string | The route identifier field of a route feature class. This property will only be set for route feature classes, namely line and polyline feature classes that are m-aware. 
| databaseRelates | [[CIMDatabaseRelateInfo]](CIMVectorLayers.md#cimdatabaserelateinfo) | Overrides for database relationships as relationship info. By default this property is null. This will contain relationship info elements for those database relationships that have overrides. 


### CIMStandaloneTableContainer 

|Property | Type | Description | 
|---------|--------|--------|
| standaloneTables | [string] | The standalone tables as an array of table repository paths. 


### CIMSubtypeGroupTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| expanded | boolean | A value indicating whether this group table is expanded in the contents pane. 






## CIMSuppressActivity
#### Represents suppress activity. 


### CIMActivity 

|Property | Type | Description | 
|---------|--------|--------|


### CIMSuppressActivity 

|Property | Type | Description | 
|---------|--------|--------|






## CIMSymbolIdentifier
#### Represents a symbol identifier. 


### CIMSymbolIdentifier 

|Property | Type | Description | 
|---------|--------|--------|
| ID | long | The ID which identifies the symbol in the collection. 
| name | string | The name of the symbol in the symbol collection. 
| symbol | [Symbol](Types.md#symbol) | The symbol. 






## CIMSymbolLayerMasking
#### Represents symbol layer masking. 


### CIMSymbolLayerMasking 

|Property | Type | Description | 
|---------|--------|--------|
| symbolLayers | [[CIMSymbolLayerIdentifier]](CIMLayer.md#cimsymbollayeridentifier) | The symbol layer identifiers. 





### Enumeration: SymbolSubstitutionType
#### Symbol substitution types. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No symbol substitution. 
| Color| 1| Substitute color. 
| IndividualSubordinate| 2| Substitute individual symbols in the collection with overrides taking precedence to symbols. 
| IndividualDominant| 3| Substitute individual symbols in the collection with the symbol taking precedence to overrides. 




## CIMTableQueryNameDataConnection
#### Represents a table query name data connection. 


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


### CIMTableQueryNameDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| subFields | string | The subfields. 
| tables | string | The tables. 
| whereClause | string | The where clause. 
| primaryKeyFields | string | The primary key fields. 
| copyLocally | boolean | A value indicating whether or not to copy data locally. 
| shapeType | [enumeration esriGeometryType](ExternalReferences.md#enumeration-esrigeometrytype) | The shape type. 
| featureType | [enumeration esriFeatureType](ExternalReferences.md#enumeration-esrifeaturetype) | The feature type. 
| extent | [Envelope](ExternalReferences.md#envelope) | The extent. 
| shapeFieldName | string | The shape field name. 






## CIMTemporalDataConnection
#### Represents a temporal data connection. 


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


### CIMTemporalDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| timeFieldLocaleID | long | The time field locale ID. 
| timeFieldAmFormat | string | The custom string representation of the AM symbol. 
| timeFieldPmFormat | string | The custom string representation of the PM symbol. 
| cachingMode | [enumeration TemporalFeatureClassCachingMode](CIMVectorLayers.md#enumeration-temporalfeatureclasscachingmode) | The caching mode. 
| startTimeField | string | The start time field. 
| endTimeField | string | The end time field. 
| timeValueFormat | string | The time value format. 
| trackIDField | string | The track ID field. 





### Enumeration: TemporalFeatureClassCachingMode
#### Temporal feature class caching modes. 

|Property | Value | Description | 
|---------|--------|--------|
| All| 0| All. 
| None| 1| None. 



### Enumeration: TemporalFeatureClassPurgeRule
#### Temporal feature class purge rules. 

|Property | Value | Description | 
|---------|--------|--------|
| KeepLatestPerTrack| 0| Keep latest per track. 
| PurgeOldest| 1| Purge oldest. 




## CIMTimeDataDefinition
#### Represents a time data definition. 


### CIMTimeDataDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| useTime | boolean | A value indicating whether or not to use time for animation purposes. 
| timeReference | [TimeReference](ExternalReferences.md#timereference) | The time reference. 
| customTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The custom time extent. 
| hasLiveData | boolean | A value indicating whether or not this dataset has live data. 
| timeExtentCanChange | boolean | A value indicating whether the data regularly changes, so the extent needs recalculated. 
| applyTimeReferenceToAllFields | boolean | A value indicating whether the time reference applies to all date fields in the layer or only the fields driving time-awareness. 






## CIMTimeDimensionDefinition
#### Represents a time dimension definition. 


### CIMTimeDimensionDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| timeDimensionName | string | The time dimension name. 
| timeDimensionFormat | string | The time dimension format. 






## CIMTimeDisplayDefinition
#### Represents a time display definition. 


### CIMTimeDisplayDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| cumulative | boolean | A value indicating whether time is cumulative. 
| timeInterval | double | The time interval. 
| timeIntervalUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time interval units. 
| timeOffset | double | The time offset. 
| timeOffsetUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time offset units. 
| uniqueTimes | [double] | A cached set of unique OLE date values. 






## CIMTimeTableDefinition
#### Represents a time table definition. 


### CIMTimeTableDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| startTimeField | string | The start time field. 
| endTimeField | string | The end time field. 
| timeValueFormat | string | The time value format. 
| trackIDField | string | The track ID field. 






## CIMTrackingServerDataConnection
#### Represents a tracking server data connection. 


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


### CIMTrackingServerDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| autoPurge | boolean | A value indicating whether to automatically purge data. 
| purgeThreshold | long | The purge threshold. 
| purgePercentage | double | The percentage of the maximum allowed number of records to delete when the purge occurs. 
| keepPerTrack | long | The minimum number of features to keep per track. 
| purgeRule | [enumeration TemporalFeatureClassPurgeRule](CIMVectorLayers.md#enumeration-temporalfeatureclasspurgerule) | The purge rule. 






## CIMTrajectoryLayer
#### Represents a trajectory layer corresponding to a trajectory dataset. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


### CIMTrajectoryLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| footprintLayer | string | The path of the footprint feature layer. 
| pointLayer | string | The path of the point feature layer. 
| trajectoryDatasetConnection | [DataConnection](Types.md#dataconnection) | The data connection of the trajectory dataset. 





### Enumeration: TrajectorySubLayerType
#### Types of trajectory sublayers. 

|Property | Value | Description | 
|---------|--------|--------|
| Footprint| 0| Footprint sublayer. 
| Point| 1| Point sublayer. 




## CIMVectorTileDataConnection
#### Represents a VectorTile layer data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMServiceDataConnectionProperties 

|Property | Type | Description | 
|---------|--------|--------|
| customParameters | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | Vendor specific parameters. 


### CIMVectorTileDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string | The URI of the VectorTile files or resources. 
| resourcesURI | string | The URI of the binary reference containing the external resources. 






## CIMVectorTileLayer
#### Represents a VectorTile layer. A VectorTileServiceLayer provides rich cartographic content in a fast and efficient vector tile format. It may have multiple styles and if so users can choose which style to use to display the layer's vector geometries. Logically a VectorTileServiceLayer is more like a basemap layer in that it is typically composed of several distinct data sources (e.g. roads, cities, hydrology, buildings) that can provide context and background but in a way that is typically more performant than raster tile layers. 


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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


### CIMVectorTileLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [CIMVectorTileDataConnection](CIMVectorLayers.md#cimvectortiledataconnection) | The data connection to the VectorTile resource. 
| currentStyle | string | The current style the vector tile layer features should be rendered with. 
| associatedFeatureLayerURI | string | The URI for a feature layer (feature service-based or portal item-based) that provides pop-up support for the vector tile layer. 






## CIMWorkspaceConnection
#### Represents a workspace connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMWorkspaceConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string | The workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory) | The workspace factory. 
| customWorkspaceFactoryCLSID | string | The classID of the custom workspace factory. 





### Enumeration: WorkspaceFactory
#### Workspace factory types. 

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
| SQLite| 13| SQLite. 
| FeatureService| 14| Feature service. 
| ArcInfo| 15| Arc/INFO Coverage. 
| Cad| 16| CAD. 
| Excel| 17| Microsoft Excel. 
| WFS| 18| Web feature service. 
| StreamService| 19| Stream service 
| BIMFile| 20| BIM file. 
| InMemoryDB| 21| In memory database. 
| NoSQL| 22| NoSQL. 
| BigDataConnection| 23| Big Data connection. 
| KnowledgeGraph| 24| Knowledge Graph connection. 
| NITF| 25| NITF connection. 
| VPF| 26| VPF. 
| Parquet| 27| Parquet. 




## CIMXYEventDataConnection
#### Represents an XY event data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMXYEventDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| XFieldName | string | The X field name. 
| YFieldName | string | The Y field name. 
| ZFieldName | string | The Z field name. 
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference. 
| XYEventTableDataConnection | [DataConnection](Types.md#dataconnection) | The data connection to the table events are created from. 



