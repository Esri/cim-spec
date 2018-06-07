


## CIMInMemoryDatasetDataConnection
#### Represents an in-memory dataset data connection 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMInMemoryDatasetDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| dataset | string|Gets and sets the dataset name. 






## CIMInMemoryWorkspaceDataConnection
#### Represents an in-memory workspace data connection 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMInMemoryWorkspaceDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| binaryReferencePath | string|Gets and sets the path to the binary reference containing the serialized workspace. 






## CIMNALayer
#### Represents a network analysis layer. 


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


### CIMNALayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| NAWorkspace | [DataConnection](Types.md#dataconnection)|Gets and sets data connection for the NA workspace. 
| networkDataset | [DataConnection](Types.md#dataconnection)|Gets and sets data connection for the network dataset. 
| standaloneTables | IStringArray|Gets and sets an array of standlone table paths. 
| solver | [NASolverDefinition](ExternalReferences.md#nasolverdefinition)|Gets and sets the NA solver. 
| locator | [NALocatorDefinition](ExternalReferences.md#nalocatordefinition)|Gets and sets the locator. 
| agents | [NAAgentDefinition](ExternalReferences.md#naagentdefinition)|Gets and sets the agents. 


### CIMGroupLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| layers | IStringArray|Gets and sets the paths of the layers in the group layer. 
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing)|Gets and sets the symbol layer drawing definition. 






## CIMNetworkDatasetElementCompositeRenderer
#### Represents a network dataset element composite renderer. 


### CIMNetworkDatasetRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| label | string|Gets and sets the renderer label. 
| visible | bool|Gets and sets a boolean value indicating whether or not the renderer is visible. 


### CIMNetworkDatasetElementCompositeRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| edgeLineRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer)|Gets and sets edge line renderer. 
| edgePointRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer)|Gets and sets edge point renderer. 
| junctionPointRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer)|Gets and sets junction point renderer. 
| turnLineRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer)|Gets and sets turn line renderer. 






## CIMNetworkDatasetLayer
#### Represents a network dataset layer. 


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


### CIMNetworkDatasetLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets data connection to the network dataset. 
| dirtyAreaRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer)|Gets and sets the dirty area renderer. 
| displayNetworkAttribute | string|Gets and sets the display network attribute. 
| edgeRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer)|Gets and sets the edge renderer. 
| junctionRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer)|Gets and sets the junction renderer. 
| missingElementRenderer | [CIMNetworkDatasetElementCompositeRenderer](CIMNetworkLayers.md#cimnetworkdatasetelementcompositerenderer)|Gets and sets the missing element renderer. 
| networkSourceDisplayFilters | [CIMNetworkSourceDisplayFilter](CIMNetworkLayers.md#cimnetworksourcedisplayfilter) |Gets and sets the network source display filters. 
| oneWayRenderer | [CIMNetworkDatasetElementCompositeRenderer](CIMNetworkLayers.md#cimnetworkdatasetelementcompositerenderer)|Gets and sets the one-way renderer. 
| restrictionNetworkAttributes | IStringArray|Gets and sets the restriction network attributes. 
| restrictionRenderer | [CIMNetworkDatasetElementCompositeRenderer](CIMNetworkLayers.md#cimnetworkdatasetelementcompositerenderer)|Gets and sets the restriction renderer. 
| systemJunctionRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer)|Gets and sets the system junction renderer. 
| trafficNetworkAttribute | string|Gets and sets the traffic network attribute. 
| trafficRenderer | [CIMNetworkDatasetTrafficRenderer](CIMNetworkLayers.md#cimnetworkdatasettrafficrenderer)|Gets and sets the traffic renderer. 
| traversableRenderer | [CIMNetworkDatasetElementCompositeRenderer](CIMNetworkLayers.md#cimnetworkdatasetelementcompositerenderer)|Gets and sets the traversable renderer. 
| turnRenderer | [CIMNetworkDatasetSimpleRenderer](CIMNetworkLayers.md#cimnetworkdatasetsimplerenderer)|Gets and sets the turn renderer. 






## CIMNetworkDatasetSimpleRenderer
#### Represents a network dataset simple renderer. 


### CIMNetworkDatasetRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| label | string|Gets and sets the renderer label. 
| visible | bool|Gets and sets a boolean value indicating whether or not the renderer is visible. 


### CIMNetworkDatasetSimpleRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the renderer description. 
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol. 






## CIMNetworkDatasetTrafficRenderer
#### Represents a network dataset traffic renderer. 


### CIMNetworkDatasetRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| label | string|Gets and sets the renderer label. 
| visible | bool|Gets and sets a boolean value indicating whether or not the renderer is visible. 


### CIMNetworkDatasetTrafficRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| breaks | [CIMClassBreak](CIMSymbolizers.md#cimclassbreak) |Gets and sets the renderer class breaks. 
| defaultDescription | string|Gets and sets the default description. 
| defaultLabel | string|Gets and sets the default label. 
| defaultSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the default symbol. 
| showLiveTrafficOnly | boolean|Gets and sets a boolean option indicating whether or not to show only live traffic. 
| useDefaultSymbol | boolean|Gets and sets a boolean option indicating whether or not to use the default symbol. 


### CIMNetworkDatasetFastTrafficRenderer 

|Property | Type | Description | 
|---------|--------|--------|
| drawLineWidthByHierarchyLevelIndex | boolean|Gets and sets a boolean value indicating whether of not to draw line width by hierarchy level index. 
| exteriorLineWidthIncrement | double|Gets and sets the exterior line width increment. 
| interiorLineWidthsByHierarchyLevelIndex | [double]|Gets and sets the interior line widths by hierarchy level index. 
| lineCasingsColor | [Color](Types.md#color)|Gets and sets the line casings color. 
| scaleFilters | [double]|Gets and sets the scale filters. 
| useDerivedLineCasingsColor | boolean|Gets and sets a boolean value indicating whether of not to use a derived line casing color. 
| useLineCasings | boolean|Gets and sets a boolean value indicating whether of not to use line casings. 
| useScaleFilters | boolean|Gets and sets a boolean value indicating whether of not to use scale filters. 






## CIMNetworkSourceDisplayFilter
#### Represents a network source display filter. 


### CIMNetworkSourceDisplayFilter 

|Property | Type | Description | 
|---------|--------|--------|
| networkSource | string|Gets and sets the network source. 
| visible | boolean|Gets and sets a boolean value indicating visiblity. 
| definitionExpression | string|Gets and sets the definition expression. 






## CIMUtilityNetworkLayer
#### Represents a utility network layer. 


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


### CIMUtilityNetworkLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection. 
| activeContainerSourceID | long|Gets and sets the active container source ID. 
| activeContainerFeatureID | string|Gets and sets the active container feature ID. 
| pointErrorLayer | string|Gets and sets the path to the point error layer. 
| lineErrorLayer | string|Gets and sets the path to the line error layer. 
| polygonErrorLayer | string|Gets and sets the path to the polygon error layer. 
| dirtyAreaLayer | string|Gets and sets the path to the dirty area layer. 



