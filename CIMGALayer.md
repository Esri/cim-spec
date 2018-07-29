


## CIMGADataConnection
Represents GA data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMGADataConnection

|Property | Type | Description |
|---------|--------|--------|
| dataConnections | [CIMDataConnection](Types.md#cimdataconnection) |A collection of data connections.
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference)|The spatial reference.
| metaData | string|The data connection metadata.






## CIMGAIsoRenderer
Represents GA iso renderer.


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


### CIMGAIsoRenderer

|Property | Type | Description |
|---------|--------|--------|
| isoQuality | number //int32|The iso quality.
| isoType | string|The iso type
| noResultSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The no result symbol.
| refineOnZoom | boolean|A boolean indicating whether to refine on zoom.






## CIMGALayer
Represents the GA layer.


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


### CIMGALayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| AOI | [Envelope](ExternalReferences.md#envelope)|The area of interest.
| method | [CIMGAMethod](CIMGALayer.md#cimgamethod)|The GA method.
| renderers | [CIMRenderer](Types.md#cimrenderer) |The renderers.






## CIMGAMethod
Represents the GA method.


### CIMGAMethod

|Property | Type | Description |
|---------|--------|--------|
| model | string|The model.
| dataConnection | [DataConnection](Types.md#dataconnection)|The data connection
