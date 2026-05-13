

### Enumeration: EmissionRateUnit
#### Units for measuring emission rate. 

|Property | Value | Description | 
|---------|--------|--------|
| GramsPerSecond| 0| Grams per second (g/s). 
| KilogramsPerHour| 1| Kilograms per hour (kg/hr). 




## CIMFloodSimulationBarrier
#### Provides access to properties of a flood simulation barrier. 


### CIMFloodSimulationObject 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the object. It holds the layer URI when a raster is used. Otherwise it holds the displayed value. 
| visible | boolean | A value indicating whether the object is visible. 


### CIMFloodSimulationBarrier 

|Property | Type | Description | 
|---------|--------|--------|
| path | [Polyline](ExternalReferences.md#polyline) | The geometry of the barrier. 
| height | double | The height of the barrier. 
| width | double | The width of the barrier. 
| unit | [LinearUnit](ExternalReferences.md#linearunit) | The unit for the height and width of the barrier. It defaults to meter if left unset. 
| densifyPath | boolean | A value indicating whether to add vertices to the path to better follow the terrain. 





### Enumeration: FloodSimulationCalibrationMode
#### Calibration mode presets. 

|Property | Value | Description | 
|---------|--------|--------|
| Slow| 0| Slow (default) 
| Moderate| 1| Moderate 
| Fast| 2| Fast 




## CIMFloodSimulationCulvert
#### Provides access to properties of a flood simulation culvert. 


### CIMFloodSimulationObject 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the object. It holds the layer URI when a raster is used. Otherwise it holds the displayed value. 
| visible | boolean | A value indicating whether the object is visible. 


### CIMFloodSimulationCulvert 

|Property | Type | Description | 
|---------|--------|--------|
| path | [Polyline](ExternalReferences.md#polyline) | The geometry of the culvert. 
| height | double | The height of the culvert. 
| width | double | The width of the culvert. 
| unit | [LinearUnit](ExternalReferences.md#linearunit) | The unit for the height and width of the culvert. It defaults to meter if left unset. 
| profileType | [enumeration FloodSimulationCulvertProfileType](CIMSimulation.md#enumeration-floodsimulationculvertprofiletype) | The culvert profile type. 
| materialRoughness | double | The material roughness which is a factor affecting the flow rate. 
| openTop | boolean | A value indicating whether water can fall into the culvert from the top. 





### Enumeration: FloodSimulationCulvertProfileType
#### Culvert profile type. 

|Property | Value | Description | 
|---------|--------|--------|
| Elliptical| 0| Elliptical. 
| Rectangular| 1| Rectangular. 
| Arched| 2| Arched. 




## CIMFloodSimulationDepthRaster
#### Provides access to properties of a depth raster for flood simulation. 


### CIMFloodSimulationObject 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the object. It holds the layer URI when a raster is used. Otherwise it holds the displayed value. 
| visible | boolean | A value indicating whether the object is visible. 


### CIMFloodSimulationDepthRaster 

|Property | Type | Description | 
|---------|--------|--------|
| rasterDataConnection | [DataConnection](Types.md#dataconnection) | The data connection for the raster source. 
| linearUnit | [LinearUnit](ExternalReferences.md#linearunit) | The linear unit. 
| rasterIndex | long | The raster index for multidimensional rasters. 






## CIMFloodSimulationLayer
#### Provides access to properties of a flood simulation layer. 


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
| transparency | double | The transparency of the layer as a percentage. 
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
| showMapTips | boolean | A value indicating whether or not the value of the display field or expression is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use a fixed time extent for layer visibility. When true, the map time must overlap this extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The fixed time extent for layer visibility. 
| enableLayerEffects | boolean | A value indicating whether to enable any type of effects on the layer. 
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


### CIMSimulationLayer 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether this is the currently active simulation. 
| areaOfInterest | [Polygon](ExternalReferences.md#polygon) | The area of interest. 
| areaOfInterestSymbol | [CIMPolygonSymbol](CIMSymbols.md#cimpolygonsymbol) | The symbol for the area of interest. 
| useAutomaticCellResolution | boolean | A value indicating whether to automatically determine the cell resolution. 
| manualCellResolution | double | The manually set cell resolution in map units. 
| maxAOIEdgeCellCount | long | The maximum number of cells allowed on any edge of the area of interest. 
| elevationDownscalingFactor | double | The downscaling factor for loading raster elevation tiles. The cell size is multiplied by this value to change elevation level of detail. The minimum value of 1 uses the most accurate elevation with the slowest performance. Higher values increase the performance speed with less accurate elevation. 
| duration | double | The simulation duration in decimal hours. 
| currentTime | double | The current time (in decimal hours) as an offset from the start of the simulation at which to start playing. 
| playbackSpeed | double | The speed to play as a multiplier of the base speed. 
| playbackStep | double | The simulation playback time step in decimal hours. 
| useDefaultNumberOfCacheSlices | boolean | A value indicating whether to use the default number of stored cache slices. 
| secondsPerSimulationCacheSlice | double | The amount of simulated time between cache slices in seconds. Only used when UseDefaultNumberOfCacheSlices is false. 
| startTime | [TimeInstant](ExternalReferences.md#timeinstant) | The simulation start time. The end time will be the start time plus the duration. 


### CIMFloodSimulationLayer 

|Property | Type | Description | 
|---------|--------|--------|
| rainfallRate | [[CIMRateDuration]](CIMSimulation.md#cimrateduration) | An array of rainfall rates (in millimeters per hour) over durations (in seconds). 
| rainfallTransitionTime | double | The time (in seconds) to transition between rainfall rates. 
| rainfallDisplayUnits | [LinearUnit](ExternalReferences.md#linearunit) | The rainfall rate display units. 
| evaporationRate | double | The evaporation rate in millimeters per hour. 
| DEMSourceLayers | [string] | An array of URIs for the layers that will contribute to the DEM for flood simulation. These are independent layers in the scene, not owned by this layer. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp for shading the water. 
| valueRangeType | [enumeration FloodSimulationValueRangeType](CIMSimulation.md#enumeration-floodsimulationvaluerangetype) | The value range type for playing the simulation. 
| displayValueRange | [CIMRange](CIMVectorLayers.md#cimrange) | The display value range. 
| initialWaterDepthRaster | [FloodSimulationDepthRaster](Types.md#floodsimulationdepthraster) | The initial water depth raster. 
| infiltrationMaxRaster | [FloodSimulationDepthRaster](Types.md#floodsimulationdepthraster) | The infiltration max raster. 
| infiltrationRateRaster | [CIMFloodSimulationRateRaster](CIMSimulation.md#cimfloodsimulationrateraster) | The infiltration rate raster. 
| surfaceRoughnessValueRaster | [CIMFloodSimulationRateRaster](CIMSimulation.md#cimfloodsimulationrateraster) | The roughness value raster. 
| floodSimulationStorageURI | string | The URI of the simulation data storage that include water sources, barriers and culverts. 
| waterColorizer | [CIMRasterClassifyColorizer](CIMImageLayers.md#cimrasterclassifycolorizer) | The color class breaks for shading the water. 
| waterDisplayType | [enumeration FloodSimulationWaterDisplayType](CIMSimulation.md#enumeration-floodsimulationwaterdisplaytype) | The water display type. 
| containWaterInAOI | boolean | A value indicating whether water is contained in the area of interest or allowed to leave through the edges. 
| overrideWeatherEffects | boolean | A value indicating whether weather effects are controlled by the simulation while playing. 
| calibrationMode | [enumeration FloodSimulationCalibrationMode](CIMSimulation.md#enumeration-floodsimulationcalibrationmode) | A value indicating the preset mode for the simulation layer. 






## CIMFloodSimulationRateRaster
#### Provides access to properties of a rate raster for flood simulation. 


### CIMFloodSimulationObject 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the object. It holds the layer URI when a raster is used. Otherwise it holds the displayed value. 
| visible | boolean | A value indicating whether the object is visible. 


### CIMFloodSimulationDepthRaster 

|Property | Type | Description | 
|---------|--------|--------|
| rasterDataConnection | [DataConnection](Types.md#dataconnection) | The data connection for the raster source. 
| linearUnit | [LinearUnit](ExternalReferences.md#linearunit) | The linear unit. 
| rasterIndex | long | The raster index for multidimensional rasters. 


### CIMFloodSimulationRateRaster 

|Property | Type | Description | 
|---------|--------|--------|
| timeUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time unit. 






## CIMFloodSimulationSinkConnection
#### Provides access to properties of a simulation sink connection object. 


### CIMFloodSimulationSinkConnection 

|Property | Type | Description | 
|---------|--------|--------|
| waterSinkName | string | The name of the water sink. 
| delayTime | double | The time (in seconds) for water to flow from the sink to the source. 






## CIMFloodSimulationStorage
#### Represents storage for flood simulation data objects. 


### CIMFloodSimulationStorage 

|Property | Type | Description | 
|---------|--------|--------|
| waterSourceAreas | [[CIMFloodSimulationWaterSourceArea]](CIMSimulation.md#cimfloodsimulationwatersourcearea) | An array of water source areas. 
| waterSources | [[CIMFloodSimulationWaterSource]](CIMSimulation.md#cimfloodsimulationwatersource) | An array of water sources. 
| barriers | [[CIMFloodSimulationBarrier]](CIMSimulation.md#cimfloodsimulationbarrier) | An array of barriers. 
| culverts | [[CIMFloodSimulationCulvert]](CIMSimulation.md#cimfloodsimulationculvert) | An array of culverts. 
| waterSinkAreas | [[CIMFloodSimulationWaterSinkArea]](CIMSimulation.md#cimfloodsimulationwatersinkarea) | An array of water sink areas. 





### Enumeration: FloodSimulationValueRangeType
#### Value range types for playing flood simulation. 

|Property | Value | Description | 
|---------|--------|--------|
| FlowIntensity| 0| Flow intensity. 
| WaterDepth| 1| Water depth. 
| WaterSpeed| 2| Water speed. 



### Enumeration: FloodSimulationWaterDisplayType
#### Water display types for playing flood simulation. 

|Property | Value | Description | 
|---------|--------|--------|
| Fill| 0| Fill. 
| Edges| 1| Edges. 
| FillAndEdges| 2| Fill and edges. 




## CIMFloodSimulationWaterSinkArea
#### Provides access to properties of a flood simulation water sink. 


### CIMFloodSimulationObject 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the object. It holds the layer URI when a raster is used. Otherwise it holds the displayed value. 
| visible | boolean | A value indicating whether the object is visible. 


### CIMFloodSimulationWaterObject 

|Property | Type | Description | 
|---------|--------|--------|
| waterFlowRate | [[CIMRateDuration]](CIMSimulation.md#cimrateduration) | An array of water flow rates (in cubic meters/second) over durations (in seconds). 
| waterRateTransitionTime | double | The time (in seconds) to transition between water rates. 
| waterRateDisplayUnit | [LinearUnit](ExternalReferences.md#linearunit) | The water rate display unit. 


### CIMFloodSimulationWaterSinkArea 

|Property | Type | Description | 
|---------|--------|--------|
| area | [Polygon](ExternalReferences.md#polygon) | The area. 
| maximumIntake | double | The maximum intake of the water sink in cubic meters. 






## CIMFloodSimulationWaterSource
#### Provides access to properties of a flood simulation water source. 


### CIMFloodSimulationObject 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the object. It holds the layer URI when a raster is used. Otherwise it holds the displayed value. 
| visible | boolean | A value indicating whether the object is visible. 


### CIMFloodSimulationWaterObject 

|Property | Type | Description | 
|---------|--------|--------|
| waterFlowRate | [[CIMRateDuration]](CIMSimulation.md#cimrateduration) | An array of water flow rates (in cubic meters/second) over durations (in seconds). 
| waterRateTransitionTime | double | The time (in seconds) to transition between water rates. 
| waterRateDisplayUnit | [LinearUnit](ExternalReferences.md#linearunit) | The water rate display unit. 


### CIMFloodSimulationWaterSource 

|Property | Type | Description | 
|---------|--------|--------|
| location | [Point](ExternalReferences.md#point) | The location. 
| waterSinkConnections | [[CIMFloodSimulationSinkConnection]](CIMSimulation.md#cimfloodsimulationsinkconnection) | An array of water sink connections. Water flows from the connected sinks to this source instead of using a fixed flow rate when set. 






## CIMFloodSimulationWaterSourceArea
#### Provides access to properties of a flood simulation water source. 


### CIMFloodSimulationObject 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the object. It holds the layer URI when a raster is used. Otherwise it holds the displayed value. 
| visible | boolean | A value indicating whether the object is visible. 


### CIMFloodSimulationWaterObject 

|Property | Type | Description | 
|---------|--------|--------|
| waterFlowRate | [[CIMRateDuration]](CIMSimulation.md#cimrateduration) | An array of water flow rates (in cubic meters/second) over durations (in seconds). 
| waterRateTransitionTime | double | The time (in seconds) to transition between water rates. 
| waterRateDisplayUnit | [LinearUnit](ExternalReferences.md#linearunit) | The water rate display unit. 


### CIMFloodSimulationWaterSourceArea 

|Property | Type | Description | 
|---------|--------|--------|
| area | [Polygon](ExternalReferences.md#polygon) | The area. 






## CIMRateDuration
#### Provides access to properties of a rate duration. 


### CIMRateDuration 

|Property | Type | Description | 
|---------|--------|--------|
| duration | double | The duration. 
| rate | double | The rate. 





### Enumeration: TemperatureUnit
#### Units for measuring temperature. 

|Property | Value | Description | 
|---------|--------|--------|
| Celsius| 0| Degrees Celsius. 
| Fahrenheit| 1| Degrees Fahrenheit. 
| Kelvin| 2| Degrees Kelvin. 

