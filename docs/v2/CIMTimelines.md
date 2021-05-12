


## CIMTimeline
#### Represents a timeline. 


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






## CIMTimelineLayer
#### Represents a layer in a timeline. 


### CIMTimelineLayer 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The Id of for the timeline layer. 
| alias | string | The timeline layer alias. 
| layerURI | string | The value of the layer uri. 
| displayField | string | The value of the display field name. 
| categoryField | string | The value of the category field name. 
| visibility | boolean | A value indicating whether the timeline layer is visible. 






## CIMTimelineSwimlane
#### Represents a swimlane in a timeline. 


### CIMTimelineSwimlane 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The Id of for the timeline swimlane. 
| alias | string | An alias for the swimlane. 
| visibility | boolean | A value indicating whether the swimlane is visible. 
| expanded | boolean | A value indicating whether the swimlane is expanded in the contents pane. 
| swimlaneExpanded | boolean | A value indicating whether the swimlane is expanded in the timeline. 
| layers | [[CIMTimelineLayer]](CIMTimelines.md#cimtimelinelayer) | The timeline layers. 



