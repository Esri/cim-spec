


## CIMInMemoryDatasetDataConnection
#### Represents an in-memory dataset data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMInMemoryDatasetDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| dataset | string | The dataset name. 






## CIMInMemoryWorkspaceDataConnection
#### Represents an in-memory workspace data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMInMemoryWorkspaceDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| binaryReferencePath | string | The path to the binary reference containing the serialized workspace. 






## CIMNALayer
#### Represents a network analysis layer. 


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


### CIMStandaloneTableContainer 

|Property | Type | Description | 
|---------|--------|--------|
| standaloneTables | [string] | The standalone tables as an array of table repository paths. 


### CIMGroupLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| layers | [string] | The layer URIs of the layers in the group layer. 
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing) | The symbol layer drawing definition. 


### CIMNALayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| NAWorkspace | [DataConnection](Types.md#dataconnection) | Data connection for the NA workspace. 
| networkDataset | [DataConnection](Types.md#dataconnection) | Data connection for the network dataset. 
| solver | [NASolverDefinition](ExternalReferences.md#nasolverdefinition) | The NA solver. 
| locator | [NALocatorDefinition](ExternalReferences.md#nalocatordefinition) | The locator. 
| locatorOverrides | [[CIMNALocatorOverrideClass]](CIMNetworkLayers.md#cimnalocatoroverrideclass) | The locator overrides. 
| agents | [NAAgentDefinition](ExternalReferences.md#naagentdefinition)| The agents. 






## CIMNALocatorOverrideClass
#### Represents locator settings for a particular class. 


### CIMNALocatorOverrideClass 

|Property | Type | Description | 
|---------|--------|--------|
| className | string | The NAClass name for the locator settings. 
| locator | [NALocatorDefinition](ExternalReferences.md#nalocatordefinition) | The locator. 





### Enumeration: NDSRendererTarget
#### Renderer target. 

|Property | Value | Description | 
|---------|--------|--------|
| Edges| 0| Edges renderer target. 
| UserJunctions| 1| User Junctions renderer target. 
| SystemJunctions| 2| System Junctions renderer target. 
| Turns| 3| Turns renderer target. 
| Traffic| 4| Traffic renderer target. 
| DirtyAreas| 5| Dirty Areas renderer target. 




## CIMNetworkAttributeParameterDefinitionValue
#### Provides access to read or update the value assigned to a network parameter of a network attribute. 


### CIMNetworkAttributeParameterDefinitionValue 

|Property | Type | Description | 
|---------|--------|--------|
| networkAttributeName | string | The network attribute name. 
| networkParameterName | string | The network parameter name. 
| isRestrictionUsage | boolean | A value indicating whether this is a restriction usage type network parameter. 
| valueType | [enumeration ValueType](CIMNetworkLayers.md#enumeration-valuetype) | The value type. Supports: Short, Long, Float, Double, Date, String, Bool. 
| value | any | The value. The type of the value should correspond with the ValueType property or be null. 






## CIMNetworkDatasetElementCompositeRenderer
#### Represents a network dataset element composite renderer. 


### CIMNetworkDatasetRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| label | string | The renderer label. 
| visible | boolean | A value indicating whether or not the renderer is visible. 


### CIMNetworkDatasetElementCompositeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| edgeLineRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer) | Edge line renderer. 
| edgePointRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer) | Edge point renderer. 
| junctionPointRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer) | Junction point renderer. 
| turnLineRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer) | Turn line renderer. 






## CIMNetworkDatasetLayer
#### Represents a network dataset layer. 


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


### CIMNetworkDatasetLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | Data connection to the network dataset. 
| dirtyAreaRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer) | The dirty area renderer. 
| displayNetworkAttribute | string | The display network attribute. 
| edgeRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer) | The edge renderer. 
| junctionRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer) | The junction renderer. 
| missingElementRenderer | [CIMNetworkDatasetElementCompositeRenderer](CIMNetworkLayers.md#cimnetworkdatasetelementcompositerenderer) | The missing element renderer. 
| networkSourceDisplayFilters | [[CIMNetworkSourceDisplayFilter]](CIMNetworkLayers.md#cimnetworksourcedisplayfilter) | The network source display filters. 
| oneWayRenderer | [CIMNetworkDatasetElementCompositeRenderer](CIMNetworkLayers.md#cimnetworkdatasetelementcompositerenderer) | The one-way renderer. 
| restrictionNetworkAttributes | [string] | The restriction network attributes. 
| restrictionRenderer | [CIMNetworkDatasetElementCompositeRenderer](CIMNetworkLayers.md#cimnetworkdatasetelementcompositerenderer) | The restriction renderer. 
| systemJunctionRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer) | The system junction renderer. 
| trafficNetworkAttribute | string | The traffic network attribute. 
| trafficRenderer | [CIMNetworkDatasetTrafficRenderer](CIMNetworkLayers.md#cimnetworkdatasettrafficrenderer) | The traffic renderer. 
| traversableRenderer | [CIMNetworkDatasetElementCompositeRenderer](CIMNetworkLayers.md#cimnetworkdatasetelementcompositerenderer) | The traversable renderer. 
| turnRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer) | The turn renderer. 
| travelModeContext | [CIMNetworkTravelModeDefinitionContext](CIMNetworkLayers.md#cimnetworktravelmodedefinitioncontext) | The travel mode context. 
| restrictionStatusRenderers | [[CIMRestrictionStatusRenderer]](CIMNetworkLayers.md#cimrestrictionstatusrenderer) | The restriction status renderers. 
| classifyRestrictionsByPreferenceLevel | boolean | A value indicating whether to classify restrictions by preference level. 






## CIMNetworkDatasetSimpleRenderer
#### Represents a network dataset simple renderer. 


### CIMNetworkDatasetRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| label | string | The renderer label. 
| visible | boolean | A value indicating whether or not the renderer is visible. 


### CIMNetworkDatasetSimpleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | The renderer description. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 






## CIMNetworkDatasetTrafficRenderer
#### Represents a network dataset traffic renderer. 


### CIMNetworkDatasetRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| label | string | The renderer label. 
| visible | boolean | A value indicating whether or not the renderer is visible. 


### CIMNetworkDatasetTrafficRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [[CIMClassBreak]](CIMRenderers.md#cimclassbreak) | The renderer class breaks. 
| defaultDescription | string | The default description. 
| defaultLabel | string | The default label. 
| defaultSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The default symbol. 
| showLiveTrafficOnly | boolean | A value indicating whether or not to show only live traffic. 
| useDefaultSymbol | boolean | A value indicating whether or not to use the default symbol. 


### CIMNetworkDatasetFastTrafficRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| drawLineWidthByHierarchyLevelIndex | boolean | A value indicating whether of not to draw line width by hierarchy level index. 
| exteriorLineWidthIncrement | double | The exterior line width increment. 
| interiorLineWidthsByHierarchyLevelIndex | [double] | The interior line widths by hierarchy level index. 
| lineCasingsColor | [Color](Types.md#color) | The line casings color. 
| scaleFilters | [double] | The scale filters. 
| useDerivedLineCasingsColor | boolean | A value indicating whether of not to use a derived line casing color. 
| useLineCasings | boolean | A value indicating whether of not to use line casings. 
| useScaleFilters | boolean | A value indicating whether of not to use scale filters. 






## CIMNetworkSourceDisplayFilter
#### Represents a network source display filter. 


### CIMNetworkSourceDisplayFilter 

|Property | Type | Description | 
|---------|--------|--------|
| networkSource | string | The network source. 
| visible | boolean | A value indicating whether the filter is visible. 
| definitionExpression | string | The definition expression. 






## CIMNetworkTraceConfiguration
#### Represents a Trace Configuration. 


### CIMNetworkTraceConfiguration 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of trace configuration. 
| ID | string | Global id of trace configuration. 






## CIMNetworkTravelModeDefinition
#### The network travel mode is used to configure a group of cost, traversability, and other analysis configurations. 


### CIMNetworkTravelModeDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| modeType | string | The mode type. 
| description | string | The description. 
| impedanceAttributeName | string | The impedance attribute name. 
| timeAttributeName | string | The time attribute name. 
| distanceAttributeName | string | The distance attribute name. 
| restrictionAttributeNames | [string] | The array of restriction attribute names. 
| attributeParameterValues | [[CIMNetworkAttributeParameterDefinitionValue]](CIMNetworkLayers.md#cimnetworkattributeparameterdefinitionvalue) | The array of network attribute parameter definition values. 
| useHierarchy | boolean | A value indicating whether to use hierarchy. 
| UTurnAtJunctionsPolicy | [enumeration esriNetworkForwardStarBacktrack](ExternalReferences.md#enumeration-esrinetworkforwardstarbacktrack) | The u-turn at junctions policy for traversal between stops. 
| useOutputGeometryPrecision | boolean | A value indicating whether to use output geometry precision. 
| outputGeometryPrecisionValue | double | The output geometry precision value. 
| outputGeometryPrecisionUnits | [LinearUnit](ExternalReferences.md#linearunit) | The output geometry precision units. 






## CIMNetworkTravelModeDefinitionContext
#### Specifies the travel mode travel mode to be applied. Depending on the SourceType, some properties are conditionally required to indicate the travel mode. 


### CIMNetworkTravelModeDefinitionContext 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| sourceType | [enumeration NetworkTravelModeSourceType](CIMNetworkLayers.md#enumeration-networktravelmodesourcetype) | The travel mode source type. 
| sourceLayerURI | string | The source Layer URI of the item. Set if sourced from another layer. 
| travelMode | [CIMNetworkTravelModeDefinition](CIMNetworkLayers.md#cimnetworktravelmodedefinition) | The travel mode. Required if not sourced from a named travel mode of a Network Dataset. 





### Enumeration: NetworkTravelModeSourceType
#### The source type of the travel mode used by the travel mode context. 

|Property | Value | Description | 
|---------|--------|--------|
| NetworkDataset| 0| Indicates the name property refers to a travel mode of the network dataset. 
| Layer| 1| Indicates the travel mode is sourced from another layer. 
| Custom| 2| Indicates the source of travel mode is a custom defined travel mode. 



### Enumeration: RestrictionStatus
#### Restriction status. 

|Property | Value | Description | 
|---------|--------|--------|
| GeneralTraversable| 0| Traversable with any preference level. Used to indicate traversable when not classifying by preference level. 
| NeutralPreferenceLevelTraversable| 1| Traversable with a neutral preference level. 
| Prohibited| 2| Prohibited. 
| AvoidPreferenceLevelTraversable| 3| Traversable with an avoid preference level. 
| PreferPreferenceLevelTraversable| 4| Traversable with a prefer preference level. 
| MixedPreferenceLevelTraversable| 5| Traversable, but with opposite preference levels in one direction from the other. Avoid in one direction and prefer in the other. 
| Invalid| 6| Invalid restriction status. 




## CIMRestrictionStatusRenderer
#### Represents a renderer that shows the restriction status of network elements. 


### CIMNetworkDatasetRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| label | string | The renderer label. 
| visible | boolean | A value indicating whether or not the renderer is visible. 


### CIMRestrictionStatusRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| rendererTarget | [enumeration NDSRendererTarget](CIMNetworkLayers.md#enumeration-ndsrenderertarget) | The renderer target. 
| restrictionStatusSymbolClasses | [[CIMRestrictionStatusSymbolClass]](CIMNetworkLayers.md#cimrestrictionstatussymbolclass) | The restriction status symbol classes. if advanced mode (is classify by preference level): all but GeneralTraversable can be applicable. if basic mode (is NOT classify by preference level): only Prohibited, GeneralTraversable, and Invalid can be applicable. MixedPreferenceLevelTraversable only applicable to NDSRendererTarget.Edges. 
| traversableDirectionsAdornerPointSymbolClasses | [[CIMTraversableDirectionsAdornerPointSymbolClass]](CIMNetworkLayers.md#cimtraversabledirectionsadornerpointsymbolclass) | The traversable directions adorner point symbol classes. Only applicable to NDSRendererTarget.Edges. Independent of classify by preference level setting. 






## CIMRestrictionStatusSymbolClass
#### Restriction status, label, and symbol. 


### CIMRestrictionStatusSymbolClass 

|Property | Type | Description | 
|---------|--------|--------|
| status | [enumeration RestrictionStatus](CIMNetworkLayers.md#enumeration-restrictionstatus) | The restriction status represented by the symbol. 
| label | string | The label. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 






## CIMTraceNetworkLayer
#### Represents a trace network layer. 


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


### CIMTraceNetworkLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| pointErrorLayer | string | The path to the point error layer. 
| lineErrorLayer | string | The path to the line error layer. 
| systemJunctionsLayer | string | The path to the junction layer. 
| dirtyAreaLayer | string | The path to the dirty area layer. 
| connectivityAssociationSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used to draw the connectivity associations of the trace network. 
| activeTraceConfigurations | [[CIMNetworkTraceConfiguration]](CIMNetworkLayers.md#cimnetworktraceconfiguration) | The active trace configurations. 





### Enumeration: TraversableDirections
#### Traversable directions. 

|Property | Value | Description | 
|---------|--------|--------|
| Prohibited| 0| Not traversable in any direction. 
| Traversable| 1| Traversable in all supported directions. 
| OneWay| 2| Traversable in one direction but not in the other. 




## CIMTraversableDirectionsAdornerPointSymbolClass
#### Traversable directions, label, and adorner point symbol. The applicable adorner point symbol is oriented and added to the restriction status symbol when drawn to indicate the directional traversability of network elements. 


### CIMTraversableDirectionsAdornerPointSymbolClass 

|Property | Type | Description | 
|---------|--------|--------|
| traversableDirections | [enumeration TraversableDirections](CIMNetworkLayers.md#enumeration-traversabledirections) | The supported traversable directions represented by the adorner point symbol. 
| label | string | The label. 
| adornerPointSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The adorner point symbol to be composed with the restriction status symbol when drawn. 






## CIMUtilityNetworkLayer
#### Represents a utility network layer. 


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


### CIMStandaloneTableContainer 

|Property | Type | Description | 
|---------|--------|--------|
| standaloneTables | [string] | The standalone tables as an array of table repository paths. 


### CIMUtilityNetworkLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| pointErrorLayer | string | The path to the point error layer. 
| lineErrorLayer | string | The path to the line error layer. 
| polygonErrorLayer | string | The path to the polygon error layer. 
| dirtyAreaLayer | string | The path to the dirty area layer. 
| connectivityAssociationSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used to draw the connectivity associations of the utility network. 
| structuralAttachmentAssociationSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used to draw the structural attachment associations of the utility network. 
| containerAssociationSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used to draw the container associations of the utility network. 
| activeTraceConfigurations | [[CIMNetworkTraceConfiguration]](CIMNetworkLayers.md#cimnetworktraceconfiguration) | The active trace configurations. 
| dirtyObjectsTable | string | The path of the dirty objects table in the utility network layer. 





### Enumeration: ValueType
#### The data type of a value. 

|Property | Value | Description | 
|---------|--------|--------|
| Short| 2| Short integer 
| Long| 3| Long integer 
| Float| 4| Float value 
| Double| 5| Double value 
| Date| 7| Date value 
| String| 8| String value 
| Bool| 11| Boolean value 

