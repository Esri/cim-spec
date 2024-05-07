

### Enumeration: CentralityRelationshipInterpretation
#### Specifies the way relationships are interpreted for centrality computations. 

|Property | Value | Description | 
|---------|--------|--------|
| Undirected| 0| Relationships are considered to be undirected. 
| Directed| 1| Relationships are considered to be directed. 
| Reversed| 2| Relationships are considered to be directed and their direction is reversed. 



### Enumeration: CentralityScoresNormalization
#### Specifies the normalization option for centrality scores. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No normalization is done. 
| Global| 1| Normalize globally. 
| ByComponent| 2| Normalize by component. 




## CIMFilteredFindPathsConfiguration
#### Represents a Knowledge Graph Filtered Find Paths Configuration. 


### CIMFilteredFindPathsConfiguration 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the configuration. 
| originEntities | [[CIMFilteredFindPathsEntity]](CIMKnowledgeGraph.md#cimfilteredfindpathsentity) | The origin entities. 
| destinationEntities | [[CIMFilteredFindPathsEntity]](CIMKnowledgeGraph.md#cimfilteredfindpathsentity) | The destination entities. 
| pathFilters | [[CIMFilteredFindPathsPathFilter]](CIMKnowledgeGraph.md#cimfilteredfindpathspathfilter) | The path filters. 
| defaultTraversalDirectionType | [enumeration KGTraversalDirectionType](CIMKnowledgeGraph.md#enumeration-kgtraversaldirectiontype) | The default traversal direction which is used for any relationship type that is not defined in the traversal directions list. 
| traversalDirections | [[CIMKGTraversalDirection]](CIMKnowledgeGraph.md#cimkgtraversaldirection) | The traversal directions. 
| entityUsage | [enumeration FilteredFindPathsEntityUsage](CIMKnowledgeGraph.md#enumeration-filteredfindpathsentityusage) | The usage of origin/destination entities in the filtered find paths algorithm. 
| pathMode | [enumeration KGPathMode](CIMKnowledgeGraph.md#enumeration-kgpathmode) | Whether the filtered find paths algorithm searches for shortest paths or for all paths. 
| minPathLength | long | The min path length. 
| maxPathLength | long | The max path length. The default of 0 means the value is unlimited. 
| maxCountPaths | long | The max number of paths the filtered find paths algorithm returns. 
| timeFilter | [CIMKGTimeFilter](CIMKnowledgeGraph.md#cimkgtimefilter) | The time filter. 






## CIMFilteredFindPathsEntity
#### Represents a Knowledge Graph Filtered Find Paths Entity. An entity can be used for a specific instance, in this case the ID has a value, or for all instances of a type, in this case the ID is null. 


### CIMFilteredFindPathsEntity 

|Property | Type | Description | 
|---------|--------|--------|
| ID | any | The id of the entity instance used as a origin/destination entity. If this id is null, then the filtered find paths algorithm uses all instances of the specified entity type. 
| entityTypeName | string | The type name of the entity (type or instance) used as an origin/destination entity. 
| propertyFilterPredicate | string | The property filter predicate (cypher syntax) associated with the path filter. 





### Enumeration: FilteredFindPathsEntityUsage
#### Specifies how origin/destination entities are used in the filtered find paths algorithm. 

|Property | Value | Description | 
|---------|--------|--------|
| AnyOriginAnyDestination| 0| The filtered find paths algorithm only returns the shortest paths for the origin entities that have the shortest shortest paths and the shortest paths for the destination entities that have the shortest shortest paths. When multiple entities are used, this option leads to faster computations. 
| AnyOriginAllDestinations| 1| The filtered find paths algorithm returns the shortest paths for the origin entities that have the shortest shortest paths and all shortest paths for all destination entities. When multiple entities are used, this option leads to longer computations. 
| AllOriginsAnyDestination| 2| The filtered find paths algorithm returns all shortest paths for all origin entities and the shortest paths for the destination entities that have the shortest shortest paths. When multiple entities are used, this option leads to longer computations. 
| AllOriginsAllDestinations| 3| The filtered find paths algorithm returns all shortest paths for all origin entities and all shortest paths for all destination entities. When multiple entities are used, this option leads to longer computations. 




## CIMFilteredFindPathsPathFilter
#### Represents a Knowledge Graph Filtered Find Paths Path Filter. A path filter can be used for a specific instance, in this case the ID has a value, or for all instances of a type, in this case the ID is null. 


### CIMFilteredFindPathsPathFilter 

|Property | Type | Description | 
|---------|--------|--------|
| ID | any | The id of the entity/relationship instance used for the path filter. If this id is null, then the path filter is used on all instances of the specified entity/relationship type. 
| itemTypeName | string | The type name of the entity/relationship (type or instance) used for the path filter. 
| itemType | [enumeration KGPathFilterItemType](CIMKnowledgeGraph.md#enumeration-kgpathfilteritemtype) | Whether the path filter is used for entities or relationships. 
| filterType | [enumeration KGPathFilterType](CIMKnowledgeGraph.md#enumeration-kgpathfiltertype) | The filter type of the path filter. 
| propertyFilterPredicate | string | The property filter predicate (cypher syntax) associated with the path filter. 






## CIMKGConsecutiveEventsRestrictions
#### Rules defining which "successor" events are allowed to be after a given "predecessor" event. One implied rule is that a successor event must start at or after the start of the predecessor event. These rules use the notions of "Gap" and "Overlap" defined hereunder. Definition of "Overlap": When the successor event start is before the predecessor event end, the overlap is the time from the successor event start to the predecessor event end. When the successor event start is after the predecessor event end, the overlap is zero. Definition of "Gap": When the successor event start is before the predecessor event end, the gap is zero. When the successor event start is after the predecessor event end, the gap is the time from the predecessor event end to the successor event start. 


### CIMKGConsecutiveEventsRestrictions 

|Property | Type | Description | 
|---------|--------|--------|
| restrictMaxOverlap | boolean | A value indicating whether the max overlap is restricted. 
| maxOverlap | double | The max overlap between consecutive events. The unit of this value is MaxOverlapUnit. This value is taken into account only if RestrictMaxOverlap is true. 
| maxOverlapUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The unit of MaxOverlap. Accepted values are { esriTimeUnitsMilliseconds, esriTimeUnitsSeconds, esriTimeUnitsMinutes, esriTimeUnitsHours, esriTimeUnitsDays, esriTimeUnitsWeeks }. 
| restrictMaxGap | boolean | A value indicating whether the max gap is restricted. 
| maxGap | double | The max gap. The unit of this value is MaxGapUnit. This value is taken into account only if RestrictMaxGap is true. 
| maxGapUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The unit of MaxGap. Accepted values are { esriTimeUnitsMilliseconds, esriTimeUnitsSeconds, esriTimeUnitsMinutes, esriTimeUnitsHours, esriTimeUnitsDays, esriTimeUnitsWeeks }. 





### Enumeration: KGDurativeEventMissingOneTimeBehaviour
#### Defines the behaviour when a durative event has a missing start or end time. 

|Property | Value | Description | 
|---------|--------|--------|
| Error| 0| Return an error. 
| Exclude| 1| Do not use the event in a path. 
| MakeNonEvent| 2| Consider the entity or relationship is not an event. 
| MakePunctualEvent| 3| Convert the durative event to a punctual event at the known time. 



### Enumeration: KGDurativeEventSwappedTimesBehaviour
#### Defines the behaviour when a durative event start time is after the end time. 

|Property | Value | Description | 
|---------|--------|--------|
| Error| 0| Return an error. 
| Exclude| 1| Do not use the event in a path. 
| MakeNonEvent| 2| Consider the entity or relationship is not an event. 
| MakeMinPunctualEvent| 3| Convert the durative event to a punctual event at the minimum time. 
| MakeMaxPunctualEvent| 4| Convert the durative event to a punctual event at the maximum time. 
| MakeDurativeEvent| 5| Swap start and end time so that start time is before end time. 




## CIMKGDurativeEventsDurationConstraint
#### Constraints on the duration of durative events. Note that this constraint does not apply to punctual events. 


### CIMKGDurativeEventsDurationConstraint 

|Property | Type | Description | 
|---------|--------|--------|
| timeUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The unit of minimum and maximum durations. Accepted values are { esriTimeUnitsMilliseconds, esriTimeUnitsSeconds, esriTimeUnitsMinutes, esriTimeUnitsHours, esriTimeUnitsDays, esriTimeUnitsWeeks }. 
| minDuration | double | The minimum duration. The unit of minimum duration is TimeUnit. 
| useMaxDuration | boolean | A value indicating whether the maximum duration should be used. 
| maxDuration | double | The maximum duration. The unit of maximum duration is TimeUnit. This value is only used if UseMaxDuration is true. 






## CIMKGEventDefinition
#### Events can be durative (with both start and end properties) or punctual (with just start or just end property). 


### CIMKGEventDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| namedType | string | The entity or relationship type name. 
| startProperty | string | The name of the property defining the start time of the event. 
| endProperty | string | The name of the property defining the end time of the event. 






## CIMKGEventErrorHandling
#### Defines the behaviours when event time(s) are missing or wrong. 


### CIMKGEventErrorHandling 

|Property | Type | Description | 
|---------|--------|--------|
| KGEventMissingAllTimesBehaviour | [enumeration KGEventMissingAllTimesBehaviour](CIMKnowledgeGraph.md#enumeration-kgeventmissingalltimesbehaviour) | The behaviour when an event has no time. 
| KGDurativeEventMissingOneTimeBehaviour | [enumeration KGDurativeEventMissingOneTimeBehaviour](CIMKnowledgeGraph.md#enumeration-kgdurativeeventmissingonetimebehaviour) | The behaviour when a durative event has one missing time. 
| KGDurativeEventSwappedTimesBehaviour | [enumeration KGDurativeEventSwappedTimesBehaviour](CIMKnowledgeGraph.md#enumeration-kgdurativeeventswappedtimesbehaviour) | The behaviour when a durative event has swapped times. 





### Enumeration: KGEventMissingAllTimesBehaviour
#### Defines the behaviour when a punctual or durative event has no time. 

|Property | Value | Description | 
|---------|--------|--------|
| Error| 0| Return an error. 
| Exclude| 1| Do not use the event in a path. 
| MakeNonEvent| 2| Consider the entity or relationship is not an event. 




## CIMKGEventsDefinitions
#### Defines which entities and relationships are "events". 


### CIMKGEventsDefinitions 

|Property | Type | Description | 
|---------|--------|--------|
| eventDefinitions | [[CIMKGEventDefinition]](CIMKnowledgeGraph.md#cimkgeventdefinition) | The list of CIMKGEventDefinition. 





### Enumeration: KGPathFilterItemType
#### Specifies whether the path filter is applied to an entity/entity type or a relationship/relationship type. 

|Property | Value | Description | 
|---------|--------|--------|
| Entity| 0| Path filter is applied to an entity or entity type. 
| Relationship| 1| Path filter is applied to a Relationship. 



### Enumeration: KGPathFilterType
#### Specifies the filter type of a path filter used in filtered find paths. 

|Property | Value | Description | 
|---------|--------|--------|
| IncludeOnly| 0| The filtered find paths algorithm will only consider paths which contain included types (type is active). If a path filter does not use the include only option, all types are active. 
| Exclude| 1| The filtered find paths algorithm will ignore paths that contain excluded types (type is not active). 
| MandatoryWaypoint| 2| The filtered find paths algorithm will only consider paths passing through the all the mandatory waypoints. 
| OptionalWaypoint| 3| The filtered find paths algorithm will only consider paths passing through at least one of the optional waypoints. 



### Enumeration: KGPathMode
#### Specifies whether the filtered find paths algorithm searches for all paths or only the shortest paths. 

|Property | Value | Description | 
|---------|--------|--------|
| Shortest| 0| The filtered find paths algorithm only searches for the shortest paths. 
| All| 1| The filtered find paths algorithm searches for all paths. 



### Enumeration: KGPathTimeFlow
#### Specifies the direction of time along the path. 

|Property | Value | Description | 
|---------|--------|--------|
| Forward| 0| Time flows forward. 
| Backward| 1| Time flows backward. 
| Unconstrained| 2| Time flows in any direction and can alternate. 




## CIMKGTimeFilter
#### Represents a Knowledge Graph Time Filter. 


### CIMKGTimeFilter 

|Property | Type | Description | 
|---------|--------|--------|
| enabled | boolean | A value indicating whether the filter is enabled. Note that having an empty list of event definitions is equivalent to not enabling the time filter, however since "Enable time filter" is a separate setting in the UI we have this member. 
| KGPathTimeFlow | [enumeration KGPathTimeFlow](CIMKnowledgeGraph.md#enumeration-kgpathtimeflow) | A value indicating how time should flow along the result paths. 
| timeWindow | [CIMKGTimeWindow](CIMKnowledgeGraph.md#cimkgtimewindow) | The time window. Any event that has a time span not intersecting the time window will be excluded. 
| eventsDefinitions | [CIMKGEventsDefinitions](CIMKnowledgeGraph.md#cimkgeventsdefinitions) | The events definitions. 
| durativeEventsDurationConstraint | [CIMKGDurativeEventsDurationConstraint](CIMKnowledgeGraph.md#cimkgdurativeeventsdurationconstraint) | The constraint on durative events duration. 
| eventErrorHandling | [CIMKGEventErrorHandling](CIMKnowledgeGraph.md#cimkgeventerrorhandling) | A value indicating how event data errors should be handled. 
| consecutiveEventsRestrictions | [CIMKGConsecutiveEventsRestrictions](CIMKnowledgeGraph.md#cimkgconsecutiveeventsrestrictions) | The consecutive events restrictions. 






## CIMKGTimeWindow
#### Defines a window of time. 


### CIMKGTimeWindow 

|Property | Type | Description | 
|---------|--------|--------|
| minTime | [TimestampOffset](ExternalReferences.md#timestampoffset) | The minimum time. Can be null if no minimum time exists. 
| maxTime | [TimestampOffset](ExternalReferences.md#timestampoffset) | The maximum time. Can be null if no maximum time exists. 






## CIMKGTraversalDirection
#### Represents a Knowledge Graph Filtered Find Paths TraversalDirection. The filtered find paths algorithm uses traversal directions to specify how relationships are traversed. When no traversal direction is defined for a specific relationship type, the default traversal direction is used. 


### CIMKGTraversalDirection 

|Property | Type | Description | 
|---------|--------|--------|
| relationshipTypeName | string | The relationship type name of the traversal direction object. 
| traversalDirectionType | [enumeration KGTraversalDirectionType](CIMKnowledgeGraph.md#enumeration-kgtraversaldirectiontype) | The traversal direction of the traversal direction object. 





### Enumeration: KGTraversalDirectionType
#### Specifies relationships traversal directions in the filtered find paths algorithm. 

|Property | Value | Description | 
|---------|--------|--------|
| Any| 0| The filtered find paths algorithm considers all relationships independent of their direction. 
| Forward| 1| The filtered find paths algorithm considers only the relationships that are traversed in forward direction. 
| Backward| 2| The filtered find paths algorithm considers only the relationships that are traversed in backward direction. 




## CIMKnowledgeGraphCoordinatePropertyValue
#### Represents a coordinate property value. 


### CIMKnowledgeGraphPropertyValue 

|Property | Type | Description | 
|---------|--------|--------|


### CIMKnowledgeGraphCoordinatePropertyValue 

|Property | Type | Description | 
|---------|--------|--------|
| fieldNames | [string] | The field names of this property value. 
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference of the coordinates. 
| interpretAsLongitudeLatitude | boolean | A value indicating whether the coordinate should be interpreted as long,lat (true) or lat,lon(false,default). This value only has meaning when the coordinate is ambiguous. For example, the coordinate "34N 22E" is not ambiguous as the latitude and longitude are both defined by the coordinate. However, "34 22" is ambiguous since it could mean either "34N 22E" or "34E 22N". In this situation the value of this property determines the recognized coordinate. 






## CIMKnowledgeGraphDataConnection
#### Represents a Knowledge Graph data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string | The workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory) | The workspace factory. 
| customWorkspaceFactoryCLSID | string | The classID of the custom workspace factory. 
| dataset | string | The dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype) | The dataset type. 


### CIMKnowledgeGraphDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| definitionQuery | string | The OpenCypher definition query. 






## CIMKnowledgeGraphDataLoadingConfiguration
#### Represents a Knowledge Graph Data Loading Configuration. 


### CIMKnowledgeGraphDataLoadingConfiguration 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the Data Loading Configuration. Names are expected to be unique within an Investigation. 
| entities | [[CIMKnowledgeGraphDataLoadingEntity]](CIMKnowledgeGraph.md#cimknowledgegraphdataloadingentity) | The entities. 
| relationships | [[CIMKnowledgeGraphDataLoadingRelationship]](CIMKnowledgeGraph.md#cimknowledgegraphdataloadingrelationship) | The relationships. 






## CIMKnowledgeGraphDataLoadingEntity
#### Represents a Knowledge Graph Data Loading Entity. 


### CIMKnowledgeGraphDataLoadingEntity 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the entity. 
| entityType | string | The type of the entity. 
| typeIsFieldName | boolean | A value indicating whether the Type property is a name itself or the name of a field. 
| entityTypeExpression | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The expression which is used to generate the entity type of this entity. This property takes precedence over the TypeIsFieldName and EntityType properties. If the EntityTypeExpression property is not null, the EntityType is generated from the script defined in the expression object. If the EntityTypeExpression property is null, the value of the EntityType property is interpreted based on the TypeIsFieldName property. 
| properties | [[CIMKnowledgeGraphProperty]](Types.md#knowledgegraphproperty) | The properties of this entity. 
| merge | boolean | A value indicating whether this entity should be merged. 






## CIMKnowledgeGraphDataLoadingRelationship
#### Represents a Knowledge Graph Data Loading Relationship. 


### CIMKnowledgeGraphDataLoadingRelationship 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the relationship. 
| sourceEntityName | string | The source entity name. 
| relationshipType | string | The type of the relationship. 
| typeIsFieldName | boolean | A value indicating whether the Type property is a name itself or the name of a field. 
| relationshipTypeExpression | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The expression which is used to generate the relationship type of this relationship. This property takes precedence over the TypeIsFieldName and RelationshipType properties. If the RelationshipTypeExpression is not null, the RelationshipType is generated from the script defined in the expression object. If the RelationshipTypeExpression is null, the value of the RelationshipType property is interpreted based on the TypeIsFieldName property. 
| targetEntityName | string | The target entity name. 
| properties | [[CIMKnowledgeGraphProperty]](Types.md#knowledgegraphproperty) | The properties of this relationship. 
| merge | boolean | A value indicating whether this relationship should be merged. 






## CIMKnowledgeGraphExpressionPropertyValue
#### Represents a property value from an expression. 


### CIMKnowledgeGraphPropertyValue 

|Property | Type | Description | 
|---------|--------|--------|


### CIMKnowledgeGraphExpressionPropertyValue 

|Property | Type | Description | 
|---------|--------|--------|
| expression | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The expression info of this property value. 






## CIMKnowledgeGraphFieldPropertyValue
#### Represents a property value from a specific import field. 


### CIMKnowledgeGraphPropertyValue 

|Property | Type | Description | 
|---------|--------|--------|


### CIMKnowledgeGraphFieldPropertyValue 

|Property | Type | Description | 
|---------|--------|--------|
| fieldName | string | The field name of this property value. 






## CIMKnowledgeGraphFixedPropertyValue
#### Represents a fixed string property value. 


### CIMKnowledgeGraphPropertyValue 

|Property | Type | Description | 
|---------|--------|--------|


### CIMKnowledgeGraphFixedPropertyValue 

|Property | Type | Description | 
|---------|--------|--------|
| fixedValue | string | The fixed value of this property value. 






## CIMKnowledgeGraphIDPropertyValue
#### Represents the ID property value from a specific CIMKnowledgeGraphDataLoadingEntity or CIMKnowledgeGraphDataLoadingRelationship. 


### CIMKnowledgeGraphPropertyValue 

|Property | Type | Description | 
|---------|--------|--------|


### CIMKnowledgeGraphIDPropertyValue 

|Property | Type | Description | 
|---------|--------|--------|
| dataLoadingItemName | string | The name of a CIMKnowledgeGraphDataLoadingEntity or CIMKnowledgeGraphDataLoadingRelationship. 






## CIMKnowledgeGraphInvestigation
#### Represents a Knowledge Graph Investigation. 


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


### CIMKnowledgeGraphInvestigation 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| dataLoadingConfigurations | [[CIMKnowledgeGraphDataLoadingConfiguration]](CIMKnowledgeGraph.md#cimknowledgegraphdataloadingconfiguration) | The array of Data Loading Configurations referenced by this Investigation. All configurations are expected to have unique names. 
| searchDefinitions | [[CIMKnowledgeGraphSearchDefinition]](CIMKnowledgeGraph.md#cimknowledgegraphsearchdefinition) | The array of search definitions referenced by this Investigation. All search definitions are expected to have unique names. 
| queryDefinitions | [[CIMKnowledgeGraphQueryDefinition]](CIMKnowledgeGraph.md#cimknowledgegraphquerydefinition) | The array of query definitions referenced by this Investigation. All query definitions are expected to have unique names. 
| filteredFindPathsConfigurations | [[CIMFilteredFindPathsConfiguration]](CIMKnowledgeGraph.md#cimfilteredfindpathsconfiguration) | The array of Filtered Find Paths Configurations referenced by this Investigation. All configurations are expected to have unique names. 
| typeInfos | [[CIMKnowledgeGraphInvestigationTypeInfo]](CIMKnowledgeGraph.md#cimknowledgegraphinvestigationtypeinfo) | The array of Knowledge Graph Investigation Type Infos referenced by this Investigation. All infos are expected to have unique type names. 






## CIMKnowledgeGraphInvestigationTypeInfo
#### Represents a Knowledge Graph Investigation Type Info. 


### CIMKnowledgeGraphInvestigationTypeInfo 

|Property | Type | Description | 
|---------|--------|--------|
| typeName | string | The name of the type. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 






## CIMKnowledgeGraphLayer
#### Provides access to properties of a Knowledge Graph layer. 


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


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The URIs of the layers used as masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| layerScaleVisibilityOptions | [CIMLayerScaleVisibilityOptions](CIMLayer.md#cimlayerscalevisibilityoptions) | The layer's scale visibility options. 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 
| enableLayerEffects | boolean | A value indicating whether to enable any type of effects on the layer. 
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. 


### CIMStandaloneTableContainer 

|Property | Type | Description | 
|---------|--------|--------|
| standaloneTables | [string] | The standalone tables as an array of table repository paths. 


### CIMKnowledgeGraphLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| layers | [string] | The layer URIs of the layers in the composite layer. 






## CIMKnowledgeGraphLinkChartCentralityConfiguration
#### Represents the Centrality computation options in a Knowledge Graph Link Chart. 


### CIMKnowledgeGraphLinkChartCentralityConfiguration 

|Property | Type | Description | 
|---------|--------|--------|
| relationshipsInterpretation | [enumeration CentralityRelationshipInterpretation](CIMKnowledgeGraph.md#enumeration-centralityrelationshipinterpretation) | The relationships interpretation. 
| multiedgeFactor | double | The multiedge factor. Acceptable values lie in [0, 1]. In centrality computations, each multiple edge is reduced to a single edge with a weight of: '(1 - MultiedgeFactor) + "count of edges in the multiple edge" * MultiedgeFactor'. Hence, if MultiedgeFactor is 0, the weight is 1, and if MultiedgeFactor is 1, the weight is "count edges in multiedge". 
| normalization | [enumeration CentralityScoresNormalization](CIMKnowledgeGraph.md#enumeration-centralityscoresnormalization) | The scores normalization. 






## CIMKnowledgeGraphLinkChartProperties
#### Represents a Knowledge Graph Link Chart Properties object. 


### CIMKnowledgeGraphLinkChartProperties 

|Property | Type | Description | 
|---------|--------|--------|
| nodesURI | string | The URI of the binary reference containing a serialized representation of the internal Nodes table. 
| linksURI | string | The URI of the binary reference containing a serialized representation of the internal Links table. 
| aggregatedNodesURI | string | The URI of the binary reference containing a serialized representation of the internal AggregatedNodes table. 
| aggregatedLinksURI | string | The URI of the binary reference containing a serialized representation of the internal AggregatedLinks table. 
| autoCollapseRelationships | boolean | A value indicating whether this Link Chart automatically collapses eligible relationships. 
| centralityConfiguration | [CIMKnowledgeGraphLinkChartCentralityConfiguration](CIMKnowledgeGraph.md#cimknowledgegraphlinkchartcentralityconfiguration) | The Configuration for Centrality computation in this Link Chart. Centrality scores found in the Nodes and AggregatedNodes tables were computed using this Configuration. 
| centralityIsUpToDate | boolean | A value indicating whether the Centrality scores found in the Nodes and AggregatedNodes tables were computed using the current Link Chart topology. 
| lastUsedLayout | [CIMKnowledgeLinkChartLayout](CIMKnowledgeGraph.md#cimknowledgelinkchartlayout) | Information about the last used layout. 






## CIMKnowledgeGraphNonspatialProperty
#### Represents a Knowledge Graph Data Loading Property used by entities and relationships. 


### CIMKnowledgeGraphProperty 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the property. 
| propertyType | [enumeration esriFieldType](ExternalReferences.md#enumeration-esrifieldtype) | The type of the property. 
| value | [KnowledgeGraphPropertyValue](Types.md#knowledgegraphpropertyvalue) | The value which is to be imported. Value will have to be tested for type in order to properly perform the import. 
| merge | boolean | A value indicating whether this property should be used to determine a merge. 


### CIMKnowledgeGraphNonspatialProperty 

|Property | Type | Description | 
|---------|--------|--------|






## CIMKnowledgeGraphQueryDefinition
#### Represents a Knowledge Graph Query Definition. 


### CIMKnowledgeGraphQueryDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | User defined name for open cypher query. 
| openCypherQuery | string | User defined open cypher query. 
| provenanceBehavior | [enumeration ProvenanceBehavior](CIMKnowledgeGraph.md#enumeration-provenancebehavior) | The query behavior for Provenance. 






## CIMKnowledgeGraphSearchDefinition
#### Represents a Knowledge Graph Search Definition. 


### CIMKnowledgeGraphSearchDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | User defined name for search. 
| searchString | string | User defined search string. Search string is based on Lucene syntax. 
| filterSetting | [CIMKnowledgeGraphSearchFilterSetting](CIMKnowledgeGraph.md#cimknowledgegraphsearchfiltersetting) | Search filter setting. 





### Enumeration: KnowledgeGraphSearchFilterScope
#### Specifies the scope to restrict search. 

|Property | Value | Description | 
|---------|--------|--------|
| Entities| 1| Search only in entities. 
| Relationships| 2| Search only in relationships. 
| BothEntitiesAndRelationships| 3| Search in entities and relationships. 
| Provenance| 4| Search in provenance. 




## CIMKnowledgeGraphSearchFilterSetting
#### Represents a Knowledge Graph Search Filter Setting. 


### CIMKnowledgeGraphSearchFilterSetting 

|Property | Type | Description | 
|---------|--------|--------|
| scope | [enumeration KnowledgeGraphSearchFilterScope](CIMKnowledgeGraph.md#enumeration-knowledgegraphsearchfilterscope) | The scope of search. 
| typeNames | [string] | The name of types to be included in search filter. 






## CIMKnowledgeGraphSpatialProperty
#### Represents a Spatial Knowledge Graph Data Loading Property used for entities. This class is expected to be used only when the Type of property is esriFieldTypeGeometry. 


### CIMKnowledgeGraphProperty 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the property. 
| propertyType | [enumeration esriFieldType](ExternalReferences.md#enumeration-esrifieldtype) | The type of the property. 
| value | [KnowledgeGraphPropertyValue](Types.md#knowledgegraphpropertyvalue) | The value which is to be imported. Value will have to be tested for type in order to properly perform the import. 
| merge | boolean | A value indicating whether this property should be used to determine a merge. 


### CIMKnowledgeGraphSpatialProperty 

|Property | Type | Description | 
|---------|--------|--------|
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference of the property. 
| geometryType | [enumeration esriGeometryType](ExternalReferences.md#enumeration-esrigeometrytype) | The geometry type of the property. Currently, only allowed values: - esriGeometryPoint - esriGeometryMultipoint - esriGeometryPolyline - esriGeometryPolygon Others will be allowed in future. 






## CIMKnowledgeGraphTableDataConnection
#### Represents a Knowledge Graph data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string | The workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory) | The workspace factory. 
| customWorkspaceFactoryCLSID | string | The classID of the custom workspace factory. 
| dataset | string | The dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype) | The dataset type. 


### CIMKnowledgeGraphDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| definitionQuery | string | The OpenCypher definition query. 


### CIMKnowledgeGraphTableDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| inclusionSetURI | string | The URI of the binary reference containing the InclusionSet for the table. 






## CIMKnowledgeLinkChartLayout
#### Represents a Knowledge Link Chart Layout Info object. 


### CIMKnowledgeLinkChartLayout 

|Property | Type | Description | 
|---------|--------|--------|
| algorithm | [enumeration KnowledgeLinkChartLayoutAlgorithm](CIMKnowledgeGraph.md#enumeration-knowledgelinkchartlayoutalgorithm) | The layout algorithm. 





### Enumeration: KnowledgeLinkChartLayoutAlgorithm
#### Specifies a Knowledge Link Chart layout algorithm. 

|Property | Value | Description | 
|---------|--------|--------|
| Organic_Standard| 0| Organic Standard. 
| Organic_LeafCircle| 1| Organic Leaf Circle. 
| Organic_Fusiform| 2| Organic Fusiform. 
| Organic_Community| 3| Organic Community. 
| Geographic_Organic_Standard| 4| A Geographic layout that positions entities geographically using their geometry. Spatial entities that have a null geometry and non-spatial entities are arranged using the Organic Standard layout. 
| Basic_Grid| 5| Basic Grid. 
| Tree_LeftToRight| 6| Tree Left To Right. 
| Tree_RightToLeft| 7| Tree Right To Left. 
| Tree_TopToBottom| 8| Tree Top To Bottom. 
| Tree_BottomToTop| 9| Tree Bottom To Top. 
| Radial_RootCentric| 10| Radial Root Centric. 
| Radial_NodeCentric| 11| Radial Node Centric. 
| Hierarchical_TopToBottom| 12| Hierarchical Top To Bottom. 
| Hierarchical_BottomToTop| 13| Hierarchical Bottom To Top. 




## CIMLinkChartFeatureLayer
#### Represents a Link Chart Feature Layer. 


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


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The URIs of the layers used as masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| layerScaleVisibilityOptions | [CIMLayerScaleVisibilityOptions](CIMLayer.md#cimlayerscalevisibilityoptions) | The layer's scale visibility options. 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 
| rasterizeOnExport | boolean | A value indicating whether layer should be rasterized when exporting. 
| useVisibilityTimeExtent | boolean | A value indicating whether or not to use the visibility time extent. When true the map time must overlap the visibility time extent for the layer to be visible. 
| visibilityTimeExtent | [TimeExtent](ExternalReferences.md#timeextent) | The visibility time extent. 
| enableLayerEffects | boolean | A value indicating whether to enable any type of effects on the layer. 
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. 


### CIMFeatureLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| autoGenerateFeatureTemplates | boolean | A value indicating whether to automatically generate feature templates from the renderer. 
| extrusion | [CIMFeatureExtrusion](CIMVectorLayers.md#cimfeatureextrusion) | The feature extrusion. 
| featureElevationExpression | string | The feature elevation expression. 
| featureTable | [CIMFeatureTable](CIMVectorLayers.md#cimfeaturetable) | The feature table. 
| featureTemplates | [[CIMEditingTemplate]](Types.md#editingtemplate) | The feature templates. 
| htmlPopupEnabled | boolean | A value indicating whether HTML pop-ups are enabled. 
| htmlPopupFormat | [CIMHtmlPopupFormat](CIMVectorLayers.md#cimhtmlpopupformat) | The HTML pop-ups format. 
| isFlattened | boolean | A value indicating whether the layer is flattened. 
| selectable | boolean | A value indicating whether the layer is selectable. 
| selectionColor | [Color](Types.md#color) | The selection color. For polygons, this is used as the outline color. 
| polygonSelectionFillColor | [Color](Types.md#color) | The selection fill color. Only used for polygons. 
| selectionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The selection symbol. 
| useSelectionSymbol | boolean | A value indicating whether to use the selection symbol. 
| pageDefinition | [CIMPageDefinition](CIMVectorLayers.md#cimpagedefinition) | The page definition which allows for using current map series page to filter features. 
| featureCacheType | [enumeration FeatureCacheType](CIMVectorLayers.md#enumeration-featurecachetype) | The feature cache type. 
| enableDisplayFilters | boolean | A value indicating whether the current set of display filters are honored during drawing. 
| displayFilters | [[CIMDisplayFilter]](CIMVectorLayers.md#cimdisplayfilter) | The current set of scale based display filters. 
| displayFiltersType | [enumeration DisplayFilterType](CIMVectorLayers.md#enumeration-displayfiltertype) | DisplayFiltersType value. 
| displayFilterName | string | The active display filter. 
| displayFilterChoices | [[CIMDisplayFilter]](CIMVectorLayers.md#cimdisplayfilter) | The current set of display filters. 
| featureElevationExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The expression for setting the feature elevation. 
| featureBlendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The per-feature blending mode which allows features in a layer to blend against other features in the same layer that have already drawn. 
| featureSortInfos | [[CIMFeatureSortInfo]](CIMVectorLayers.md#cimfeaturesortinfo) | The collection of field names and sort directions used to sort features during draw. 
| layerEffectsMode | [enumeration LayerEffectsMode](CIMLayer.md#enumeration-layereffectsmode) | The layer effects mode. 
| featureEffects | [CIMFeatureLayerEffect](CIMLayer.md#cimfeaturelayereffect) | The collection of layer effects that apply to subset of features. 


### CIMGeoFeatureLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| actions | [[CIMLayerAction]](CIMVectorLayers.md#cimlayeraction) | The layer actions. 
| exclusionSet | [long long] | The set of excluded features. 
| featureMasks | [[CIMDataConnection]](Types.md#dataconnection) | The data connection of the masking data. 
| labelClasses | [[CIMLabelClass]](CIMLabelPlacement.md#cimlabelclass) | The collection of label class definitions. 
| labelVisibility | boolean | A value indicating whether to display labels for this layer's label classes. 
| maskedSymbolLayers | [[CIMSymbolLayerMasking]](CIMVectorLayers.md#cimsymbollayermasking) | The masked symbol layers. Each SymbolLayerMasking gives the symbol layers that are masked by that masking layer. 
| renderer | [Renderer](Types.md#renderer) | The primary symbol renderer. 
| scaleSymbols | boolean | A value indicating whether to scale the symbols in this layer based on the map's reference scale. 
| snappable | boolean | A value indicating whether this layer participates in snapping in the editor. 
| symbolLayerDrawing | [CIMSymbolLayerDrawing](CIMLayer.md#cimsymbollayerdrawing) | The symbol layer drawing properties. 
| trackLinesRenderer | [Renderer](Types.md#renderer) | The track renderer when displaying tracks. 
| previousObservationsRenderer | [Renderer](Types.md#renderer) | The previous observations renderer. 
| previousObservationsCount | long | The previous observation count. 
| useRealWorldSymbolSizes | boolean | A value indicating whether to use real world symbols sizes (meters) vs. points. This value should always be in sync with the UseRealWorldSymbolSizes property at the symbol level. 
| showPreviousObservations | boolean | A value indicating whether previous observations are being drawn. 
| featureReduction | [FeatureReduction](Types.md#featurereduction) | The feature reduction technique in use by this layer. 
| showTracks | boolean | A value indicating whether track lines are being drawn. 


### CIMLinkChartFeatureLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| aggregationLayerURI | string | The layer URI of the aggregation layer. 





### Enumeration: ProvenanceBehavior
#### Controls query behavior with respect to the Provenance Entity Type. 

|Property | Value | Description | 
|---------|--------|--------|
| Exclude| 0| Query behaves as if there were no Provenance records in the graph, nor Provenance Entity Type defined in the data model. 
| Include| 1| Query can reference the Provenance Entity Type. The result set may return provenance records. 

