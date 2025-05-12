


## CIMGADataConnection
#### Represents GA data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMGADataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnections | [[CIMDataConnection]](Types.md#dataconnection) | A collection of data connections. 
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference. 
| metaData | string | The data connection metadata. 






## CIMGAIsoRenderer
#### Represents GA iso renderer. 


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


### CIMGAIsoRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| isoQuality | long | The iso quality. 
| isoType | string | The iso type. 
| noResultSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The no result symbol. 
| refineOnZoom | boolean | A value indicating whether to refine on zoom. 






## CIMGALayer
#### Represents the GA layer. 


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


### CIMGALayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| AOI | [Envelope](ExternalReferences.md#envelope) | The area of interest. 
| method | [CIMGAMethod](CIMGALayer.md#cimgamethod) | The GA method. 
| renderers | [[CIMRenderer]](Types.md#renderer) | The renderers. 
| rangeDefinitions | [[CIMRangeDefinition]](CIMVectorLayers.md#cimrangedefinition) | The range definitions. 
| activeRangeName | string | The name of the active range. 
| isFlattened | boolean | A value indicating whether the layer is flattened. 






## CIMGAMethod
#### Represents the GA method. 


### CIMGAMethod 

|Property | Type | Description | 
|---------|--------|--------|
| model | string | The model. 
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 



