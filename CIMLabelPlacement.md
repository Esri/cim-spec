

### Enumeration: FeaturesToLabel
#### A list of types of features to label. 

|Property | Value | Description | 
|---------|--------|--------|
| AllVisibleFeatures| 0| All visible features. 
| MostCurrentTrackFeatures| 1| The most current feature when a track is initialized. 




## CIMLabelClass
#### Represents a label class which describes how to generate a set of text labels from a group of features in a feature layer. 


### CIMLabelClass 

|Property | Type | Description | 
|---------|--------|--------|
| expression | string|Gets and sets the label expression. 
| expressionEngine | [enumeration LabelExpressionEngine](CIMLabelPlacement.md#enumeration-labelexpressionengine)|Gets and sets the label expression engine (the language the expression is written in). 
| featuresToLabel | [enumeration FeaturesToLabel](CIMLabelPlacement.md#enumeration-featurestolabel)|Gets and sets a parameter indicating which features to label. 
| maplexLabelPlacementProperties | [CIMMaplexLabelPlacementProperties](CIMLabelPlacement.md#cimmaplexlabelplacementproperties)|Gets and sets the Maplex placement properties which are used when the map uses the Maplex label engine. 
| maximumScale | double|Gets and sets the maximum scale for labeling (set as the denominator of the scale's representative fraction) 
| minimumScale | double|Gets and sets the minimum scale for labeling (set as the denominator of the scale's representative fraction) 
| name | string|Gets and sets the name of the label class. 
| priority | long|Gets and sets the priority of the label class. 
| standardLabelPlacementProperties | [CIMStandardLabelPlacementProperties](CIMLabelPlacement.md#cimstandardlabelplacementproperties)|Gets and sets the standard placement properties which are used when the map uses the standard label engine. 
| textSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the text symbol of the label class. 
| useCodedValue | boolean|Gets and sets a boolean value indicating whether or not to use coded value domain descriptions when labeling. 
| whereClause | string|Gets and sets the SQL where clause of which features to label with this label class. 
| visibility | boolean|Gets and sets a boolean value indicating whether this label class is visible. 
| ID | long|Gets and sets the ID of the label class. This property is only used in the context of annotation. 






## CIMLabelClassProperties
#### Represents label class properties. 





### Enumeration: LabelExpressionEngine
#### Label expression engine types. 

|Property | Value | Description | 
|---------|--------|--------|
| VBScript| 0| VBScript 
| JScript| 1| JScript 
| Python| 2| Python 
| Arcade| 3| Arcade 



### Enumeration: LabelFeatureType
#### The label feature types. 

|Property | Value | Description | 
|---------|--------|--------|
| Point| 0| Point or multipoint. 
| Line| 1| Polyline. 
| Polygon| 2| Polygon or multipatch. 



### Enumeration: MaplexAbbreviationType
#### Maplex abbreviation types. 

|Property | Value | Description | 
|---------|--------|--------|
| Translation| 0| Translation type which always abbreviates. 
| Keyword| 1| Keyword type which abbreviates when needed for space. 
| Ending| 2| Ending type which abbreviates when needed for space for words at the end of the string (like a street type). 



### Enumeration: MaplexAnchorPointType
#### Maplex anchor point types. 

|Property | Value | Description | 
|---------|--------|--------|
| GeometricCenter| 0| Geometric center (of the potentially clipped geoemtry). 
| ErodedCenter| 1| Eroded center. 
| Perimeter| 2| Perimeter. 
| UnclippedGeometricCenter| 3| Unclipped geometric center. 



### Enumeration: MaplexConnectionType
#### Maplex connection types. 

|Property | Value | Description | 
|---------|--------|--------|
| MinimizeLabels| 0| Minimize labels. 
| Unambiguous| 1| Unambiguous (place extra labels to prevent ambiguity) 



### Enumeration: MaplexConstrainOffset
#### Maplex offset constraint types. 

|Property | Value | Description | 
|---------|--------|--------|
| NoConstraint| 0| No constraint. 
| AboveLine| 1| Above the line. 
| BelowLine| 2| Below the line. 
| LeftOfLine| 3| Left of the line. 
| RightOfLine| 4| Right of the line. 



### Enumeration: MaplexContourAlignmentType
#### Maplex contour alignment types. 

|Property | Value | Description | 
|---------|--------|--------|
| Uphill| 0| Align labels according to the terrain so the tops point uphill. 
| Page| 1| Align labels according to the page (or display). 



### Enumeration: MaplexContourLadderType
#### Maplex contour ladder types. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No ladders. 
| Straight| 1| Straight ladders. 
| Curved| 2| Curved ladders. 




## CIMMaplexDictionary
#### Represents a Maplex dictionary. 


### CIMMaplexDictionary 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the Maplex dictionary name. 
| maplexDictionary | [CIMMaplexDictionaryEntry](CIMLabelPlacement.md#cimmaplexdictionaryentry) |Gets and sets the Maplex dictionary entries. 






## CIMMaplexDictionaryEntry
#### Represents a Maplex dictionary entry. 


### CIMMaplexDictionaryEntry 

|Property | Type | Description | 
|---------|--------|--------|
| abbreviation | string|Gets and sets the abbreviation. 
| text | string|Gets and sets the text to abbreviate. 
| maplexAbbreviationType | [enumeration MaplexAbbreviationType](CIMLabelPlacement.md#enumeration-maplexabbreviationtype)|Gets and sets the abbreviation type. 






## CIMMaplexExternalZonePriorities
#### Represents Maplex external zone priorities. 


### CIMMaplexExternalZonePriorities 

|Property | Type | Description | 
|---------|--------|--------|
| aboveLeft | long|Gets and sets priortiy for this position. 
| aboveCenter | long|Gets and sets priortiy for this position. 
| aboveRight | long|Gets and sets priortiy for this position. 
| centerRight | long|Gets and sets priortiy for this position. 
| belowRight | long|Gets and sets priortiy for this position. 
| belowCenter | long|Gets and sets priortiy for this position. 
| belowLeft | long|Gets and sets priortiy for this position. 
| centerLeft | long|Gets and sets priortiy for this position. 






## CIMMaplexGeneralPlacementProperties
#### Represents Maplex general placement properties. 


### CIMGeneralPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| drawUnplacedLabels | boolean|Gets and sets a boolean option indicating whether or not to draw unplaced labels 
| invertedLabelTolerance | double|Gets and sets the inverted label tolerance which is the angle at which the label orientation is switched. 
| rotateLabelWithDisplay | boolean|Gets and sets a boolean option indicating whether or not rotate labels when the display rotates. 
| unplacedLabelColor | [Color](Types.md#color)|Gets and sets the unplaced label color. 


### CIMMaplexGeneralPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| allowBorderOverlap | boolean|Gets and sets a boolean value for whether or not to allow border overlap. 
| dictionaries | [CIMMaplexDictionary](CIMLabelPlacement.md#cimmaplexdictionary) |Gets and sets the Maplex dictionaries. 
| keyNumberGroups | [CIMMaplexKeyNumberGroup](CIMLabelPlacement.md#cimmaplexkeynumbergroup) |Gets and sets the key number groups. 
| placementQuality | [enumeration MaplexQualityType](CIMLabelPlacement.md#enumeration-maplexqualitytype)|Gets and sets the placement quality. 





### Enumeration: MaplexGraticuleAlignmentType
#### Maplex graticule alignment types. 

|Property | Value | Description | 
|---------|--------|--------|
| Straight| 0| Straight alignment, may flip. 
| StraightNoFlip| 1| Straight alignment, no flip. 
| Curved| 2| Curved alignment, may flip. 
| CurvedNoFlip| 3| Curved alignment, no flip. 




## CIMMaplexInternalZonePriorities
#### Represents Maplex internal zone priorities. 


### CIMMaplexInternalZonePriorities 

|Property | Type | Description | 
|---------|--------|--------|
| aboveLeft | long|Gets and sets priortiy for this position. 
| aboveCenter | long|Gets and sets priortiy for this position. 
| aboveRight | long|Gets and sets priortiy for this position. 
| centerRight | long|Gets and sets priortiy for this position. 
| belowRight | long|Gets and sets priortiy for this position. 
| belowCenter | long|Gets and sets priortiy for this position. 
| belowLeft | long|Gets and sets priortiy for this position. 
| centerLeft | long|Gets and sets priortiy for this position. 
| center | long|Gets and sets priortiy for this position. 






## CIMMaplexKeyNumberGroup
#### Represents a Maplex key number group. 


### CIMMaplexKeyNumberGroup 

|Property | Type | Description | 
|---------|--------|--------|
| delimiterCharacter | string|Gets and sets the delimiter character of the key number. 
| horizontalAlignment | [enumeration MaplexKeyNumberHorizontalAlignment](CIMLabelPlacement.md#enumeration-maplexkeynumberhorizontalalignment)|Gets and sets the horizontal alignment. 
| maximumNumberOfLines | long|Gets and sets the maximum number of lines. 
| minimumNumberOfLines | long|Gets and sets the minimum number of lines. 
| name | string|Gets and sets the name of the group. 
| numberResetType | [enumeration MaplexKeyNumberResetType](CIMLabelPlacement.md#enumeration-maplexkeynumberresettype)|Gets and sets the number reset type. 





### Enumeration: MaplexKeyNumberHorizontalAlignment
#### Maplex key number group horizontal alignment types. 

|Property | Value | Description | 
|---------|--------|--------|
| Auto| 0| Automatic alignment. 
| Left| 1| Left alignment. 
| Right| 2| Right alignment. 



### Enumeration: MaplexKeyNumberResetType
#### Identifies the options for reseting the key numbers in a Maplex key numbering group. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Key numbers are not reset. 
| Maybe| 1| Key numbers may be reset. 
| Always| 2| Key numbers are always reset. 



### Enumeration: MaplexLabelAnchorPoint
#### Maplex label anchor point. 

|Property | Value | Description | 
|---------|--------|--------|
| CenterOfLabel| 0| Anchor to the center of the label. 
| NearestSideOfLabel| 1| Anchor to the nearest side of the label. 
| FurthestSideOfLabel| 2| Anchor to the furthest side of the label. 




## CIMMaplexLabelPlacementProperties
#### Represents Maplex label placement properties. 


### CIMLabelPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| featureType | [enumeration LabelFeatureType](CIMLabelPlacement.md#enumeration-labelfeaturetype)|Gets and sets the feature type being labeled. 


### CIMMaplexLabelPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| alignLabelToLineDirection | boolean|Gets and sets a boolean which indicates whether to align the label with the label direction so the label may appear upside down. 
| allowAsymmetricOverrun | boolean|Gets and sets a boolean which indicates whether a label may overrun one side of a polygon feature. 
| allowStraddleStacking | boolean|Gets and sets a boolean which indicates whether a stacked label may straddle the line feature. 
| avoidPolygonHoles | boolean|Gets and sets a boolean which indicates whether labels should avoid holes in polygons. 
| backgroundLabel | boolean|Gets and sets a boolean which indicates whether to place the label first and allow other labels to be placed over it. 
| boundaryLabelingAllowHoles | boolean|Gets and sets a boolean which indicates whether to allow holes in boundary labeling. 
| boundaryLabelingAllowSingleSided | boolean|Gets and sets a boolean which indicates whether to allow single sided boundary labeling. 
| boundaryLabelingSingleSidedOnLine | boolean|Gets and sets a boolean which indicates whether single sided boundary label is centered on line. 
| canAbbreviateLabel | boolean|Gets and sets a boolean which indicates whether to abbreviate the label using an abbreviation dictionary. 
| canFlipStackedStreetLabel | boolean|Gets and sets a boolean which indicates whether a stacked label may be flipped over to obtain a better position. 
| canKeyNumberLabel | boolean|Gets and sets a boolean which indicates whether to key number the label and feature. 
| canOverrunFeature | boolean|Gets and sets a boolean which indicates whether to place the label over end of line or over polygon boundary. 
| canPlaceLabelOnTopOfFeature | boolean|Gets and sets a boolean which indicates whether the label can be placed on top of the street feature. 
| canPlaceLabelOutsidePolygon | boolean|Gets and sets a boolean which indicates whether to place a label outside the polygon if it does not fit inside. 
| canReduceFontSize | boolean|Gets and sets a boolean which indicates whether to reduce the size of the font. 
| canReduceLeading | boolean|Gets and sets a boolean which indicates whether the leading can be reduced for a stacked label. 
| canRemoveOverlappingLabel | boolean|Gets and sets a boolean which indicates whether to remove the label if it overlaps with other labels. 
| canShiftPointLabel | boolean|Gets and sets a boolean which indicates whether to allow the point label to be shifted upon a fixed position. 
| canStackLabel | boolean|Gets and sets a boolean which indicates whether to stack the label to obtain a better position. 
| canTruncateLabel | boolean|Gets and sets a boolean which indicates whether to truncate the label using an algorithm. 
| connectionType | [enumeration MaplexConnectionType](CIMLabelPlacement.md#enumeration-maplexconnectiontype)|Gets and sets the options for connecting line features. 
| constrainOffset | [enumeration MaplexConstrainOffset](CIMLabelPlacement.md#enumeration-maplexconstrainoffset)|Gets and sets the label constraint options. 
| contourAlignmentType | [enumeration MaplexContourAlignmentType](CIMLabelPlacement.md#enumeration-maplexcontouralignmenttype)|Gets and sets the options for the contour label alignment. 
| contourLadderType | [enumeration MaplexContourLadderType](CIMLabelPlacement.md#enumeration-maplexcontourladdertype)|Gets and sets the options for the contour label ladder types. 
| contourMaximumAngle | long|Gets and sets the maximum angle at which a contour label may be placed. 
| dictionaryName | string|Gets and sets the name of the abbreviations dictionary referenced by this layer. 
| enableConnection | boolean|Gets and sets a boolean which indicates whether to turn off line connection. 
| enablePointPlacementPriorities | boolean|Gets and sets a boolean which indicates whether to use user-defined point placement priorities. 
| enablePolygonFixedPosition | boolean|Gets and sets a boolean which indicates whether a label is to be placed at a fixed position in the polygon. 
| enableSecondaryOffset | boolean|Gets and sets a boolean which indicates whether to place a label at a secondary offset from the line feature. 
| featureWeight | long|Gets and sets the feature weight which controls which features may be overlapped and to what extent. 
| fontHeightReductionLimit | double|Gets and sets font height reduction limit. The font may be reduced in height until this limit is reached. 
| fontHeightReductionStep | double|Gets and sets font height reduction step. This is the step interval for font height reduction. 
| fontWidthReductionLimit | double|Gets and sets font width reduction limit. The font may be reduced in width until this limit is reached. 
| fontWidthReductionStep | double|Gets and sets font width reduction step. This is the step interval for font width reduction. 
| graticuleAlignment | boolean|Gets and sets a boolean which indicates whether to enable graticule alignment. 
| graticuleAlignmentType | [enumeration MaplexGraticuleAlignmentType](CIMLabelPlacement.md#enumeration-maplexgraticulealignmenttype)|Gets and sets the options for the graticule alignment type. 
| isLabelBufferHardConstraint | boolean|Gets and sets a boolean which indicates whether the label buffer is a hard constraint and must be honored. 
| isMinimumSizeBasedOnArea | boolean|Gets and sets a boolean which indicates whether the minimum feature size for labeling is based on area. 
| isOffsetFromFeatureGeometry | boolean|Gets and sets a boolean which indicates whether to measure the label offset from the feature geometry. 
| keyNumberGroupName | string|Gets and sets the name of the key number group to use for key numbering the labels. 
| labelBuffer | long|Gets and sets the label buffer. Increase buffer to stop labels from being placed too close to each other. 
| labelLargestPolygon | boolean|Gets and sets a boolean which indicates whether to label only the largest polygon in a compound polygon feature. 
| labelPriority | long|Gets and sets the label priority. Label prority controls approximate placement order. 
| labelStackingProperties | [CIMMaplexLabelStackingProperties](CIMLabelPlacement.md#cimmaplexlabelstackingproperties)|Gets and sets the label stacking properties for a layer. 
| lineFeatureType | [enumeration MaplexLineFeatureType](CIMLabelPlacement.md#enumeration-maplexlinefeaturetype)|Gets and sets the line feature type. 
| linePlacementMethod | [enumeration MaplexLinePlacementMethod](CIMLabelPlacement.md#enumeration-maplexlineplacementmethod)|Gets and sets the line placement method. 
| maximumCharacterSpacing | double|Gets and sets the maximum character spacing. Character spacing may be increased up to this limit. 
| maximumLabelOverrun | double|Gets and sets the maximum distance that a label is allowed to overrun the end of its feature. 
| maximumLabelOverrunUnit | [enumeration MaplexUnit](CIMLabelPlacement.md#enumeration-maplexunit)|Gets and sets the label overrun unit. 
| maximumWordSpacing | double|Gets and sets maximum word spacing. The word spacing may be increased upto this limit. 
| minimumEndOfStreetClearance | double|Gets and sets minimum clearance between street label and street end. 
| minimumFeatureSizeUnit | [enumeration MaplexUnit](CIMLabelPlacement.md#enumeration-maplexunit)|Gets and sets minimum feature size unit. 
| minimumRepetitionInterval | double|Gets and sets the interval that must elapse before label is repeated. 
| minimumSizeForLabeling | double|Gets and sets the minimum size of a line or area feature for it to be labeled. 
| multiPartOption | [enumeration MaplexMultiPartOption](CIMLabelPlacement.md#enumeration-maplexmultipartoption)|Gets and sets the option for labeling multi-part shapes. 
| neverRemoveLabel | boolean|Gets and sets a boolean which indicates whether to not remove the label if no position is found. 
| offsetAlongLineProperties | [CIMMaplexOffsetAlongLineProperties](CIMLabelPlacement.md#cimmaplexoffsetalonglineproperties)|Gets and sets the offset along line properties for a layer. 
| pointExternalZonePriorities | [CIMMaplexExternalZonePriorities](CIMLabelPlacement.md#cimmaplexexternalzonepriorities)|Gets and sets the proprties which control placement of a label around point feature. 
| pointPlacementMethod | [enumeration MaplexPointPlacementMethod](CIMLabelPlacement.md#enumeration-maplexpointplacementmethod)|Gets and sets the point placement method. 
| polygonAnchorPointType | [enumeration MaplexAnchorPointType](CIMLabelPlacement.md#enumeration-maplexanchorpointtype)|Gets and sets the polygon anchor point type. 
| polygonBoundaryWeight | long|Gets and sets the feature weight for the boundary of the polygon. 
| polygonExternalZones | [CIMMaplexExternalZonePriorities](CIMLabelPlacement.md#cimmaplexexternalzonepriorities)|Gets and sets the placement priorities associated with zones external to the polygon. 
| polygonFeatureType | [enumeration MaplexPolygonFeatureType](CIMLabelPlacement.md#enumeration-maplexpolygonfeaturetype)|Gets and sets the polygon feature type. 
| polygonInternalZones | [CIMMaplexInternalZonePriorities](CIMLabelPlacement.md#cimmaplexinternalzonepriorities)|Gets and sets the placement priorities associated with zones internal to the polygon. 
| polygonPlacementMethod | [enumeration MaplexPolygonPlacementMethod](CIMLabelPlacement.md#enumeration-maplexpolygonplacementmethod)|Gets and sets the polygon placement method. 
| preferHorizontalPlacement | boolean|Gets and sets a boolean which indicates if there is a preference to place the label horizontally. 
| preferLabelNearJunction | boolean|Gets and sets a boolean which indicates a preference for placing a line label near a junction. 
| preferLabelNearJunctionClearance | double|Gets and sets the preferred clearance for placing a line label near a junction. 
| preferLabelNearMapBorder | boolean|Gets and sets a boolean which indicates a preference for placing a line label near the map border. 
| preferLabelNearMapBorderClearance | double|Gets and sets the preferred clearance for placing a line label near the map border. 
| preferredEndOfStreetClearance | double|Gets and sets the preferred clearance between street label and street end. 
| primaryOffset | double|Gets and sets the primary offset between label and symbol. 
| primaryOffsetUnit | [enumeration MaplexUnit](CIMLabelPlacement.md#enumeration-maplexunit)|Gets and sets the unit of the primary offset. 
| removeExtraLineBreaks | boolean|Gets and sets a boolean which indicates whether extra line breaks are removed from the label text. 
| removeExtraWhiteSpace | boolean|Gets and sets a boolean which indicates whether extra white space characters are removed from the label text. 
| repeatLabel | boolean|Gets and sets a boolean which indicates whether to enable the repetition of label along line feature. 
| repetitionIntervalUnit | [enumeration MaplexUnit](CIMLabelPlacement.md#enumeration-maplexunit)|Gets and sets the label repetition interval unit. 
| rotationProperties | [CIMMaplexRotationProperties](CIMLabelPlacement.md#cimmaplexrotationproperties)|Gets and sets the label label rotation properties. 
| secondaryOffset | double|Gets and sets the secondary offset between label and symbol. 
| secondaryOffsetMaximum | double|Gets and sets the secondary offset maximum. 
| secondaryOffsetMinimum | double|Gets and sets the secondary offset minimum. 
| spreadCharacters | boolean|Gets and sets a boolean which indicates whether to spread label characters along line features. 
| spreadWords | boolean|Gets and sets a boolean which indicates whether to whether to spread words along line features. 
| strategyPriorities | [CIMMaplexStrategyPriorities](CIMLabelPlacement.md#cimmaplexstrategypriorities)|Gets and sets the priority of a placement strategy when placing text. 
| thinDuplicateLabels | boolean|Gets and sets a boolean which indicates whether to remove duplicate labels that lie within a specified distance of each other. 
| thinningDistance | double|Gets and sets the distance used to control the thinning of duplicate labels. 
| thinningDistanceUnit | [enumeration MaplexUnit](CIMLabelPlacement.md#enumeration-maplexunit)|Gets and sets the thinning distance unit. 
| truncationMarkerCharacter | string|Gets and sets the marker character used by the truncation strategy. 
| truncationMinimumLength | long|Gets and sets the minimum length of a label used by the truncation strategy. 
| truncationPreferredCharacters | string|Gets and sets the preferred characters used by the truncation strategy. These characters will be removed as needed. 
| useExactSymbolOutline | boolean|Gets and sets a boolean which indicates whether to use the exact polygon outline of a symbol when measuring the label offset. 





### Enumeration: MaplexLabelRotationType
#### Maplex rotation types. 

|Property | Value | Description | 
|---------|--------|--------|
| Geographic| 0| Geographic rotation. 
| Arithmetic| 1| Arithmetic rotation. 
| Radians| 2| Rotation in radians. 
| AV3| 3| ArcView 3 rotation. 




## CIMMaplexLabelStackingProperties
#### Represents Maplex label stacking properties. 


### CIMMaplexLabelStackingProperties 

|Property | Type | Description | 
|---------|--------|--------|
| stackAlignment | [enumeration MaplexStackingAlignment](CIMLabelPlacement.md#enumeration-maplexstackingalignment)|Gets and sets the stacking alignment. 
| maximumNumberOfLines | long|Gets and sets the maximum number of lines. 
| minimumNumberOfCharsPerLine | long|Gets and sets the minimum number of characters per line. 
| maximumNumberOfCharsPerLine | long|Gets and sets the maximum number of characters per line. 
| separators | [CIMMaplexStackingSeparator](CIMLabelPlacement.md#cimmaplexstackingseparator) |Gets and sets the stacking separators. 





### Enumeration: MaplexLineFeatureType
#### Maplex line feature types. 

|Property | Value | Description | 
|---------|--------|--------|
| General| 0| General line labeling. 
| Street| 1| Street labeling. 
| StreetAddressRange| 2| Street address labeling. 
| Contour| 3| Contour labeling. 
| River| 4| River labeling. 



### Enumeration: MaplexLinePlacementMethod
#### Maplex line placement methods. 

|Property | Value | Description | 
|---------|--------|--------|
| CenteredHorizontalOnLine| 0| Centered horizontal on the line. 
| CenteredStraightOnLine| 1| Centered straight on the line. 
| CenteredCurvedOnLine| 2| Centered curved on the line. 
| CenteredPerpendicularOnLine| 3| Centered perpendicular on the line. 
| OffsetHorizontalFromLine| 4| Offset and horizontal from the line. 
| OffsetStraightFromLine| 5| Offset and straight from the line. 
| OffsetCurvedFromLine| 6| Offset and curved from the line. 
| OffsetPerpendicularFromLine| 7| Offset perpendicular from the line. 



### Enumeration: MaplexMultiPartOption
#### Maplex multipart options 

|Property | Value | Description | 
|---------|--------|--------|
| OneLabelPerFeature| 0| One label per feature. 
| OneLabelPerPart| 1| One label per feature part. 
| OneLabelPerSegment| 2| One label per segment. 



### Enumeration: MaplexOffsetAlongLineMethod
#### Maplex offset along the line methods. 

|Property | Value | Description | 
|---------|--------|--------|
| BestPositionAlongLine| 0| Best position along the line. 
| BeforeStartOfLine| 1| Before the start of the line. 
| AlongLineFromStart| 2| Along the line from the start. 
| AlongLineFromEnd| 3| Along the line from the end. 
| AfterEndOfLine| 4| After the end of the line. 




## CIMMaplexOffsetAlongLineProperties
#### Represents Maplex offset along the line properties. 


### CIMMaplexOffsetAlongLineProperties 

|Property | Type | Description | 
|---------|--------|--------|
| placementMethod | [enumeration MaplexOffsetAlongLineMethod](CIMLabelPlacement.md#enumeration-maplexoffsetalonglinemethod)|Gets and sets the placement method. 
| labelAnchorPoint | [enumeration MaplexLabelAnchorPoint](CIMLabelPlacement.md#enumeration-maplexlabelanchorpoint)|Gets and sets the label anchor point for positioning along the line. 
| distance | double|Gets and sets the distance along the line. 
| tolerance | double|Gets and sets the tolerance. 
| distanceUnit | [enumeration MaplexUnit](CIMLabelPlacement.md#enumeration-maplexunit)|Gets and sets the distance unit. 
| useLineDirection | boolean|Gets and sets a boolean value indicating whether or not use the line direction. 





### Enumeration: MaplexPointPlacementMethod
#### Maplex point placement methods. 

|Property | Value | Description | 
|---------|--------|--------|
| AroundPoint| 0| Around the point. 
| CenteredOnPoint| 1| Centered on the point. 
| NorthOfPoint| 2| Above the point. 
| NorthEastOfPoint| 3| Above and right of the point. 
| EastOfPoint| 4| Right of the point. 
| SouthEastOfPoint| 5| Below and to the right of the point. 
| SouthOfPoint| 6| Below the point. 
| SouthWestOfPoint| 7| Below and to the left of the point. 
| WestOfPoint| 8| Left of the point, 
| NorthWestOfPoint| 9| Above and left of the point. 



### Enumeration: MaplexPolygonFeatureType
#### Maplex polygon feature types. 

|Property | Value | Description | 
|---------|--------|--------|
| General| 0| General polygon placement. 
| LandParcel| 1| Land parcel polygon placement. 
| River| 2| River polygon placement. 
| Boundary| 3| Boundary polygon placement. 



### Enumeration: MaplexPolygonPlacementMethod
#### Maplex polygon placement methods. 

|Property | Value | Description | 
|---------|--------|--------|
| HorizontalInPolygon| 0| Horizontal in the polygon. 
| StraightInPolygon| 1| Straight in the polygon. 
| CurvedInPolygon| 2| Curved in the polygon. 
| HorizontalAroundPolygon| 3| Horizontal around the polygon. 
| RepeatAlongBoundary| 4| Boundary placement. 
| CurvedAroundPolygon| 5| Curved outside the polygon. 



### Enumeration: MaplexQualityType
#### Maplex quality types. 

|Property | Value | Description | 
|---------|--------|--------|
| Low| 0| Draft quality. 
| Medium| 1| Fast quality. 
| High| 2| Best quality. 



### Enumeration: MaplexRotationAlignmentType
#### Maplex rotation alignment types. 

|Property | Value | Description | 
|---------|--------|--------|
| Straight| 0| Straight placement. 
| Horizontal| 1| Horizontal placement. 
| Perpendicular| 2| Perpendicular placement. 




## CIMMaplexRotationProperties
#### Represents Maplex rotation properties. 


### CIMMaplexRotationProperties 

|Property | Type | Description | 
|---------|--------|--------|
| enable | boolean|Gets and sets a boolean value indicating whether or enable rotation. 
| rotationType | [enumeration MaplexLabelRotationType](CIMLabelPlacement.md#enumeration-maplexlabelrotationtype)|Gets and sets the rotation type. 
| rotationField | string|Gets and sets the rotation field to get values from. 
| perpendicularToAngle | boolean|Gets and sets a boolean value indicating whether or place the label perpendicular to the angle. 
| alignLabelToAngle | boolean|Gets and sets a boolean value indicating whether or not to align the label to the angle. 
| alignmentType | [enumeration MaplexRotationAlignmentType](CIMLabelPlacement.md#enumeration-maplexrotationalignmenttype)|Gets and sets the alignment type. 
| additionalAngle | long|Gets and sets additional angle to add to the data value. 





### Enumeration: MaplexStackingAlignment
#### Maplex stacking alignment. 

|Property | Value | Description | 
|---------|--------|--------|
| ChooseBest| 0| Allow the label engine to choose the best alignment. 
| ConstrainLeftOrRight| 1| Constrain alignment of the left or right. 
| ConstrainLeft| 2| Constrain alignment of the left. 
| ConstrainRight| 3| Constrain alignment of the right. 
| ConstrainCenter| 4| Constrain alignment of the center. 




## CIMMaplexStackingSeparator
#### Represents a Maplex stacking separator. 


### CIMMaplexStackingSeparator 

|Property | Type | Description | 
|---------|--------|--------|
| separator | string|Gets and sets the separator as a string of one character. 
| visible | boolean|Gets and sets a boolean value indicating whether or not the separator should be visible after stacking. 
| splitForced | boolean|Gets and sets a boolean value indicating whether or not to force a split at every instance of the separator. 
| splitAfter | boolean|Gets and sets a boolean value indicating whether or not to split after the separator. 






## CIMMaplexStrategyPriorities
#### Represents Maplex strategy priorities. 


### CIMMaplexStrategyPriorities 

|Property | Type | Description | 
|---------|--------|--------|
| stacking | long|Gets and sets the priority for stacking. 
| overrun | long|Gets and sets the priority for overrun. 
| fontCompression | long|Gets and sets the priority for font compression. 
| fontReduction | long|Gets and sets the priority for font reduction. 
| abbreviation | long|Gets and sets the priority for abbreviation. 





### Enumeration: MaplexUnit
#### Maplex units. 

|Property | Value | Description | 
|---------|--------|--------|
| Map| 0| Use the map units. 
| MM| 1| Millimeters. 
| Inch| 2| Inch. 
| Point| 3| Point. 
| Percentage| 4| Percentage. 



### Enumeration: StandardFeatureWeight
#### Standard label engine feature weights. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No weight. 
| Low| 1| Low weight. 
| Medium| 2| Medium weight. 
| High| 3| High weight. 




## CIMStandardGeneralPlacementProperties
#### Represents standard label engine general placement properties. 


### CIMGeneralPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| drawUnplacedLabels | boolean|Gets and sets a boolean option indicating whether or not to draw unplaced labels 
| invertedLabelTolerance | double|Gets and sets the inverted label tolerance which is the angle at which the label orientation is switched. 
| rotateLabelWithDisplay | boolean|Gets and sets a boolean option indicating whether or not rotate labels when the display rotates. 
| unplacedLabelColor | [Color](Types.md#color)|Gets and sets the unplaced label color. 


### CIMStandardGeneralPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|






## CIMStandardLabelPlacementProperties
#### Represents standard label engine label placement properties. 


### CIMLabelPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| featureType | [enumeration LabelFeatureType](CIMLabelPlacement.md#enumeration-labelfeaturetype)|Gets and sets the feature type being labeled. 


### CIMStandardLabelPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| featureWeight | [enumeration StandardFeatureWeight](CIMLabelPlacement.md#enumeration-standardfeatureweight)|Gets and sets the feature weight. 
| labelWeight | [enumeration StandardLabelWeight](CIMLabelPlacement.md#enumeration-standardlabelweight)|Gets and sets the label weight. 
| numLabelsOption | [enumeration StandardNumLabelsOption](CIMLabelPlacement.md#enumeration-standardnumlabelsoption)|Gets and sets the option for number of labels. 
| lineLabelPosition | [CIMStandardLineLabelPosition](CIMLabelPlacement.md#cimstandardlinelabelposition)|Gets and sets the line label position. 
| lineLabelPriorities | [CIMStandardLineLabelPriorities](CIMLabelPlacement.md#cimstandardlinelabelpriorities)|Gets and sets the line label priorities. 
| pointPlacementMethod | [enumeration StandardPointPlacementMethod](CIMLabelPlacement.md#enumeration-standardpointplacementmethod)|Gets and sets the point placement method. 
| pointPlacementPriorities | [CIMStandardPointPlacementPriorities](CIMLabelPlacement.md#cimstandardpointplacementpriorities)|Gets and sets the point placement priorities. 
| pointPlacementAngles | [double]|Gets and sets an array of point placement angles. 
| bufferRatio | double|Gets and sets the buffer ratio. 
| lineOffset | double|Gets and sets the line offset. 
| maxDistanceFromTarget | double|Gets and sets the max distance from target. 
| rotationType | [enumeration StandardLabelRotationType](CIMLabelPlacement.md#enumeration-standardlabelrotationtype)|Gets and sets the rotation type. 
| rotationField | string|Gets and sets the rotation field. 
| perpendicularToAngle | boolean|Gets and sets a boolean value indicating whether or not to place the label perpendicular to the angle. 
| polygonPlacementMethod | [enumeration StandardPolygonPlacementMethod](CIMLabelPlacement.md#enumeration-standardpolygonplacementmethod)|Gets and sets the polygon placement method. 
| placeOnlyInsidePolygon | boolean|Gets and sets a boolean value indicating whether or not to place the label only inside a polygon. 
| allowOverlappingLabels | boolean|Gets and sets a boolean value indicating whether or not to allow overlapping labels. 





### Enumeration: StandardLabelRotationType
#### Standard label engine label rotation types. 

|Property | Value | Description | 
|---------|--------|--------|
| Geographic| 0| Geographic rotation. 
| Arithmetic| 1| Arithmetic rotation. 
| Radians| 2| Rotation in radians. 
| AV3| 3| ArcView 3 rotation. 



### Enumeration: StandardLabelWeight
#### Standard label engine label weight. 

|Property | Value | Description | 
|---------|--------|--------|
| Low| 0| Low weight. 
| Medium| 1| Medium weight. 
| High| 2| High weight. 




## CIMStandardLineLabelPosition
#### Represents standard label engine line label position. 


### CIMStandardLineLabelPosition 

|Property | Type | Description | 
|---------|--------|--------|
| produceCurvedLabels | boolean|Gets and sets a boolean value indicating whether or not to produce curved labels. 
| above | boolean|Gets and sets a boolean value indicating whether or not to allow placement above lines. 
| below | boolean|Gets and sets a boolean value indicating whether or not to allow placement below lines. 
| onTop | boolean|Gets and sets a boolean value indicating whether or not to allow placement on top of lines. 
| left | boolean|Gets and sets a boolean value indicating whether or not to allow placement to the left of the line. 
| right | boolean|Gets and sets a boolean value indicating whether or not to allow placement to the right of the line. 
| inLine | boolean|Gets and sets a boolean value indicating whether or not to allow along lines at the best position. 
| atStart | boolean|Gets and sets a boolean value indicating whether or not to allow placement at the start of lines. 
| atEnd | boolean|Gets and sets a boolean value indicating whether or not to allow placement at the end of lines. 
| parallel | boolean|Gets and sets a boolean value indicating whether or not to allow placement parallel to lines. 
| perpendicular | boolean|Gets and sets a boolean value indicating whether or not to allow placement perpendicular to lines. 
| horizontal | boolean|Gets and sets a boolean value indicating whether or not to allow placement horizontally. 
| offset | double|Gets and sets a the offset from the line. 






## CIMStandardLineLabelPriorities
#### Represents standard label engine line label priorities. 


### CIMStandardLineLabelPriorities 

|Property | Type | Description | 
|---------|--------|--------|
| aboveBefore | long|Gets and sets a the label position priority for above and before the line. 
| aboveStart | long|Gets and sets a the label position priority for above and at the start of the line. 
| aboveAlong | long|Gets and sets a the label position priority for above and along the line. 
| aboveEnd | long|Gets and sets a the label position priority for above and at the end of the line. 
| aboveAfter | long|Gets and sets a the label position priority for above and after the line. 
| centerBefore | long|Gets and sets a the label position priority for centered and before the line. 
| centerStart | long|Gets and sets a the label position priority for centered and at the start of the line. 
| centerAlong | long|Gets and sets a the label position priority for centered and along the line. 
| centerEnd | long|Gets and sets a the label position priority for centered and at the end of the line. 
| centerAfter | long|Gets and sets a the label position priority for centered and after the line. 
| belowBefore | long|Gets and sets a the label position priority for below and before the line. 
| belowStart | long|Gets and sets a the label position priority for below and at the start of the line. 
| belowAlong | long|Gets and sets a the label position priority for below and along the line. 
| belowEnd | long|Gets and sets a the label position priority for below and at the end of the line. 
| belowAfter | long|Gets and sets a the label position priority for below and after the line. 





### Enumeration: StandardNumLabelsOption
#### Standard label engine number of labels options. 

|Property | Value | Description | 
|---------|--------|--------|
| NoLabelRestrictions| 0| No restrictions. 
| OneLabelPerName| 1| One label per name. 
| OneLabelPerShape| 2| One label per feature. 
| OneLabelPerPart| 3| One label per feature part. 



### Enumeration: StandardPointPlacementMethod
#### Standard label engine point placement methods. 

|Property | Value | Description | 
|---------|--------|--------|
| AroundPoint| 0| Placement around the point. 
| OnTopPoint| 1| Placement on top of the point. 
| SpecifiedAngles| 2| Placement at specified angles. 
| RotationField| 3| Placement by rotation field. 




## CIMStandardPointPlacementPriorities
#### Represents standard label engine point placement priorities. 


### CIMStandardPointPlacementPriorities 

|Property | Type | Description | 
|---------|--------|--------|
| aboveLeft | long|Gets and sets a the label position priority for the above left position. 
| aboveCenter | long|Gets and sets a the label position priority for the above center position. 
| aboveRight | long|Gets and sets a the label position priority for the above right position. 
| centerLeft | long|Gets and sets a the label position priority for the center left position. 
| centerRight | long|Gets and sets a the label position priority for the center right position. 
| belowLeft | long|Gets and sets a the label position priority for the below left position. 
| belowCenter | long|Gets and sets a the label position priority for the below center position. 
| belowRight | long|Gets and sets a the label position priority for the below right position. 





### Enumeration: StandardPolygonPlacementMethod
#### Standard label engine polygon placement methods. 

|Property | Value | Description | 
|---------|--------|--------|
| AlwaysHorizontal| 0| Always horizontal. 
| AlwaysStraight| 1| Always straight. 
| MixedStrategy| 2| Mixed strategy, prefer horizontal before placing straight. 

