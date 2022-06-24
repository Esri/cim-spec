


## CIMDataEngineeringFieldStatistics
#### Contains the field statistics. 


### CIMDataEngineeringFieldStatistics 

|Property | Type | Description | 
|---------|--------|--------|
| fieldName | string | Field name. 
| treatFieldAs | [enumeration DataEngineeringTreatFieldAsType](CIMDataEngineeringView.md#enumeration-dataengineeringtreatfieldastype) | An option for treating a field as another statistic type. 
| values | [[CIMDataEngineeringStatisticValue]](CIMDataEngineeringView.md#cimdataengineeringstatisticvalue) | Statistic values. 
| previewChart | [CIMDataEngineeringPreviewChart](CIMDataEngineeringView.md#cimdataengineeringpreviewchart) | The preview chart. 






## CIMDataEngineeringPreviewChart
#### Provide information of a preview chart. 


### CIMDataEngineeringPreviewChart 

|Property | Type | Description | 
|---------|--------|--------|
| minimum | any | Minimum/first in the X axis. 
| maximum | any | Maximum/last in the X axis. 
| values | [[any]]| Preiew chart values. 





### Enumeration: DataEngineeringSourceFilterType
#### Source filter to update the statistics. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| None. 
| Selection| 1| Selection. 
| Extent| 2| Extent. 
| SelectionAndExtent| 3| Selection. 



### Enumeration: DataEngineeringStatType
#### Data engineering statistic type. 

|Property | Value | Description | 
|---------|--------|--------|
| Mean| 0| Mean. 
| StandardDeviation| 1| Standard deviation. 
| Maximum| 2| Maximum. 
| Minimum| 3| Minimum. 
| Median| 4| Median. 
| Mode| 5| Mode. 
| FirstQuartile| 6| First Quartile. 
| ThirdQuartile| 7| Third Quartile. 
| Sum| 8| Sum. 
| NumberOfNulls| 9| Number of Nulls. 
| Outliers| 10| Number of Outliers 
| NumberUniqueValues| 11| Number of unique values. 
| LeastCommon| 12| Least Common. 
| Kurtosis| 13| Kurtosis. 
| Skewness| 14| Skewness. 
| CoefficientOfVariation| 15| Coefficient of Variation. 
| Range| 16| Range. 
| IQR| 17| Interquartile range. 
| Count| 18| Count. 




## CIMDataEngineeringStatisticColumn
#### Provide access to the statistic column. 


### CIMDataEngineeringStatisticColumn 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The column name. 
| isFrozen | boolean | A value indicating whether the column is frozen. 
| isSorted | boolean | A value indicating whether the column is sorted. 
| isVisible | boolean | A value indicating whether the column is visible. 
| sortDirection | [enumeration SortOrderType](CIMLayer.md#enumeration-sortordertype) | A value indicating the sort direction. 






## CIMDataEngineeringStatisticValue
#### Contains a statistic value. 


### CIMDataEngineeringStatisticValue 

|Property | Type | Description | 
|---------|--------|--------|
| statisticType | [enumeration DataEngineeringStatType](CIMDataEngineeringView.md#enumeration-dataengineeringstattype) | The statistic type. 
| value | any | Statistic Value. 





### Enumeration: DataEngineeringTreatFieldAsType
#### Treat Field as Type. 

|Property | Value | Description | 
|---------|--------|--------|
| Numerical| 0| Numerical. 
| Categorical| 1| Categorical. 
| DateTime| 2| Date time. 
| Other| 3| Other. 




## CIMDataEngineeringView
#### Represents a data engineering statistics view. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
| viewableObjectPath | string | The path of the item in the view. 
| viewType | string | The view type as a string. 
| instanceID | long | The instance identifier of this view. 


### CIMDataEngineeringView 

|Property | Type | Description | 
|---------|--------|--------|
| mapURI | string | The path of the Map for the item in the view. 
| sourceFilter | [enumeration DataEngineeringSourceFilterType](CIMDataEngineeringView.md#enumeration-dataengineeringsourcefiltertype) | The source filter applied for calculating the statistics. 
| useFieldAliases | boolean | A value indicating whether to show field aliases in the view. 
| rowHeight | long | The row height in pixels. 
| zoomPercent | long | The zoom level of the summary statistics table. 
| layoutType | [enumeration DataEngineeringViewLayoutType](CIMDataEngineeringView.md#enumeration-dataengineeringviewlayouttype) | The view layout style. 
| columns | [[CIMDataEngineeringStatisticColumn]](CIMDataEngineeringView.md#cimdataengineeringstatisticcolumn) | The properties of statistics to display in the summary statistic view. 
| fieldTypeFilter | [enumeration ArrayOfFieldType](ExternalReferences.md#enumeration-arrayoffieldtype) | The list of field type filters. 
| fieldStatistics | [[CIMDataEngineeringFieldStatistics]](CIMDataEngineeringView.md#cimdataengineeringfieldstatistics) | A collection of field statistics. 
| displayNumericStatistics | boolean | A value indicating whether to show numeric statistics in the table. 
| displayDateTimeStatistics | boolean | A value indicating whether to show date statistics in the table. 
| displayTextStatistics | boolean | A value indicating whether to show text statistics in the table. 





### Enumeration: DataEngineeringViewLayoutType
#### Statistic View Layout Type. 

|Property | Value | Description | 
|---------|--------|--------|
| FieldsAndStatistics| 0| View fields and statistics. 
| OnlyStatistics| 1| View only statistics. 

