


## CIMGADataConnection
#### Represents GA data connection. 


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
#### Represents GA iso renderer. 


### CIMRenderer 

|Property | Type | Description | 
|---------|--------|--------|


### CIMClassBreaksRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the background symbol used for graduated symbols. 
| barrierWeight | [enumeration BarrierWeight](CIMVectorLayers.md#enumeration-barrierweight)|Gets and sets the barrier weight used for graduate symbols to avoid labels. 
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |Gets and sets the class breaks. 
| classBreakType | [enumeration ClassBreakType](CIMSymbolizers.md#enumeration-classbreaktype)|Gets and sets the class break type. 
| classificationMethod | [enumeration ClassificationMethod](CIMSymbolizers.md#enumeration-classificationmethod)|Gets and sets the classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp)|Gets and sets the color ramp. 
| field | string|Gets and sets the field for rendering. 
| minimumBreak | double|Gets and sets the minimum break for the renderer. 
| numberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format. 
| showClassGaps | boolean|Gets and sets a boolean value indicating whether or not to show class gaps. 
| showInAscendingOrder | boolean|Gets and sets a boolean value indicating whether or not to show classes in ascending order. 
| heading | string|Gets and sets the heading. 
| sampleSize | long|Gets and sets the sample size used for creating the classification. 
| useDefaultSymbol | boolean|Gets and sets a boolean value indicating whether or not to use the default symbol. 
| defaultSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the default symbol. 
| minimumLabel | string|Gets and sets the minimum label. 
| defaultLabel | string|Gets and sets the default label. 
| defaultDescription | string|Gets and sets the default description. 
| valueExpressionInfo | [CIMExpressionInfo](CIMSymbolizers.md#cimexpressioninfo)|Gets and sets ExpressionInfo that contains the Arcade expression that returns value as a number. When both Fields and ValueExpressionInfo are present ValueExpressionInfo is used. 


### CIMGAIsoRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| isoQuality | long|Gets and sets the iso quality. 
| isoType | string|Gets and sets the iso type 
| noResultSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the no result symbol. 
| refineOnZoom | boolean|Gets and sets a boolean indicating whether to refine on zoom. 






## CIMGALayer
#### Represents the GA layer. 


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


### CIMGALayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| AOI | [Envelope](ExternalReferences.md#envelope)|Gets and sets the area of interest. 
| method | [CIMGAMethod](CIMGALayer.md#cimgamethod)|Gets and sets the GA method. 
| renderers | [CIMRenderer](Types.md#cimrenderer) |Gets and sets the renderers. 






## CIMGAMethod
#### Represents the GA method. 


### CIMGAMethod 

|Property | Type | Description | 
|---------|--------|--------|
| model | string|Gets and sets the model. 
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection 



