

### Enumeration: TimeIndicatorSize
#### Represents the timeline time indicator size. 

|Property | Value | Description | 
|---------|--------|--------|
| Small| 0| Timeline time indicator size small. 
| Medium| 1| Timeline time indicator size medium. 
| Large| 2| Timeline time indicator size large. 



### Enumeration: TimeSpanSymbolBoundary
#### Options for how a time span symbol will symbolize boundaries. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Time span symbol with no boundaries. 
| StartPoint| 1| Time span symbol with start boundary. 
| EndPoint| 2| Time span symbol with end boundary. 
| StartAndEndPoint| 3| Time span symbol with start and end boundary. 




## CIMTimeline
#### Represents a timeline. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| uRI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the source was last modified, as of the last sync. Used to detect when another sync is needed. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 
| sourcePortalUrl | string | The source portal URI of the item. Set if sourced from an external item such as an item on a portal. 


### CIMTimelineDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| units | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | Time units used in the timeline scale. 
| startTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time at the beginning of the timeline. 
| endTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time at the end of the timeline. 
| showSwimlanes | boolean | A value indicating whether the timeline shows swimlanes. 
| showSwimlaneLabels | boolean | A value indicating whether the timeline swimlanes show labels. 
| honorTimeSlider | boolean | A value indicating whether the timeline syncs with the map time slider. 
| expanded | boolean | A value indicating whether the timeline is expanded in the contents pane. 
| swimlanes | [[CIMTimelineSwimlane]](CIMTimelines.md#cimtimelineswimlane) | The timeline swimlanes. 
| honorSelection | boolean | A value indicating whether the items in the timeline are visible based on the map selection. 
| honorExtent | boolean | A value indicating whether the items in the timeline are visible based on the map extent. 
| honorRange | boolean | A value indicating whether the items in the timeline are visible based on range. 
| viewType | [enumeration TimelineViewType](CIMTimelines.md#enumeration-timelineviewtype) | The timeline view type. 
| binningTimespan | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The time units used in summary view bin time. 
| selectionSetURI | string | The URI of the binary reference containing the selection set. 
| timelineTextSymbol | [CIMTextSymbol](CIMSymbols.md#cimtextsymbol) | The text symbol for the timeline. 
| theme | [enumeration TimelineTheme](CIMTimelines.md#enumeration-timelinetheme) | The theme of the timeline. e.g. Light, Medium, or Dark. 
| timeIndicator | [enumeration TimeIndicatorSize](CIMTimelines.md#enumeration-timeindicatorsize) | The time indicator. e.g. Small, Medium, or Large. 






## CIMTimelineLaneDataSource
#### Represents a source of temporal data. 


### CIMTimelineLaneDataSource 

|Property | Type | Description | 
|---------|--------|--------|
| iD | string | The value of the lane data source ID. 






## CIMTimelineLaneDrawingInfo
#### Represents the timeline lane drawing information. 


### CIMTimelineLaneDrawingInfo 

|Property | Type | Description | 
|---------|--------|--------|
| viewType | [enumeration TimelineLaneViewType](CIMTimelines.md#enumeration-timelinelaneviewtype) | The timeline lane view type. 
| maxNumberOfCascadeRows | long | The max number of cascade rows for this timeline lane. 
| timeSpanSymbolBoundary | [enumeration TimeSpanSymbolBoundary](CIMTimelines.md#enumeration-timespansymbolboundary) | The time span symbol boundary preference. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp for the time span symbols. 
| timeSpanSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol) | The line symbol for the timeline time spans. 
| symbolStyleType | [enumeration TimelineSymbolStyleType](CIMTimelines.md#enumeration-timelinesymbolstyletype) | The timeline symbol style type. 






## CIMTimelineLaneMapMemberDataSource
#### Represents a map member source of temporal data. 


### CIMTimelineLaneDataSource 

|Property | Type | Description | 
|---------|--------|--------|
| iD | string | The value of the lane data source ID. 


### CIMTimelineLaneMapMemberDataSource 

|Property | Type | Description | 
|---------|--------|--------|
| mapMemberURI | string | The value of the map member uri. 
| displayField | string | The value of the display field name. 
| categoryField | string | The value of the category field name. 
| categoryValue | any | The value of the category field value. 
| categoryValueType | [enumeration esriFieldType](ExternalReferences.md#enumeration-esrifieldtype) | The value of the category field value type. 





### Enumeration: TimelineLaneViewType
#### Timeline lane type. 

|Property | Value | Description | 
|---------|--------|--------|
| Overlap| 0| Lane view where data is allowed to overlap. 
| Cascade| 1| Lane view where overlapping data is cascaded into new rows. 




## CIMTimelineLayer
#### Represents a layer in a timeline. 


### CIMTimelineLayer 

|Property | Type | Description | 
|---------|--------|--------|
| iD | string | The Id of for the timeline layer. 
| alias | string | The timeline layer alias. 
| layerURI | string | The value of the layer uri. 
| displayField | string | The value of the display field name. 
| categoryField | string | The value of the category field name. 
| visibility | boolean | A value indicating whether the timeline layer is visible. 
| drawingInfo | [CIMTimelineLaneDrawingInfo](CIMTimelines.md#cimtimelinelanedrawinginfo) | The timeline layer drawing information. 
| dataSources | [[CIMTimelineLaneDataSource]](Types.md#timelinelanedatasource) | Timeline layer data sources. 
| layerType | [enumeration TimelineLayerType](CIMTimelines.md#enumeration-timelinelayertype) | The timeline layer view type. 





### Enumeration: TimelineLayerType
#### Timeline layer type. 

|Property | Value | Description | 
|---------|--------|--------|
| Individual| 0| Timeline layer containing data that is expandable. 
| Leftover| 1| Timeline layer containing data that is not expandable. 




## CIMTimelineSwimlane
#### Represents a swimlane in a timeline. 


### CIMTimelineSwimlane 

|Property | Type | Description | 
|---------|--------|--------|
| iD | string | The Id of for the timeline swimlane. 
| alias | string | An alias for the swimlane. 
| visibility | boolean | A value indicating whether the swimlane is visible. 
| expanded | boolean | A value indicating whether the swimlane is expanded in the contents pane. 
| swimlaneExpanded | boolean | A value indicating whether the swimlane is expanded in the timeline. 
| layers | [[CIMTimelineLayer]](CIMTimelines.md#cimtimelinelayer) | The timeline layers. 
| drawingInfo | [CIMTimelineLaneDrawingInfo](CIMTimelines.md#cimtimelinelanedrawinginfo) | The timeline swimlane drawing information. 





### Enumeration: TimelineSymbolStyleType
#### Represents the timeline symbol style types. 

|Property | Value | Description | 
|---------|--------|--------|
| SingleColor| 0| Symbol Single Color. 
| AlternatingColor| 1| Symbol Alternating Colors. 



### Enumeration: TimelineTheme
#### Represents the timeline theme. 

|Property | Value | Description | 
|---------|--------|--------|
| Light| 0| Timeline light theme. 
| Medium| 1| Timeline medium theme. 
| Dark| 2| Timeline dark theme. 



### Enumeration: TimelineViewType
#### Timeline view type. 

|Property | Value | Description | 
|---------|--------|--------|
| DefaultView| 0| Default timeline view. 
| SummaryView| 1| Timeline Summary View. 

