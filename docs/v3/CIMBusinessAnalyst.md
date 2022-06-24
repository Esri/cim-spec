


## CIMBAVariableList
#### Represents Business Analyst variable list. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMBAVariableList 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | Name of variable list. 
| iconData | string | Base64 encoded icon. 
| author | string | The name of the author of the variable list. 
| tags | string | The tags for the variable list. Tags are keywords or short phrases that facilitate discovery of the variable list. Separate terms with commas. 
| dataSource | string | Data source of the variable list. Structure of the value is TYPE;COUNTRY_INFO;LOCAL_DATA_INFO where TYPE can be ONLINE, LOCAL, or CUSTOM. COUNTRY_INFO is country_id{|hierarchy}. For example, US|census or US. LOCAL_DATA_INFO is ID of local dataset. For example, USA_ESRI_2019. For example, for local US 2019 dataset it will be: "LOCAL;;USA_ESRI_2019". If online US data source is used, it may be "ONLINE;US|census;". Can be value of baDataSource GP GPEnvironment variable. https://pro.arcgis.com/en/pro-app/tool-reference/environment-settings/ba-data-source.htm. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant) | Creation date of the variable list. 
| lastRevisionDate | [TimeInstant](ExternalReferences.md#timeinstant) | Last revision date of the variable list. 
| variables | [[CIMBAVariableListVariable]](CIMBusinessAnalyst.md#cimbavariablelistvariable) | Variables. 





### Enumeration: BAVariableListValueType
#### Represents variable value type. 

|Property | Value | Description | 
|---------|--------|--------|
| Number| 0| Number value type. 
| Percent| 1| Percent value type. 
| Average| 2| Average value type. 
| Index| 3| Index value type. 




## CIMBAVariableListVariable
#### Represents variable of at variable list. 


### CIMBAVariableListVariable 

|Property | Type | Description | 
|---------|--------|--------|
| names | [string] | Names of the variable. 
| valueTypes | [[CIMBAVariableListValueType]](CIMBusinessAnalyst.md#cimbavariablelistvaluetype) | Value types of the variable. If null, Number value type is used. 






## CIMHuffModelAttractivenessVariable
#### Represents attractiveness variable used in Huff Model. 


### CIMHuffModelAttractivenessVariable 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the variable. 
| exponent | double | The exponent of the variable. 






## CIMHuffModelCalibrationDocument
#### Represents a Huff Model calibration. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMHuffModelCalibrationDocument 

|Property | Type | Description | 
|---------|--------|--------|
| RMSError | double | RMS error of Huff Model calibration. 
| RMSErrorLinear | double | Linearized RMS error of Huff Model calibration. 
| attractivenessVariables | [[CIMHuffModelAttractivenessVariable]](CIMBusinessAnalyst.md#cimhuffmodelattractivenessvariable) | Attractiveness variables of Huff Model calibration. 
| distanceParameters | [CIMHuffModelDistanceParameters](CIMBusinessAnalyst.md#cimhuffmodeldistanceparameters) | Distance parameters of Huff Model calibration. 
| facilities | [DataConnection](Types.md#dataconnection) | Facilities dataset used in Huff Model calibration. 
| facilitiesIDFieldName | string | Facility ID field name used in Huff Model calibration. 
| customers | [DataConnection](Types.md#dataconnection) | Customers dataset used in Huff Model calibration. 
| customersIDFieldName | string | Customer ID field name used in Huff Model calibration. 
| customerWeightFieldName | string | Customer weight field name used in Huff Model calibration. 
| salesPotential | [DataConnection](Types.md#dataconnection) | Sales potential dataset used in Huff Model calibration. 
| salesPotentialIDFieldName | string | Sales potential ID field name used in Huff Model calibration. 
| author | string | Author of Huff Model calibration. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant) | Creation date of Huff Model calibration. 
| lastRevisionDate | [TimeInstant](ExternalReferences.md#timeinstant) | Last revision date of Huff Model calibration. 






## CIMHuffModelDistanceParameters
#### Distance properties of the Huff Model calibration item. 


### CIMHuffModelDistanceParameters 

|Property | Type | Description | 
|---------|--------|--------|
| exponent | double | The exponent. 
| dataSource | string | Data source used in calculation of distances. Structure of the value is TYPE;COUNTRY_INFO;LOCAL_DATA_INFO where TYPE can be ONLINE, LOCAL, or CUSTOM. COUNTRY_INFO is country_id{|hierarchy}. For example, US|census or US. LOCAL_DATA_INFO is ID of local dataset. For example, USA_ESRI_2019. For example, for local US 2019 dataset it will be: "LOCAL;;USA_ESRI_2019". If online US data source is used, it may be "ONLINE;US|census;". Can be value of baDataSource GP GPEnvironment variable. https://pro.arcgis.com/en/pro-app/tool-reference/environment-settings/ba-data-source.htm. 
| distanceUnits | [LinearUnit](ExternalReferences.md#linearunit) | Distance units used in calculation of distances. 
| useTimeUnits | boolean | A value indicating whether to use time units. 
| timeUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | Time units used in calculation of distances. 
| useNetworkDistance | boolean | A value indicating whether to use network dataset to calculate distances. 
| travelModeId | string | ID of travel mode used in calculation of distances. 
| towardsFacility | boolean | A value indicating whether to calculate distances toward facilities. 
| timeOfDay | [TimeInstant](ExternalReferences.md#timeinstant) | Time of day used in calculation of distances. 
| timeZone | string | Time zone used in calculation of distances. 






## CIMSegmentationProfile
#### Business Analyst segmentation profile. Segmentation profile represents distribution of the market (e.g. people or households) between the segments of the segmentation system. For example, it could represent the distribution of the customer base between the segments. Segmentation profile can include the volumetric information in addition to the counts, e.g. it could also provide the distribution of the sales between segments. 


### CIMSegmentationProfile 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the segmentation profile. 
| segmentationSystem | string | The segmentation system of the segmentation profile. 
| segmentationBase | string | Segmentation base of the segmentation profile. 
| hasVolumetricData | boolean | A value indicating whether the segmentation profile contains volumetric information. 
| author | string | The name of the author of the segmentation profile. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant) | Creation date of the segmentation profile. 
| lastRevisionDate | [TimeInstant](ExternalReferences.md#timeinstant) | Last revision date of the segmentation profile. 
| counts | [long] | The counts of the segmentation profile. 
| volumetricValues | [double] | The volumetric values of the segmentation profile. 






## CIMSegmentationProfileDocument
#### Represents a document used for saving segmentation profile. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMSegmentationProfileDocument 

|Property | Type | Description | 
|---------|--------|--------|
| profile | [CIMSegmentationProfile](CIMBusinessAnalyst.md#cimsegmentationprofile) | The segmentation profile. 






## CIMSegmentationTarget
#### Business Analyst segmentation target. Target is a collection of market segments that are treated as a whole. A user might apply the same marketing strategy to all segments in a target, for example. 


### CIMSegmentationTarget 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of target. 
| segmentIDs | [string] | The segment IDs of the target. 
| color | [Color](Types.md#color) | The color of the target. 






## CIMSegmentationTargetGroup
#### Business Analyst target group. Target group represents a collection of targets. 


### CIMSegmentationTargetGroup 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the target group. 
| segmentationSystem | string | The segmentation system of the target group. 
| description | string | Description of the target group. 
| author | string | The name of the author of the target group. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant) | Creation date of the target group. 
| lastRevisionDate | [TimeInstant](ExternalReferences.md#timeinstant) | Last revision date of the target group. 
| targets | [[CIMSegmentationTarget]](CIMBusinessAnalyst.md#cimsegmentationtarget) | The targets of the target group. 
| visualizationProperties | [CIMSegmentationTargetGroupVisualizationProperties](CIMBusinessAnalyst.md#cimsegmentationtargetgroupvisualizationproperties) | Visualization properties of the target group. 






## CIMSegmentationTargetGroupDocument
#### Represents a document used for saving target group. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMSegmentationTargetGroupDocument 

|Property | Type | Description | 
|---------|--------|--------|
| targetGroup | [CIMSegmentationTargetGroup](CIMBusinessAnalyst.md#cimsegmentationtargetgroup) | The target group. 






## CIMSegmentationTargetGroupVisualizationProperties
#### Visualization properties of Business Analyst Segmentation target group. 


### CIMSegmentationTargetGroupVisualizationProperties 

|Property | Type | Description | 
|---------|--------|--------|
| targetProfile | [CIMSegmentationProfile](CIMBusinessAnalyst.md#cimsegmentationprofile) | The target profile of the target group. 
| baseProfile | [CIMSegmentationProfile](CIMBusinessAnalyst.md#cimsegmentationprofile) | The base profile of the target group. 
| thresholdIndex | double | The Threshold Index of the target group. 
| thresholdComposition | double | The Threshold Composition of the target group. 



