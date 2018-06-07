


## CIM3DLayerProperties
#### Represents 3D layer properties which contain properties used for 3D draw. 


### CIM3DLayerProperties 

|Property | Type | Description | 
|---------|--------|--------|
| castShadows | boolean|Gets and sets a boolean value indicating if shadows are enabled. If true, this layer's features contribute to shadows. 
| isLayerLit | boolean|Gets and sets a boolean value indicating if this layer is lit. 
| layerFaceCulling | [enumeration FaceCulling3D](CIMEnumerations.md#enumeration-faceculling3d)|Gets and sets the layer's face culling setting. 
| maxDistance | double|Gets and sets the maximum distance at which objects in view are visible. Objects beyond this point don't get rendered. 
| maxPreloadDistance | double|Gets and sets the maximum radius from the camera at which objects outside the view are loaded. Values are in Meters. 
| minDistance | double|Gets and sets the minimum distance at which objects in view are visible. Objects closer than this don't get rendered. 
| minPreloadDistance | double|Gets and sets the minimum radius from the camera at which objects at which objects outside the view are loaded. Values are in Meters. 
| preloadTextureCutoffHigh | double|Gets and sets the distance (in visible range) at which high resolution textures change to low resolution textures for objects outside the view. Range is 0 to 1. 
| preloadTextureCutoffLow | double|Gets and sets the distance (in visible range) at which low resolution textures change to solid colors for objects outside the view. Range is 0 to 1. 
| textureCutoffHigh | double|Gets and sets the distance (in visible range) at which the high resolution textures change to low resolution textures. Range is 0 to 1. 
| textureCutoffLow | double|Gets and sets the distance (in visible range) at which the high resolution textures change to solid colors. Range is 0 to 1. 
| textureDownscalingFactor | long|Gets and sets the downscaling factor. All textures for this layer are downscaled by this additional factor on loading. 
| useCompressedTextures | boolean|Gets and sets a boolean value indicating if uncompressed textures are compressed using DXT5 at load time. 
| verticalExaggeration | double|Gets and sets the layer's vertical exaggeration. 
| verticalUnit | [Unit](ExternalReferences.md#unit)|Gets and sets the layer's vertical unit. 
| depthPriority | long|Gets and Sets the depth priority of a 3D layer. 
| lighting | [enumeration Lighting3D](CIMLayer.md#enumeration-lighting3d)|Gets and sets the layer's lighting setting. 
| optimizeMarkerTransparency | boolean|Gets and sets a boolean value indicating when true alpha is quantized to fully opaque or transparent When false, actual values are used in marker drawing. 
| useDepthWritingForTransparency | boolean|Gets and sets a boolean value indicating whether to use depth writing for transparency. This should be set to true if anomalies are seen in drawing order of transparent features in the same feature class. 






## CIMChart
#### Provides access to members that control chart properties. 


### CIMChart 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Name of the chart. 
| series | [CIMChartSeries](Types.md#cimchartseries) |Series properties of the chart. 
| generalProperties | [CIMChartGeneralProperties](CIMLayer.md#cimchartgeneralproperties)|General properties of the chart. 
| legend | [CIMChartLegend](CIMLayer.md#cimchartlegend)|Legend properties of the chart. 
| axes | [CIMChartAxis](CIMLayer.md#cimchartaxis) |Properties of chart axis. 
| mapSelectionHandling | [enumeration ChartMapSelectionHandling](CIMLayer.md#enumeration-chartmapselectionhandling)|Indicates whether chart handles selection in the input layer by creating series only from the selected data or highlights selected values on the chart made from entire dataset. 
| metaData | string|Client metadata about the chart. 






## CIMChartAxis
#### Provides access to members that control chart axis properties. 


### CIMChartAxis 

|Property | Type | Description | 
|---------|--------|--------|
| visible | boolean|Indicates whether the chart axis is visible. 
| isLogarithmic | boolean|Indicates whether the chart axis has logarithmic scale. 
| title | string|Title of an axis. 
| valueFormat | string|Format string for axis value labels. 
| valueNumberFormat | [NumberFormat](Types.md#numberformat)|Gets and sets the number format of the axis labels. ValueNumberFormat takes precedence over ValueFormat when both are specified. 
| dateTimeFormat | string|Format string for axis date/time labels. 
| calculateAutomaticMinimum | boolean|Indicates whether the chart axis calculates it's minimum. 
| calculateAutomaticMaximum | boolean|Indicates whether the chart axis calculates it's maximum. 
| minimum | VARIANT|Minimum of the axis. 
| maximum | VARIANT|Maximum of the axis. 
| titleText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties)|Title symbol properties. 
| labelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties)|Label symbol properties. 
| axisLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Gets and sets the line symbol properties for axis. 






## CIMChartBarSeries
#### Provides access to members that control bar chart series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Name of the series shown in the legend. 
| uniqueName | string|Default and unique name of the series. 
| fields | IStringArray|Data field names in the series. Optional depending on series type. 
| orderFields | IStringArray|Sort field names in the series. 
| groupFields | IStringArray|Groiup field names in the series. 
| whereClause | string|Format string for series value labels. 
| showLabels | boolean|Indicates if series shows data labels. 
| horizontalAxis | long|Index of horizontal axis. 
| verticalAxis | long|Index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series. 
| fieldAggregation | IStringArray|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending) 
| visible | boolean|Gets or sets the flag to indicate whether the series is visible or not 


### CIMChartBarSeries 

|Property | Type | Description | 
|---------|--------|--------|
| multipleBarType | [enumeration ChartMultiBarType](CIMLayer.md#enumeration-chartmultibartype)|Type of multiple bar-series chart. 
| barSize | long|Relative width of the bar. 
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties)|Properties of the fill symbol border. 
| verticalOrientation | boolean|Gets and sets whether this bar chart is vertically oriented. 






## CIMChartBoxPlotSeries
#### Provides access to members that control bar chart box plot series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Name of the series shown in the legend. 
| uniqueName | string|Default and unique name of the series. 
| fields | IStringArray|Data field names in the series. Optional depending on series type. 
| orderFields | IStringArray|Sort field names in the series. 
| groupFields | IStringArray|Groiup field names in the series. 
| whereClause | string|Format string for series value labels. 
| showLabels | boolean|Indicates if series shows data labels. 
| horizontalAxis | long|Index of horizontal axis. 
| verticalAxis | long|Index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series. 
| fieldAggregation | IStringArray|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending) 
| visible | boolean|Gets or sets the flag to indicate whether the series is visible or not 


### CIMChartBoxPlotSeries 

|Property | Type | Description | 
|---------|--------|--------|
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties)|Properties of the box plot symbol. 
| verticalOrientation | bool|Gets or sets the box plot vertical orientation flag. 
| showOutliers | bool|Gets or sets the flag indicating whether to show the box plot outliers. 
| showInnerPoints | bool|Gets or sets the flag indicating whether to show the box plot inner points. 
| showMean | bool|Gets or sets the flag indicating whether to show the box plot mean marker. 
| standardizeValues | bool|Gets or sets the flag indicating whether to calculate standardized values for box plot. 





### Enumeration: ChartColorType
#### Provides a type of coloring that chart series uses. 

|Property | Value | Description | 
|---------|--------|--------|
| SingleColor| 0| Uses a single color for series. 
| ColorMatch| 1| Matches series colors with the layer. 



### Enumeration: ChartDataTransformationType
#### Types of a data transformation to apply before calculating histogram bins and counts 

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
| color | [Color](Types.md#color)|Color of the fill. 
| opacity | long|Transparency level of histogram bars. 
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Properties of the fill symbol border. 





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
| title | string|Title of the chart. 
| subTitle | string|Subtitle of the chart. 
| footer | string|Footer of the chart. 
| theme | string|Theme of the chart. 
| titleText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties)|Title symbol properties. 
| subTitleText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties)|Subtitle symbol properties. 
| footerText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties)|Footer symbol properties. 
| backgroundSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties)|Gets and sets the background fill symbol properties for the chart. 
| gridLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Gets and sets the line symbol properties for grid lines. 






## CIMChartHistogramSeries
#### Provides access to members that control histogram series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Name of the series shown in the legend. 
| uniqueName | string|Default and unique name of the series. 
| fields | IStringArray|Data field names in the series. Optional depending on series type. 
| orderFields | IStringArray|Sort field names in the series. 
| groupFields | IStringArray|Groiup field names in the series. 
| whereClause | string|Format string for series value labels. 
| showLabels | boolean|Indicates if series shows data labels. 
| horizontalAxis | long|Index of horizontal axis. 
| verticalAxis | long|Index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series. 
| fieldAggregation | IStringArray|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending) 
| visible | boolean|Gets or sets the flag to indicate whether the series is visible or not 


### CIMChartHistogramSeries 

|Property | Type | Description | 
|---------|--------|--------|
| binCount | long|Number of bins in classifying input values. 
| showMean | boolean|Show the mean line on the histogram. 
| showMedian | boolean|Show the median line on a histogram. 
| showStandardDeviation | boolean|Show the standard deviation band on the histogram. 
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties)|Properties of the fill symbol border. 
| meanLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Mean line symbol properties of the line series. 
| medianLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Median line symbol properties of the line series. 
| standardDeviationFillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties)|Properties of the fill symbol border. 
| showComparisonDistribution | boolean|Show comparison distribution line overlay for the histogram chart. 
| dataTransformationType | [enumeration ChartDataTransformationType](CIMLayer.md#enumeration-chartdatatransformationtype)|Gets or sets the type of a data transformation to apply before calculating histogram bins and counts. 






## CIMChartLegend
#### Provides access to members that control chart legend properties. 


### CIMChartLegend 

|Property | Type | Description | 
|---------|--------|--------|
| visible | boolean|Indicates if chart legend is visible. 
| title | string|Title of the legend. 
| alignment | [enumeration ChartLegendAlignment](CIMLayer.md#enumeration-chartlegendalignment)|Options in arranging chart legend. 
| valueFormat | string|Format string for series value labels. 
| legendText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties)|Text symbol properties. 





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
| name | string|Name of the series shown in the legend. 
| uniqueName | string|Default and unique name of the series. 
| fields | IStringArray|Data field names in the series. Optional depending on series type. 
| orderFields | IStringArray|Sort field names in the series. 
| groupFields | IStringArray|Groiup field names in the series. 
| whereClause | string|Format string for series value labels. 
| showLabels | boolean|Indicates if series shows data labels. 
| horizontalAxis | long|Index of horizontal axis. 
| verticalAxis | long|Index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series. 
| fieldAggregation | IStringArray|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending) 
| visible | boolean|Gets or sets the flag to indicate whether the series is visible or not 


### CIMChartLineSeries 

|Property | Type | Description | 
|---------|--------|--------|
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Line symbol properties of the line series. 
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties)|Marker symbol properties of the line series. 
| timeAggregationType | [enumeration ChartTimeAggregationType](CIMLayer.md#enumeration-charttimeaggregationtype)|Gets and sets the time aggregation type. 
| timeIntervalUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|Gets and sets the units used for the time interval size. 
| timeIntervalSize | double|Gets and sets the time interval size. 
| trimIncompleteTimeInterval | boolean|Gets and sets whether incomplete time intervals at the ends of time interval ranges are trimmed in order to avoid bias. 
| nullPolicy | [enumeration ChartNullPolicy](CIMLayer.md#enumeration-chartnullpolicy)|Gets and sets the policy for handling null values. 






## CIMChartLineSymbolProperties
#### Provides access to members that control properties of the line symbol. 


### CIMChartLineSymbolProperties 

|Property | Type | Description | 
|---------|--------|--------|
| visible | boolean|Indicates if line is visible. 
| width | double|Width of the line. 
| style | [enumeration ChartLineDashStyle](CIMLayer.md#enumeration-chartlinedashstyle)|Style of the line. 
| color | [Color](Types.md#color)|Color of the line. 





### Enumeration: ChartMapSelectionHandling
#### Provides a choice of how map selection is processed in the chart. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Do not handle map selection. 
| Highlight| 1| Highlight selection set on a chart. 
| BuildFromSelectionSet| 2| Build a chart exclusively from the selection set. 




## CIMChartMarkerSymbolProperties
#### Provides access to members that control properties of the marker symbol 


### CIMChartMarkerSymbolProperties 

|Property | Type | Description | 
|---------|--------|--------|
| visible | boolean|Indicates if symbol is visible. 
| width | double|Width of the symbol. 
| height | double|Height of the symbol. 
| style | [enumeration ChartMarkerSymbolStyle](CIMLayer.md#enumeration-chartmarkersymbolstyle)|Style of the symbol. 
| color | [Color](Types.md#color)|Color of the symbol fill. 
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Properties of the symbol border. 





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




## CIMChartProbabilityPlotSeries
#### Provides access to members that control probability plot series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Name of the series shown in the legend. 
| uniqueName | string|Default and unique name of the series. 
| fields | IStringArray|Data field names in the series. Optional depending on series type. 
| orderFields | IStringArray|Sort field names in the series. 
| groupFields | IStringArray|Groiup field names in the series. 
| whereClause | string|Format string for series value labels. 
| showLabels | boolean|Indicates if series shows data labels. 
| horizontalAxis | long|Index of horizontal axis. 
| verticalAxis | long|Index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series. 
| fieldAggregation | IStringArray|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending) 
| visible | boolean|Gets or sets the flag to indicate whether the series is visible or not 


### CIMChartProbabilityPlotSeries 

|Property | Type | Description | 
|---------|--------|--------|
| probabilityPlotType | [enumeration ChartProbabilityPlotType](CIMLayer.md#enumeration-chartprobabilityplottype)|Gets or sets the type of a probability plot. 
| dataTransformationType | [enumeration ChartDataTransformationType](CIMLayer.md#enumeration-chartdatatransformationtype)|Gets or sets the type of data transformation to apply before calculating Normal Q-Q Plot. 
| showReferenceLine | boolean|Shows or hides a reference line overlay for the probability plot. 
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties)|Gets or sets the marker symbol properties of the probability plot series. 
| referenceLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Gets or sets the line symbol properties of the probability plot series' reference line. 





### Enumeration: ChartProbabilityPlotType
#### 

|Property | Value | Description | 
|---------|--------|--------|
| NormalQQPlot| 0| Normal Q-Q plot. 
| QQPlot| 1| General Q-Q plot. 




## CIMChartProfileGraphSeries
#### Provides access to members that control profile graph series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Name of the series shown in the legend. 
| uniqueName | string|Default and unique name of the series. 
| fields | IStringArray|Data field names in the series. Optional depending on series type. 
| orderFields | IStringArray|Sort field names in the series. 
| groupFields | IStringArray|Groiup field names in the series. 
| whereClause | string|Format string for series value labels. 
| showLabels | boolean|Indicates if series shows data labels. 
| horizontalAxis | long|Index of horizontal axis. 
| verticalAxis | long|Index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series. 
| fieldAggregation | IStringArray|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending) 
| visible | boolean|Gets or sets the flag to indicate whether the series is visible or not 


### CIMChartProfileGraphSeries 

|Property | Type | Description | 
|---------|--------|--------|
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Line symbol properties of the profile graph series. 
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties)|Marker symbol properties of the profile graph series. 
| horizontalUnit | [Unit](ExternalReferences.md#unit)|The unit of measure to be used for horizontal distance. The default value is layer's spatial reference XY unit. 
| verticalUnit | [Unit](ExternalReferences.md#unit)|The unit of measure to be used for elevation. The default value is the layer's vertical coordinate system's Z unit, if there is one. 






## CIMChartScatterSeries
#### Provides access to members that control point chart series. 


### CIMChartSeries 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Name of the series shown in the legend. 
| uniqueName | string|Default and unique name of the series. 
| fields | IStringArray|Data field names in the series. Optional depending on series type. 
| orderFields | IStringArray|Sort field names in the series. 
| groupFields | IStringArray|Groiup field names in the series. 
| whereClause | string|Format string for series value labels. 
| showLabels | boolean|Indicates if series shows data labels. 
| horizontalAxis | long|Index of horizontal axis. 
| verticalAxis | long|Index of vertical axis. 
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series. 
| fieldAggregation | IStringArray|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string. 
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending) 
| visible | boolean|Gets or sets the flag to indicate whether the series is visible or not 


### CIMChartScatterSeries 

|Property | Type | Description | 
|---------|--------|--------|
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties)|Marker symbol properties of the point series. 
| showTrendLine | boolean|Defines whether to show the trend line or not. 
| trendLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Defines the style for the trend line symbol. 





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
| fontFillColor | [Color](Types.md#color)|Gets or sets the fill color for the font. 
| fontOutlineColor | [Color](Types.md#color)|Gets or sets the outline color for the font. 
| fontFamilyName | string|Gets or sets the font family name. 
| fontItalic | bool|Gets or sets the font style if it is italic or not. 
| fontSize | double|Gets or sets the font size in points. 
| fontWeight | [enumeration ChartFontWeight](CIMLayer.md#enumeration-chartfontweight)|Gets or sets the font weight. 
| textCase | [enumeration ChartTextCase](CIMLayer.md#enumeration-charttextcase)|Gets or sets the text case. 
| textUnderline | bool|Gets or sets the text underline. 
| textStrikethrough | bool|Gets or sets the text strikethrough. 
| textOverline | bool|Gets or sets the text overline. 





### Enumeration: ChartTimeAggregationType
#### Options for choosing how time intervals are built for the aggregation of a time based X-axis field. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No time aggregation is performed. 
| EqualIntervalsFromStartTime| 1| Time intervals start with the first (earliest) data point. 
| EqualIntervalsFromEndTime| 2| Time intervals start with the last (latest) data point. 
| CalendarIntervals| 3| Time intervals follow calendar breaks. 




## CIMCompositeSubLayer
#### Represents a composite sublayer. 


### CIMSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| expanded | boolean|Gets and sets whether this layer is expanded in the contents pane. 
| maxScale | double|Gets and sets the maximum scale for layer draw (set as the denominator of the scale's representative fraction) 
| minScale | double|Gets and sets the minimum scale for layer draw (set as the denominator of the scale's representative fraction) 
| name | string|Gets and sets the name. 
| showLegends | boolean|Gets and sets a boolean indicating whether or not to show legends. 
| subLayerID | string|Gets and sets the sublayer ID. 
| visibility | boolean|Gets and sets a boolean indicating whether or not this layer is visibile. 
| serviceLayerID | long|Gets and sets identifier that will be used to identify the layer in server 


### CIMCompositeSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) |Gets and sets the composite sublayers. 





### Enumeration: DisplayCacheType
#### Display cache types. 

|Property | Value | Description | 
|---------|--------|--------|
| Permanent| 0| Cache is permanent. 
| InSession| 1| Cache is maintained in session. 
| None| 2| No cache. 
| MaxAge| 3| Cache expires when it reaches the set max age. 




## CIMGroupLayer
#### Represents a group layer which is a simple ordered collection of other layers. 


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


### CIMGroupLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| layers | IStringArray|Gets and sets the paths of the layers in the group layer. 
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing)|Gets and sets the symbol layer drawing definition. 






## CIMKMLDataConnection
#### Represents a KML data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMKMLDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| KMLURI | string|Gets and sets the URI of the KML file or resource. 






## CIMKMLLayer
#### Represents a KML layer. 


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


### CIMKMLLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [CIMKMLDataConnection](CIMLayer.md#cimkmldataconnection)|Gets and sets the data connection to the KML resource. 
| selectable | boolean|Gets and sets a boolean option indicating whether the layer is selectable. 
| selectionColor | [Color](Types.md#color)|Gets and sets the selection color. 
| useSelectionColor | boolean|Gets and sets a boolean option indicating whether to use the selection color. 
| labelVisibility | boolean|Gets and sets a boolean option indicating whether to display labels for this KML layer's placemarks. 
| textSymbol | [CIMTextSymbol](CIMSymbols.md#cimtextsymbol)|Gets and sets the text symbol used to label placemarks. 






## CIMLayerElevationSurface
#### Represents a layer elevation surface. 


### CIMLayerElevationSurface 

|Property | Type | Description | 
|---------|--------|--------|
| offsetZ | double|Gets and sets Z offset. 
| mapElevationID | string|Gets and sets the map elevation ID. 






## CIMLayerTemplate
#### Represents a layer template. 


### CIMLayerTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string|Gets and sets the layer template URI. 
| layerTemplateId | string|Gets and sets the layer template ID. 
| parameters | {JSON_object}|Gets and sets the layer template parameters. 





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
| Descending| 1| Sort decending. 




## CIMSubLayer
#### Represents sublayer. Defines a sublayer for a containing parent layer. The parent layer is a full-fledged layer, and it controls the sublayer, which is subordinate to the parent. The sublayer is not a layer definition itself rather, it is a property of its parent layer. 


### CIMSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| description | string|Gets and sets the description. 
| expanded | boolean|Gets and sets whether this layer is expanded in the contents pane. 
| maxScale | double|Gets and sets the maximum scale for layer draw (set as the denominator of the scale's representative fraction) 
| minScale | double|Gets and sets the minimum scale for layer draw (set as the denominator of the scale's representative fraction) 
| name | string|Gets and sets the name. 
| showLegends | boolean|Gets and sets a boolean indicating whether or not to show legends. 
| subLayerID | string|Gets and sets the sublayer ID. 
| visibility | boolean|Gets and sets a boolean indicating whether or not this layer is visibile. 
| serviceLayerID | long|Gets and sets identifier that will be used to identify the layer in server 






## CIMSymbolLayerDrawing
#### Represents symbol layer drawing properties. 


### CIMSymbolLayerDrawing 

|Property | Type | Description | 
|---------|--------|--------|
| symbolLayers | [CIMSymbolLayerIdentifier](CIMLayer.md#cimsymbollayeridentifier) |Gets and sets the symbol layer identifiers. 
| useSymbolLayerDrawing | boolean|Gets and sets a boolean value indicating if symbol layer drawing is enabled. 






## CIMSymbolLayerIdentifier
#### Represents symbol layer identifier. 


### CIMSymbolLayerIdentifier 

|Property | Type | Description | 
|---------|--------|--------|
| symbolLayerName | string|Gets and sets the symbol layer name. 






## CIMTopologyLayer
#### Represents a topology dataset as a layer and draws its errors, exceptions, and areas in need of validation. 


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


### CIMTopologyLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| allLayers | IStringArray|Gets and sets the paths of the layers in the topology layer. 
| topologyConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the topology data connection. 



