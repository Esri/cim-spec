


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
| graphMLURI | string | The GraphML CIMPath. 
| expanded | boolean | A value indicating whether this link chart is expanded in the contents pane. 
| locked | boolean | A value indicating whether this link chart is locked. 
| interactiveLayoutMode | boolean | A value indicating whether this link chart layout updates when the user moves nodes or links. 






## CIMLinkChartEntity
#### Represents a link chart entity. 


### CIMLinkChartEntity 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The Id of for the entity. 
| name | string | The name of the entity. 
| layerURI | string | The CIMPath for the layer used to create the entity. 
| keyFieldName | string | The field used to uniquely identify nodes. If duplicate values exist you can CollapseDuplicates. 
| labelFieldName | string | The field used to label nodes. 
| nonSpatial | boolean | A value indicating whether the entity is non spatial. Where it has coordinates on the map. This is used to prevent drawing links on the map to the wrong nodes. 
| drawingInfo | [CIMLinkChartNodeDrawingInfo](CIMLinkCharts.md#cimlinkchartnodedrawinginfo) | The node drawing information. 
| labelingInfo | [CIMLinkChartNodeLabelingInfo](CIMLinkCharts.md#cimlinkchartnodelabelinginfo) | The node labeling information. 
| expanded | boolean | A value indicating whether this entity is expanded in the contents pane. 





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





### Enumeration: LinkChartSymbolizationSource
#### Link chart node and entity symbolization source. 

|Property | Value | Description | 
|---------|--------|--------|
| MapSymbology| 0| Use default symbology for the nodes in the entity as defined by the associated layer. 
| SingleSymbology| 1| Use overriden single symbology for the nodes in the entity. 

