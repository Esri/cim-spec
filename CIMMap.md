


## CIMAltitudeParams
#### Represents altitude parameters. 


### CIMAltitudeParams 

|Property | Type | Description | 
|---------|--------|--------|
| altitudeValue | double|Gets and sets the altitude value. 
| mode | [enumeration AltitudeMode](CIMEnumerations.md#enumeration-altitudemode)|Gets and sets the altitude mode. 






## CIMAnimationScreenGraphic
#### Represents a graphic and list of keyframes indicating properties that can be changed during the animation. 


### CIMAnimationScreenGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| graphic | [Graphic](Types.md#graphic)|Gets and sets the graphic to be displayed. 
| alias | string|Gets and sets an identifier for the user. 
| keyframes | [CIMAnimationScreenGraphicKeyframe](CIMMap.md#cimanimationscreengraphickeyframe) |Gets and sets the graphic properties keyframes. 






## CIMAnimationScreenGraphicKeyframe
#### Properties defining the graphic at a single point in time for the animation. 


### CIMAnimationScreenGraphicKeyframe 

|Property | Type | Description | 
|---------|--------|--------|
| trackTime | double|Gets and sets the time in seconds relative to the beginning of the track. 
| anchorX | double|Gets and sets the horizontal placement percent of the graphic anchor position on the viewer (0 is left edge, 1 is right edge). 
| anchorY | double|Gets and sets the vertical placement percent of the graphic anchor position on the viewer (0 is top edge, 1 is bottom edge). 
| transparency | double|Gets and sets the transparency of the graphic. 
| scale | double|Gets and sets the size multiplier for the graphic. 






## CIMBookmark
#### Represents a spatial bookmark. 


### CIMBookmark 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the bookmark name. 
| thumbnailImagePath | string|Gets and sets the thumbnail image path. 
| camera | [CIMViewCamera](CIMMap.md#cimviewcamera)|Gets and sets the camera. 
| location | [Envelope](ExternalReferences.md#envelope)|Gets and sets the location. 
| timeExtent | [TimeExtent](ExternalReferences.md#timeextent)|Gets and sets the time extent. 
| description | string|Gets and sets the bookmark description. 
| videoURI | string|Gets and sets the URI to the standalone video. 
| videoElapsedTime | double|Gets and sets the video elapsed time in seconds. 






## CIMCutbacksRule
#### Represents a cutbacks rule which is used to detect high-angle turns that cause features to turn back toward themselves. 


### CIMValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleID | string|Unique identifier of the validation rule. 
| title | string|Gets and sets the title for the validation rule. The title can be used to describe the conditions you are looking for with the validation rule. This is useful when you have multiple instances of the same RuleType to validate the same layers or standalone tables but with different validation parameters. This property is optional. 
| notes | string|Gets and sets the notes for the validation rule. This is the descriptive text for the validation results. This property is optional. 
| severity | long|Gets and sets the severity for the validation rule. This is the value that indicates the relative priority of the validation results on a scale of 1 (highest) to 5 (lowest). The default value of this property is 3. 
| tags | string|Gets and sets the tags for the validation rule. Tags are keywords or short phrases that facilitate discovery of the validation rule. Separate terms with commas. Overlapping Geometry is considered one tag, while Overlapping, geometry is considered two tags. This property is optional. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been created. 
| createdBy | string|The Portal login name of the user that created the validation rule. 
| lastModifiedDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been last modified. 
| lastModifiedBy | string|The Portal login name of the user that last modified the validation rule. 
| participatingLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layer URI strings on which the rule is applied to. 


### CIMReviewerValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleDefinitionExpression | string|Gets and sets the definition expression to run the validation rule on specific features in a layer or standalone table. This property is optional. 
| ignoreFields | IStringArray|An array of layer field names that need to be ignored for the validation rule. This property is optional. 


### CIMReviewerIndependentValidationRule 

|Property | Type | Description | 
|---------|--------|--------|


### CIMCutbacksRule 

|Property | Type | Description | 
|---------|--------|--------|
| minAngle | double|The minimum angle value in Degrees for the cutback. This is the minimum angle between segments on a polyline or polygon feature. Features with an angle that is below the minimum value are returned as validation results. The default value is 0. 






## CIMDatumTransform
#### Represents a datum transform. 


### CIMDatumTransform 

|Property | Type | Description | 
|---------|--------|--------|
| forward | boolean|Gets and sets a boolean value indicating whether or not this is a forward transformation. 
| geoTransformation | [GeoTransformation](ExternalReferences.md#geotransformation)|Gets and sets the transformation. 






## CIMDomainRule
#### Represents a domain rule which validates domain values to ensure they meet all constraints for a field. 


### CIMValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleID | string|Unique identifier of the validation rule. 
| title | string|Gets and sets the title for the validation rule. The title can be used to describe the conditions you are looking for with the validation rule. This is useful when you have multiple instances of the same RuleType to validate the same layers or standalone tables but with different validation parameters. This property is optional. 
| notes | string|Gets and sets the notes for the validation rule. This is the descriptive text for the validation results. This property is optional. 
| severity | long|Gets and sets the severity for the validation rule. This is the value that indicates the relative priority of the validation results on a scale of 1 (highest) to 5 (lowest). The default value of this property is 3. 
| tags | string|Gets and sets the tags for the validation rule. Tags are keywords or short phrases that facilitate discovery of the validation rule. Separate terms with commas. Overlapping Geometry is considered one tag, while Overlapping, geometry is considered two tags. This property is optional. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been created. 
| createdBy | string|The Portal login name of the user that created the validation rule. 
| lastModifiedDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been last modified. 
| lastModifiedBy | string|The Portal login name of the user that last modified the validation rule. 
| participatingLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layer URI strings on which the rule is applied to. 


### CIMReviewerValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleDefinitionExpression | string|Gets and sets the definition expression to run the validation rule on specific features in a layer or standalone table. This property is optional. 
| ignoreFields | IStringArray|An array of layer field names that need to be ignored for the validation rule. This property is optional. 


### CIMReviewerIndependentValidationRule 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDomainRule 

|Property | Type | Description | 
|---------|--------|--------|
| checkNulls | boolean|Boolean value indicating if a feature or row should be returned as validation result when it's attribute value for a domain constrained field is null. The default value is false. 
| domainFieldsToInclude | IStringArray|String array of Domain Field names to check domain validity. 






## CIMDuplicateFeatureRule
#### Duplicate Feature Rule will identify duplicate features based on geometry and attributes of the input layers. It will take 2 inputs and a configuration parameter 


### CIMValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleID | string|Unique identifier of the validation rule. 
| title | string|Gets and sets the title for the validation rule. The title can be used to describe the conditions you are looking for with the validation rule. This is useful when you have multiple instances of the same RuleType to validate the same layers or standalone tables but with different validation parameters. This property is optional. 
| notes | string|Gets and sets the notes for the validation rule. This is the descriptive text for the validation results. This property is optional. 
| severity | long|Gets and sets the severity for the validation rule. This is the value that indicates the relative priority of the validation results on a scale of 1 (highest) to 5 (lowest). The default value of this property is 3. 
| tags | string|Gets and sets the tags for the validation rule. Tags are keywords or short phrases that facilitate discovery of the validation rule. Separate terms with commas. Overlapping Geometry is considered one tag, while Overlapping, geometry is considered two tags. This property is optional. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been created. 
| createdBy | string|The Portal login name of the user that created the validation rule. 
| lastModifiedDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been last modified. 
| lastModifiedBy | string|The Portal login name of the user that last modified the validation rule. 
| participatingLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layer URI strings on which the rule is applied to. 


### CIMReviewerValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleDefinitionExpression | string|Gets and sets the definition expression to run the validation rule on specific features in a layer or standalone table. This property is optional. 
| ignoreFields | IStringArray|An array of layer field names that need to be ignored for the validation rule. This property is optional. 


### CIMReviewerDependentValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| secondaryDatasets | [CIMRuleDatasetParameter](CIMMap.md#cimruledatasetparameter) |Array of dataset parameters used for validation rule. 
| secondaryLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layers used for validation rule. 


### CIMDuplicateFeatureRule 

|Property | Type | Description | 
|---------|--------|--------|
| fieldsToCompare | IStringArray|An array of field names that need to be compared when evaluating duplicating features. 






## CIMElevationSource
#### Represents an elevation source. 


### CIMElevationSource 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection. 
| verticalUnit | [Unit](ExternalReferences.md#unit)|Gets and sets the vertical unit. 






## CIMEventOnEventRule
#### 


### CIMValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleID | string|Unique identifier of the validation rule. 
| title | string|Gets and sets the title for the validation rule. The title can be used to describe the conditions you are looking for with the validation rule. This is useful when you have multiple instances of the same RuleType to validate the same layers or standalone tables but with different validation parameters. This property is optional. 
| notes | string|Gets and sets the notes for the validation rule. This is the descriptive text for the validation results. This property is optional. 
| severity | long|Gets and sets the severity for the validation rule. This is the value that indicates the relative priority of the validation results on a scale of 1 (highest) to 5 (lowest). The default value of this property is 3. 
| tags | string|Gets and sets the tags for the validation rule. Tags are keywords or short phrases that facilitate discovery of the validation rule. Separate terms with commas. Overlapping Geometry is considered one tag, while Overlapping, geometry is considered two tags. This property is optional. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been created. 
| createdBy | string|The Portal login name of the user that created the validation rule. 
| lastModifiedDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been last modified. 
| lastModifiedBy | string|The Portal login name of the user that last modified the validation rule. 
| participatingLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layer URI strings on which the rule is applied to. 


### CIMReviewerValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleDefinitionExpression | string|Gets and sets the definition expression to run the validation rule on specific features in a layer or standalone table. This property is optional. 
| ignoreFields | IStringArray|An array of layer field names that need to be ignored for the validation rule. This property is optional. 


### CIMReviewerDependentValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| secondaryDatasets | [CIMRuleDatasetParameter](CIMMap.md#cimruledatasetparameter) |Array of dataset parameters used for validation rule. 
| secondaryLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layers used for validation rule. 


### CIMEventOnEventRule 

|Property | Type | Description | 
|---------|--------|--------|
| overlayEventsWhereClause | string|Gets and sets where clause to filter errors from the dynamic segmentation table which is created from overlaying input events. 
| notQuery | boolean|Boolean value indicating if the validation results should be inverted. The default value is false. 






## CIMFeatureOnFeatureRule
#### Represents a feature on feature rule which validates features against other features based on rule criteria. 


### CIMValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleID | string|Unique identifier of the validation rule. 
| title | string|Gets and sets the title for the validation rule. The title can be used to describe the conditions you are looking for with the validation rule. This is useful when you have multiple instances of the same RuleType to validate the same layers or standalone tables but with different validation parameters. This property is optional. 
| notes | string|Gets and sets the notes for the validation rule. This is the descriptive text for the validation results. This property is optional. 
| severity | long|Gets and sets the severity for the validation rule. This is the value that indicates the relative priority of the validation results on a scale of 1 (highest) to 5 (lowest). The default value of this property is 3. 
| tags | string|Gets and sets the tags for the validation rule. Tags are keywords or short phrases that facilitate discovery of the validation rule. Separate terms with commas. Overlapping Geometry is considered one tag, while Overlapping, geometry is considered two tags. This property is optional. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been created. 
| createdBy | string|The Portal login name of the user that created the validation rule. 
| lastModifiedDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been last modified. 
| lastModifiedBy | string|The Portal login name of the user that last modified the validation rule. 
| participatingLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layer URI strings on which the rule is applied to. 


### CIMReviewerValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleDefinitionExpression | string|Gets and sets the definition expression to run the validation rule on specific features in a layer or standalone table. This property is optional. 
| ignoreFields | IStringArray|An array of layer field names that need to be ignored for the validation rule. This property is optional. 


### CIMReviewerDependentValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| secondaryDatasets | [CIMRuleDatasetParameter](CIMMap.md#cimruledatasetparameter) |Array of dataset parameters used for validation rule. 
| secondaryLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layers used for validation rule. 


### CIMFeatureOnFeatureRule 

|Property | Type | Description | 
|---------|--------|--------|
| spatialRelationship | [enumeration esriSpatialRelEnum](ExternalReferences.md#enumeration-esrispatialrelenum)|The spatial relationship between primary and secondary layer for the validation rule. The default value is esriSpatialRelIntersects. 
| customSpatialRelation | string|Gets and sets the custom spatial relation. 
| checkAttributes | boolean|Boolean value indicating if the layer field attributes should be used for the validation rule. The default value is false. 
| tolerance | double|Number of units to use for the tolerance in the spatial query. The default value is layer's spatial reference XY tolerance. 
| toleranceUnits | [Unit](ExternalReferences.md#unit)|Units of measurement to use with the tolerance. The default value is layer's spatial reference XY tolerance unit. 
| notQuery | boolean|Boolean value indicating if the validation results should be inverted. The default value is false. 
| mergeFeatures | boolean|Boolean value indicating if features from secondary layer need to be merged before executing the spatial query between primary and secondary layer. This property is used only for Contains, Relation, or Within spatial relationship with a line and polygon layers or two line or polygon layers. The default value is false. 
| attributeComparisons | [CIMFieldComparison](CIMMap.md#cimfieldcomparison) |FieldComparisonExpression object to filter features. This property is optional. 






## CIMFieldComparison
#### Represents a field comparison rule. 


### CIMFieldComparison 

|Property | Type | Description | 
|---------|--------|--------|
| searchFieldName | string|The RHS (right hand side) field for the expression. 
| valueFieldName | string|The LHS (left hand side) field for the expression. 
| comparisonOperator | string|The comparison operator used between LHS and RHS fields. The default value is = operator (equal to operator). 
| joinOperator | string|The join operator (AND or OR operator) used between two expressions. The default value is AND. 






## CIMFieldComparisonExpression
#### Represents a field comparison expression. 


### CIMFieldComparisonExpression 

|Property | Type | Description | 
|---------|--------|--------|
| fieldComparisons | [CIMFieldComparison](CIMMap.md#cimfieldcomparison) |Array of FieldComparison objects 
| fieldComparisonExpressions | [CIMFieldComparisonExpression](CIMMap.md#cimfieldcomparisonexpression) |Array of FieldComparisonExpression objects. 
| joinOperator | string|The join operator (AND or OR operator) used between two expressions. The default value is AND. 
| notOperator | boolean|Boolean value indicating if Not operator to inverse the expression need to be applied. The default value is false. 






## CIMIlluminationProperties
#### Represents illumination properties. 


### CIMIlluminationProperties 

|Property | Type | Description | 
|---------|--------|--------|
| ambientLight | double|Gets and sets the ambient light value. 
| sunPositionX | double|Gets and sets the sun position X. 
| sunPositionY | double|Gets and sets the sun position Y. 
| sunPositionZ | double|Gets and sets the sun position Z. 
| showAtmosphericEffects | boolean|Gets and sets a boolean value indicating whether or not to show atmospheric effects. 
| showShadows3D | boolean|Gets and sets a boolean value indicating whether or not to show shadows in 3D. 
| dateTime | [TimeInstant](ExternalReferences.md#timeinstant)|Gets and sets the time instant. 
| illuminationSource | [enumeration IlluminationSource](CIMMap.md#enumeration-illuminationsource)|Gets and sets the illumination source. 
| sunAzimuth | double|Gets and sets the sun azimuth. 
| sunAltitude | double|Gets and sets the sun altitude. 
| showStars | boolean|Boolean property for showing the stars and the atmospheric halo for a global scene. 





### Enumeration: IlluminationSource
#### Illumination source types. 

|Property | Value | Description | 
|---------|--------|--------|
| NoonAtCameraPosition| 0| Noon at the camera position. 
| DateTime| 1| Set for a specific date and time. 
| AbsoluteSunPosition| 2| An absolute sun position. 
| MapTime| 3| Synchronized with the current map time. 




## CIMInvalidEventRule
#### Represents an invalid event rule. 


### CIMValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleID | string|Unique identifier of the validation rule. 
| title | string|Gets and sets the title for the validation rule. The title can be used to describe the conditions you are looking for with the validation rule. This is useful when you have multiple instances of the same RuleType to validate the same layers or standalone tables but with different validation parameters. This property is optional. 
| notes | string|Gets and sets the notes for the validation rule. This is the descriptive text for the validation results. This property is optional. 
| severity | long|Gets and sets the severity for the validation rule. This is the value that indicates the relative priority of the validation results on a scale of 1 (highest) to 5 (lowest). The default value of this property is 3. 
| tags | string|Gets and sets the tags for the validation rule. Tags are keywords or short phrases that facilitate discovery of the validation rule. Separate terms with commas. Overlapping Geometry is considered one tag, while Overlapping, geometry is considered two tags. This property is optional. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been created. 
| createdBy | string|The Portal login name of the user that created the validation rule. 
| lastModifiedDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been last modified. 
| lastModifiedBy | string|The Portal login name of the user that last modified the validation rule. 
| participatingLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layer URI strings on which the rule is applied to. 


### CIMReviewerValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleDefinitionExpression | string|Gets and sets the definition expression to run the validation rule on specific features in a layer or standalone table. This property is optional. 
| ignoreFields | IStringArray|An array of layer field names that need to be ignored for the validation rule. This property is optional. 


### CIMReviewerDependentValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| secondaryDatasets | [CIMRuleDatasetParameter](CIMMap.md#cimruledatasetparameter) |Array of dataset parameters used for validation rule. 
| secondaryLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layers used for validation rule. 


### CIMInvalidEventRule 

|Property | Type | Description | 
|---------|--------|--------|
| eventSourceRouteID | string|The RouteID field name for the Event layer. 
| eventSourceFromMeasure | string|The From Measure field name for the Event layer. 
| eventSourceToMeasure | string|The To Measure field name for the Event layer. This property is optional if the Event is a point Event. 
| routeSourceRouteID | string|The RouteID field name for the Route layer. 
| findOrphans | boolean|Boolean value indicating if Events that do not have an associated Route are returned as a validation result. The default value is false. 
| findGaps | boolean|Boolean value indicating if Events having gaps in the measure values are returned as a validation result. The default value is false. 
| measureTolerance | double|Measure tolerance for the validation rule. The default value is the layer's spatial reference M tolerance. 
| findInvalidMeasures | boolean|Boolean value indicating if Events that do not have valid measure values are returned as a validation result. The default value is false. 
| findOverlaps | boolean|Boolean value indicating if Events that have overlapping measure values are returned as a validation result. The default value is false. 






## CIMKeyframeCamera
#### Represents a camera keyframe. 


### CIMKeyframeCamera 

|Property | Type | Description | 
|---------|--------|--------|
| camera | [CIMViewCamera](CIMMap.md#cimviewcamera)|Gets or sets the camera for the keyframe. 
| headingTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition)|Gets or sets the method of transition for the heading of the camera. 
| pitchTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition)|Gets or sets the method of transition for the pitch of the camera. 
| rollTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition)|Gets or sets the method of transition for the roll of the camera. 
| scaleTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition)|Gets or sets the method of transition for the scale of the camera. 
| XTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition)|Gets or sets the method of transition for the x of the camera. 
| YTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition)|Gets or sets the method of transition for the y of the camera. 
| ZTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition)|Gets or sets the method of transition for the z of the camera. 
| transitionScale | double|Gets or sets the value of adjustable transitions. The value must be between 0.0 and 1.0. Smaller values will result in a tighter / smaller curve than larger values. 
| cameraTransitionMode | [enumeration esriAnimationTransitionMode](ExternalReferences.md#enumeration-esrianimationtransitionmode)|The transition mode determines whether the camera path follows a Geodesic or Cartesian interpolation. 






## CIMKeyframeLayer
#### Represents a layer keyframe. 


### CIMKeyframeLayer 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string|Gets or sets the path to the layer. 
| transparency | double|Gets or sets the method of transition for the visibility of the layer. 
| transparencyTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition)|Gets or sets the method of transition for the transparency of the layer. 
| visible | boolean|Gets or sets value indicating the visibility of the layer. 






## CIMKeyframeRange
#### Represents a range keyframe. 


### CIMKeyframeRange 

|Property | Type | Description | 
|---------|--------|--------|
| range | [CIMRange](CIMVectorLayers.md#cimrange)|Gets or sets the value of the range. 
| minTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition)|Gets or sets the method of transition for the minimum value of the range. 
| maxTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition)|Gets or sets the method of transition for the maximum value of the range. 
| isExclusion | boolean|Gets or sets a value indicating if the range should be all values less than the min value and greater than the max value. 






## CIMKeyframeTime
#### Represents a time keyframe. 


### CIMKeyframeTime 

|Property | Type | Description | 
|---------|--------|--------|
| time | [TimeExtent](ExternalReferences.md#timeextent)|Gets or sets the value of the time extent. 
| endTimeTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition)|Gets or sets the method of transition for the end value of the time extent. 
| startTimeTransition | [enumeration AnimationTransition](CIMEnumerations.md#enumeration-animationtransition)|Gets or sets the method of transition for the start value of the time extent. 






## CIMLocator
#### Represents properties of locator for the map. 


### CIMLocator 

|Property | Type | Description | 
|---------|--------|--------|
| locatorType | [enumeration LocatorType](CIMMap.md#enumeration-locatortype)|Gets and sets the type of locator for the LocatorURI specified. 
| name | string|Gets and sets the name of the locator. 
| locatorURI | string|Gets and sets locator source URI. It can either be a local path, url or a layer URI from this map. e.g. file://&lt;folder_path&gt;, http://&lt;url&gt;, CIMPATH=&lt;cim_layer_UR&gt; 
| suggestionsEnabled | boolean|Gets and sets a boolean indicating whether or not to suggestions should enabled if the locator supports suggestions. 
| enabled | boolean|Gets and sets a boolean indicating whether or not to this locator is enabled. 





### Enumeration: LocatorType
#### Type of locators. 

|Property | Value | Description | 
|---------|--------|--------|
| Locator| 0| Locator is based on local locator file or url. 
| Layer| 1| LocatorURI is based on a Layer in the map 




## CIMMap
#### Represents a map or scene. A map is a container of geographic information. There are different kinds of geographic information within a map: imagery, terrain, and different kinds of vector data. The information in a map is organized into layers. A map contains an ordered list of layers, and draws each layer on top of its preceeding layers. In 3D layers may be drawn in Z order and not layer order. A map has a single spatial reference system. Each of its layers can be stored natively in different spatial reference systems. If a layer has a different spatial reference system than a map it is displayed in, the map reprojects the data to its spatial reference system before drawing it. A map can dynamically place labels for its features. It finds optimal label locations for each map extent to maximize typographic clarity and to avoid overlaps. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| URI | string|Gets and sets the URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string|Gets and sets the source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|Gets and sets the time the definition was last modfied. 
| metadataURI | string|Gets and sets the metadata URI. 
| useSourceMetadata | bool|Gets and sets if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 


### CIMMap 

|Property | Type | Description | 
|---------|--------|--------|
| defaultCamera | [CIMViewCamera](CIMMap.md#cimviewcamera)|Gets and sets the default camera. 
| illumination | [CIMIlluminationProperties](CIMMap.md#cimilluminationproperties)|Gets and sets the illumination properties. 
| layers | IStringArray|Gets and sets the layers as an array of layer repository paths. 
| standaloneTables | IStringArray|Gets and sets the standalone tables as an array of table repository paths. 
| stereoProperties | [CIMMapStereoProperties](CIMMap.md#cimmapstereoproperties)|Gets and sets the stereo properties. 
| defaultViewingMode | [enumeration MapViewingMode](CIMEnumerations.md#enumeration-mapviewingmode)|Gets and sets the default viewing mode. 
| mapType | [enumeration MapType](CIMMap.md#enumeration-maptype)|Gets and sets the map type. 
| rangeSliderSettings | [CIMSliderSettings](CIMMap.md#cimslidersettings)|Gets and sets the range slider settings. 
| timeSliderSettings | [CIMSliderSettings](CIMMap.md#cimslidersettings)|Gets and sets the time slider settings. 
| animationViewTracks | [CIMViewTrack](CIMMap.md#cimviewtrack) |Gets or sets the collection of view tracks in the animation. 
| locators | [CIMLocator](CIMMap.md#cimlocator) |Gets and sets the locators as an ordered array. 
| validationRules | [CIMValidationRule](Types.md#cimvalidationrule) |Gets and sets the validation rules used for validating the layer's features. 
| mapContexts | IStringArray|Gets and sets an array string values used to provide a hint for the intended context for the map. 
| standaloneVideos | IStringArray|Gets and sets the standalone videos as an array of video repository paths. 


### CIMMapDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundColor | [Color](Types.md#color)|Gets and sets the background color. 
| bookmarks | [CIMBookmark](CIMMap.md#cimbookmark) |Gets and sets the bookmarks. 
| clipToFullExtent | boolean|Gets and sets a boolean value indicating whether or not to clip to full extent. 
| attribution | string|Gets and sets the attribution text that will appear on the map when it is drawn. 
| customFullExtent | [Polygon](ExternalReferences.md#polygon)|Gets and sets the custom full extent as a polygon. 
| datumTransforms | [CIMDatumTransform](CIMMap.md#cimdatumtransform) |Gets and sets the set of geographic transformations used by the map for spatial references that do not have vertical coordinate system. 
| defaultExtent | [Envelope](ExternalReferences.md#envelope)|Gets and sets the extent shown when you open new views of the map. The application automatically updates this property whenever you save a project with an active map view. 
| defaultScale | double|Gets and sets the scale used when you open new views of the map. When set, the application automatically applies this property after DefaultExtent to ensure the view is at the correct scale. 
| defaultGlobeTransparency | double|Gets and sets the transparency of the spheroid's combined terrain mesh and draped content. 
| defaultRotation | double|Gets and sets the default rotation. 
| description | string|Gets and sets the long description of the map. 
| elevationSurfaces | [CIMMapElevationSurface](CIMMap.md#cimmapelevationsurface) |Gets and sets the elevation surfaces. 
| generalPlacementProperties | [GeneralPlacementProperties](Types.md#generalplacementproperties)|Gets and sets the general label placement properties for dynamic labels in the map. 
| scaleLevels | [double]|Gets and sets the scale levels of the map. 
| snappingProperties | [CIMSnappingProperties](CIMMap.md#cimsnappingproperties)|Gets and sets the snapping properties of the map. 
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference)|Gets and sets the map's spatial reference. 
| surfaceColor | [Color](Types.md#color)|Gets and sets the color of the default spheroid. 
| timeDisplay | [CIMMapTimeDisplay](CIMMap.md#cimmaptimedisplay)|Gets and sets the time display properties. 
| enableNavigationBelowGround | boolean|Gets and sets a boolean value indicating whether or to enable navigation below the ground. 
| referenceScale | double|Gets and sets the map reference scale. 
| enableWraparound | boolean|Gets and sets a boolean value indicating whether or to enable wraparound when the coordinate system supports it. 
| includeMaximumInScaleRanges | boolean|Gets and sets a boolean value indicating whether or not to draw up to and including the maximum scale in scale ranges. 
| colorModel | [enumeration ColorModel](CIMEnumerations.md#enumeration-colormodel)|Gets and Sets the color model for a map. 
| scales | [CIMScale](CIMMap.md#cimscale) |Array of CIMScale objects, describing the full list of named scales for the map. 
| scaleFormat | [CIMScaleFormat](CIMMap.md#cimscaleformat)|ScaleFormat describing the formatting of the Scale value. 
| scaleDisplayFormat | [enumeration ScaleDisplayFormat](CIMMap.md#enumeration-scaledisplayformat)|Display mode for the map's Scales in the user interface 
| HVDatumTransforms | [ArrayOfCompositeHVDatumTransformation](ExternalReferences.md#arrayofcompositehvdatumtransformation)|Gets and sets the set of geographic transformations used by the map for spatial references with vertical coordinate system. 
| useServiceLayerIDs | boolean|Gets or sets the flag to indicate whether to allow the use of unique numeric IDs on layers that will be used when publishing services. 






## CIMMapElevationSurface
#### Represents a map elevation surface. 


### CIMMapElevationSurface 

|Property | Type | Description | 
|---------|--------|--------|
| baseSources | [CIMElevationSource](CIMMap.md#cimelevationsource) |Gets and sets the elevation sources. 
| elevationMode | [enumeration ElevationMode](CIMEnumerations.md#enumeration-elevationmode)|Gets and sets the elevation mode. 
| name | string|Gets and sets the elevation name. 
| verticalExaggeration | double|Gets and sets the vertical exaggeration. 
| mapElevationID | string|Gets and sets the map elevation ID. 
| color | [Color](Types.md#color)|Gets and sets the surface color. 
| enableSurfaceShading | boolean|Gets and sets a boolean value indicating whether this elevation surface has shadows. 
| surfaceTINShadingMode | [enumeration SurfaceTINShadingMode](CIMMap.md#enumeration-surfacetinshadingmode)|Represents an elevation surface shading mode for TIN elevation sources. 






## CIMMapStereoProperties
#### Represents map stereo properties. 


### CIMMapStereoProperties 

|Property | Type | Description | 
|---------|--------|--------|
| leftImage | [DataConnection](Types.md#dataconnection)|Gets and sets the left image of the stereo pair. 
| rightImage | [DataConnection](Types.md#dataconnection)|Gets and sets the right image of the stereo pair. 
| sourceType | [enumeration StereoSourceType](CIMMap.md#enumeration-stereosourcetype)|Gets and sets the stereo source type. 
| stereoModelCollection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection to the source stereo model collection. 
| leftImageID | __int64|Gets and sets the OID of the left image of the current stereo model in a collection. 
| rightImageID | __int64|Gets and sets the OID of the right image of the current stereo model in a collection. 
| leftImageColorizer | [CIMRasterColorizer](CIMImageLayers.md#cimrastercolorizer)|Gets and sets the colorizer for the left image. 
| rightImageColorizer | [CIMRasterColorizer](CIMImageLayers.md#cimrastercolorizer)|Gets and sets the colorizer for the right image. 
| adjustColorizersInSync | bool|Gets and sets the flag indicating adjustments to either colorizer should be synced to the other. 
| isInverted | bool|Gets and sets the flag indicating the left and right images of the stereo model should be swapped. 
| stereoModelDisplayMode | [enumeration StereoModelDisplayMode](CIMMap.md#enumeration-stereomodeldisplaymode)|Gets and sets the stereo model display mode. 






## CIMMapTimeDisplay
#### Represents map time display. 


### CIMMapTimeDisplay 

|Property | Type | Description | 
|---------|--------|--------|
| currentTimeExtent | [TimeExtent](ExternalReferences.md#timeextent)|Gets and sets the current time extent. 
| defaultTimeInterval | double|Gets and sets the default time interval. 
| defaultTimeIntervalUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|Gets and sets the default time interval units. 
| defaultTimeWindow | double|Gets and sets the default time window. 
| fullTimeExtent | [TimeExtent](ExternalReferences.md#timeextent)|Gets and sets the full time extent. 
| timeReference | [TimeReference](ExternalReferences.md#timereference)|Gets and sets the time reference. 
| timeValue | [TimeValue](ExternalReferences.md#timevalue)|Gets and sets the time value. 
| hasLiveData | boolean|Gets and sets a boolean value indicating whether or not this map has live data. 
| timeRelation | [enumeration esriTimeRelation](ExternalReferences.md#enumeration-esritimerelation)|Gets and sets the time relation. 





### Enumeration: MapType
#### Types of maps. 

|Property | Value | Description | 
|---------|--------|--------|
| Map| 0| A 2D map. 
| Scene| 1| A scene. 
| Basemap| 2| A basemap. 
| NetworkDiagram| 3| A network diagram. 
| ContainmentMap| 4| A containment map. 




## CIMMonotonicityRule
#### Represents an monotonicity rule. 


### CIMValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleID | string|Unique identifier of the validation rule. 
| title | string|Gets and sets the title for the validation rule. The title can be used to describe the conditions you are looking for with the validation rule. This is useful when you have multiple instances of the same RuleType to validate the same layers or standalone tables but with different validation parameters. This property is optional. 
| notes | string|Gets and sets the notes for the validation rule. This is the descriptive text for the validation results. This property is optional. 
| severity | long|Gets and sets the severity for the validation rule. This is the value that indicates the relative priority of the validation results on a scale of 1 (highest) to 5 (lowest). The default value of this property is 3. 
| tags | string|Gets and sets the tags for the validation rule. Tags are keywords or short phrases that facilitate discovery of the validation rule. Separate terms with commas. Overlapping Geometry is considered one tag, while Overlapping, geometry is considered two tags. This property is optional. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been created. 
| createdBy | string|The Portal login name of the user that created the validation rule. 
| lastModifiedDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been last modified. 
| lastModifiedBy | string|The Portal login name of the user that last modified the validation rule. 
| participatingLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layer URI strings on which the rule is applied to. 


### CIMReviewerValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleDefinitionExpression | string|Gets and sets the definition expression to run the validation rule on specific features in a layer or standalone table. This property is optional. 
| ignoreFields | IStringArray|An array of layer field names that need to be ignored for the validation rule. This property is optional. 


### CIMReviewerIndependentValidationRule 

|Property | Type | Description | 
|---------|--------|--------|


### CIMMonotonicityRule 

|Property | Type | Description | 
|---------|--------|--------|
| levelValuesAreError | boolean|Boolean value indicating if a feature should be returned as validation result when it's From node is equal to the To node. The default value is false. 
| nonMonotonicValuesAreError | boolean|Boolean value indicating if a feature should be returned as validation result when it's vertices are not strictly increasing or decreasing in value. The From node of the feature is used as the point of reference when comparing vertex values. The default value is false. 
| evaluationType | [enumeration ReviewerMonotonicityEvaluationType](CIMMap.md#enumeration-reviewermonotonicityevaluationtype)|Indicates the type of evaluation. The default value is EvaluateNone. 
| monotonicityDirection | [enumeration ReviewerMonotonicityDirection](CIMMap.md#enumeration-reviewermonotonicitydirection)|Indicates the monotonicity direction. The default value is NoneAsError. 





### Enumeration: ReviewerMonotonicityDirection
#### Reviewer monotonicity direction types. 

|Property | Value | Description | 
|---------|--------|--------|
| NoneAsError| 0| No monotonicity direction as error. 
| DecreasingValueAsError| 1| Indicates decreasing values as error. 
| IncreasingValueAsError| 2| Indicates increasing values as error. 



### Enumeration: ReviewerMonotonicityEvaluationType
#### Reviewer monotonicity evaluation types. 

|Property | Value | Description | 
|---------|--------|--------|
| EvaluateNone| 0|  
| EvaluateZ| 1|  
| EvaluateM| 2|  




## CIMReviewerSimpleValidationRule
#### Represents a simple validation rule. 


### CIMValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleID | string|Unique identifier of the validation rule. 
| title | string|Gets and sets the title for the validation rule. The title can be used to describe the conditions you are looking for with the validation rule. This is useful when you have multiple instances of the same RuleType to validate the same layers or standalone tables but with different validation parameters. This property is optional. 
| notes | string|Gets and sets the notes for the validation rule. This is the descriptive text for the validation results. This property is optional. 
| severity | long|Gets and sets the severity for the validation rule. This is the value that indicates the relative priority of the validation results on a scale of 1 (highest) to 5 (lowest). The default value of this property is 3. 
| tags | string|Gets and sets the tags for the validation rule. Tags are keywords or short phrases that facilitate discovery of the validation rule. Separate terms with commas. Overlapping Geometry is considered one tag, while Overlapping, geometry is considered two tags. This property is optional. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been created. 
| createdBy | string|The Portal login name of the user that created the validation rule. 
| lastModifiedDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been last modified. 
| lastModifiedBy | string|The Portal login name of the user that last modified the validation rule. 
| participatingLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layer URI strings on which the rule is applied to. 


### CIMReviewerValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleDefinitionExpression | string|Gets and sets the definition expression to run the validation rule on specific features in a layer or standalone table. This property is optional. 
| ignoreFields | IStringArray|An array of layer field names that need to be ignored for the validation rule. This property is optional. 


### CIMReviewerSimpleValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleType | [enumeration ReviewerSimpleValidationRuleType](CIMMap.md#enumeration-reviewersimplevalidationruletype)|Inidcates the reviewer's simple validation rule type to be used. 





### Enumeration: ReviewerSimpleValidationRuleType
#### Reviewer simple validate rule types. 

|Property | Value | Description | 
|---------|--------|--------|
| QueryAttributesRule| 0| The Execute Query rule allows you to run predefined WHERE clauses in a batch on the layers or standalone tables. All features or rows whose parameters match those defined in the SQL query are returned as validation results. 
| InvalidGeometryRule| 1| Invalid Geometry Rule will identify feature geometries that are considered invalid based on certain criteria (Empty, Nothing, Not Simple and has an Empty envelope). 




## CIMRuleDatasetParameter
#### Represents a rule dataset parameter. 


### CIMRuleDatasetParameter 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection. 
| definitionExpression | string|Gets and sets the definition expression to filter features in the dataset. This property is optional. 






## CIMRuleEventLayerDescription
#### Describes the validation rule properties for event layer in the map. 


### CIMRuleLayerDescription 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string|Gets and sets the layer URI. 
| definitionExpression | string|Gets and sets the definition expression. 
| enabled | boolean|Indicates if the rule is enabled. 


### CIMRuleLRSLayerDescription 

|Property | Type | Description | 
|---------|--------|--------|
| routeIDFieldName | string|Gets or sets RouteID field name for the Route/Event layer. 
| fieldsToCompare | IStringArray|Gets or sets fields from the Route/Event layer that will be included in the dynamic segmentation table. 


### CIMRuleEventLayerDescription 

|Property | Type | Description | 
|---------|--------|--------|
| fromMeasureFieldName | string|Gets or sets from measure field name for the event layer. 
| toMeasureFieldName | string|Gets or sets to measure field name for the event layer. 






## CIMRuleLRSLayerDescription
#### Describes the validation rule properties for a location refrernce layer in the map. 


### CIMRuleLayerDescription 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string|Gets and sets the layer URI. 
| definitionExpression | string|Gets and sets the definition expression. 
| enabled | boolean|Indicates if the rule is enabled. 


### CIMRuleLRSLayerDescription 

|Property | Type | Description | 
|---------|--------|--------|
| routeIDFieldName | string|Gets or sets RouteID field name for the Route/Event layer. 
| fieldsToCompare | IStringArray|Gets or sets fields from the Route/Event layer that will be included in the dynamic segmentation table. 






## CIMRuleLayerDescription
#### Describes the validation rule properties for each layer in the map. 


### CIMRuleLayerDescription 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string|Gets and sets the layer URI. 
| definitionExpression | string|Gets and sets the definition expression. 
| enabled | boolean|Indicates if the rule is enabled. 






## CIMRuleRouteLayerDescription
#### Describes the validation rule properties for route layer in the map. 


### CIMRuleLayerDescription 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string|Gets and sets the layer URI. 
| definitionExpression | string|Gets and sets the definition expression. 
| enabled | boolean|Indicates if the rule is enabled. 


### CIMRuleLRSLayerDescription 

|Property | Type | Description | 
|---------|--------|--------|
| routeIDFieldName | string|Gets or sets RouteID field name for the Route/Event layer. 
| fieldsToCompare | IStringArray|Gets or sets fields from the Route/Event layer that will be included in the dynamic segmentation table. 


### CIMRuleRouteLayerDescription 

|Property | Type | Description | 
|---------|--------|--------|






## CIMScale
#### Represents a 2D scale or 3D Distance. 


### CIMScale 

|Property | Type | Description | 
|---------|--------|--------|
| value | double|Numeric value representing the 2D scale or 3D distance 
| alias | string|String value for the alias name of the Scale. 





### Enumeration: ScaleDisplayFormat
#### Scale display formats 

|Property | Value | Description | 
|---------|--------|--------|
| Value| 0| Show just the Scale value. 
| Alias| 1| Show just the Scale alias name. 
| ValueAndAlias| 2| Show the Scale value, and then the Scale alias name. 
| AliasAndValue| 3| Show the Scale alias name, and then the Scale value. 




## CIMScaleFormat
#### Represents the scale formatting options. 


### CIMScaleFormat 

|Property | Type | Description | 
|---------|--------|--------|
| formatType | [enumeration ScaleFormatType](CIMMap.md#enumeration-scaleformattype)|Format used to display scale, i.e., 1:20000 or 1 inch equals 5 miles. 
| separator | string|Character(s) used to separate '1' from the scale in an absolute scale, e.g ':' in 1:20000. 
| reverseOrder | boolean|Reverse the standard order. e.g. [1:1000] becomes [1000:1] and [1 in=10 mi] becomes [10 mi=1 in]. 
| decimalPlacesThreshold | double|The number the scale has to be less than or equal to display decimal places. 
| decimalPlaces | int|The number decimal places. 
| showThousandSeparator | boolean|Show thousands separator, e.g., 1:20,000. 
| pageUnits | [LinearUnit](ExternalReferences.md#linearunit)|The page units used to display a scale,e.g, the 'inch' in 1 inch=5 miles. 
| pageUnitValue | double|The number preceding the page units in a scale, i.e., the '1' in 1 inch=5 miles. 
| equalsSign | string|The text used for 'equals', e.g, '=' in 1 inch=5 miles. 
| mapUnits | [LinearUnit](ExternalReferences.md#linearunit)|The map units used to display a scale, e.g, the 'miles' in 1 inch=5 miles. 
| capitalizeUnits | boolean|Capitalize the units in the scale string. 
| abbreviateUnits | boolean|Capitalize the units in the scale string. 





### Enumeration: ScaleFormatType
#### Scale format types. 

|Property | Value | Description | 
|---------|--------|--------|
| Absolute| 0| Display absolute format, e.g. 1:20000. 
| Imperial| 1| Display imperial format, e.g. 1 in = 1 mi. 



### Enumeration: SliderExtentType
#### Slider extent types. 

|Property | Value | Description | 
|---------|--------|--------|
| AllLayers| 0| All layers. 
| VisibleLayers| 1| Visible layers. 
| SingleLayer| 2| A single layer. 
| CustomRange| 3| A custom range. 



### Enumeration: SliderInteractionMode
#### Slider interaction modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Slider| 0| Present the values on a slider as a range 
| Picker| 1| Present the values individually 




## CIMSliderSettings
#### Represents slider settings. 


### CIMSliderSettings 

|Property | Type | Description | 
|---------|--------|--------|
| sliderExtent | [CIMRange](CIMVectorLayers.md#cimrange)|Gets and sets the extent shown on the slider. 
| sliderExtentLocked | boolean|Gets and sets a boolean value that when true, the slider extent will not change due to scrolling or using the mouse wheel. 
| startValueLocked | boolean|Gets and sets a boolean value that when true, the slider's start thumb will not accept mouse events. 
| endValueLocked | boolean|Gets and sets a boolean value that when true, the slider's end thumb will not accept mouse events. 
| flipVertically | boolean|Gets and sets a boolean value that when true, the slider is flipped vertically to put larger values at the bottom and smaller values at the top. 
| useWindowValue | boolean|Gets and sets a boolean value that when true, the distance between the start and end thumbs will remain constant. 
| windowValue | double|Gets and sets the value of the window on the slider. 
| windowUnit | string|Gets and sets the unit of the window on the slider (for time it could be days, weeks, months, etc.). 
| stepUsesWindow | boolean|Gets and sets a boolean value that when true, the step interval value will stay in sync with the sliders value window when possible. 
| stepIntervalValue | double|Gets and sets the specific distance to move the thumbs by when stepping or playing. 
| stepIntervalUnit | string|Gets and sets the unit the interval value is in (for time it could by days, weeks, months, etc..) 
| stepCount | double|Gets and sets the number of steps to divide the slider extent into. 
| stepOption | [enumeration SliderStepType](CIMMap.md#enumeration-slidersteptype)|Gets and sets the chosen method of determining the step size. 
| playWaitSeconds | double|Gets and sets the amount of time to wait between steps. 
| playForward | boolean|Gets and sets a boolean value indicating if the play direction is forward. 
| playRepeats | boolean|Gets and sets a boolean value indicating whether play continuously repeats until interrupted by user interaction. 
| playReverses | boolean|Gets and sets a boolean value indicating whether play direction will reverse after playing to the end (if repeat is false play will move each direction once then stop). 
| fullExtentOption | [enumeration SliderExtentType](CIMMap.md#enumeration-sliderextenttype)|Gets and sets the option that determines the extent used by the full extent button. 
| fullExtentLayerURI | string|Gets and sets the URI of the layer used for the full extent with single layer full extent option. 
| fullExtentCustomRange | [CIMRange](CIMVectorLayers.md#cimrange)|Gets and sets the custom full extent used with the custom range full extent option. 
| interactionMode | [enumeration SliderInteractionMode](CIMMap.md#enumeration-sliderinteractionmode)|Gets or sets slider interaction mode 
| useTimeSnapping | boolean|Gets or sets flag to indicate whether automatic snapping for the map's current time settings is enabled. 
| timeSnapMode | [enumeration TimeSnapMode](CIMMap.md#enumeration-timesnapmode)|Gets and sets the option that determines mode used for snapping the map's current time settings. 
| singleTimeSnapUnit | string|Gets and sets the time unit to snap to when in 'Single' time snapping mode 
| aliasExpressionLayerURI | string|Gets or sets the string containing URI of the layer that contains the alias definition 
| isMinimized | boolean|Collapse the slider over the map view. 





### Enumeration: SliderStepType
#### Slider step types. 

|Property | Value | Description | 
|---------|--------|--------|
| Interval| 0| Interval. 
| Count| 1| Count. 
| Feature| 2| Feature. 



### Enumeration: SnapRequestType
#### Snap request types. 

|Property | Value | Description | 
|---------|--------|--------|
| SnapRequestType_None| 0| No snapping. 
| SnapRequestType_GeometricSnapping| 1| Geometric snapping. 
| SnapRequestType_VisualSnapping| 2| Visual snapping. 
| SnapRequestType_GeometricAndVisualSnapping| 3| Geometric and visual snapping. 



### Enumeration: SnapXYToleranceUnit
#### Snap XY tolerance units. 

|Property | Value | Description | 
|---------|--------|--------|
| SnapXYToleranceUnitPixel| 0| Pixels. 
| SnapXYToleranceUnitMap| 1| Map units. 




## CIMSnappingProperties
#### Represents snapping properties. 


### CIMSnappingProperties 

|Property | Type | Description | 
|---------|--------|--------|
| XYTolerance | double|Gets and sets the XY tolerance. 
| XYToleranceUnit | [enumeration SnapXYToleranceUnit](CIMMap.md#enumeration-snapxytoleranceunit)|Gets and sets the XY tolerance unit. 
| ZTolerance | double|Gets and sets the Z tolerance. 
| ZToleranceEnabled | boolean|Gets and sets a boolean value indicating if Z tolerance is enabled. 
| snapToSketchEnabled | boolean|Gets and sets a boolean value indicating if snapping to the sketch is enabled. 
| snapRequestType | [enumeration SnapRequestType](CIMMap.md#enumeration-snaprequesttype)|Gets and sets the snap request type. 
| geometricFeedbackColor | [Color](Types.md#color)|Gets and sets geometric feedback color. 
| visualFeedbackColor | [Color](Types.md#color)|Gets and sets the visual feedback color. 





### Enumeration: StereoModelDisplayMode
#### 

|Property | Value | Description | 
|---------|--------|--------|
| Default| 0| Display both the left and right images of the stereo model. 
| OnlyLeftImage| 1| Display only the left image of the stereo model. 
| OnlyRightImage| 2| Display only the right image of the stereo model. 
| None| 3| Turn off stereo model. 



### Enumeration: StereoSourceType
#### 

|Property | Value | Description | 
|---------|--------|--------|
| StereoModel| 0| Stereo source is a single stereo model (image pair). 
| StereoModelCollection| 1| Stereo source is a collection of stereo models (image pairs). 




## CIMSubtypeRule
#### Represents rule that will identify invalid and null subtypes on features. 


### CIMValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleID | string|Unique identifier of the validation rule. 
| title | string|Gets and sets the title for the validation rule. The title can be used to describe the conditions you are looking for with the validation rule. This is useful when you have multiple instances of the same RuleType to validate the same layers or standalone tables but with different validation parameters. This property is optional. 
| notes | string|Gets and sets the notes for the validation rule. This is the descriptive text for the validation results. This property is optional. 
| severity | long|Gets and sets the severity for the validation rule. This is the value that indicates the relative priority of the validation results on a scale of 1 (highest) to 5 (lowest). The default value of this property is 3. 
| tags | string|Gets and sets the tags for the validation rule. Tags are keywords or short phrases that facilitate discovery of the validation rule. Separate terms with commas. Overlapping Geometry is considered one tag, while Overlapping, geometry is considered two tags. This property is optional. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been created. 
| createdBy | string|The Portal login name of the user that created the validation rule. 
| lastModifiedDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been last modified. 
| lastModifiedBy | string|The Portal login name of the user that last modified the validation rule. 
| participatingLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layer URI strings on which the rule is applied to. 


### CIMReviewerValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleDefinitionExpression | string|Gets and sets the definition expression to run the validation rule on specific features in a layer or standalone table. This property is optional. 
| ignoreFields | IStringArray|An array of layer field names that need to be ignored for the validation rule. This property is optional. 


### CIMReviewerIndependentValidationRule 

|Property | Type | Description | 
|---------|--------|--------|


### CIMSubtypeRule 

|Property | Type | Description | 
|---------|--------|--------|
| checkNulls | boolean|Gets and sets whether or not to check for null subtypes. 





### Enumeration: SurfaceTINShadingMode
#### Surface TIN shading modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Smooth| 0| Smooth shading. 
| Flat| 1| Flat shading. 




## CIMTableToTableAttributeRule
#### Represents rule that will identify records based on comparing attributes values. It will take two inputs and some configuration parameter 


### CIMValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleID | string|Unique identifier of the validation rule. 
| title | string|Gets and sets the title for the validation rule. The title can be used to describe the conditions you are looking for with the validation rule. This is useful when you have multiple instances of the same RuleType to validate the same layers or standalone tables but with different validation parameters. This property is optional. 
| notes | string|Gets and sets the notes for the validation rule. This is the descriptive text for the validation results. This property is optional. 
| severity | long|Gets and sets the severity for the validation rule. This is the value that indicates the relative priority of the validation results on a scale of 1 (highest) to 5 (lowest). The default value of this property is 3. 
| tags | string|Gets and sets the tags for the validation rule. Tags are keywords or short phrases that facilitate discovery of the validation rule. Separate terms with commas. Overlapping Geometry is considered one tag, while Overlapping, geometry is considered two tags. This property is optional. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been created. 
| createdBy | string|The Portal login name of the user that created the validation rule. 
| lastModifiedDate | [TimeInstant](ExternalReferences.md#timeinstant)|The UTC date and time on which the validation rule has been last modified. 
| lastModifiedBy | string|The Portal login name of the user that last modified the validation rule. 
| participatingLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layer URI strings on which the rule is applied to. 


### CIMReviewerValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| ruleDefinitionExpression | string|Gets and sets the definition expression to run the validation rule on specific features in a layer or standalone table. This property is optional. 
| ignoreFields | IStringArray|An array of layer field names that need to be ignored for the validation rule. This property is optional. 


### CIMReviewerDependentValidationRule 

|Property | Type | Description | 
|---------|--------|--------|
| secondaryDatasets | [CIMRuleDatasetParameter](CIMMap.md#cimruledatasetparameter) |Array of dataset parameters used for validation rule. 
| secondaryLayers | [CIMRuleLayerDescription](Types.md#cimrulelayerdescription) |Array of layers used for validation rule. 


### CIMTableToTableAttributeRule 

|Property | Type | Description | 
|---------|--------|--------|
| checkAttributes | boolean| 
| attributeComparisons | [CIMFieldComparisonExpression](CIMMap.md#cimfieldcomparisonexpression)|Array Of CIMFieldComparisonExpresion 
| notQuery | boolean| 





### Enumeration: TimeSnapMode
#### Summary Mode used for snapping the map's current time settings Summary

|Property | Value | Description | 
|---------|--------|--------|
| Automatic| 0| Snap to an automatically-calculated time unit, based on the map's full time extent and view window size 
| Single| 1| Snap to a user-specified time unit, such as "Minute" or "Year" 
| Interval| 2| Snap to the time-interval value that has been defined for the Range Slider 




## CIMViewCamera
#### Represents a view camera. 


### CIMViewCamera 

|Property | Type | Description | 
|---------|--------|--------|
| heading | double|Gets and sets the heading. 
| pitch | double|Gets and sets the pitch. 
| roll | double|Gets and sets the roll. 
| scale | double|Gets and sets the scale. 
| x | double|Gets and sets X. 
| y | double|Gets and sets Y. 
| z | double|Gets and sets Z. 






## CIMViewKeyframe
#### Represents a view keyframe. 


### CIMViewKeyframe 

|Property | Type | Description | 
|---------|--------|--------|
| trackTime | double|Gets or sets the value of time in seconds that the keyframe exists in the track. 
| camera | [CIMKeyframeCamera](CIMMap.md#cimkeyframecamera)|Gets or sets the camera keyframe. 
| layers | [CIMKeyframeLayer](CIMMap.md#cimkeyframelayer) |Gets or sets the collection of layer keyframes. 
| range | [CIMKeyframeRange](CIMMap.md#cimkeyframerange)|Gets or sets the range keyframe. 
| time | [CIMKeyframeTime](CIMMap.md#cimkeyframetime)|Gets or sets the time keyframe. 






## CIMViewTrack
#### Represents a animation view track. 


### CIMViewTrack 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets or sets the name of the track. 
| keyframes | [CIMViewKeyframe](CIMMap.md#cimviewkeyframe) |Gets or sets the collection of view keyframes. 
| screenGraphics | [CIMAnimationScreenGraphic](CIMMap.md#cimanimationscreengraphic) |Gets or sets the list of graphic overlays used in the animation. 
| referenceResolutionWidth | int|Gets or sets the desired pixel width the animation was made to export at. 
| referenceResolutionHeight | int|Gets or sets the desired pixel height the animation was made to export at. 



