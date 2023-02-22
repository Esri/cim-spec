

### Enumeration: AttachmentDisplayType
#### Attachment display types. 

|Property | Value | Description | 
|---------|--------|--------|
| PreviewFirst| 0| Preview first. 
| PreviewAll| 1| Preview all. 
| List| 2| List. 




## CIMAttachmentsMediaInfo
#### Represents attachment media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long | The row. 
| column | long | The column. 
| refreshRate | double | The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the media. 
| rowSpan | long | The row span. 
| columnSpan | long | The column span. 
| isCarousel | boolean | A value indicating whether this is a carousel element. 


### CIMAttachmentsMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| caption | string | The caption. 
| title | string | The title. 
| contentType | string | The content MIME type. Example: (image/png, image/jpeg, audio/mp3). 
| displayType | [enumeration AttachmentDisplayType](CIMPopup.md#enumeration-attachmentdisplaytype) | The display type. 






## CIMBarChartMediaInfo
#### Represents bar chart media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long | The row. 
| column | long | The column. 
| refreshRate | double | The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the media. 
| rowSpan | long | The row span. 
| columnSpan | long | The column span. 
| isCarousel | boolean | A value indicating whether this is a carousel element. 


### CIMChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| fields | [string] | The fields. 
| normalizeField | string | The normalization field. 
| caption | string | The caption. 
| title | string | The title. 


### CIMBarChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|






## CIMColumnChartMediaInfo
#### Represents column chart media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long | The row. 
| column | long | The column. 
| refreshRate | double | The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the media. 
| rowSpan | long | The row span. 
| columnSpan | long | The column span. 
| isCarousel | boolean | A value indicating whether this is a carousel element. 


### CIMChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| fields | [string] | The fields. 
| normalizeField | string | The normalization field. 
| caption | string | The caption. 
| title | string | The title. 


### CIMColumnChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|






## CIMExpressionMediaInfo
#### Represents expression media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long | The row. 
| column | long | The column. 
| refreshRate | double | The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the media. 
| rowSpan | long | The row span. 
| columnSpan | long | The column span. 
| isCarousel | boolean | A value indicating whether this is a carousel element. 


### CIMExpressionMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| expression | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The Arcade expression used to evaluate and return the media infos. 






## CIMImageMediaInfo
#### Represents image media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long | The row. 
| column | long | The column. 
| refreshRate | double | The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the media. 
| rowSpan | long | The row span. 
| columnSpan | long | The column span. 
| isCarousel | boolean | A value indicating whether this is a carousel element. 


### CIMImageMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| sourceURL | string | The source URL. 
| linkURL | string | The link URL. 
| caption | string | The caption. 
| title | string | The title. 






## CIMLineChartMediaInfo
#### Represents line chart media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long | The row. 
| column | long | The column. 
| refreshRate | double | The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the media. 
| rowSpan | long | The row span. 
| columnSpan | long | The column span. 
| isCarousel | boolean | A value indicating whether this is a carousel element. 


### CIMChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| fields | [string] | The fields. 
| normalizeField | string | The normalization field. 
| caption | string | The caption. 
| title | string | The title. 


### CIMLineChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|






## CIMPieChartMediaInfo
#### Represents pie chart media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long | The row. 
| column | long | The column. 
| refreshRate | double | The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the media. 
| rowSpan | long | The row span. 
| columnSpan | long | The column span. 
| isCarousel | boolean | A value indicating whether this is a carousel element. 


### CIMChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| fields | [string] | The fields. 
| normalizeField | string | The normalization field. 
| caption | string | The caption. 
| title | string | The title. 


### CIMPieChartMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|






## CIMPopupFieldDescription
#### Represents a pop-up field description. 


### CIMPopupFieldDescription 

|Property | Type | Description | 
|---------|--------|--------|
| alias | string | The field alias. 
| fieldName | string | The field name. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 






## CIMPopupInfo
#### Represents pop-up info. 


### CIMPopupInfo 

|Property | Type | Description | 
|---------|--------|--------|
| title | string | The title. 
| expressionInfos | [[CIMExpressionInfo]](CIMRenderers.md#cimexpressioninfo) | Arcade expressions that are referenced as fields in one or more elements in MediaInfos. 
| mediaInfos | [[CIMMediaInfo]](Types.md#mediainfo) | The media infos. 
| relatedRecordSortOrder | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The field name and the sort order by which the related records will be ordered. The items are defined by the related field name (Format: RelationshipName\\FieldName) as the Keys and the sort order (Enum: Asc, Desc) as the Values. 
| gridLayout | [CIMPopupLayout](CIMPopup.md#cimpopuplayout) | The grid layout for the media infos. 
| fieldDescriptions | [[CIMPopupFieldDescription]](CIMPopup.md#cimpopupfielddescription) | The pop-up field descriptions. 






## CIMPopupLayout
#### Represents a grid layout for pop-up media infos. 


### CIMPopupLayout 

|Property | Type | Description | 
|---------|--------|--------|
| columnWidths | [double] | The array of column width values in percentage of the table width (0-100). The sum of the array of width percentage values should be equal to 100. 
| borderWidth | double | The border width in points. 
| borderColor | [Color](Types.md#color) | The border color. 






## CIMRelationshipMediaInfo
#### Represents relationship media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long | The row. 
| column | long | The column. 
| refreshRate | double | The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the media. 
| rowSpan | long | The row span. 
| columnSpan | long | The column span. 
| isCarousel | boolean | A value indicating whether this is a carousel element. 


### CIMRelationshipMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| caption | string | The caption. 
| title | string | The title. 
| displayCount | long | The maximum number of related records to display. 
| relationshipName | string | The name of the relationship. 
| relatedRecordSortOrder | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The field names and the types of sort order by which the related records will be ordered. The items are defined by the related field name as the Keys and the sort order (Enum: Asc, Desc) as the Values. 






## CIMTableMediaInfo
#### Represents table media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long | The row. 
| column | long | The column. 
| refreshRate | double | The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the media. 
| rowSpan | long | The row span. 
| columnSpan | long | The column span. 
| isCarousel | boolean | A value indicating whether this is a carousel element. 


### CIMTableMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| fields | [string] | The fields. 
| useLayerFields | boolean | A value indicating whether or not the table is generated using the layer's visible fields. 
| caption | string | The caption. 
| title | string | The title. 






## CIMTextMediaInfo
#### Represents text media info. 


### CIMMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| row | long | The row. 
| column | long | The column. 
| refreshRate | double | The amount of time in RefreshRateUnit to wait between refreshing the media info. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the media. 
| rowSpan | long | The row span. 
| columnSpan | long | The column span. 
| isCarousel | boolean | A value indicating whether this is a carousel element. 


### CIMTextMediaInfo 

|Property | Type | Description | 
|---------|--------|--------|
| text | string | The text. 



