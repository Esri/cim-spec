


## CIM3DLayerProperties
#### Represents 3D layer properties which contain properties used for 3D draw. 


### CIM3DLayerProperties 

|Property | Type | Description | 
|---------|--------|--------|
| castShadows | boolean | A value indicating whether shadows are enabled. If true, this layer's features contribute to shadows. 
| isLayerLit | boolean | A value indicating whether this layer is lit. This property determines whether an object in 3D is shaded based on the angle of its normal compared to the lighting properties of the scene (where the "sun" is) or is lit uniformly as if by only ambient light (light with no distinct directionality). 
| layerFaceCulling | [enumeration FaceCulling3D](CIMEnumerations.md#enumeration-faceculling3d) | The layer's face culling setting. 
| maxDistance | double | The maximum distance at which objects in view are visible. Objects beyond this point don't get rendered. 
| maxPreloadDistance | double | The maximum radius from the camera at which objects outside the view are loaded. Values are in Meters. 
| minDistance | double | The minimum distance at which objects in view are visible. Objects closer than this don't get rendered. 
| minPreloadDistance | double | The minimum radius from the camera at which objects at which objects outside the view are loaded. Values are in Meters. 
| preloadTextureCutoffHigh | double | The distance (in visible range) at which high resolution textures change to low resolution textures for objects outside the view. Range is 0 to 1. 
| preloadTextureCutoffLow | double | The distance (in visible range) at which low resolution textures change to solid colors for objects outside the view. Range is 0 to 1. 
| textureCutoffHigh | double | The distance (in visible range) at which the high resolution textures change to low resolution textures. Range is 0 to 1. 
| textureCutoffLow | double | The distance (in visible range) at which the high resolution textures change to solid colors. Range is 0 to 1. 
| textureDownscalingFactor | long | The downscaling factor. All textures for this layer are downscaled by this additional factor on loading. 
| useCompressedTextures | boolean | A value indicating whether uncompressed textures are compressed using DXT5 at load time. 
| verticalExaggeration | double | The layer's vertical exaggeration. 
| verticalUnit | [Unit](ExternalReferences.md#unit) | The layer's vertical unit. 
| depthPriority | long | The depth priority of a 3D layer. 
| lighting | [enumeration Lighting3D](CIMLayer.md#enumeration-lighting3d) | The layer's lighting setting. 
| optimizeMarkerTransparency | boolean | A value indicating whether true alpha is quantized to fully opaque or transparent when false, actual values are used in marker drawing. 
| useDepthWritingForTransparency | boolean | A value indicating whether to use depth writing for transparency. This should be set to true if anomalies are seen in drawing order of transparent features in the same feature class. 






## CIMChart
#### Provides access to members that control chart properties. 


### CIMChart 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the chart. 
| series | [[CIMChartSeries]](Types.md#cimchartseries) | The series properties of the chart. 
| generalProperties | [CIMChartGeneralProperties](CIMLayer.md#cimchartgeneralproperties) | The general properties of the chart. 
| legend | [CIMChartLegend](CIMLayer.md#cimchartlegend) | The legend properties of the chart. 
| axes | [[CIMChartAxis]](CIMLayer.md#cimchartaxis) | The properties of chart axis. 
| mapSelectionHandling | [enumeration ChartMapSelectionHandling](CIMLayer.md#enumeration-chartmapselectionhandling) | A setting which indicates whether chart handles selection in the input layer by creating series only from the selected data or highlights selected values on the chart made from entire dataset. 
| metaData | string | The client metadata about the chart. 






## CIMChartAxis
#### Provides access to members that control chart axis properties. 


### CIMChartAxis 

|Property | Type | Description | 
|---------|--------|--------|
| visible | boolean | A value indicating whether the chart axis is visible. 
| isLogarithmic | boolean | A value indicating whether the chart axis has logarithmic scale. 
| title | string | The title of an axis. 
| showTitle | boolean | A value indicating whether the axis title is visible. 
| valueFormat | string | The format string for axis value labels. 
| valueNumberFormat | [NumberFormat](Types.md#numberformat) | The number format of the axis labels. ValueNumberFormat takes precedence over ValueFormat when both are specified. 
| dateTimeFormat | string | The format string for axis date/time labels. 
| calculateAutomaticMinimum | boolean | A value indicating whether the chart axis calculates its minimum. 
| calculateAutomaticMaximum | boolean | A value indicating whether the chart axis calculates its maximum. 
| minimum | any | The minimum of the axis. 
| maximum | any | The maximum of the axis. 
| titleText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The title symbol properties. 
| labelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The label symbol properties. 
| axisLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The line symbol properties for axis. 
| guides | [[CIMChartGuide]](CIMLayer.md#cimchartguide) | The array of guides. 






## CIMChartBarSeries
#### Provides access to members that control bar chart series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the series shown in the legend. 
| uniqueName | string | The default and unique name of the series. 
| fields | [string] | The data field names in the series. Optional depending on series type. 
| orderFields | [string] | The sort field names in the series. 
| groupFields | [string] | The group field names in the series. 
| whereClause | string | The format string for series value labels. 
| showLabels | boolean | A value indicating whether the series shows data labels. 
| horizontalAxis | long | The index of horizontal axis. 
| verticalAxis | long | The index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi-series. 
| locations | [[CIMChartLocationDefinition]](CIMLayer.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartBarSeries 

|Property | Type | Description | 
|---------|--------|--------|
| multipleBarType | [enumeration ChartMultiBarType](CIMLayer.md#enumeration-chartmultibartype) | The type of multiple bar-series chart. 
| barSize | long | The relative width of the bar. 
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties) | The properties of the fill symbol border. 
| verticalOrientation | boolean | A value indicating whether this bar chart is vertically oriented. 






## CIMChartBoxPlotSeries
#### Provides access to members that control bar chart box plot series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the series shown in the legend. 
| uniqueName | string | The default and unique name of the series. 
| fields | [string] | The data field names in the series. Optional depending on series type. 
| orderFields | [string] | The sort field names in the series. 
| groupFields | [string] | The group field names in the series. 
| whereClause | string | The format string for series value labels. 
| showLabels | boolean | A value indicating whether the series shows data labels. 
| horizontalAxis | long | The index of horizontal axis. 
| verticalAxis | long | The index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi-series. 
| locations | [[CIMChartLocationDefinition]](CIMLayer.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartBoxPlotSeries 

|Property | Type | Description | 
|---------|--------|--------|
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties) | The properties of the box plot symbol. 
| verticalOrientation | boolean | A value indicating whether the box plot is vertically oriented. 
| showOutliers | boolean | A value indicating whether to show the box plot outliers. 
| showInnerPoints | boolean | A value indicating whether to show the box plot inner points. 
| showMean | boolean | A value indicating whether to show the box plot mean marker. 
| standardizeValues | boolean | A value indicating whether to calculate standardized values for box plot. 






## CIMChartCalendarHeatSeries
#### Provides access to members that control CalendarHeat series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the series shown in the legend. 
| uniqueName | string | The default and unique name of the series. 
| fields | [string] | The data field names in the series. Optional depending on series type. 
| orderFields | [string] | The sort field names in the series. 
| groupFields | [string] | The group field names in the series. 
| whereClause | string | The format string for series value labels. 
| showLabels | boolean | A value indicating whether the series shows data labels. 
| horizontalAxis | long | The index of horizontal axis. 
| verticalAxis | long | The index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi-series. 
| locations | [[CIMChartLocationDefinition]](CIMLayer.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartCalendarHeatSeries 

|Property | Type | Description | 
|---------|--------|--------|
| columnTimeUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time units for columns. 
| rowTimeUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time units for rows. 
| nullPolicy | [enumeration ChartNullPolicy](CIMLayer.md#enumeration-chartnullpolicy) | The policy for handling missing data. 
| noDataColor | [Color](Types.md#color) | Color properties for empty cells. 
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method with which breaks are created. 
| breaksCount | long | The number of breaks for automatic breaks creation. 
| minimumBreak | double | The lower bound of the first range. 
| breaks | [double] | The upper bound breaks. 
| breakColors | [[CIMColor]](Types.md#cimcolor) | The color for each break. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp from which break colors are created. 





### Enumeration: ChartColorType
#### Provides a type of coloring that chart series uses. 

|Property | Value | Description | 
|---------|--------|--------|
| SingleColor| 0| Uses a single color for series. 
| ColorMatch| 1| Matches series colors with the layer. 




## CIMChartDataClockSeries
#### Provides access to members that control DataClock series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the series shown in the legend. 
| uniqueName | string | The default and unique name of the series. 
| fields | [string] | The data field names in the series. Optional depending on series type. 
| orderFields | [string] | The sort field names in the series. 
| groupFields | [string] | The group field names in the series. 
| whereClause | string | The format string for series value labels. 
| showLabels | boolean | A value indicating whether the series shows data labels. 
| horizontalAxis | long | The index of horizontal axis. 
| verticalAxis | long | The index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi-series. 
| locations | [[CIMChartLocationDefinition]](CIMLayer.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartDataClockSeries 

|Property | Type | Description | 
|---------|--------|--------|
| wedgeTimeUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time units for wedges. 
| ringTimeUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time units for rings. 
| trimIncompleteTimeInterval | boolean | A value indicating whether incomplete time intervals at the ends of time interval ranges are trimmed in order to avoid bias. 
| nullPolicy | [enumeration ChartNullPolicy](CIMLayer.md#enumeration-chartnullpolicy) | The policy for handling missing data. 
| noDataColor | [Color](Types.md#color) | Color properties for empty cells. 
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method with which breaks are created. 
| breaksCount | long | The number of breaks for automatic breaks creation. 
| minimumBreak | double | The lower bound of the first range. 
| breaks | [double] | The upper bound breaks. 
| breakColors | [[CIMColor]](Types.md#cimcolor) | The color for each break. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp from which break colors are created. 
| showWedgeLabel | boolean | A value indicating whether the wedge label is visible. 
| wedgeLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text symbol properties for the wedge label. 





### Enumeration: ChartDataTransformationType
#### Types of a data transformation to apply before calculating histogram bins and counts. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No data transformations. 
| Logarithmic| 1| Apply logarithmic data transformation. 
| SquareRoot| 2| Apply square root for data transformation. 




## CIMChartFillSymbolProperties
#### Provides access to members that control properties of the fill symbol. 


### CIMChartFillSymbolProperties 

|Property | Type | Description | 
|---------|--------|--------|
| color | [Color](Types.md#color) | The color of the fill. 
| opacity | long | The transparency level of histogram bars. 
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The properties of the fill symbol border. 





### Enumeration: ChartFontWeight
#### Chart font weight types. 

|Property | Value | Description | 
|---------|--------|--------|
| Lighter| 0| Defines lighter characters. 
| Normal| 1| Defines normal characters. 
| Bold| 2| Defines bold characters. 




## CIMChartGeneralProperties
#### Provides access to members that control general chart properties. 


### CIMChartGeneralProperties 

|Property | Type | Description | 
|---------|--------|--------|
| title | string | The title of the chart. 
| showTitle | boolean | A value indicating whether the chart title is visible. 
| subTitle | string | The subtitle of the chart. 
| showSubTitle | boolean | A value indicating whether the chart subtitle is visible. 
| footer | string | The footer of the chart. 
| showFooter | boolean | A value indicating whether the chart footer is visible. 
| theme | string | The theme of the chart. 
| titleText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The title symbol properties. 
| subTitleText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The subtitle symbol properties. 
| footerText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The footer symbol properties. 
| backgroundSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties) | The background fill symbol properties for the chart. 
| gridLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The line symbol properties for grid lines. 






## CIMChartGuide
#### Define the properties to define a chart guide. 


### CIMChartGuide 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name / title for the guide. 
| label | string | The label for the guide. 
| labelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text format for the guide label. 
| labelPosition | [enumeration ChartPosition](CIMLayer.md#enumeration-chartposition) | The relative position of the label to the guide. 
| valueFrom | double | The numeric coordinate of the from value for the guide. This value will be used when guide value type is set to numeric. 
| valueTo | double | The numeric coordinate of the to value for the guide. This value will be used when guide value type is set to numeric. 
| timeFrom | [TimeInstant](ExternalReferences.md#timeinstant) | The temporal coordinate of the from value for the guide. This value will be used when guide value type is set to temporal. 
| timeTo | [TimeInstant](ExternalReferences.md#timeinstant) | The temporal coordinate of the to value for the guide. This value will be used when guide value type is set to temporal. 
| visible | boolean | A value indicating whether the guide is visible. 
| guideType | [enumeration ChartGuideType](CIMLayer.md#enumeration-chartguidetype) | The type of the guide. 
| guideValueType | [enumeration ChartValueType](CIMLayer.md#enumeration-chartvaluetype) | The type of the coordinate value used in the guide. 
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties) | The symbol properties for the guide. 





### Enumeration: ChartGuideType
#### Specifies the type of guide. 

|Property | Value | Description | 
|---------|--------|--------|
| ChartGuideType_Line| 0| Guide is a line 
| ChartGuideType_Range| 1| Guide is a range 




## CIMChartHistogramSeries
#### Provides access to members that control histogram series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the series shown in the legend. 
| uniqueName | string | The default and unique name of the series. 
| fields | [string] | The data field names in the series. Optional depending on series type. 
| orderFields | [string] | The sort field names in the series. 
| groupFields | [string] | The group field names in the series. 
| whereClause | string | The format string for series value labels. 
| showLabels | boolean | A value indicating whether the series shows data labels. 
| horizontalAxis | long | The index of horizontal axis. 
| verticalAxis | long | The index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi-series. 
| locations | [[CIMChartLocationDefinition]](CIMLayer.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartHistogramSeries 

|Property | Type | Description | 
|---------|--------|--------|
| binCount | long | The number of bins in classifying input values. 
| showMean | boolean | A value indicating whether to show the mean line on the histogram. 
| showMedian | boolean | A value indicating whether to show the median line on a histogram. 
| showStandardDeviation | boolean | A value indicating whether to show the standard deviation band on the histogram. 
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties) | The properties of the fill symbol border. 
| meanLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The mean line symbol properties of the line series. 
| medianLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The median line symbol properties of the line series. 
| standardDeviationLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The line symbol for the standard deviation. 
| showComparisonDistribution | boolean | A value indicating whether to show a comparison distribution line overlay for the histogram chart. 
| dataTransformationType | [enumeration ChartDataTransformationType](CIMLayer.md#enumeration-chartdatatransformationtype) | The type of a data transformation to apply before calculating histogram bins and counts. 
| distributionLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The line symbol for the comparison distribution. 
| countField | string | A raster attribute table count field in order to calculate a histogram and statistics for fields that have to be adjusted for counts. 






## CIMChartLegend
#### Provides access to members that control chart legend properties. 


### CIMChartLegend 

|Property | Type | Description | 
|---------|--------|--------|
| visible | boolean | A value indicating whether the chart legend is visible. 
| title | string | The title of the legend. 
| showTitle | boolean | A value indicating whether the legend title is visible. 
| alignment | [enumeration ChartLegendAlignment](CIMLayer.md#enumeration-chartlegendalignment) | The options in arranging the chart legend. 
| valueFormat | string | The format string for series value labels. 
| legendText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text symbol properties. 
| legendTitle | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text symbol properties for legend title. 





### Enumeration: ChartLegendAlignment
#### Chart legend alignment options. 

|Property | Value | Description | 
|---------|--------|--------|
| Left| 0| The legend is arranged along the left side of the chart. 
| Right| 1| The legend is arranged along the right side of the chart. 
| Top| 2| The legend is arranged along the top of the chart 
| Bottom| 3| The legend is arranged along the bottom of the chart. 



### Enumeration: ChartLineDashStyle
#### Chart line dash style. 

|Property | Value | Description | 
|---------|--------|--------|
| Solid| 0| Uses solid line to draw the chart line. 
| Dot| 1| Uses dotted line to draw the chart line. 
| Dash| 2| Uses dashed line to draw the chart line. 
| DashDot| 3| Uses dash-dotted line to draw the chart line. 
| LongDash| 4| Uses long dashed line to draw the chart line. 
| LongDashDot| 5| Uses long dash-dotted line to draw the chart line. 




## CIMChartLineSeries
#### Provides access to members that control line series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the series shown in the legend. 
| uniqueName | string | The default and unique name of the series. 
| fields | [string] | The data field names in the series. Optional depending on series type. 
| orderFields | [string] | The sort field names in the series. 
| groupFields | [string] | The group field names in the series. 
| whereClause | string | The format string for series value labels. 
| showLabels | boolean | A value indicating whether the series shows data labels. 
| horizontalAxis | long | The index of horizontal axis. 
| verticalAxis | long | The index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi-series. 
| locations | [[CIMChartLocationDefinition]](CIMLayer.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartLineSeries 

|Property | Type | Description | 
|---------|--------|--------|
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The line symbol properties of the line series. 
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties) | The marker symbol properties of the line series. 
| timeAggregationType | [enumeration ChartTimeAggregationType](CIMLayer.md#enumeration-charttimeaggregationtype) | The time aggregation type. 
| timeIntervalUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units used for the time interval size. 
| timeIntervalSize | double | The time interval size. 
| calculateAutomaticTimeInterval | boolean | A value indicating whether the time interval is automatically calculated. 
| trimIncompleteTimeInterval | boolean | A value indicating whether incomplete time intervals at the ends of time interval ranges are trimmed in order to avoid bias. 
| nullPolicy | [enumeration ChartNullPolicy](CIMLayer.md#enumeration-chartnullpolicy) | The policy for handling missing data. 
| verticalOrientation | boolean | A value indicating whether this is a vertical (true) or horizontal (false) orientation of a line series. 






## CIMChartLineSymbolProperties
#### Provides access to members that control properties of the line symbol. 


### CIMChartLineSymbolProperties 

|Property | Type | Description | 
|---------|--------|--------|
| visible | boolean | A value indicating whether the line is visible. 
| width | double | The width of the line. 
| style | [enumeration ChartLineDashStyle](CIMLayer.md#enumeration-chartlinedashstyle) | The style of the line. 
| color | [Color](Types.md#color) | The color of the line. 






## CIMChartLocationDefinition
#### Represents the definition of a location for which data is to be plotted. 


### CIMChartLocationDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| geometry | [Geometry](ExternalReferences.md#geometry) | The geometry. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 
| label | string | The label. 
| enabled | boolean | A value indicating whether this location is enabled or not. 





### Enumeration: ChartMapSelectionHandling
#### Provides a choice of how map selection is processed in the chart. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Do not handle map selection. 
| Highlight| 1| Highlight selection set on a chart. 
| BuildFromSelectionSet| 2| Build a chart exclusively from the selection set. 




## CIMChartMarkerSymbolProperties
#### Provides access to members that control properties of the marker symbol. 


### CIMChartMarkerSymbolProperties 

|Property | Type | Description | 
|---------|--------|--------|
| visible | boolean | A value indicating whether the symbol is visible. 
| width | double | The width of the symbol. 
| height | double | The height of the symbol. 
| style | [enumeration ChartMarkerSymbolStyle](CIMLayer.md#enumeration-chartmarkersymbolstyle) | The style of the symbol. 
| color | [Color](Types.md#color) | The color of the symbol fill. 
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The properties of the symbol border. 





### Enumeration: ChartMarkerSymbolStyle
#### Chart marker symbol style. 

|Property | Value | Description | 
|---------|--------|--------|
| Circle| 0| Uses circle to draw the marker symbol. 
| Square| 1| Uses square to draw the marker symbol. 
| Diamond| 2| Uses diamond to draw the marker symbol. 
| Triangle| 3| Uses triangle to draw the marker symbol. 



### Enumeration: ChartMultiBarType
#### Standard multiple bar series placement options. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Do no use multiple bar series placement options. 
| SideBySide| 1| Uses side by side multiple bar series placement option. 
| Stacked| 2| Uses stacked bar series placement options. 
| Stacked100| 3| Uses stacked 100% multiple bar series placement options. 



### Enumeration: ChartNullPolicy
#### Options to handle null values. 

|Property | Value | Description | 
|---------|--------|--------|
| Null| 0| Leave the break in the line. 
| Zero| 1| Substitute nulls with zeros. 
| Interpolate| 2| Substitute nulls with interpolated values 



### Enumeration: ChartPosition
#### Specifies the position of the content for a target. 

|Property | Value | Description | 
|---------|--------|--------|
| ChartPosition_Center| 0| Content is placed at the center of the target 
| ChartPosition_Top| 1| Content is placed at the top of the target 
| ChartPosition_Bottom| 2| Content is placed at the bottom of the target 
| ChartPosition_Left| 3| Content is placed at the left of the target 
| ChartPosition_Right| 4| Content is placed at the right of the target 




## CIMChartProbabilityPlotSeries
#### Provides access to members that control probability plot series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the series shown in the legend. 
| uniqueName | string | The default and unique name of the series. 
| fields | [string] | The data field names in the series. Optional depending on series type. 
| orderFields | [string] | The sort field names in the series. 
| groupFields | [string] | The group field names in the series. 
| whereClause | string | The format string for series value labels. 
| showLabels | boolean | A value indicating whether the series shows data labels. 
| horizontalAxis | long | The index of horizontal axis. 
| verticalAxis | long | The index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi-series. 
| locations | [[CIMChartLocationDefinition]](CIMLayer.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartProbabilityPlotSeries 

|Property | Type | Description | 
|---------|--------|--------|
| probabilityPlotType | [enumeration ChartProbabilityPlotType](CIMLayer.md#enumeration-chartprobabilityplottype) | The type of a probability plot. 
| dataTransformationType | [enumeration ChartDataTransformationType](CIMLayer.md#enumeration-chartdatatransformationtype) | The type of data transformation to apply before calculating Normal Q-Q Plot. 
| showReferenceLine | boolean | A value indicating whether to show a reference line overlay for the probability plot. 
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties) | The marker symbol properties of the probability plot series. 
| referenceLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The line symbol properties of the probability plot series' reference line. 





### Enumeration: ChartProbabilityPlotType
#### Chart probability plot types. 

|Property | Value | Description | 
|---------|--------|--------|
| NormalQQPlot| 0| Normal Q-Q plot. 
| QQPlot| 1| General Q-Q plot. 




## CIMChartProfileGraphSeries
#### Provides access to members that control profile graph series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the series shown in the legend. 
| uniqueName | string | The default and unique name of the series. 
| fields | [string] | The data field names in the series. Optional depending on series type. 
| orderFields | [string] | The sort field names in the series. 
| groupFields | [string] | The group field names in the series. 
| whereClause | string | The format string for series value labels. 
| showLabels | boolean | A value indicating whether the series shows data labels. 
| horizontalAxis | long | The index of horizontal axis. 
| verticalAxis | long | The index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi-series. 
| locations | [[CIMChartLocationDefinition]](CIMLayer.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartProfileGraphSeries 

|Property | Type | Description | 
|---------|--------|--------|
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The line symbol properties of the profile graph series. 
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties) | The marker symbol properties of the profile graph series. 
| horizontalUnit | [Unit](ExternalReferences.md#unit) | The unit of measure to be used for horizontal distance. The default value is layer's spatial reference XY unit. 
| verticalUnit | [Unit](ExternalReferences.md#unit) | The the unit of measure to be used for elevation. The default value is the layer's vertical coordinate system's Z unit, if there is one. 






## CIMChartScatterPlotMatrixSeries
#### Provides access to members that control scatter plot matrix series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the series shown in the legend. 
| uniqueName | string | The default and unique name of the series. 
| fields | [string] | The data field names in the series. Optional depending on series type. 
| orderFields | [string] | The sort field names in the series. 
| groupFields | [string] | The group field names in the series. 
| whereClause | string | The format string for series value labels. 
| showLabels | boolean | A value indicating whether the series shows data labels. 
| horizontalAxis | long | The index of horizontal axis. 
| verticalAxis | long | The index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi-series. 
| locations | [[CIMChartLocationDefinition]](CIMLayer.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartScatterPlotMatrixSeries 

|Property | Type | Description | 
|---------|--------|--------|
| showHistograms | boolean | A value indicating whether to show histograms for all fields. 
| showTrendLine | boolean | A value indicating whether to show a trend line overlay for all scatter plots. 
| showAsRSquared | boolean | A value indicating whether show scatter plots as R squared values. 
| fieldLabels | [string] | The labels for scatter plot and histogram series' axes. 
| scatterMarkerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties) | The marker symbol properties of scatter plot series. 
| trendLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The line symbol properties of the scatter plot series' trend line. 
| histogramFillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties) | The fill symbol properties of histograms. 
| selectedMiniPlot | long | The index of the selected mini plot (-1 stands for non selected, -2 for uninitialized). 
| RSquareText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text symbol properties for the RSquare. 
| selectionLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The line symbol properties of the selection line for the mini plot. 






## CIMChartScatterSeries
#### Provides access to members that control point chart series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the series shown in the legend. 
| uniqueName | string | The default and unique name of the series. 
| fields | [string] | The data field names in the series. Optional depending on series type. 
| orderFields | [string] | The sort field names in the series. 
| groupFields | [string] | The group field names in the series. 
| whereClause | string | The format string for series value labels. 
| showLabels | boolean | A value indicating whether the series shows data labels. 
| horizontalAxis | long | The index of horizontal axis. 
| verticalAxis | long | The index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi-series. 
| locations | [[CIMChartLocationDefinition]](CIMLayer.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartScatterSeries 

|Property | Type | Description | 
|---------|--------|--------|
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties) | The marker symbol properties of the point series. 
| showTrendLine | boolean | A value indicating whether to show the trend line or not. 
| trendLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties) | The symbol properties for the trend line symbol. 
| trendLineFitType | [enumeration ChartTrendLineFitType](CIMLayer.md#enumeration-charttrendlinefittype) | A trend line fit type. 
| trendOrder | long | The number of terms in a polynomial or Fourier equation. 
| showTrendEquation | boolean | A value indicating whether or not to hows a trend equation overlay. 
| bubbleMinimumSize | double | Minimum size of the bubbles. 
| bubbleMaximumSize | double | Maximum size of the bubbles. 






## CIMChartSpectralProfileSeries
#### Represents a chart spectral profile series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the series shown in the legend. 
| uniqueName | string | The default and unique name of the series. 
| fields | [string] | The data field names in the series. Optional depending on series type. 
| orderFields | [string] | The sort field names in the series. 
| groupFields | [string] | The group field names in the series. 
| whereClause | string | The format string for series value labels. 
| showLabels | boolean | A value indicating whether the series shows data labels. 
| horizontalAxis | long | The index of horizontal axis. 
| verticalAxis | long | The index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi-series. 
| locations | [[CIMChartLocationDefinition]](CIMLayer.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartSpectralProfileSeries 

|Property | Type | Description | 
|---------|--------|--------|
| displayMode | [enumeration SpectralProfileDisplayMode](CIMLayer.md#enumeration-spectralprofiledisplaymode) | How this spectral profile is displayed. 
| showOutliers | boolean | A value indicating whether to show the box plot outliers. 
| standardizeValues | boolean | A value indicating whether to calculate standardized values for box plot. 






## CIMChartTemporalProfileBand
#### Represents a band for a variable to be plotted over time. 


### CIMChartTemporalProfileBand 

|Property | Type | Description | 
|---------|--------|--------|
| bandID | long | The band ID. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 
| label | string | The label. 
| locationID | long | The index of the location this definition corresponds to. 
| dimension | string | The dimension to be plotted on the y axis. 
| dimensionValues | [double] | The dimension values corresponding to the dimension to be plotted on the y axis. 






## CIMChartTemporalProfileBands
#### Represents the bands for a variable to be plotted over time. 


### CIMChartTemporalProfileBands 

|Property | Type | Description | 
|---------|--------|--------|
| variable | string | The variable name for which the bands are to be plotted. 
| bands | [[CIMChartTemporalProfileBand]](CIMLayer.md#cimcharttemporalprofileband) | The bands for a variable to be plotted. 






## CIMChartTemporalProfileDimensionValue
#### Represents a dimension value for a given variable to be plotted over time. 


### CIMChartTemporalProfileDimensionValue 

|Property | Type | Description | 
|---------|--------|--------|
| value | double | The value. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 
| label | string | The label. 
| locationID | long | The index of the location this definition corresponds to. 






## CIMChartTemporalProfileDimensionValues
#### Represents dimension values for a given variable to be plotted over time. 


### CIMChartTemporalProfileDimensionValues 

|Property | Type | Description | 
|---------|--------|--------|
| variable | string | The name of the variable for which the values are to be plotted. 
| dimension | string | The name of the dimension for which the values are to be plotted. 
| values | [[CIMChartTemporalProfileDimensionValue]](CIMLayer.md#cimcharttemporalprofiledimensionvalue) | Dimension values for a variable to be plotted. 





### Enumeration: ChartTemporalProfilePlotType
#### Represents the temporal profile plot type. 

|Property | Value | Description | 
|---------|--------|--------|
| Variables| 0| Plot of one or more variables over time. 
| Bands| 1| Plot of bands of a variable over time. 
| DimensionValues| 2| Plot of a variable at specific dimension values over time. 




## CIMChartTemporalProfileSeries
#### Represents a temporal profile chart series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the series shown in the legend. 
| uniqueName | string | The default and unique name of the series. 
| fields | [string] | The data field names in the series. Optional depending on series type. 
| orderFields | [string] | The sort field names in the series. 
| groupFields | [string] | The group field names in the series. 
| whereClause | string | The format string for series value labels. 
| showLabels | boolean | A value indicating whether the series shows data labels. 
| horizontalAxis | long | The index of horizontal axis. 
| verticalAxis | long | The index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi-series. 
| locations | [[CIMChartLocationDefinition]](CIMLayer.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartTemporalProfileSeries 

|Property | Type | Description | 
|---------|--------|--------|
| plotType | [enumeration ChartTemporalProfilePlotType](CIMLayer.md#enumeration-charttemporalprofileplottype) | The type of plot for this chart. 
| variables | [[CIMChartTemporalProfileVariable]](CIMLayer.md#cimcharttemporalprofilevariable) | The variables to be plotted over time. 
| bands | [CIMChartTemporalProfileBands](CIMLayer.md#cimcharttemporalprofilebands) | The bands for a variable to be plotted over time. 
| dimensionValues | [CIMChartTemporalProfileDimensionValues](CIMLayer.md#cimcharttemporalprofiledimensionvalues) | The dimension values for a variable to be plotted over time. 
| standardizeValues | boolean | A value indicating whether to calculate standardized values. 
| timeIntervalSize | double | The interval size for the time plotted on the x axis. 
| timeIntervalUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The unit of time for the interval size. 
| timeAggregationType | [enumeration ChartTimeAggregationType](CIMLayer.md#enumeration-charttimeaggregationtype) | The type of grouping to be applied on the time values plotted on the x axis. 
| trimIncompleteTimeInterval | boolean | A value indicating whether incomplete time intervals at the ends of time interval ranges are trimmed in order to avoid bias. 
| dateTimeFormat | string | The format of the date plotted on the x axis. 






## CIMChartTemporalProfileVariable
#### Represents a variable to be plotted over time. 


### CIMChartTemporalProfileVariable 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol. 
| label | string | The label. 
| dimension | string | The dimension to be plotted on the y axis. 
| dimensionValues | [double] | The dimension values corresponding to the dimension to be plotted on the y axis. 





### Enumeration: ChartTextCase
#### Options for choosing text cases for charts. 

|Property | Value | Description | 
|---------|--------|--------|
| Normal| 0| No capitalization. 
| Uppercase| 1| Transforms all characters to uppercase. 
| Lowercase| 2| Transforms all characters to lowercase. 
| Capitalize| 3| Transforms the first character of each word to uppercase. 
| SmallCaps| 4| All characters to uppercase but in small caps font. 




## CIMChartTextProperties
#### Represents chart text properties. 


### CIMChartTextProperties 

|Property | Type | Description | 
|---------|--------|--------|
| fontFillColor | [Color](Types.md#color) | The fill color for the font. 
| fontOutlineColor | [Color](Types.md#color) | The outline color for the font. 
| fontFamilyName | string | The font family name. 
| fontItalic | boolean | A value indicating whether the font style if it is italic or not. 
| fontSize | double | The font size in points. 
| fontWeight | [enumeration ChartFontWeight](CIMLayer.md#enumeration-chartfontweight) | The font weight. 
| textCase | [enumeration ChartTextCase](CIMLayer.md#enumeration-charttextcase) | The text case. 
| textUnderline | boolean | A value indicating whether the text is drawn with an underline. 
| textStrikethrough | boolean | A value indicating whether the text is drawn with a strikethrough. 
| textOverline | boolean | A value indicating whether the text is drawn with an overline. 





### Enumeration: ChartTimeAggregationType
#### Options for choosing how time intervals are built for the aggregation of a time based X-axis field. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No time aggregation is performed. 
| EqualIntervalsFromStartTime| 1| Time intervals start with the first (earliest) data point. 
| EqualIntervalsFromEndTime| 2| Time intervals start with the last (latest) data point. 
| CalendarIntervals| 3| Time intervals follow calendar breaks. 



### Enumeration: ChartTrendLineFitType
#### A fit type for a trend line. 

|Property | Value | Description | 
|---------|--------|--------|
| ChartTrendLineFitType_Linear| 0| A straight line that most closely approximates the data. Y(x) = a * x + b 
| ChartTrendLineFitType_Exponential| 1| Regression fit to the equation Y(x) = a * exp(b*x) 
| ChartTrendLineFitType_Logarithmic| 2| Regression fit to the equation Y(x) = a * ln(x) + b 
| ChartTrendLineFitType_Power| 3| Regression fit to the equation Y(x) = a * pow(x, b) 
| ChartTrendLineFitType_Fourier| 4| Regression fit to the equation Y(x) = a + b * cos(x) + c * sin(x) + d * cos(2x) + e * sin(2x) + ... 
| ChartTrendLineFitType_Polynomial| 5| Regression fit to the equation Y(x) = a * x^n + b * x^n-1 + c * x^n-2 + ... + z 
| ChartTrendLineFitType_MinX| 6| The minimum X-value 
| ChartTrendLineFitType_MinY| 7| The minimum Y-value 
| ChartTrendLineFitType_MaxX| 8| The maximum X-value 
| ChartTrendLineFitType_MaxY| 9| The maximum Y-value 
| ChartTrendLineFitType_AverageX| 10| The average X-value 
| ChartTrendLineFitType_AverageY| 11| The average Y-value 



### Enumeration: ChartValueType
#### Specifies the type of value. 

|Property | Value | Description | 
|---------|--------|--------|
| ChartValueType_Numeric| 0| Value is numeric 
| ChartValueType_Temporal| 1| Value is temporal 




## CIMCompositeSubLayer
#### Represents a composite sublayer. 


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


### CIMCompositeSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| subLayers | [[CIMSubLayerBase]](CIMLayer.md#cimsublayerbase) | The composite sublayers. 






## CIMDefinitionFilter
#### Contains filters so that only features satisfying these definitions will be displayed. 


### CIMDefinitionFilter 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the Definition Filter item. 
| definitionExpression | string | The definition expression to filter features in the dataset. 





### Enumeration: DisplayCacheType
#### Display cache types. 

|Property | Value | Description | 
|---------|--------|--------|
| Permanent| 0| Cache is permanent. 
| InSession| 1| Cache is maintained in session. 
| None| 2| No cache. 
| MaxAge| 3| Cache expires when it reaches the set maximum age. 




## CIMEyeDomeLighting
#### Represents eye-dome lighting properties. 


### CIMEyeDomeLighting 

|Property | Type | Description | 
|---------|--------|--------|
| isEnabled | boolean | A value indicating whether eye-dome lighting is enabled. 
| strength | double | The strength of the eye-dome lighting. This property can have a value between 0 and 1. 
| radius | double | The radius of the eye-dome lighting. This property can have a value between 1 and 5. 






## CIMGeodatabaseErrorLayer
#### Represents GDB Error tables as a composite layer and draws the errors. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the definition was last modified. 
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


### CIMGeodatabaseErrorLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| pointLayer | string | The path of the point layer in the Geodatabase Error layer. 
| lineLayer | string | The path of the line layer in the Geodatabase Error layer. 
| polygonLayer | string | The path of the polygon layer in the Geodatabase Error layer. 
| objectTable | string | The path of the object table in the Geodatabase Error layer. 
| workspaceConnection | [CIMWorkspaceConnection](CIMVectorLayers.md#cimworkspaceconnection) | The Geodatabase Errors data connection to the parent workspace. 






## CIMGroupLayer
#### Represents a group layer which is a simple ordered collection of other layers. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the definition was last modified. 
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


### CIMGroupLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| layers | [string] | The layer URIs of the layers in the group layer. 
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing) | The symbol layer drawing definition. 






## CIMKMLDataConnection
#### Represents a KML data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMKMLDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| KMLURI | string | The URI of the KML file or resource. 






## CIMKMLLayer
#### Represents a KML layer. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the definition was last modified. 
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


### CIMKMLLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [CIMKMLDataConnection](CIMLayer.md#cimkmldataconnection) | The data connection to the KML resource. 
| selectable | boolean | A value indicating whether the layer is selectable. 
| selectionColor | [Color](Types.md#color) | The selection color. 
| useSelectionColor | boolean | A value indicating whether to use the selection color. 
| labelVisibility | boolean | A value indicating whether to display labels for this KML layer's placemarks. 
| textSymbol | [CIMTextSymbol](CIMSymbols.md#cimtextsymbol) | The text symbol used to label placemarks. 






## CIMLayerElevationSurface
#### Represents a layer elevation surface. 


### CIMLayerElevationSurface 

|Property | Type | Description | 
|---------|--------|--------|
| offsetZ | double | Z offset. 
| mapElevationID | string | The map elevation ID. 






## CIMLayerTemplate
#### Represents a layer template. 


### CIMLayerTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string | The layer template URI. 
| layerTemplateId | string | The layer template ID. 
| parameters | {JSON_object}| The layer template parameters. 





### Enumeration: Lighting3D
#### The types of lighting. 

|Property | Value | Description | 
|---------|--------|--------|
| OneSideDataNormal| 0| Lights one side of each face using the original data normals. 
| OneSideResetNormal| 1| Lights one side of each face using recalculated normals. 
| TwoSideDataNormal| 2| Lights both sides of each face using original data normals. 
| TwoSideResetNormal| 3| Lights both sides of each face using recalculated normals. 
| TwoSideDataNormalFromWindingOrder| 4| Lights both sides of each face using original data normals, and the winding order for the "out" direction. 
| TwoSideResetNormalFromWindingOrder| 5| Lights both sides of each face using recalculated normal, and the winding order for the "out" direction. 



### Enumeration: SortOrderType
#### Options to choose sort order type. 

|Property | Value | Description | 
|---------|--------|--------|
| Ascending| 0| Sort ascending. 
| Descending| 1| Sort descending. 



### Enumeration: SpectralProfileDisplayMode
#### Spectral profile display modes. 

|Property | Value | Description | 
|---------|--------|--------|
| MeanLine| 0| Show spectral profile as line joining mean values of each raster band. 
| Boxes| 1| Show spectral profile as a series of boxes for each raster band. 
| BoxesAndMeanLine| 2| Show spectral profile as both a series of boxes for each raster band and lines joining mean values of each raster band. 
| ConsolidatedBoxesAndMeanLine| 3| Show spectral profile as both consolidated boxes for each raster band and lines joining mean values of each raster band. 




## CIMSubLayer
#### Represents sublayer. Defines a sublayer for a containing parent layer. The parent layer is a full-fledged layer, and it controls the sublayer, which is subordinate to the parent. The sublayer is not a layer definition itself rather, it is a property of its parent layer. 


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






## CIMSymbolLayerDrawing
#### Represents symbol layer drawing properties. 


### CIMSymbolLayerDrawing 

|Property | Type | Description | 
|---------|--------|--------|
| symbolLayers | [[CIMSymbolLayerIdentifier]](CIMLayer.md#cimsymbollayeridentifier) | The symbol layer identifiers. 
| useSymbolLayerDrawing | boolean | A value indicating whether symbol layer drawing is enabled. 






## CIMSymbolLayerIdentifier
#### Represents symbol layer identifier. 


### CIMSymbolLayerIdentifier 

|Property | Type | Description | 
|---------|--------|--------|
| symbolLayerName | string | The symbol layer name. 






## CIMTopologyLayer
#### Represents a topology dataset as a layer and draws its errors, exceptions, and areas in need of validation. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the definition was last modified. 
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


### CIMTopologyLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| allLayers | [string] | The paths of the layers in the topology layer. 
| topologyConnection | [DataConnection](Types.md#dataconnection) | The topology data connection. 



