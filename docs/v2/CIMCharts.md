


## CIMChart
#### Provides access to members that control chart properties. 


### CIMChart 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the chart. 
| series | [[CIMChartSeries]](Types.md#chartseries) | The series properties of the chart. 
| generalProperties | [CIMChartGeneralProperties](CIMCharts.md#cimchartgeneralproperties) | The general properties of the chart. 
| legend | [CIMChartLegend](CIMCharts.md#cimchartlegend) | The legend properties of the chart. 
| axes | [[CIMChartAxis]](CIMCharts.md#cimchartaxis) | The properties of chart axis. 
| mapSelectionHandling | [enumeration ChartMapSelectionHandling](CIMCharts.md#enumeration-chartmapselectionhandling) | A setting which indicates whether chart handles selection in the input layer by creating series only from the selected data or highlights selected values on the chart made from entire dataset. 
| metaData | string | The client metadata about the chart. 
| multiSeriesChartProperties | [MultiSeriesChartProperties](Types.md#multiserieschartproperties) | The multi series chart properties for supported chart types. 





### Enumeration: ChartAggregationType
#### Options for choosing what aggregation type is to be used while calculating values. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No aggregation is performed. 
| Minimum| 1| The minimum value is used. 
| Maximum| 2| The maximum value is used. 
| Mean| 3| The mean value is used. 
| Median| 4| The median value is used. 
| Sum| 5| The sum of values is used. 
| Majority| 6| The majority of values is used. 
| Minority| 7| The minority of values is used. 




## CIMChartAxis
#### Provides access to members that control chart axis properties. 


### CIMChartAxis 

|Property | Type | Description | 
|---------|--------|--------|
| visible | boolean | A value indicating whether the chart axis is visible. 
| isLogarithmic | boolean | A value indicating whether the chart axis has logarithmic scale. 
| title | string | The title of an axis. 
| showTitle | boolean | A value indicating whether the axis title is visible. 
| useAutomaticTitle | boolean | A value indicating whether the axis title is auto generated. 
| valueFormat | string | The format string for axis value labels. 
| valueNumberFormat | [NumberFormat](Types.md#numberformat) | The number format of the axis labels. ValueNumberFormat takes precedence over ValueFormat when both are specified. 
| dateTimeFormat | string | The format string for axis date/time labels. 
| calculateAutomaticMinimum | boolean | A value indicating whether the chart axis calculates its minimum. 
| calculateAutomaticMaximum | boolean | A value indicating whether the chart axis calculates its maximum. 
| minimum | any | The minimum of the axis. 
| maximum | any | The maximum of the axis. 
| titleText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The title symbol properties. 
| labelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The label symbol properties. 
| axisLineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The line symbol properties for axis. 
| guides | [[CIMChartGuide]](CIMCharts.md#cimchartguide) | The array of guides. 
| labelCharacterLimit | long | The character limit for axis labels. 
| navigationScaleFactor | double | The scale factor for zoom/pan navigation. The value should be positive. This property can have a value more than 0 and less or equal to 1. Deprecated at 2.6. 
| navigationPosition | double | The relative start position for zoom/pan navigation. The value range is normalized between 0 and 1. This property can have a value between 0 and 1. Deprecated at 2.6. 






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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartBarSeries 

|Property | Type | Description | 
|---------|--------|--------|
| multipleBarType | [enumeration ChartMultiBarType](CIMCharts.md#enumeration-chartmultibartype) | The type of multiple bar-series chart. 
| barSize | long | The relative width of the bar. 
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMCharts.md#cimchartfillsymbolproperties) | The properties of the fill symbol border. 
| verticalOrientation | boolean | A value indicating whether this bar chart is vertically oriented. 
| sortedCategoryValues | [string] | The array of sorted category values for custom sort. 
| showMovingAverage | boolean | A value indicating whether to show a moving average line overlay for the time based bar chart. 
| movingAverageLineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The line symbol for the moving average. 
| movingAveragePeriod | long long | A period value for moving average calculation. 






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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartBoxPlotSeries 

|Property | Type | Description | 
|---------|--------|--------|
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMCharts.md#cimchartfillsymbolproperties) | The properties of the box plot symbol. 
| verticalOrientation | boolean | A value indicating whether the box plot is vertically oriented. 
| showOutliers | boolean | A value indicating whether to show the box plot outliers. 
| showInnerPoints | boolean | A value indicating whether to show the box plot inner points. 
| showMean | boolean | A value indicating whether to show the box plot mean marker. 
| standardizeValues | boolean | A value indicating whether to calculate standardized values for box plot. 
| sortedCategoryValues | [string] | The array of sorted category values for custom sort. 






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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartCalendarHeatSeries 

|Property | Type | Description | 
|---------|--------|--------|
| columnTimeUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time units for columns. 
| rowTimeUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time units for rows. 
| nullPolicy | [enumeration ChartNullPolicy](CIMCharts.md#enumeration-chartnullpolicy) | The policy for handling missing data. 
| noDataColor | [Color](Types.md#color) | Color properties for empty cells. 
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method with which breaks are created. 
| breaksCount | long | The number of breaks for automatic breaks creation. 
| minimumBreak | double | The lower bound of the first range. 
| breaks | [double] | The upper bound breaks. 
| breakColors | [[CIMColor]](Types.md#color) | The color for each break. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp from which break colors are created. 
| includeLeapDay | boolean | A value indicating whether a leap day (February 29) cell is a part of a chart. 





### Enumeration: ChartColorType
#### Provides a type of coloring that chart series uses. 

|Property | Value | Description | 
|---------|--------|--------|
| SingleColor| 0| Uses a single color from the palette for series. 
| ColorMatch| 1| Matches series colors with the layer. 
| CustomColor| 2| Uses the user-picked color for series. 




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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartDataClockSeries 

|Property | Type | Description | 
|---------|--------|--------|
| wedgeTimeUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time units for wedges. 
| ringTimeUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time units for rings. 
| trimIncompleteTimeInterval | boolean | A value indicating whether incomplete time intervals at the ends of time interval ranges are trimmed in order to avoid bias. 
| nullPolicy | [enumeration ChartNullPolicy](CIMCharts.md#enumeration-chartnullpolicy) | The policy for handling missing data. 
| noDataColor | [Color](Types.md#color) | Color properties for empty cells. 
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method with which breaks are created. 
| breaksCount | long | The number of breaks for automatic breaks creation. 
| minimumBreak | double | The lower bound of the first range. 
| breaks | [double] | The upper bound breaks. 
| breakColors | [[CIMColor]](Types.md#color) | The color for each break. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp from which break colors are created. 
| showWedgeLabel | boolean | A value indicating whether the wedge label is visible. 
| wedgeLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text symbol properties for the wedge label. 





### Enumeration: ChartDataTransformationType
#### Types of a data transformation to apply before calculating histogram bins and counts. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No data transformations. 
| Logarithmic| 1| Apply logarithmic data transformation. 
| SquareRoot| 2| Apply square root for data transformation. 
| Inverse| 3| Apply inverse data transformation. 
| BoxCox| 4| Apply Box-Cox data transformation. 




## CIMChartFillSymbolProperties
#### Provides access to members that control properties of the fill symbol. 


### CIMChartFillSymbolProperties 

|Property | Type | Description | 
|---------|--------|--------|
| color | [Color](Types.md#color) | The color of the fill. 
| opacity | long | The transparency level of histogram bars. 
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The properties of the fill symbol border. 





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
| useAutomaticTitle | boolean | A value indicating whether the chart title is auto generated. 
| subTitle | string | The subtitle of the chart. 
| showSubTitle | boolean | A value indicating whether the chart subtitle is visible. 
| footer | string | The footer of the chart. 
| showFooter | boolean | A value indicating whether the chart footer is visible. 
| theme | string | The theme of the chart. 
| titleText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The title symbol properties. 
| subTitleText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The subtitle symbol properties. 
| footerText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The footer symbol properties. 
| backgroundSymbolProperties | [CIMChartFillSymbolProperties](CIMCharts.md#cimchartfillsymbolproperties) | The background fill symbol properties for the chart. 
| gridLineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The line symbol properties for grid lines. 






## CIMChartGuide
#### Define the properties to define a chart guide. 


### CIMChartGuide 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name / title for the guide. 
| label | string | The label for the guide. 
| labelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text format for the guide label. 
| labelPosition | [enumeration ChartPosition](CIMCharts.md#enumeration-chartposition) | The relative position of the label to the guide. 
| valueFrom | double | The numeric coordinate of the from value for the guide. This value will be used when guide value type is set to numeric. 
| valueTo | double | The numeric coordinate of the to value for the guide. This value will be used when guide value type is set to numeric. 
| timeFrom | [TimeInstant](ExternalReferences.md#timeinstant) | The temporal coordinate of the from value for the guide. This value will be used when guide value type is set to temporal. 
| timeTo | [TimeInstant](ExternalReferences.md#timeinstant) | The temporal coordinate of the to value for the guide. This value will be used when guide value type is set to temporal. 
| visible | boolean | A value indicating whether the guide is visible. 
| guideType | [enumeration ChartGuideType](CIMCharts.md#enumeration-chartguidetype) | The type of the guide. 
| guideValueType | [enumeration ChartValueType](CIMCharts.md#enumeration-chartvaluetype) | The type of the coordinate value used in the guide. 
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMCharts.md#cimchartfillsymbolproperties) | The symbol properties for the guide. 





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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartHistogramSeries 

|Property | Type | Description | 
|---------|--------|--------|
| binCount | long | The number of bins in classifying input values. 
| showMean | boolean | A value indicating whether to show the mean line on the histogram. 
| showMedian | boolean | A value indicating whether to show the median line on a histogram. 
| showStandardDeviation | boolean | A value indicating whether to show the standard deviation band on the histogram. 
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMCharts.md#cimchartfillsymbolproperties) | The properties of the fill symbol border. 
| meanLineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The mean line symbol properties of the line series. 
| medianLineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The median line symbol properties of the line series. 
| standardDeviationLineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The line symbol for the standard deviation. 
| showComparisonDistribution | boolean | A value indicating whether to show a comparison distribution line overlay for the histogram chart. 
| dataTransformationType | [enumeration ChartDataTransformationType](CIMCharts.md#enumeration-chartdatatransformationtype) | The type of a data transformation to apply before calculating histogram bins and counts. 
| dataTransformationParameters | [double] | Parameters of a data transformation. 
| distributionLineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The line symbol for the comparison distribution. 
| countField | string | A raster attribute table count field in order to calculate a histogram and statistics for fields that have to be adjusted for counts. 






## CIMChartLegend
#### Provides access to members that control chart legend properties. 


### CIMChartLegend 

|Property | Type | Description | 
|---------|--------|--------|
| visible | boolean | A value indicating whether the chart legend is visible. 
| title | string | The title of the legend. 
| showTitle | boolean | A value indicating whether the legend title is visible. 
| alignment | [enumeration ChartLegendAlignment](CIMCharts.md#enumeration-chartlegendalignment) | The options in arranging the chart legend. 
| valueFormat | string | The format string for series value labels. 
| legendText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text symbol properties. 
| legendTitle | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text symbol properties for legend title. 





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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartLineSeries 

|Property | Type | Description | 
|---------|--------|--------|
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The line symbol properties of the line series. 
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMCharts.md#cimchartmarkersymbolproperties) | The marker symbol properties of the line series. 
| timeAggregationType | [enumeration ChartTimeAggregationType](CIMCharts.md#enumeration-charttimeaggregationtype) | The time aggregation type. 
| timeIntervalUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units used for the time interval size. 
| timeIntervalSize | double | The time interval size. 
| calculateAutomaticTimeInterval | boolean | A value indicating whether the time interval is automatically calculated. 
| trimIncompleteTimeInterval | boolean | A value indicating whether incomplete time intervals at the ends of time interval ranges are trimmed in order to avoid bias. 
| nullPolicy | [enumeration ChartNullPolicy](CIMCharts.md#enumeration-chartnullpolicy) | The policy for handling missing data. 
| verticalOrientation | boolean | A value indicating whether this is a vertical (true) or horizontal (false) orientation of a line series. 
| sortedCategoryValues | [string] | The array of sorted category values for custom sort. 






## CIMChartLineSymbolProperties
#### Provides access to members that control properties of the line symbol. 


### CIMChartLineSymbolProperties 

|Property | Type | Description | 
|---------|--------|--------|
| visible | boolean | A value indicating whether the line is visible. 
| width | double | The width of the line. 
| style | [enumeration ChartLineDashStyle](CIMCharts.md#enumeration-chartlinedashstyle) | The style of the line. 
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
| style | [enumeration ChartMarkerSymbolStyle](CIMCharts.md#enumeration-chartmarkersymbolstyle) | The style of the symbol. 
| color | [Color](Types.md#color) | The color of the symbol fill. 
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The properties of the symbol border. 





### Enumeration: ChartMarkerSymbolStyle
#### Chart marker symbol style. 

|Property | Value | Description | 
|---------|--------|--------|
| Circle| 0| Uses circle to draw the marker symbol. 
| Square| 1| Uses square to draw the marker symbol. 
| Diamond| 2| Uses diamond to draw the marker symbol. 
| Triangle| 3| Uses triangle to draw the marker symbol. 




## CIMChartMatrixHeatSeries
#### Provides access to members that control MatrixHeat series. 


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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartMatrixHeatSeries 

|Property | Type | Description | 
|---------|--------|--------|
| nullPolicy | [enumeration ChartNullPolicy](CIMCharts.md#enumeration-chartnullpolicy) | The policy for handling missing data. 
| noDataColor | [Color](Types.md#color) | Color properties for empty cells. 
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method with which breaks are created. 
| breaksCount | long | The number of breaks for automatic breaks creation. 
| minimumBreak | double | The lower bound of the first range. 
| breaks | [double] | The upper bound breaks. 
| breakColors | [[CIMColor]](Types.md#color) | The color for each break. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp from which break colors are created. 





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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartProbabilityPlotSeries 

|Property | Type | Description | 
|---------|--------|--------|
| probabilityPlotType | [enumeration ChartProbabilityPlotType](CIMCharts.md#enumeration-chartprobabilityplottype) | The type of a probability plot. 
| dataTransformationType | [enumeration ChartDataTransformationType](CIMCharts.md#enumeration-chartdatatransformationtype) | The type of data transformation to apply before calculating Normal Q-Q Plot. 
| dataTransformationParameters | [double] | Parameters of a data transformation. 
| showReferenceLine | boolean | A value indicating whether to show a reference line overlay for the probability plot. 
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMCharts.md#cimchartmarkersymbolproperties) | The marker symbol properties of the probability plot series. 
| referenceLineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The line symbol properties of the probability plot series' reference line. 





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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartProfileGraphSeries 

|Property | Type | Description | 
|---------|--------|--------|
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The line symbol properties of the profile graph series. 
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMCharts.md#cimchartmarkersymbolproperties) | The marker symbol properties of the profile graph series. 
| horizontalUnit | [Unit](ExternalReferences.md#unit) | The unit of measure to be used for horizontal distance. The default value is layer's spatial reference XY unit. 
| verticalUnit | [Unit](ExternalReferences.md#unit) | The the unit of measure to be used for elevation. The default value is the layer's vertical coordinate system's Z unit, if there is one. 





### Enumeration: ChartSPMDiagonalOption
#### Scatter plot matrix diagonal display options. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Display nothing in the diagonal. 
| Histogram| 1| Display the histogram in the diagonal. 
| FieldName| 2| Display the field names in the diagonal. 



### Enumeration: ChartSPMDisplayOption
#### Scatter plot matrix display options. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Display nothing in the other half. 
| PreviewPlot| 1| Display the zoomed-in preview plot in the other half. 
| ScatterPlots| 2| Display the mirrored scatter plots in the other half. 
| RSquared| 3| Display the R squared values in the other half. 
| PearsonsR| 4| Display the Pearson's R values in the other half. 



### Enumeration: ChartSPMSortByType
#### Scatter plot matrix sort-by type. 

|Property | Value | Description | 
|---------|--------|--------|
| RSquared| 0| Sort by R Squared value. 
| PearsonsR| 1| Sort by Pearson's R value. 
| Alphabetical| 2| Sort by alphabetical value. 
| Custom| 3| Sort by custom order. 




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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartScatterPlotMatrixSeries 

|Property | Type | Description | 
|---------|--------|--------|
| showHistograms | boolean | A value indicating whether to show histograms for all fields. Deprecated at 2.8. Use DiagonalOption instead. 
| showTrendLine | boolean | A value indicating whether to show a trend line overlay for all scatter plots. 
| showAsRSquared | boolean | A value indicating whether show scatter plots as R squared values. Deprecated at 2.8. Use LowerLeftDisplayOption instead. 
| fieldLabels | [string] | The labels for scatter plot and histogram series' axes. 
| scatterMarkerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMCharts.md#cimchartmarkersymbolproperties) | The marker symbol properties of scatter plot series. 
| trendLineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The line symbol properties of the scatter plot series' trend line. 
| histogramFillSymbolProperties | [CIMChartFillSymbolProperties](CIMCharts.md#cimchartfillsymbolproperties) | The fill symbol properties of histograms. 
| selectedMiniPlot | long | The index of the selected mini plot (-1 stands for non selected, -2 for uninitialized). 
| RSquareText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text symbol properties for the RSquare. 
| selectionLineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The line symbol properties of the selection line for the mini plot. 
| displayOption | [enumeration ChartSPMDisplayOption](CIMCharts.md#enumeration-chartspmdisplayoption) | The display option for the upper right of the scatter plot matrix. 
| lowerLeftDisplayOption | [enumeration ChartSPMDisplayOption](CIMCharts.md#enumeration-chartspmdisplayoption) | The display option for the lower left of the scatter plot matrix. PreviewPlot currently is not supported in lower left. 
| lowerLeftColorRamp | [ColorRamp](Types.md#colorramp) | The color ramp for the lower left when RSquared or Pearson's R is selected. 
| lowerLeftBreakColors | [[CIMColor]](Types.md#color) | The color for each break in the lower left. 
| upperRightColorRamp | [ColorRamp](Types.md#colorramp) | The color ramp for the upper right when RSquared or Pearson's R is selected. 
| upperRightBreakColors | [[CIMColor]](Types.md#color) | The color for each break in the upper right. 
| diagonalOption | [enumeration ChartSPMDiagonalOption](CIMCharts.md#enumeration-chartspmdiagonaloption) | The display option for the diagonal. 
| sortByType | [enumeration ChartSPMSortByType](CIMCharts.md#enumeration-chartspmsortbytype) | The sort by type. 
| sortDirection | [enumeration ChartSortDirection](CIMCharts.md#enumeration-chartsortdirection) | The direction type of sort order. 






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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartScatterSeries 

|Property | Type | Description | 
|---------|--------|--------|
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMCharts.md#cimchartmarkersymbolproperties) | The marker symbol properties of the point series. 
| showTrendLine | boolean | A value indicating whether to show the trend line or not. 
| trendLineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The symbol properties for the trend line symbol. 
| trendLineFitType | [enumeration ChartTrendLineFitType](CIMCharts.md#enumeration-charttrendlinefittype) | A trend line fit type. 
| trendOrder | long | The number of terms in a polynomial or Fourier equation. 
| showTrendEquation | boolean | A value indicating whether or not to have a trend equation overlay. 
| bubbleMinimumSize | double | Minimum size of the bubbles. 
| bubbleMaximumSize | double | Maximum size of the bubbles. 





### Enumeration: ChartSortDirection
#### Chart sort direction. 

|Property | Value | Description | 
|---------|--------|--------|
| Ascending| 0| Ascending sort. 
| Descending| 1| Descending sort. 




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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartSpectralProfileSeries 

|Property | Type | Description | 
|---------|--------|--------|
| displayMode | [enumeration SpectralProfileDisplayMode](CIMCharts.md#enumeration-spectralprofiledisplaymode) | How this spectral profile is displayed. 
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
| bands | [[CIMChartTemporalProfileBand]](CIMCharts.md#cimcharttemporalprofileband) | The bands for a variable to be plotted. 






## CIMChartTemporalProfileCCDCArguments
#### Represents arguments to be used to plot change detection over time. 


### CIMChartTemporalProfileCCDCArguments 

|Property | Type | Description | 
|---------|--------|--------|
| bands | [[CIMChartTemporalProfileBand]](CIMCharts.md#cimcharttemporalprofileband) | The bands to be used for change detection. 
| temporalMaskBandIDs | [long] | The bandIDs for temporal masking. 
| updatingFrequency | double | The frequency in years at which to update the time series model with new observations. 
| chiSquaredThreshold | double | The chi squared statictic change probablity threshold. 
| minimumAnomaly | long | The minimum number of consecutive anomaly observations that must occur before an event is considered a change. 






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
| values | [[CIMChartTemporalProfileDimensionValue]](CIMCharts.md#cimcharttemporalprofiledimensionvalue) | Dimension values for a variable to be plotted. 






## CIMChartTemporalProfileLandTrendRArguments
#### Represents arguments to be used to plot change detection over time. 


### CIMChartTemporalProfileLandTrendRArguments 

|Property | Type | Description | 
|---------|--------|--------|
| band | [CIMChartTemporalProfileBand](CIMCharts.md#cimcharttemporalprofileband) | The the band to use for segmenting the pixel value trajectories over time. 
| snappingDate | string | The date in the format MM-DD used to select a slice for each year. 
| maximumSegments | long | The maximum number of segments to be fitted to the time series for each pixel. 
| vertexCountOvershoot | long | The the number of additional vertices beyond MaximumSegments + 1 that can be used to fit the model during the initial stage of identifying vertices. 
| spikeThreshold | double | The threshold to use for dampening spikes or anomalies in the pixel value trajectory. 
| recoveryThreshold | double | The recovery threshold value in years. 
| preventOneYearRecovery | boolean | A value indicating whether segments that exhibit a one year recovery will be excluded. 
| recoveryIncreasingTrend | boolean | A value indicating whether the recovery has an increasing (positive) trend. 
| outputOtherBands | boolean | A value indicating whether other bands will be included in the segmentation process. 
| minimumObservations | long | The minimum number of valid observations required to perform fitting. 
| bestModelProportion | double | The best model proportion value. 
| PValueThreshold | double | The p-value threshold for a model to be selected. 





### Enumeration: ChartTemporalProfilePlotType
#### Represents the temporal profile plot type. 

|Property | Value | Description | 
|---------|--------|--------|
| Variables| 0| Plot of multiple variables over time at a location. 
| Bands| 1| Plot of multiple bands of a variable over time at a location. 
| DimensionValues| 2| Plot of a variable with specific dimension values over time at multiple locations. 
| Variable| 3| Plot of one variable over time at multiple locations. 
| Band| 4| Plot of one band of a variable over time at multiple locations. 
| CCDC| 5| Plot of the result of CCDC analysis over one or more bands. 
| LandTrendR| 6| Plot of the result of LandTrendR analysis over one band. 




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
| colorType | [enumeration ChartColorType](CIMCharts.md#enumeration-chartcolortype) | The type of color for the series. 
| fieldAggregation | [string] | The aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long] | The array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending). 
| visible | boolean | A value indicating whether the series is visible or not. 
| dataLabelText | [CIMChartTextProperties](CIMCharts.md#cimcharttextproperties) | The text style for the data label. 
| multiSeries | boolean | A value indicating whether this series is a multi series. 
| locations | [[CIMChartLocationDefinition]](CIMCharts.md#cimchartlocationdefinition) | The locations for which data is to be plotted. 


### CIMChartTemporalProfileSeries 

|Property | Type | Description | 
|---------|--------|--------|
| plotType | [enumeration ChartTemporalProfilePlotType](CIMCharts.md#enumeration-charttemporalprofileplottype) | The type of plot for this chart. 
| variables | [[CIMChartTemporalProfileVariable]](CIMCharts.md#cimcharttemporalprofilevariable) | The variables to be plotted over time. 
| bands | [CIMChartTemporalProfileBands](CIMCharts.md#cimcharttemporalprofilebands) | The bands for a variable to be plotted over time. 
| dimensionValues | [CIMChartTemporalProfileDimensionValues](CIMCharts.md#cimcharttemporalprofiledimensionvalues) | The dimension values for a variable to be plotted over time. 
| standardizeValues | boolean | A value indicating whether to calculate standardized values. 
| timeIntervalSize | double | The interval size for the time plotted on the x axis. 
| timeIntervalUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The unit of time for the interval size. 
| timeAggregationType | [enumeration ChartTimeAggregationType](CIMCharts.md#enumeration-charttimeaggregationtype) | The type of grouping to be applied on the time values plotted on the x axis. 
| trimIncompleteTimeInterval | boolean | A value indicating whether incomplete time intervals at the ends of time interval ranges are trimmed in order to avoid bias. 
| dateTimeFormat | string | The format of the date plotted on the x axis. 
| trendLineSymbolProperties | [CIMChartLineSymbolProperties](CIMCharts.md#cimchartlinesymbolproperties) | The symbol properties for the trend line. 
| showTrendLine | boolean | A value indicating whether to show the trend line or not. 
| trendLineFitType | [enumeration ChartTrendLineFitType](CIMCharts.md#enumeration-charttrendlinefittype) | A trend line fit type. 
| trendOrder | long | The order of the equation when a polynomial or Fourier fit type is used. 
| showTrendEquation | boolean | A value indicating whether or not to have a trend equation overlay. 
| spatialAggregationType | [enumeration ChartAggregationType](CIMCharts.md#enumeration-chartaggregationtype) | The spatial aggregation type to be used to calculate cell values. 
| CCDCArguments | [CIMChartTemporalProfileCCDCArguments](CIMCharts.md#cimcharttemporalprofileccdcarguments) | The CCDC options. 
| landTrendRArguments | [CIMChartTemporalProfileLandTrendRArguments](CIMCharts.md#cimcharttemporalprofilelandtrendrarguments) | The LandTrendR options. 
| timeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The time extent used by the chart. 






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
| dimensionValuesSymbols | [[CIMSymbolReference]](CIMRenderers.md#cimsymbolreference) | The symbols for dimension values. 





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
| fontWeight | [enumeration ChartFontWeight](CIMCharts.md#enumeration-chartfontweight) | The font weight. 
| textCase | [enumeration ChartTextCase](CIMCharts.md#enumeration-charttextcase) | The text case. 
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




## CIMGridChartProperties
#### Provides access to members that control grid chart properties. 


### CIMMultiSeriesChartProperties 

|Property | Type | Description | 
|---------|--------|--------|
| enabled | boolean | A value indicating whether multi series chart properties are enabled. 


### CIMGridChartProperties 

|Property | Type | Description | 
|---------|--------|--------|
| miniChartsPerRow | long | The number of mini charts per row of a grid chart. 
| selectedMiniChart | long | The index of the selected mini chart. 
| showPreviewChart | boolean | A value indicating whether to show a zoomed-in preview chart. 
| useSeriesMinMaxForAxisX | boolean | A value indicating whether each mini chart will use corresponding series' minimum and maximum of x values for axis X. If false it will use the combined series' minimum and maximum. 
| useSeriesMinMaxForAxisY | boolean | A value indicating whether each mini chart will use corresponding series' minimum and maximum of y values for axis Y. If false it will use the combined series' minimum and maximum. 






## CIMMultiSeriesChartProperties
#### Provides access to members that control multi series chart properties. 


### CIMMultiSeriesChartProperties 

|Property | Type | Description | 
|---------|--------|--------|
| enabled | boolean | A value indicating whether multi series chart properties are enabled. 





### Enumeration: SpectralProfileDisplayMode
#### Spectral profile display modes. 

|Property | Value | Description | 
|---------|--------|--------|
| MeanLine| 0| Show spectral profile as line joining mean values of each raster band. 
| Boxes| 1| Show spectral profile as a series of boxes for each raster band. 
| BoxesAndMeanLine| 2| Show spectral profile as both a series of boxes for each raster band and lines joining mean values of each raster band. 
| ConsolidatedBoxesAndMeanLine| 3| Show spectral profile as both consolidated boxes for each raster band and lines joining mean values of each raster band. 

