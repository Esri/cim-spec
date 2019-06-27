


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
| targets | [CIMSegmentationTarget](CIMBusinessAnalyst.md#cimsegmentationtarget) | The targets of the target group. 






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



