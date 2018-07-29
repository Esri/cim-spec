


## CIM3DLayerProperties
Represents 3D layer properties which contain properties used for 3D draw.


### CIM3DLayerProperties

|Property | Type | Description |
|---------|--------|--------|
| castShadows | boolean|A boolean value indicating if shadows are enabled. If true, this layer's features contribute to shadows.
| isLayerLit | boolean|A boolean value indicating if this layer is lit.
| layerFaceCulling | [enumeration FaceCulling3D](CIMEnumerations.md#enumeration-faceculling3d)|The layer's face culling setting.
| maxDistance | number //double|The maximum distance at which objects in view are visible. Objects beyond this point don't get rendered.
| maxPreloadDistance | number //double|The maximum radius from the camera at which objects outside the view are loaded. Values are in Meters.
| minDistance | number //double|The minimum distance at which objects in view are visible. Objects closer than this don't get rendered.
| minPreloadDistance | number //double|The minimum radius from the camera at which objects at which objects outside the view are loaded. Values are in Meters.
| preloadTextureCutoffHigh | number //double|The distance (in visible range) at which high resolution textures change to low resolution textures for objects outside the view. Range is 0 to 1.
| preloadTextureCutoffLow | number //double|The distance (in visible range) at which low resolution textures change to solid colors for objects outside the view. Range is 0 to 1.
| textureCutoffHigh | number //double|The distance (in visible range) at which the high resolution textures change to low resolution textures. Range is 0 to 1.
| textureCutoffLow | number //double|The distance (in visible range) at which the high resolution textures change to solid colors. Range is 0 to 1.
| textureDownscalingFactor | number //int32|The downscaling factor. All textures for this layer are downscaled by this additional factor on loading.
| useCompressedTextures | boolean|A boolean value indicating if uncompressed textures are compressed using DXT5 at load time.
| verticalExaggeration | number //double|The layer's vertical exaggeration.
| verticalUnit | [Unit](ExternalReferences.md#unit)|The layer's vertical unit.
| depthPriority | number //int32|The depth priority of a 3D layer.
| lighting | [enumeration Lighting3D](CIMLayer.md#enumeration-lighting3d)|The layer's lighting setting.
| optimizeMarkerTransparency | boolean|A boolean value indicating when true alpha is quantized to fully opaque or transparent When false, actual values are used in marker drawing.
| useDepthWritingForTransparency | boolean|A boolean value indicating whether to use depth writing for transparency. This should be set to true if anomalies are seen in drawing order of transparent features in the same feature class.






## CIMChart
Provides access to members that control chart properties.


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
Provides access to members that control chart axis properties.


### CIMChartAxis

|Property | Type | Description |
|---------|--------|--------|
| visible | boolean|Indicates whether the chart axis is visible.
| isLogarithmic | boolean|Indicates whether the chart axis has logarithmic scale.
| title | string|Title of an axis.
| valueFormat | string|Format string for axis value labels.
| valueNumberFormat | [NumberFormat](Types.md#numberformat)|The number format of the axis labels. ValueNumberFormat takes precedence over ValueFormat when both are specified.
| dateTimeFormat | string|Format string for axis date/time labels.
| calculateAutomaticMinimum | boolean|Indicates whether the chart axis calculates it's minimum.
| calculateAutomaticMaximum | boolean|Indicates whether the chart axis calculates it's maximum.
| minimum | VARIANT|Minimum of the axis.
| maximum | VARIANT|Maximum of the axis.
| titleText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties)|Title symbol properties.
| labelText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties)|Label symbol properties.
| axisLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|The line symbol properties for axis.






## CIMChartBarSeries
Provides access to members that control bar chart series.


### CIMChartSeries

|Property | Type | Description |
|---------|--------|--------|
| name | string|Name of the series shown in the legend.
| uniqueName | string|Default and unique name of the series.
| fields | [string,]|Data field names in the series. Optional depending on series type.
| orderFields | [string,]|Sort field names in the series.
| groupFields | [string,]|Groiup field names in the series.
| whereClause | string|Format string for series value labels.
| showLabels | boolean|Indicates if series shows data labels.
| horizontalAxis | number //int32|Index of horizontal axis.
| verticalAxis | number //int32|Index of vertical axis.
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series.
| fieldAggregation | [string,]|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string.
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending)
| visible | boolean|The flag to indicate whether the series is visible or not


### CIMChartBarSeries

|Property | Type | Description |
|---------|--------|--------|
| multipleBarType | [enumeration ChartMultiBarType](CIMLayer.md#enumeration-chartmultibartype)|Type of multiple bar-series chart.
| barSize | number //int32|Relative width of the bar.
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties)|Properties of the fill symbol border.
| verticalOrientation | boolean|A boolean indicating whether this bar chart is vertically oriented.






## CIMChartBoxPlotSeries
Provides access to members that control bar chart box plot series.


### CIMChartSeries

|Property | Type | Description |
|---------|--------|--------|
| name | string|Name of the series shown in the legend.
| uniqueName | string|Default and unique name of the series.
| fields | [string,]|Data field names in the series. Optional depending on series type.
| orderFields | [string,]|Sort field names in the series.
| groupFields | [string,]|Groiup field names in the series.
| whereClause | string|Format string for series value labels.
| showLabels | boolean|Indicates if series shows data labels.
| horizontalAxis | number //int32|Index of horizontal axis.
| verticalAxis | number //int32|Index of vertical axis.
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series.
| fieldAggregation | [string,]|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string.
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending)
| visible | boolean|The flag to indicate whether the series is visible or not


### CIMChartBoxPlotSeries

|Property | Type | Description |
|---------|--------|--------|
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties)|Properties of the box plot symbol.
| verticalOrientation | boolean|The box plot vertical orientation flag.
| showOutliers | boolean|The flag indicating whether to show the box plot outliers.
| showInnerPoints | boolean|The flag indicating whether to show the box plot inner points.
| showMean | boolean|The flag indicating whether to show the box plot mean marker.
| standardizeValues | boolean|The flag indicating whether to calculate standardized values for box plot.





### Enumeration: ChartColorType
Provides a type of coloring that chart series uses.

|Property | Value | Description |
|---------|--------|--------|
| SingleColor| 0| Uses a single color for series.
| ColorMatch| 1| Matches series colors with the layer.



### Enumeration: ChartDataTransformationType
Types of a data transformation to apply before calculating histogram bins and counts

|Property | Value | Description |
|---------|--------|--------|
| None| 0| No data transformations.
| Logarithmic| 1| Apply logarithmic data transformation.
| SquareRoot| 2| Apply square root for data transformation.




## CIMChartFillSymbolProperties
Provides access to members that control properties of the fill symbol.


### CIMChartFillSymbolProperties

|Property | Type | Description |
|---------|--------|--------|
| color | [Color](Types.md#color)|Color of the fill.
| opacity | number //int32|Transparency level of histogram bars.
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Properties of the fill symbol border.





### Enumeration: ChartFontWeight
Chart font weight types.

|Property | Value | Description |
|---------|--------|--------|
| Lighter| 0| Defines lighter characters.
| Normal| 1| Defines normal characters.
| Bold| 2| Defines bold characters.




## CIMChartGeneralProperties
Provides access to members that control general chart properties.


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
| backgroundSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties)|The background fill symbol properties for the chart.
| gridLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|The line symbol properties for grid lines.






## CIMChartHistogramSeries
Provides access to members that control histogram series.


### CIMChartSeries

|Property | Type | Description |
|---------|--------|--------|
| name | string|Name of the series shown in the legend.
| uniqueName | string|Default and unique name of the series.
| fields | [string,]|Data field names in the series. Optional depending on series type.
| orderFields | [string,]|Sort field names in the series.
| groupFields | [string,]|Groiup field names in the series.
| whereClause | string|Format string for series value labels.
| showLabels | boolean|Indicates if series shows data labels.
| horizontalAxis | number //int32|Index of horizontal axis.
| verticalAxis | number //int32|Index of vertical axis.
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series.
| fieldAggregation | [string,]|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string.
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending)
| visible | boolean|The flag to indicate whether the series is visible or not


### CIMChartHistogramSeries

|Property | Type | Description |
|---------|--------|--------|
| binCount | number //int32|Number of bins in classifying input values.
| showMean | boolean|Show the mean line on the histogram.
| showMedian | boolean|Show the median line on a histogram.
| showStandardDeviation | boolean|Show the standard deviation band on the histogram.
| fillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties)|Properties of the fill symbol border.
| meanLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Mean line symbol properties of the line series.
| medianLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Median line symbol properties of the line series.
| standardDeviationFillSymbolProperties | [CIMChartFillSymbolProperties](CIMLayer.md#cimchartfillsymbolproperties)|Properties of the fill symbol border.
| showComparisonDistribution | boolean|Show comparison distribution line overlay for the histogram chart.
| dataTransformationType | [enumeration ChartDataTransformationType](CIMLayer.md#enumeration-chartdatatransformationtype)|The type of a data transformation to apply before calculating histogram bins and counts.






## CIMChartLegend
Provides access to members that control chart legend properties.


### CIMChartLegend

|Property | Type | Description |
|---------|--------|--------|
| visible | boolean|Indicates if chart legend is visible.
| title | string|Title of the legend.
| alignment | [enumeration ChartLegendAlignment](CIMLayer.md#enumeration-chartlegendalignment)|Options in arranging chart legend.
| valueFormat | string|Format string for series value labels.
| legendText | [CIMChartTextProperties](CIMLayer.md#cimcharttextproperties)|Text symbol properties.





### Enumeration: ChartLegendAlignment
Chart legend alignment options.

|Property | Value | Description |
|---------|--------|--------|
| Left| 0| The legend is arranged along the left side of the chart.
| Right| 1| The legend is arranged along the right side of the chart.
| Top| 2| The legend is arranged along the top of the chart
| Bottom| 3| The legend is arranged along the bottom of the chart.



### Enumeration: ChartLineDashStyle
Chart line dash style.

|Property | Value | Description |
|---------|--------|--------|
| Solid| 0| Uses solid line to draw the chart line.
| Dot| 1| Uses dotted line to draw the chart line.
| Dash| 2| Uses dashed line to draw the chart line.
| DashDot| 3| Uses dash-dotted line to draw the chart line.
| LongDash| 4| Uses long dashed line to draw the chart line.
| LongDashDot| 5| Uses long dash-dotted line to draw the chart line.




## CIMChartLineSeries
Provides access to members that control line series.


### CIMChartSeries

|Property | Type | Description |
|---------|--------|--------|
| name | string|Name of the series shown in the legend.
| uniqueName | string|Default and unique name of the series.
| fields | [string,]|Data field names in the series. Optional depending on series type.
| orderFields | [string,]|Sort field names in the series.
| groupFields | [string,]|Groiup field names in the series.
| whereClause | string|Format string for series value labels.
| showLabels | boolean|Indicates if series shows data labels.
| horizontalAxis | number //int32|Index of horizontal axis.
| verticalAxis | number //int32|Index of vertical axis.
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series.
| fieldAggregation | [string,]|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string.
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending)
| visible | boolean|The flag to indicate whether the series is visible or not


### CIMChartLineSeries

|Property | Type | Description |
|---------|--------|--------|
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Line symbol properties of the line series.
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties)|Marker symbol properties of the line series.
| timeAggregationType | [enumeration ChartTimeAggregationType](CIMLayer.md#enumeration-charttimeaggregationtype)|The time aggregation type.
| timeIntervalUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The units used for the time interval size.
| timeIntervalSize | number //double|The time interval size.
| trimIncompleteTimeInterval | boolean|A boolean indicating whether incomplete time intervals at the ends of time interval ranges are trimmed in order to avoid bias.
| nullPolicy | [enumeration ChartNullPolicy](CIMLayer.md#enumeration-chartnullpolicy)|The policy for handling null values.






## CIMChartLineSymbolProperties
Provides access to members that control properties of the line symbol.


### CIMChartLineSymbolProperties

|Property | Type | Description |
|---------|--------|--------|
| visible | boolean|Indicates if line is visible.
| width | number //double|Width of the line.
| style | [enumeration ChartLineDashStyle](CIMLayer.md#enumeration-chartlinedashstyle)|Style of the line.
| color | [Color](Types.md#color)|Color of the line.





### Enumeration: ChartMapSelectionHandling
Provides a choice of how map selection is processed in the chart.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| Do not handle map selection.
| Highlight| 1| Highlight selection set on a chart.
| BuildFromSelectionSet| 2| Build a chart exclusively from the selection set.




## CIMChartMarkerSymbolProperties
Provides access to members that control properties of the marker symbol


### CIMChartMarkerSymbolProperties

|Property | Type | Description |
|---------|--------|--------|
| visible | boolean|Indicates if symbol is visible.
| width | number //double|Width of the symbol.
| height | number //double|Height of the symbol.
| style | [enumeration ChartMarkerSymbolStyle](CIMLayer.md#enumeration-chartmarkersymbolstyle)|Style of the symbol.
| color | [Color](Types.md#color)|Color of the symbol fill.
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Properties of the symbol border.





### Enumeration: ChartMarkerSymbolStyle
Chart marker symbol style.

|Property | Value | Description |
|---------|--------|--------|
| Circle| 0| Uses circle to draw the marker symbol.
| Square| 1| Uses square to draw the marker symbol.
| Diamond| 2| Uses diamond to draw the marker symbol.
| Triangle| 3| Uses triangle to draw the marker symbol.



### Enumeration: ChartMultiBarType
Standard multiple bar series placement options.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| Do no use multiple bar series placement options.
| SideBySide| 1| Uses side by side multiple bar series placement option.
| Stacked| 2| Uses stacked bar series placement options.
| Stacked100| 3| Uses stacked 100% multiple bar series placement options.



### Enumeration: ChartNullPolicy
Options to handle null values.

|Property | Value | Description |
|---------|--------|--------|
| Null| 0| Leave the break in the line.
| Zero| 1| Substitute nulls with zeros.
| Interpolate| 2| Substitute nulls with interpolated values




## CIMChartProbabilityPlotSeries
Provides access to members that control probability plot series.


### CIMChartSeries

|Property | Type | Description |
|---------|--------|--------|
| name | string|Name of the series shown in the legend.
| uniqueName | string|Default and unique name of the series.
| fields | [string,]|Data field names in the series. Optional depending on series type.
| orderFields | [string,]|Sort field names in the series.
| groupFields | [string,]|Groiup field names in the series.
| whereClause | string|Format string for series value labels.
| showLabels | boolean|Indicates if series shows data labels.
| horizontalAxis | number //int32|Index of horizontal axis.
| verticalAxis | number //int32|Index of vertical axis.
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series.
| fieldAggregation | [string,]|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string.
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending)
| visible | boolean|The flag to indicate whether the series is visible or not


### CIMChartProbabilityPlotSeries

|Property | Type | Description |
|---------|--------|--------|
| probabilityPlotType | [enumeration ChartProbabilityPlotType](CIMLayer.md#enumeration-chartprobabilityplottype)|The type of a probability plot.
| dataTransformationType | [enumeration ChartDataTransformationType](CIMLayer.md#enumeration-chartdatatransformationtype)|The type of data transformation to apply before calculating Normal Q-Q Plot.
| showReferenceLine | boolean|Shows or hides a reference line overlay for the probability plot.
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties)|The marker symbol properties of the probability plot series.
| referenceLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|The line symbol properties of the probability plot series' reference line.





### Enumeration: ChartProbabilityPlotType
####

|Property | Value | Description |
|---------|--------|--------|
| NormalQQPlot| 0| Normal Q-Q plot.
| QQPlot| 1| General Q-Q plot.




## CIMChartProfileGraphSeries
Provides access to members that control profile graph series.


### CIMChartSeries

|Property | Type | Description |
|---------|--------|--------|
| name | string|Name of the series shown in the legend.
| uniqueName | string|Default and unique name of the series.
| fields | [string,]|Data field names in the series. Optional depending on series type.
| orderFields | [string,]|Sort field names in the series.
| groupFields | [string,]|Groiup field names in the series.
| whereClause | string|Format string for series value labels.
| showLabels | boolean|Indicates if series shows data labels.
| horizontalAxis | number //int32|Index of horizontal axis.
| verticalAxis | number //int32|Index of vertical axis.
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series.
| fieldAggregation | [string,]|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string.
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending)
| visible | boolean|The flag to indicate whether the series is visible or not


### CIMChartProfileGraphSeries

|Property | Type | Description |
|---------|--------|--------|
| lineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Line symbol properties of the profile graph series.
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties)|Marker symbol properties of the profile graph series.
| horizontalUnit | [Unit](ExternalReferences.md#unit)|The unit of measure to be used for horizontal distance. The default value is layer's spatial reference XY unit.
| verticalUnit | [Unit](ExternalReferences.md#unit)|The unit of measure to be used for elevation. The default value is the layer's vertical coordinate system's Z unit, if there is one.






## CIMChartScatterSeries
Provides access to members that control point chart series.


### CIMChartSeries

|Property | Type | Description |
|---------|--------|--------|
| name | string|Name of the series shown in the legend.
| uniqueName | string|Default and unique name of the series.
| fields | [string,]|Data field names in the series. Optional depending on series type.
| orderFields | [string,]|Sort field names in the series.
| groupFields | [string,]|Groiup field names in the series.
| whereClause | string|Format string for series value labels.
| showLabels | boolean|Indicates if series shows data labels.
| horizontalAxis | number //int32|Index of horizontal axis.
| verticalAxis | number //int32|Index of vertical axis.
| colorType | [enumeration ChartColorType](CIMLayer.md#enumeration-chartcolortype)|Type of color for the series.
| fieldAggregation | [string,]|Aggregate field values if series data has a group field. Allowed values are count, sum, median, mean, and empty string.
| orderFieldsSortTypes | [long]|Array of sort order types for fields in OrderFields property Allowed values 0(Ascending), 1(Descending)
| visible | boolean|The flag to indicate whether the series is visible or not


### CIMChartScatterSeries

|Property | Type | Description |
|---------|--------|--------|
| markerSymbolProperties | [CIMChartMarkerSymbolProperties](CIMLayer.md#cimchartmarkersymbolproperties)|Marker symbol properties of the point series.
| showTrendLine | boolean|Defines whether to show the trend line or not.
| trendLineSymbolProperties | [CIMChartLineSymbolProperties](CIMLayer.md#cimchartlinesymbolproperties)|Defines the style for the trend line symbol.





### Enumeration: ChartTextCase
Options for choosing text cases for charts.

|Property | Value | Description |
|---------|--------|--------|
| Normal| 0| No capitalization.
| Uppercase| 1| Transforms all characters to uppercase.
| Lowercase| 2| Transforms all characters to lowercase.
| Capitalize| 3| Transforms the first character of each word to uppercase.
| SmallCaps| 4| All characters to uppercase but in small caps font.




## CIMChartTextProperties
Represents chart text properties.


### CIMChartTextProperties

|Property | Type | Description |
|---------|--------|--------|
| fontFillColor | [Color](Types.md#color)|The fill color for the font.
| fontOutlineColor | [Color](Types.md#color)|The outline color for the font.
| fontFamilyName | string|The font family name.
| fontItalic | boolean|The font style if it is italic or not.
| fontSize | number //double|The font size in points.
| fontWeight | [enumeration ChartFontWeight](CIMLayer.md#enumeration-chartfontweight)|The font weight.
| textCase | [enumeration ChartTextCase](CIMLayer.md#enumeration-charttextcase)|The text case.
| textUnderline | boolean|The text underline.
| textStrikethrough | boolean|The text strikethrough.
| textOverline | boolean|The text overline.





### Enumeration: ChartTimeAggregationType
Options for choosing how time intervals are built for the aggregation of a time based X-axis field.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| No time aggregation is performed.
| EqualIntervalsFromStartTime| 1| Time intervals start with the first (earliest) data point.
| EqualIntervalsFromEndTime| 2| Time intervals start with the last (latest) data point.
| CalendarIntervals| 3| Time intervals follow calendar breaks.




## CIMCompositeSubLayer
Represents a composite sublayer.


### CIMSubLayer

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| expanded | boolean|A boolean indicating whether this layer is expanded in the contents pane.
| maxScale | number //double|The maximum scale for layer draw (set as the denominator of the scale's representative fraction)
| minScale | number //double|The minimum scale for layer draw (set as the denominator of the scale's representative fraction)
| name | string|The name.
| showLegends | boolean|A boolean indicating whether or not to show legends.
| subLayerID | string|The sublayer ID.
| visibility | boolean|A boolean indicating whether or not this layer is visibile.
| serviceLayerID | number //int32|The identifier that will be used to identify the layer in server


### CIMCompositeSubLayer

|Property | Type | Description |
|---------|--------|--------|
| subLayers | [CIMSubLayerBase](CIMLayer.md#cimsublayerbase) |The composite sublayers.





### Enumeration: DisplayCacheType
Display cache types.

|Property | Value | Description |
|---------|--------|--------|
| Permanent| 0| Cache is permanent.
| InSession| 1| Cache is maintained in session.
| None| 2| No cache.
| MaxAge| 3| Cache expires when it reaches the set max age.




## CIMGroupLayer
Represents a group layer which is a simple ordered collection of other layers.


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


### CIMGroupLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| layers | [string,]|The paths of the layers in the group layer.
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing)|The symbol layer drawing definition.






## CIMKMLDataConnection
Represents a KML data connection.


### CIMDataConnection

|Property | Type | Description |
|---------|--------|--------|


### CIMKMLDataConnection

|Property | Type | Description |
|---------|--------|--------|
| KMLURI | string|The URI of the KML file or resource.






## CIMKMLLayer
Represents a KML layer.


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


### CIMKMLLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| dataConnection | [CIMKMLDataConnection](CIMLayer.md#cimkmldataconnection)|The data connection to the KML resource.
| selectable | boolean|A boolean option indicating whether the layer is selectable.
| selectionColor | [Color](Types.md#color)|The selection color.
| useSelectionColor | boolean|A boolean option indicating whether to use the selection color.
| labelVisibility | boolean|A boolean option indicating whether to display labels for this KML layer's placemarks.
| textSymbol | [CIMTextSymbol](CIMSymbols.md#cimtextsymbol)|The text symbol used to label placemarks.






## CIMLayerElevationSurface
Represents a layer elevation surface.


### CIMLayerElevationSurface

|Property | Type | Description |
|---------|--------|--------|
| offsetZ | number //double|The Z offset.
| mapElevationID | string|The map elevation ID.






## CIMLayerTemplate
Represents a layer template.


### CIMLayerTemplate

|Property | Type | Description |
|---------|--------|--------|
| URI | string|The layer template URI.
| layerTemplateId | string|The layer template ID.
| parameters | Object|The layer template parameters.





### Enumeration: Lighting3D
The types of lighting.

|Property | Value | Description |
|---------|--------|--------|
| OneSideDataNormal| 0| Lights one side of each face using the original data normals.
| OneSideResetNormal| 1| Lights one side of each face using recalculated normals.
| TwoSideDataNormal| 2| Lights both sides of each face using original data normals.
| TwoSideResetNormal| 3| Lights both sides of each face using recalculated normals.
| TwoSideDataNormalFromWindingOrder| 4| Lights both sides of each face using original data normals, and the winding order for the "out" direction.
| TwoSideResetNormalFromWindingOrder| 5| Lights both sides of each face using recalculated normal, and the winding order for the "out" direction.



### Enumeration: SortOrderType
Options to choose sort order type.

|Property | Value | Description |
|---------|--------|--------|
| Ascending| 0| Sort ascending.
| Descending| 1| Sort decending.




## CIMSubLayer
Represents sublayer. Defines a sublayer for a containing parent layer. The parent layer is a full-fledged layer, and it controls the sublayer, which is subordinate to the parent. The sublayer is not a layer definition itself rather, it is a property of its parent layer.


### CIMSubLayer

|Property | Type | Description |
|---------|--------|--------|
| description | string|The description.
| expanded | boolean|A boolean indicating whether this layer is expanded in the contents pane.
| maxScale | number //double|The maximum scale for layer draw (set as the denominator of the scale's representative fraction)
| minScale | number //double|The minimum scale for layer draw (set as the denominator of the scale's representative fraction)
| name | string|The name.
| showLegends | boolean|A boolean indicating whether or not to show legends.
| subLayerID | string|The sublayer ID.
| visibility | boolean|A boolean indicating whether or not this layer is visibile.
| serviceLayerID | number //int32|The identifier that will be used to identify the layer in server






## CIMSymbolLayerDrawing
Represents symbol layer drawing properties.


### CIMSymbolLayerDrawing

|Property | Type | Description |
|---------|--------|--------|
| symbolLayers | [CIMSymbolLayerIdentifier](CIMLayer.md#cimsymbollayeridentifier) |The symbol layer identifiers.
| useSymbolLayerDrawing | boolean|A boolean value indicating if symbol layer drawing is enabled.






## CIMSymbolLayerIdentifier
Represents symbol layer identifier.


### CIMSymbolLayerIdentifier

|Property | Type | Description |
|---------|--------|--------|
| symbolLayerName | string|The symbol layer name.






## CIMTopologyLayer
Represents a topology dataset as a layer and draws its errors, exceptions, and areas in need of validation.


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


### CIMTopologyLayerDefinition

|Property | Type | Description |
|---------|--------|--------|
| allLayers | [string,]|The paths of the layers in the topology layer.
| topologyConnection | [DataConnection](Types.md#dataconnection)|The topology data connection.
