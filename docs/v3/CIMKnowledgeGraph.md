

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



### Enumeration: EventsTicksVisualization
#### Represents how events ticks are displayed. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Events ticks are not shown. 
| StartOnly| 1| Only start ticks are shown. 
| StartAndEnd| 2| Start and End ticks are shown. 



### Enumeration: FFPConfigurationWarning
#### Describes Filtered Find Paths configuration warnings. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No warning. 
| AllOriginsAreExcluded| 1| All origin entities are excluded, hence no path will be found. 
| AllDestinationsAreExcluded| 2| All destination entities are excluded, hence no path will be found. 
| AllOptionalWaypointsAreExcluded| 3| All optional waypoints are excluded, hence no path will be found. 
| AtLeastOneMandatoryEntityWaypointIsExcluded| 4| At least one mandatory entity waypoint is excluded, hence no path will be found. 
| AtLeastOneMandatoryRelationshipWaypointIsExcluded| 5| At least one mandatory relationship waypoint is excluded, hence no path will be found. 
| ReachedMaxPathLength| 6| No path was found, but increasing or disabling the max path length could help find some paths. 




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
| maxCountPaths | long | The max number of paths the filtered find paths algorithm returns. This parameter is only taken into account when PathMode is KGPathMode.All. 
| timeFilter | [CIMKGTimeFilter](CIMKnowledgeGraph.md#cimkgtimefilter) | The time filter. 






## CIMFilteredFindPathsEntity
#### When the ID property has a value, represents a single entity. When the ID property is null, represents entities of a given entity type, filtered by PropertyFilterPredicate if it is not empty. 


### CIMFilteredFindPathsEntity 

|Property | Type | Description | 
|---------|--------|--------|
| ID | any | The id of the entity instance used as a origin/destination entity. If this id is null, then the filtered find paths algorithm uses all instances of the specified entity type. 
| entityTypeName | string | The type name of the entity (type or instance) used as an origin/destination entity. 
| propertyFilterPredicate | string | The property filter predicate (openCypher syntax) associated with the path filter. The predicate is only taken into account when ID has no value. 





### Enumeration: FilteredFindPathsEntityUsage
#### Specifies how origin/destination entities are used in the filtered find paths algorithm. 

|Property | Value | Description | 
|---------|--------|--------|
| AnyOriginAnyDestination| 0| The filtered find paths algorithm only returns the shortest paths for the origin entities that have the shortest shortest paths and the shortest paths for the destination entities that have the shortest shortest paths. When multiple entities are used, this option leads to faster computations. 
| AnyOriginAllDestinations| 1| The filtered find paths algorithm returns the shortest paths for the origin entities that have the shortest shortest paths and one shortest path (if it exists) per destination entity. When multiple entities are used, this option leads to longer computations. 
| AllOriginsAnyDestination| 2| The filtered find paths algorithm returns one shortest path (if it exists) per origin entity and the shortest paths for the destination entities that have the shortest shortest paths. When multiple entities are used, this option leads to longer computations. 
| AllOriginsAllDestinations| 3| The filtered find paths algorithm returns one shortest path (if it exists) per origin entity and one shortest path (if it exists) per destination entity. When multiple entities are used, this option leads to longer computations. 
| EachPair| 4| The filtered find paths algorithm returns one shortest path (if it exists) per pair of origin and destination entity. When multiple entities are used, this option leads to longer computations. An error will be returned if strictly more than 10 origin entities are defined or if strictly more than 10 destination entities are defined. 




## CIMFilteredFindPathsError
#### Represents an error of a Filtered Find Paths search. 


### CIMFilteredFindPathsError 

|Property | Type | Description | 
|---------|--------|--------|
| error | [enumeration KGPathFindingError](CIMKnowledgeGraph.md#enumeration-kgpathfindingerror) | The error. 
| detailedErrorMessage | string | The detailed error message. This string may or may not be internationalized. 






## CIMFilteredFindPathsPathFilter
#### Represents a Knowledge Graph Filtered Find Paths Path Filter. A path filter can be used for a specific instance, in this case the ID has a value, or for all instances of a type, in this case the ID is null. 


### CIMFilteredFindPathsPathFilter 

|Property | Type | Description | 
|---------|--------|--------|
| ID | any | The id of the entity/relationship instance used for the path filter. If this id is null, then the path filter is used on all instances of the specified entity/relationship type. 
| itemTypeName | string | The type name of the entity/relationship (type or instance) used for the path filter. 
| itemType | [enumeration KGPathFilterItemType](CIMKnowledgeGraph.md#enumeration-kgpathfilteritemtype) | Whether the path filter is used for entities or relationships. 
| filterType | [enumeration KGPathFilterType](CIMKnowledgeGraph.md#enumeration-kgpathfiltertype) | The filter type of the path filter. 
| propertyFilterPredicate | string | The property filter predicate (openCypher syntax) associated with the path filter. The predicate is only taken into account when ID has no value. 






## CIMFilteredFindPathsResult
#### Represents results of a Filtered Find Paths search. 


### CIMFilteredFindPathsResult 

|Property | Type | Description | 
|---------|--------|--------|
| error | [CIMFilteredFindPathsError](CIMKnowledgeGraph.md#cimfilteredfindpathserror) | The error. An error occurred if this object is not null. 
| configurationWarning | [enumeration FFPConfigurationWarning](CIMKnowledgeGraph.md#enumeration-ffpconfigurationwarning) | The configuration warning. When no path has been found, and the value is different from FFPConfigurationWarning.None, it is likely that the user made an unintended mistake in the configuration. 
| statistics | [CIMFilteredFindPathsStatistics](CIMKnowledgeGraph.md#cimfilteredfindpathsstatistics) | The statistics of the Filtered Find Paths search. 
| paths | [CIMKGPaths](CIMKnowledgeGraph.md#cimkgpaths) | The paths found by the Filtered Find Paths search. 






## CIMFilteredFindPathsStatistics
#### Represents the statistics related to a Filtered Find Paths search. It contains the size of the local graph, and the number of openCypher "expansion" queries that have been issued to construct the local graph. The local graph is an in-memory graph used for pathfinding where a node represents an entity in the Knowledge Graph and an edge represents one or many parallel relationships in the Knowledge Graph. The local graph typically contains (much) less nodes than the Knowledge Graph, but enough nodes and edges to ensure that the pathfinding results are accurate. For example, to guarantee that all paths of length up to 'L' between 'A' and 'B' are present in the local graph, we ensure that the sum of counts of "expansion" queries related to 'A' and 'B' is greater or equal to 'L'. 


### CIMFilteredFindPathsStatistics 

|Property | Type | Description | 
|---------|--------|--------|
| countLocalGraphNodes | long long | The count of nodes in the local graph. 
| countLocalGraphEdges | long long | The count of edges in the local graph. 
| countOriginExpansionQueries | long long | The count of expansion queries that were done to discover the neighborhood of some origin entities. 
| countDestinationExpansionQueries | long long | The count of expansion queries that were done to discover the neighborhood of some destination entities. 
| countWaypointsExpansionQueries | long long | The count of expansion queries that were done to discover the neighborhood of entity or relationship waypoints. 






## CIMKGColorInfo
#### Represents a Knowledge Graph Color Info. 


### CIMKGColorInfo 

|Property | Type | Description | 
|---------|--------|--------|
| useCustomColors | boolean | A value indicating whether the parent type is rendered using its custom colors. 
| defaultItemColor | [Color](Types.md#color) | The default item color of the parent type. 
| defaultTextColor | [Color](Types.md#color) | The default text color of the parent type. 
| customItemColor | [Color](Types.md#color) | The custom color of the parent type. 
| customTextColor | [Color](Types.md#color) | The custom text color of the parent type. 






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






## CIMKGDataModelVisualization
#### Represents a Knowledge Graph Data Model Visualization. 


### CIMKGDataModelVisualization 

|Property | Type | Description | 
|---------|--------|--------|
| configurationName | string | The name of the Data Model Visualization. Names are expected to be unique within an Investigation. 
| entityTypes | [[CIMKGEntityType]](CIMKnowledgeGraph.md#cimkgentitytype) | The configured entity types. 
| relationshipTypes | [[CIMKGRelationshipType]](CIMKnowledgeGraph.md#cimkgrelationshiptype) | The configured relationship types. 






## CIMKGDiagramPosition
#### Represents a Knowledge Graph Diagram Position. 


### CIMKGDiagramPosition 

|Property | Type | Description | 
|---------|--------|--------|
| x | double | The x position within a diagram. 
| y | double | The y position within a diagram. 





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






## CIMKGEntityType
#### Represents a Knowledge Graph Entity Type. 


### CIMKGType 

|Property | Type | Description | 
|---------|--------|--------|
| typeName | string | The name of the type. 
| geometryType | [enumeration esriGeometryType](ExternalReferences.md#enumeration-esrigeometrytype) | The geometry type of the type. 
| properties | [[CIMKGTypeProperty]](CIMKnowledgeGraph.md#cimkgtypeproperty) | The properties of the type. 
| colorInfo | [CIMKGColorInfo](CIMKnowledgeGraph.md#cimkgcolorinfo) | The color information for the type. 


### CIMKGEntityType 

|Property | Type | Description | 
|---------|--------|--------|
| diagramPosition | [CIMKGDiagramPosition](CIMKnowledgeGraph.md#cimkgdiagramposition) | The diagram position of the entity. 






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



### Enumeration: KGPathFindingError
#### Describes errors related to the time value(s) of a time event. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No error. 
| ConfigurationHasTooManyInputEntities| 1| The configuration has too many input entities. 
| ConfigurationIsTooComplex| 2| The configuration is too complex, this generally occurs when too many mandatory waypoints are defined. 
| PunctualEventHasNoTime| 3| A punctual event has a null time. 
| DurativeEventHasNoTime| 4| A durative event has a null start time and a null end time. 
| DurativeEventHasOneMissingTime| 5| A durative event has either a null start time or a null end time. 
| DurativeEventHasSwappedTimes| 6| A durative event start time is strictly greater than the end time. 



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




## CIMKGPaths
#### Represents the paths found by the Filtered Find Paths search. We use a memory-optimized representation to avoid storing redundant information because it is often the case that a path shares some entities and relationships with many other paths, especially if the Filtered Find Paths configuration uses 'KGPathMode.All'. Definition: a relationship group contains Knowledge Graph relationships associated to a single edge in the local graph. Paths are encoded this way: The path 'p' uses relationships groups PathsBuffer[PathsEndIndex[p-1] .. PathsEndIndex[p]], and: - the origin of the first relationship group is the origin of the path - the destination of the last relationship group is the destination of the path A path of length zero (with entity 'e') has a single relationship group containing no relationship and where the origin and the destination are 'e'. The relationships group 'g' has origin EntitiesUIDs[RelationshipsGroupsFrom[g]] and destination EntitiesUIDs[RelationshipsGroupsTo[g]]. Its relationships are RelationshipsGroupsUIDsBuffer[RelationshipsGroupsUIDsEndIndex[g-1] .. RelationshipsGroupsUIDsEndIndex[g]] if RelationshipsFrom[i] >= 0, relationship RelationshipsGroupsUIDsBuffer[i] has origin EntitiesUIDs[RelationshipsFrom[i]] else the relationship has been deleted after pathfinding. if RelationshipsTo[i] >= 0, relationship RelationshipsGroupsUIDsBuffer[i] has destination EntitiesUIDs[RelationshipsTo[i]] else the relationship has been deleted after pathfinding. Note that origin and destination of a relationship may not match origin and destination of the relationship group because the relationship can be traversed backwards. 


### CIMKGPaths 

|Property | Type | Description | 
|---------|--------|--------|
| entitiesUIDs | [[any]]| The list of entities that may be used in paths (not all entities are guaranteed to be used). 
| entityTypes | [long long] | A list parallel to EntitiesUIDs representing entity type indices. if EntityTypes[i] >= 0, EntitiesUIDs[i] has type IndexedEntityTypes[EntityTypes[i]] else the entity has been deleted after the find path operation. 
| indexedEntityTypes | [string] | The list of entity types, indexed by 'EntityTypes'. 
| relationshipsGroupsUIDsBuffer | [[any]]| The list of relationships that may be used in paths (not all relationships are guaranteed to be used). The list may contain duplicate elements. 
| relationshipTypes | [long long] | A list parallel to RelationshipsGroupsUIDsBuffer representing relationship type indices. if RelationshipTypes[i] >= 0, RelationshipsGroupsUIDsBuffer[i] has type IndexedRelationshipTypes[RelationshipTypes[i]] else the relationship has been deleted after the find path operation. 
| indexedRelationshipTypes | [string] | The list of relationship types, indexed by 'RelationshipTypes'. 
| relationshipsGroupsUIDsEndIndex | [long long] | The list of relationships groups relationship end indices (indexes into 'RelationshipsGroupsUIDsBuffer'). Values must be positive. 
| relationshipsGroupsFrom | [long long] | The list of relationships groups origin entity index (indexes into 'EntitiesUIDs'). Values must be positive. 
| relationshipsGroupsTo | [long long] | The list of relationships groups destination entity index (indexes into 'EntitiesUIDs'). Values must be positive. 
| relationshipsFrom | [long long] | The list of relationships origin entity index (indexes into 'EntitiesUIDs'). 
| relationshipsTo | [long long] | The list of relationships destination entity index (indexes into 'EntitiesUIDs'). 
| pathsBuffer | [long long] | The list of relationships groups indices used by paths. Values must be positive. 
| pathsEndIndex | [long long] | The list of paths relationships groups end indices (indexes into 'PathsBuffer'). Values must be positive. 






## CIMKGRelationshipType
#### Represents a Knowledge Graph Relationship Type. 


### CIMKGType 

|Property | Type | Description | 
|---------|--------|--------|
| typeName | string | The name of the type. 
| geometryType | [enumeration esriGeometryType](ExternalReferences.md#enumeration-esrigeometrytype) | The geometry type of the type. 
| properties | [[CIMKGTypeProperty]](CIMKnowledgeGraph.md#cimkgtypeproperty) | The properties of the type. 
| colorInfo | [CIMKGColorInfo](CIMKnowledgeGraph.md#cimkgcolorinfo) | The color information for the type. 


### CIMKGRelationshipType 

|Property | Type | Description | 
|---------|--------|--------|
| endpoints | [[CIMKGRelationshipTypeEndpoint]](CIMKnowledgeGraph.md#cimkgrelationshiptypeendpoint) | The relationship types' endpoints. 






## CIMKGRelationshipTypeEndpoint
#### Represents a Knowledge Graph Relationship Type Endpoint. 


### CIMKGRelationshipTypeEndpoint 

|Property | Type | Description | 
|---------|--------|--------|
| originEntityTypeName | string | The name of the entity type the relationship type is connected to on its origin side. 
| destinationEntityTypeName | string | The name of the entity type the relationship type is connected to on its destination side. 






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




## CIMKGTypeProperty
#### Represents a Knowledge Graph Type Property. It is primarily used to configure a property of an entity type or a relationship type within the data model visualization view. 


### CIMKGTypeProperty 

|Property | Type | Description | 
|---------|--------|--------|
| propertyName | string | The name of the property. 
| propertyType | [enumeration esriFieldType](ExternalReferences.md#enumeration-esrifieldtype) | The type of the type property. 
| aliasName | string | The alias name of the property. 
| isNullable | boolean | A value indicating whether the property can be null. 
| defaultVisibility | boolean | A value indicating whether the property is visible by default. 
| editable | boolean | A value indicating whether the property is editable. 
| domainName | string | The domain associated with the property. 
| defaultValue | any | The default value for the property. 






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
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the investigation. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| dataModelVisualizations | [[CIMKGDataModelVisualization]](CIMKnowledgeGraph.md#cimkgdatamodelvisualization) | The array of Data Model Visualizations referenced by this Investigation. All Data Model Visualizations are expected to have unique names. 






## CIMKnowledgeGraphInvestigationTypeInfo
#### Represents a Knowledge Graph Investigation Type Info. 


### CIMKnowledgeGraphInvestigationTypeInfo 

|Property | Type | Description | 
|---------|--------|--------|
| typeName | string | The name of the type. 
| popupInfo | [CIMPopupInfo](CIMPopup.md#cimpopupinfo) | The pop-up info. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol for the type. 
| displayExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The expression information used to create the display name for members of the type. 
| propertyInfos | [[CIMKnowledgeGraphTypePropertyInfo]](CIMKnowledgeGraph.md#cimknowledgegraphtypepropertyinfo) | The array of Knowledge Graph Type Property Infos. All infos are expected to have unique property name. 






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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


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
#### Represents the Centrality computation options in a Knowledge Graph Link Chart. Several measures of centrality are supported: Degree, Indegree, Outdegree, PageRank, Eigenvector, Betweenness, Closeness and Harmonic. These measures fall in two broad categories: degree based measures are Degree, Indegree, Outdegree, PageRank, and Eigenvector while shortest paths based measures are Betweenness, Closeness and Harmonic. The "importance" relationship weight is taken into account in degree based measures: a relationship with higher importance will increase the centrality scores of nearby related entities. The "cost" relationship weight is taken into account in shortest paths based measures: a relationship with higher cost will decrease the centrality scores of nearby related entities. 


### CIMKnowledgeGraphLinkChartCentralityConfiguration 

|Property | Type | Description | 
|---------|--------|--------|
| relationshipsInterpretation | [enumeration CentralityRelationshipInterpretation](CIMKnowledgeGraph.md#enumeration-centralityrelationshipinterpretation) | The relationships interpretation. 
| computeShortestPathsBasedMeasures | boolean | A value indicating whether the shortest paths based measures will be computed. This setting exists because shortest paths based measures can be costly to compute for larger link charts. 
| includeDocumentEntities | boolean | A value indicating whether entities of type 'Document' are considered to be part of the graph for centrality computations. 
| defaultRelationshipImportance | double | The default importance of a relationship. 
| relationshipImportanceProperty | string | The property defining the importance of a relationship. When the string is empty, or the property doesn't exist, or the property value is null, the default relationship importance is used instead. Negative property values are ignored and replaced by zero. 
| defaultRelationshipCost | double | The default cost of a relationship. 
| relationshipCostProperty | string | The property defining the cost of a relationship. When the string is empty, or the property doesn't exist, or the property value is null, the default relationship cost is used instead. Negative property values are ignored and replaced by zero. 
| multiedgeFactor | double | The multiedge factor. Acceptable values lie in [0, 1]. In centrality computations, we reduce parallel relationships of a graph to a single edge. The computation of the importance of the single edge depends on the value of MultiedgeFactor. If MultiedgeFactor is 0, the importance of the single edge is the average of parallel relationships. If MultiedgeFactor is 1, the importance of the single edge is the sum of importances of parallel relationships. For values of MultiedgeFactor between 0 and 1, the importance of the single edge is linearly interpolated. 
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
| nonspatialDataDisplay | [CIMKnowledgeNonspatialDataDisplay](CIMKnowledgeGraph.md#cimknowledgenonspatialdatadisplay) | The Nonspatial Data Display information in this Link Chart. 






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






## CIMKnowledgeGraphTypePropertyInfo
#### Represents a Knowledge Graph Type Property Info. It is primarily used to configure property visibility within the investigation view. 


### CIMKnowledgeGraphTypePropertyInfo 

|Property | Type | Description | 
|---------|--------|--------|
| propertyName | string | The name of the property. 
| isVisible | boolean | A value indicating whether the property is visible. 






## CIMKnowledgeLinkChartChronologicalLayoutSettings
#### Contains settings to be used in chronological layout calculations. 


### CIMKnowledgeLinkChartChronologicalLayoutSettings 

|Property | Type | Description | 
|---------|--------|--------|
| timeDirection | [enumeration LinkChartLayoutDirection](CIMKnowledgeGraph.md#enumeration-linkchartlayoutdirection) | The time axis direction. 
| timeBannerUTCOffsetInMinutes | long | The UTC offset of the time banner, in minutes. 
| eventsTicksVisualization | [enumeration EventsTicksVisualization](CIMKnowledgeGraph.md#enumeration-eventsticksvisualization) | The event ticks visualization option. Event ticks are displayed in the time banner. 
| showDurationLineForNonZeroDurationEntityEvents | boolean | A value indicating whether lines representing the duration of events with non-zero durations are shown. 
| durationLineWidth | long | A value indicating the width of the line, in points, representing the duration of an event with non-zero duration. 
| entityPositionAtDurationRatio | double | A value indicating where the entity of a non-zero duration event will be placed. 0.0 represents the start of the duration interval, 1.0 represents the end of the duration interval. Used in multi-timeline layout only. 
| showNonZeroDurationIntervalBounds | boolean | A value indicating whether duration interval bounds are represented in relationship lines of events that have non-zero durations. Used in multi-timeline layout only. 
| separateTimeOverlaps | boolean | A value indicating whether events that overlap in time are separated. 
| separateTimelineOverlaps | boolean | A value indicating whether events that overlap on a timeline are separated. 
| moveFirstBends | boolean | A value indicating whether the first bend on a relationship line related to an event is moved higher up from the event location when some events are separated. Used only in the mono-timeline layout, when 'SeparateTimelineOverlaps' is true. 
| secondBendRatio | double | The ratio at which the second bend or a relationship occurs, for event relationships and non-event relationships between events and non-event entities. Used only in the mono-timeline layout. 
| lineSeparationMultiplier | double | The multiplier used for line separation. Lines will be more separated with a higher multiplier. 
| spaceSeparatedLinesEvenly | boolean | A value indicating whether separated lines are spaced evenly. When true, the offset for the i-th overlapping line is proportional to 'i'. When false, the offset for the i-th overlapping line is proportional to 'squareRoot(i)'. 
| useBezierCurves | boolean | A value indicating whether to use Bezier curves to represent separated lines. 
| separatedLineShapeRatio | double | The separated line shape ratio. When the ratio is high, the angle between the extremities of the separated line geometry and the original line is small. 






## CIMKnowledgeLinkChartLayout
#### Represents a Knowledge Link Chart Layout Info object. 


### CIMKnowledgeLinkChartLayout 

|Property | Type | Description | 
|---------|--------|--------|
| algorithm | [enumeration KnowledgeLinkChartLayoutAlgorithm](CIMKnowledgeGraph.md#enumeration-knowledgelinkchartlayoutalgorithm) | The layout algorithm. 
| organicLayoutSettings | [CIMKnowledgeLinkChartOrganicLayoutSettings](CIMKnowledgeGraph.md#cimknowledgelinkchartorganiclayoutsettings) | The organic layout settings. 
| chronologicalLayoutSettings | [CIMKnowledgeLinkChartChronologicalLayoutSettings](CIMKnowledgeGraph.md#cimknowledgelinkchartchronologicallayoutsettings) | The chronological layout settings. 
| autoApply | boolean | A value indicating whether the layout is automatically redone when a setting value changes. 
| preserveExtent | boolean | A value indicating whether the current Link Chart extent is preserved by the layout (only applies to Chronological and Geographical layouts). 





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
| Chronological_MonoTimeline| 14| Chronological Mono-Timeline. 
| Chronological_MultiTimeline| 15| Chronological Multi-Timeline. 




## CIMKnowledgeLinkChartOrganicLayoutSettings
#### Contains settings to be used in organic layout calculations. 


### CIMKnowledgeLinkChartOrganicLayoutSettings 

|Property | Type | Description | 
|---------|--------|--------|
| computationTimeBudget | double | The computation time budget, in seconds. The maximum count of iterations of the force directed algorithm is computed based on the size of the link chart and this computation budget, assuming computations are executed by a theoretical CPU with some known characteristics. Higher values lead to better looking layouts. 
| absoluteIdealEdgeLength | double | The value, in degrees, to use for the ideal edge length during layout calculations when the IdealEdgeLengthType is 'absoluteValue'. Only used for geographic layouts. 
| multiplicativeIdealEdgeLength | double | The value used to multiply the default edge length to determine the ideal edge length during layout calculations, when the IdealEdgeLengthType is 'multiplier'. Only used for geographic layouts. 
| idealEdgeLengthType | [enumeration LinkChartLayoutIdealEdgeLengthType](CIMKnowledgeGraph.md#enumeration-linkchartlayoutidealedgelengthtype) | The ideal edge length type which determines which property to use to compute the ideal edge length. Only used for geographic layouts. When the value is 'AbsoluteValue', the 'AbsoluteIdealEdgeLength' property is used. When the value is 'Multiplier', the 'MultiplicativeIdealEdgeLength' property is used. 
| autoComputeRepulsionRadius | boolean | A value indicating whether the repulsion radius is automatically computed or if it is computed according to 'RepulsionRadiusMultiplier'. 
| repulsionRadiusMultiplier | double | The value to be used for the repulsion radius multiplier. The repulsion radius is computed as the repulsion radius multiplier multiplied by the actual ideal edge length. Only used when 'AutoComputeRepulsionRadius' is false. 






## CIMKnowledgeNonspatialDataDisplay
#### Represents a Knowledge Nonspatial Data Display object. 


### CIMKnowledgeNonspatialDataDisplay 

|Property | Type | Description | 
|---------|--------|--------|
| mode | [enumeration KnowledgeNonspatialDataDisplayMode](CIMKnowledgeGraph.md#enumeration-knowledgenonspatialdatadisplaymode) | The display mode. 





### Enumeration: KnowledgeNonspatialDataDisplayMode
#### Specifies a Knowledge Nonspatial Data Display Mode. 

|Property | Value | Description | 
|---------|--------|--------|
| Visible| 0| Visible. 
| Hidden| 1| Hidden. 




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
| layerEffects | [[CIMLayerEffect]](CIMLayer.md#cimlayereffect) | The layer effects for the layer. This property will contain either a list of all scale-dependent layer effects, or a single layer effect. 


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





### Enumeration: LinkChartLayoutDirection
#### Represents the direction of a Link Chart layout. 

|Property | Value | Description | 
|---------|--------|--------|
| Top| 0| Top 
| Bottom| 1| Bottom 
| Left| 2| Left 
| Right| 3| Right 



### Enumeration: LinkChartLayoutIdealEdgeLengthType
#### Determines how the ideal edge length is computed. 

|Property | Value | Description | 
|---------|--------|--------|
| AbsoluteValue| 0| The ideal edge length is specified as an absolute value. 
| Multiplier| 1| The ideal edge length is the computed ideal edge length multiplied by a value. 



### Enumeration: ProvenanceBehavior
#### Controls query behavior with respect to the Provenance Entity Type. 

|Property | Value | Description | 
|---------|--------|--------|
| Exclude| 0| Query behaves as if there were no Provenance records in the graph, nor Provenance Entity Type defined in the data model. 
| Include| 1| Query can reference the Provenance Entity Type. The result set may return provenance records. 

