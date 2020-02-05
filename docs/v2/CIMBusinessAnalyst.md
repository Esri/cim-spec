


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
| dataSource | string | Data source used in calculation of distances. 
| distanceUnits | [enumeration esriUnits](ExternalReferences.md#enumeration-esriunits) | Distance units used in calculation of distances. 
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
| volumetricInformation | [long] | The volumetric values of the segmentation profile. 
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



