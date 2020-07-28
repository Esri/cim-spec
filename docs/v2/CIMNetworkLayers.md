


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
| layerMasks | [string] | The layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMLayer.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 


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
| agents | [NAAgentDefinition](ExternalReferences.md#naagentdefinition)| The agents. 






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
| layerMasks | [string] | The layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMLayer.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 


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
| layerMasks | [string] | The layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMLayer.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 


### CIMTraceNetworkLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| pointErrorLayer | string | The path to the point error layer. 
| lineErrorLayer | string | The path to the line error layer. 
| systemJunctionsLayer | string | The path to the junction layer. 
| dirtyAreaLayer | string | The path to the dirty area layer. 
| connectivityAssociationSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used to draw the connectivity associations of the trace network. 






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
| layerMasks | [string] | The layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMLayer.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not to this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 


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



