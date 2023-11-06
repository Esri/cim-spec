


## CIMLinkChart
#### Represents a link chart. 


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


### CIMLinkChartBaseDefinition 

|Property | Type | Description | 
|---------|--------|--------|


### CIMLinkChartDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| entities | [[CIMLinkChartEntity]](CIMLinkCharts.md#cimlinkchartentity) | The link chart entities. 
| relationships | [[CIMLinkChartRelationship]](CIMLinkCharts.md#cimlinkchartrelationship) | The link chart relationships. 
| layout | [enumeration LinkChartLayoutAlgorithm](CIMLinkCharts.md#enumeration-linkchartlayoutalgorithm) | The link chart layout algorithm. 
| graphMLURI | string | The URI of the binary reference containing the GraphML. 
| expanded | boolean | A value indicating whether this link chart is expanded in the contents pane. 
| locked | boolean | A value indicating whether this link chart is locked. 
| interactiveLayoutMode | boolean | A value indicating whether this link chart layout updates when the user moves nodes or links. 
| viewport | [CIMLinkChartViewport](CIMLinkCharts.md#cimlinkchartviewport) | The link chart viewport. 
| filterByMinLinks | boolean | A value indicating whether this link chart is filtered by the minimum number of links. 
| minLinks | long | The minimum number of links allowed in the filter. 
| filterGroups | [[CIMLinkChartFilterGroup]](CIMLinkCharts.md#cimlinkchartfiltergroup) | The link chart filter groups. 






## CIMLinkChartEntity
#### Represents a link chart entity. 


### CIMLinkChartEntity 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The Id of for the entity. 
| name | string | The name of the entity. 
| layerURI | string | The CIMPath for the layer used to create the entity. 
| labelFieldName | string | The field used to label nodes. 
| nonSpatial | boolean | A value indicating whether the entity is non spatial. Where it has coordinates on the map. This is used to prevent drawing links on the map to the wrong nodes. 
| drawingInfo | [CIMLinkChartNodeDrawingInfo](CIMLinkCharts.md#cimlinkchartnodedrawinginfo) | The node drawing information. 
| labelingInfo | [CIMLinkChartNodeLabelingInfo](CIMLinkCharts.md#cimlinkchartnodelabelinginfo) | The node labeling information. 
| expanded | boolean | A value indicating whether this entity is expanded in the contents pane. 
| keyFieldNames | [string] | The fields used to uniquely identify nodes. If duplicate values exist you can CollapseDuplicates. 






## CIMLinkChartFieldFilter
#### Represents additional settings used by a Link chart field filter. 


### CIMLinkChartFilter 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The ID of the link chart filter. 
| name | string | The name of the link chart filter. 
| description | string | The description of the link chart filter. 
| enabled | boolean | A value indicating whether the link chart filter is enabled or not. 
| isExclusion | boolean | A value indicating whether or not this is an exclusion filter. 
| filterStage | [enumeration LinkChartFilterStage](CIMLinkCharts.md#enumeration-linkchartfilterstage) | The value that indicates when the link chart filter is applied. 
| filterType | [enumeration LinkChartFilterType](CIMLinkCharts.md#enumeration-linkchartfiltertype) | The filter type of the link chart filter. 
| filterScope | [enumeration LinkChartFilterScope](CIMLinkCharts.md#enumeration-linkchartfilterscope) | The value that indicates what link chart component is filtered: entities, relationships, or both. 
| targetIds | [string] | The entity and or relationship Ids to filter. 
| valueSetURI | string | The binary reference of the filter values for the link chart filter. 


### CIMLinkChartFieldFilter 

|Property | Type | Description | 
|---------|--------|--------|
| field | string | The field that is used to filter the link chart entity or relationship. 
| fieldType | [enumeration esriFieldType](ExternalReferences.md#enumeration-esrifieldtype) | The field type that is used to filter the link chart entity or relationship. 






## CIMLinkChartFilter
#### Represents the link chart filter information. 


### CIMLinkChartFilter 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The ID of the link chart filter. 
| name | string | The name of the link chart filter. 
| description | string | The description of the link chart filter. 
| enabled | boolean | A value indicating whether the link chart filter is enabled or not. 
| isExclusion | boolean | A value indicating whether or not this is an exclusion filter. 
| filterStage | [enumeration LinkChartFilterStage](CIMLinkCharts.md#enumeration-linkchartfilterstage) | The value that indicates when the link chart filter is applied. 
| filterType | [enumeration LinkChartFilterType](CIMLinkCharts.md#enumeration-linkchartfiltertype) | The filter type of the link chart filter. 
| filterScope | [enumeration LinkChartFilterScope](CIMLinkCharts.md#enumeration-linkchartfilterscope) | The value that indicates what link chart component is filtered: entities, relationships, or both. 
| targetIds | [string] | The entity and or relationship Ids to filter. 
| valueSetURI | string | The binary reference of the filter values for the link chart filter. 






## CIMLinkChartFilterGroup
#### Represents a group of link chart filters. 


### CIMLinkChartFilterGroup 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The ID of the link chart filter group. 
| name | string | The name of the link chart filter group. 
| description | string | The description of the link chart filter group. 
| enabled | boolean | A value indicating whether the link chart filter group is enabled or not. 
| filters | [[CIMLinkChartFilter]](Types.md#linkchartfilter) | The link chart filters in the group. 





### Enumeration: LinkChartFilterPropertyDataType
#### Link chart filter type property data types. Used when specifying link chart filter type as PropertyData. 

|Property | Value | Description | 
|---------|--------|--------|
| EntityKeyValue| 0| Entity key value. 
| LabelValue| 1| Entity or relationship label value. 



### Enumeration: LinkChartFilterScope
#### Link chart filter scope. 

|Property | Value | Description | 
|---------|--------|--------|
| Entities| 0| Filter applies to entities. 
| Relationships| 1| Filter applies to relationships. 
| Both| 2| Filter applies to both entities and relationships. 



### Enumeration: LinkChartFilterStage
#### Link chart filter stage. 

|Property | Value | Description | 
|---------|--------|--------|
| Unknown| 0| Unknown. 
| Data| 1| Filter is applied at the data source. 
| Visual| 2| Filter is applied at visualization. 



### Enumeration: LinkChartFilterType
#### Link chart filter type. 

|Property | Value | Description | 
|---------|--------|--------|
| Unknown| 0| Unknown filter type. 
| FieldData| 1| Filter is applied to a field in the source data. 
| PropertyData| 2| Filter is applied to a property of the link chart or its components. For example, entity key value, entity node label, computed values, analysis results, counts, etc. 



### Enumeration: LinkChartLayoutAlgorithm
#### Link chart layout algorithm. 

|Property | Value | Description | 
|---------|--------|--------|
| Clustered| 0| Clustered layout. 
| Organic| 1| Organic layout. 
| Hierarchy_TopToBottom| 2| Hierarchy layout oriented top to bottom. 
| Hierarchy_BottomToTop| 3| Hierarchy layout oriented bottom to top. 
| Hierarchy_LeftToRight| 4| Hierarchy layout oriented left to right. 
| Hierarchy_RightToLeft| 5| Hierarchy layout oriented right to left. 



### Enumeration: LinkChartLinkDashStyle
#### Link chart link dash style. 

|Property | Value | Description | 
|---------|--------|--------|
| Solid| 0| Uses solid line to draw the link chart link. 
| Dot| 1| Uses dotted line to draw the link chart link. 
| Dash| 2| Uses dashed line to draw the chart line. 
| DashDot| 3| Uses dash-dotted line to draw the link chart link. 
| DashDotDot| 4| Uses dash-dot-dot line to draw link chart link. 




## CIMLinkChartLinkDrawingInfo
#### Represents the link chart link drawing information. 


### CIMLinkChartLinkDrawingInfo 

|Property | Type | Description | 
|---------|--------|--------|
| linkColor | [Color](Types.md#color) | Link color. 
| linkWidth | long | A value for the link width. 
| linkDashStyle | [enumeration LinkChartLinkDashStyle](CIMLinkCharts.md#enumeration-linkchartlinkdashstyle) | A value for the link dash style. 
| showDirection | boolean | A value indicating whether to show the directional arrowhead of a link. 





### Enumeration: LinkChartLinkLabelPlacement
#### Link chart link label placement. 

|Property | Value | Description | 
|---------|--------|--------|
| Parallel| 0| Parallel to link. 
| Perpendicular| 1| Perpendicular to link. 




## CIMLinkChartLinkLabelingInfo
#### Represents the link chart link labeling information. 


### CIMLinkChartLabelingInfo 

|Property | Type | Description | 
|---------|--------|--------|
| showLabels | boolean | A value indicating whether the labels are shown. 
| labelFontFamilyName | string | The link label font family name of the font. e.g. Comic Sans. 
| labelFontStyleName | string | The style name for the link label font family. e.g. Regular, Bold, or Italic. 
| labelFontType | [enumeration FontType](CIMSymbols.md#enumeration-fonttype) | Link label font type. 
| labelFontSize | double | Link label font size. 
| labelFontColor | [Color](Types.md#color) | Link Label font color. 
| labelBackgroundColor | [Color](Types.md#color) | Link label background color. 


### CIMLinkChartLinkLabelingInfo 

|Property | Type | Description | 
|---------|--------|--------|
| labelPlacement | [enumeration LinkChartLinkLabelPlacement](CIMLinkCharts.md#enumeration-linkchartlinklabelplacement) | The link label placement. 
| defaultLabel | string | The default label. 






## CIMLinkChartNodeDrawingInfo
#### Represents the link chart node drawing information. 


### CIMLinkChartNodeDrawingInfo 

|Property | Type | Description | 
|---------|--------|--------|
| collapseDuplicates | boolean | A value indicating whether the entity whether duplicate node values are consolidated. The result is one node for multiple values. 
| nodeSymbology | [enumeration LinkChartSymbolizationSource](CIMLinkCharts.md#enumeration-linkchartsymbolizationsource) | The entity symbology preference. 
| overrideSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The override symbol. 
| overrideOverviewSymbolColor | boolean | A value indicating whether the overview symbol color is calculated or specified. 
| overviewSymbolColor | [Color](Types.md#color) | The override overview symbol color. 
| showNodeFrames | boolean | A value indicating whether the node frames are shown. 






## CIMLinkChartNodeLabelingInfo
#### Represents the link chart node labeling information. 


### CIMLinkChartLabelingInfo 

|Property | Type | Description | 
|---------|--------|--------|
| showLabels | boolean | A value indicating whether the labels are shown. 
| labelFontFamilyName | string | The link label font family name of the font. e.g. Comic Sans. 
| labelFontStyleName | string | The style name for the link label font family. e.g. Regular, Bold, or Italic. 
| labelFontType | [enumeration FontType](CIMSymbols.md#enumeration-fonttype) | Link label font type. 
| labelFontSize | double | Link label font size. 
| labelFontColor | [Color](Types.md#color) | Link Label font color. 
| labelBackgroundColor | [Color](Types.md#color) | Link label background color. 


### CIMLinkChartNodeLabelingInfo 

|Property | Type | Description | 
|---------|--------|--------|






## CIMLinkChartPropertyFilter
#### Represents additional settings used by a Link chart property filter. 


### CIMLinkChartFilter 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The ID of the link chart filter. 
| name | string | The name of the link chart filter. 
| description | string | The description of the link chart filter. 
| enabled | boolean | A value indicating whether the link chart filter is enabled or not. 
| isExclusion | boolean | A value indicating whether or not this is an exclusion filter. 
| filterStage | [enumeration LinkChartFilterStage](CIMLinkCharts.md#enumeration-linkchartfilterstage) | The value that indicates when the link chart filter is applied. 
| filterType | [enumeration LinkChartFilterType](CIMLinkCharts.md#enumeration-linkchartfiltertype) | The filter type of the link chart filter. 
| filterScope | [enumeration LinkChartFilterScope](CIMLinkCharts.md#enumeration-linkchartfilterscope) | The value that indicates what link chart component is filtered: entities, relationships, or both. 
| targetIds | [string] | The entity and or relationship Ids to filter. 
| valueSetURI | string | The binary reference of the filter values for the link chart filter. 


### CIMLinkChartPropertyFilter 

|Property | Type | Description | 
|---------|--------|--------|
| dataType | [enumeration LinkChartFilterPropertyDataType](CIMLinkCharts.md#enumeration-linkchartfilterpropertydatatype) | The property data type that will be filtered. 






## CIMLinkChartRelationship
#### Represents a link chart relationship. 


### CIMLinkChartRelationship 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The Id of for the relationship. 
| name | string | The name of the relationship. 
| sourceEntityId | string | The source entity id for the relationship. 
| sourceEntityBackingField | string | The source entity backing field for the relationship. 
| targetEntityId | string | The target entity id for the relationship. 
| targetEntityBackingField | string | The target entity backing field for the relationship. 
| drawingInfo | [CIMLinkChartLinkDrawingInfo](CIMLinkCharts.md#cimlinkchartlinkdrawinginfo) | The link drawing information. This specifies the link color, width, and dash style. 
| labelingInfo | [CIMLinkChartLinkLabelingInfo](CIMLinkCharts.md#cimlinkchartlinklabelinginfo) | The link labeling information. 
| expanded | boolean | A value indicating whether this relationship is expanded in the contents pane. 
| keyType | [enumeration LinkChartRelationshipKeyType](CIMLinkCharts.md#enumeration-linkchartrelationshipkeytype) | The KeyType. This specifies where the key fields are located. 
| mapMemberURI | string | The path to the foreign table or layer used to create the relationship. 
| sourceEntityKeyField | string | The source entity key field for the relationship. 
| targetEntityKeyField | string | The target entity key field for the relationship. 





### Enumeration: LinkChartRelationshipKeyType
#### Link chart relationship key type. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Link chart relationship has no keys. 
| Entities| 1| Link chart relationship has keys from entities. 
| Foreign| 2| Link chart relationship has foreign keys. 



### Enumeration: LinkChartSymbolizationSource
#### Link chart node and entity symbolization source. 

|Property | Value | Description | 
|---------|--------|--------|
| MapSymbology| 0| Use default symbology for the nodes in the entity as defined by the associated layer. 
| SingleSymbology| 1| Use overriden single symbology for the nodes in the entity. 




## CIMLinkChartViewport
#### Represents the link chart viewport. 


### CIMLinkChartViewport 

|Property | Type | Description | 
|---------|--------|--------|
| centerX | double | The center X coordinate in the world coordinate system. 
| centerY | double | The center Y coordinate in the world coordinate system. 
| zoomLevel | double | The zoom level. 



