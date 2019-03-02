

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
| expression | string | The label expression. 
| expressionEngine | [enumeration LabelExpressionEngine](CIMLabelPlacement.md#enumeration-labelexpressionengine) | The label expression engine (the language the expression is written in). 
| featuresToLabel | [enumeration FeaturesToLabel](CIMLabelPlacement.md#enumeration-featurestolabel) | A parameter indicating which features to label. 
| maplexLabelPlacementProperties | [CIMMaplexLabelPlacementProperties](CIMLabelPlacement.md#cimmaplexlabelplacementproperties) | The Maplex placement properties which are used when the map uses the Maplex label engine. 
| maximumScale | double | The maximum scale for labeling (set as the denominator of the scale's representative fraction). 
| minimumScale | double | The minimum scale for labeling (set as the denominator of the scale's representative fraction). 
| name | string | The name of the label class. 
| priority | long | The priority of the label class. 
| standardLabelPlacementProperties | [CIMStandardLabelPlacementProperties](CIMLabelPlacement.md#cimstandardlabelplacementproperties) | The standard placement properties which are used when the map uses the standard label engine. 
| textSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol of the label class. 
| useCodedValue | boolean | A value indicating whether or not to use coded value domain descriptions when labeling. 
| whereClause | string | The SQL where clause of which features to label with this label class. 
| visibility | boolean | A value indicating whether this label class is visible. 
| ID | long | The ID of the label class. This property is only used in the context of annotation. 






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
| GeometricCenter| 0| Geometric center (of the potentially clipped geometry). 
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
| name | string | The Maplex dictionary name. 
| maplexDictionary | [CIMMaplexDictionaryEntry](CIMLabelPlacement.md#cimmaplexdictionaryentry) | The Maplex dictionary entries. 






## CIMMaplexDictionaryEntry
#### Represents a Maplex dictionary entry. 


### CIMMaplexDictionaryEntry 

|Property | Type | Description | 
|---------|--------|--------|
| abbreviation | string | The abbreviation. 
| text | string | The text to abbreviate. 
| maplexAbbreviationType | [enumeration MaplexAbbreviationType](CIMLabelPlacement.md#enumeration-maplexabbreviationtype) | The abbreviation type. 






## CIMMaplexExternalZonePriorities
#### Represents Maplex external zone priorities. 


### CIMMaplexExternalZonePriorities 

|Property | Type | Description | 
|---------|--------|--------|
| aboveLeft | long | Priority for this position. 
| aboveCenter | long | Priority for this position. 
| aboveRight | long | Priority for this position. 
| centerRight | long | Priority for this position. 
| belowRight | long | Priority for this position. 
| belowCenter | long | Priority for this position. 
| belowLeft | long | Priority for this position. 
| centerLeft | long | Priority for this position. 






## CIMMaplexGeneralPlacementProperties
#### Represents Maplex general placement properties. 


### CIMGeneralPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| drawUnplacedLabels | boolean | A value indicating whether or not to draw unplaced labels. 
| invertedLabelTolerance | double | The inverted label tolerance which is the angle at which the label orientation is switched. 
| rotateLabelWithDisplay | boolean | A value indicating whether or not rotate labels when the display rotates. 
| unplacedLabelColor | [Color](Types.md#color) | The unplaced label color. 


### CIMMaplexGeneralPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| allowBorderOverlap | boolean | A value indicating whether or not to allow border overlap. 
| dictionaries | [CIMMaplexDictionary](CIMLabelPlacement.md#cimmaplexdictionary) | The Maplex dictionaries. 
| keyNumberGroups | [CIMMaplexKeyNumberGroup](CIMLabelPlacement.md#cimmaplexkeynumbergroup) | The key number groups. 
| placementQuality | [enumeration MaplexQualityType](CIMLabelPlacement.md#enumeration-maplexqualitytype) | The placement quality. 





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
| aboveLeft | long | Priority for this position. 
| aboveCenter | long | Priority for this position. 
| aboveRight | long | Priority for this position. 
| centerRight | long | Priority for this position. 
| belowRight | long | Priority for this position. 
| belowCenter | long | Priority for this position. 
| belowLeft | long | Priority for this position. 
| centerLeft | long | Priority for this position. 
| center | long | Priority for this position. 






## CIMMaplexKeyNumberGroup
#### Represents a Maplex key number group. 


### CIMMaplexKeyNumberGroup 

|Property | Type | Description | 
|---------|--------|--------|
| delimiterCharacter | string | The delimiter character of the key number. 
| horizontalAlignment | [enumeration MaplexKeyNumberHorizontalAlignment](CIMLabelPlacement.md#enumeration-maplexkeynumberhorizontalalignment) | The horizontal alignment. 
| maximumNumberOfLines | long | The maximum number of lines. 
| minimumNumberOfLines | long | The minimum number of lines. 
| name | string | The name of the group. 
| numberResetType | [enumeration MaplexKeyNumberResetType](CIMLabelPlacement.md#enumeration-maplexkeynumberresettype) | The number reset type. 





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
| featureType | [enumeration LabelFeatureType](CIMLabelPlacement.md#enumeration-labelfeaturetype) | The feature type being labeled. 


### CIMMaplexLabelPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| alignLabelToLineDirection | boolean | A value indicating whether to align the label with the label direction so the label may appear upside down. 
| allowAsymmetricOverrun | boolean | A value indicating whether a label may overrun one side of a polygon feature. 
| allowStraddleStacking | boolean | A value indicating whether a stacked label may straddle the line feature. 
| alternateLabelExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The ExpressionInfo for the alternate label expression. 
| avoidPolygonHoles | boolean | A value indicating whether labels should avoid holes in polygons. 
| backgroundLabel | boolean | A value indicating whether to place the label first and allow other labels to be placed over it. 
| boundaryLabelingAllowHoles | boolean | A value indicating whether to allow holes in boundary labeling. 
| boundaryLabelingAllowSingleSided | boolean | A value indicating whether to allow single sided boundary labeling. 
| boundaryLabelingSingleSidedOnLine | boolean | A value indicating whether single sided boundary label is centered on line. 
| canAbbreviateLabel | boolean | A value indicating whether to abbreviate the label using an abbreviation dictionary. 
| canFlipStackedStreetLabel | boolean | A value indicating whether a stacked label may be flipped over to obtain a better position. 
| canKeyNumberLabel | boolean | A value indicating whether to key number the label and feature. 
| canOverrunFeature | boolean | A value indicating whether to place the label over end of line or over polygon boundary. 
| canPlaceLabelOnTopOfFeature | boolean | A value indicating whether the label can be placed on top of the street feature. 
| canPlaceLabelOutsidePolygon | boolean | A value indicating whether to place a label outside the polygon if it does not fit inside. 
| canReduceFontSize | boolean | A value indicating whether to reduce the size of the font. 
| canReduceLeading | boolean | A value indicating whether the leading can be reduced for a stacked label. 
| canRemoveOverlappingLabel | boolean | A value indicating whether to remove the label if it overlaps with other labels. 
| canShiftPointLabel | boolean | A value indicating whether to allow the point label to be shifted upon a fixed position. 
| canStackLabel | boolean | A value indicating whether to stack the label to obtain a better position. 
| canTruncateLabel | boolean | A value indicating whether to truncate the label using an algorithm. 
| canUseAlternateLabelExpression | boolean | A value indicating whether an alternate label expression is allowed to be used. 
| connectionType | [enumeration MaplexConnectionType](CIMLabelPlacement.md#enumeration-maplexconnectiontype) | The options for connecting line features. 
| constrainOffset | [enumeration MaplexConstrainOffset](CIMLabelPlacement.md#enumeration-maplexconstrainoffset) | The label constraint options. 
| contourAlignmentType | [enumeration MaplexContourAlignmentType](CIMLabelPlacement.md#enumeration-maplexcontouralignmenttype) | The options for the contour label alignment. 
| contourLadderType | [enumeration MaplexContourLadderType](CIMLabelPlacement.md#enumeration-maplexcontourladdertype) | The options for the contour label ladder types. 
| contourMaximumAngle | long | The maximum angle at which a contour label may be placed. 
| dictionaryName | string | The name of the abbreviations dictionary referenced by this layer. 
| enableConnection | boolean | A value indicating whether to turn off line connection. 
| enablePointPlacementPriorities | boolean | A value indicating whether to use user-defined point placement priorities. 
| enablePolygonFixedPosition | boolean | A value indicating whether a label is to be placed at a fixed position in the polygon. 
| enableSecondaryOffset | boolean | A value indicating whether to place a label at a secondary offset from the line feature. 
| featureWeight | long | The feature weight which controls which features may be overlapped and to what extent. 
| fontHeightReductionLimit | double | Font height reduction limit. The font may be reduced in height until this limit is reached. 
| fontHeightReductionStep | double | Font height reduction step. This is the step interval for font height reduction. 
| fontWidthReductionLimit | double | Font width reduction limit. The font may be reduced in width until this limit is reached. 
| fontWidthReductionStep | double | Font width reduction step. This is the step interval for font width reduction. 
| graticuleAlignment | boolean | A value indicating whether to enable graticule alignment. 
| graticuleAlignmentType | [enumeration MaplexGraticuleAlignmentType](CIMLabelPlacement.md#enumeration-maplexgraticulealignmenttype) | The options for the graticule alignment type. 
| isLabelBufferHardConstraint | boolean | A value indicating whether the label buffer is a hard constraint and must be honored. 
| isMinimumSizeBasedOnArea | boolean | A value indicating whether the minimum feature size for labeling is based on area. 
| isOffsetFromFeatureGeometry | boolean | A value indicating whether to measure the label offset from the feature geometry. 
| keyNumberGroupName | string | The name of the key number group to use for key numbering the labels. 
| labelBuffer | long | The label buffer. Increase buffer to stop labels from being placed too close to each other. 
| labelLargestPolygon | boolean | A value indicating whether to label only the largest polygon in a compound polygon feature. 
| labelPriority | long | The label priority. Label priority controls approximate placement order. 
| labelStackingProperties | [CIMMaplexLabelStackingProperties](CIMLabelPlacement.md#cimmaplexlabelstackingproperties) | The label stacking properties for a layer. 
| lineFeatureType | [enumeration MaplexLineFeatureType](CIMLabelPlacement.md#enumeration-maplexlinefeaturetype) | The line feature type. 
| linePlacementMethod | [enumeration MaplexLinePlacementMethod](CIMLabelPlacement.md#enumeration-maplexlineplacementmethod) | The line placement method. 
| maximumCharacterSpacing | double | The maximum character spacing. Character spacing may be increased up to this limit. 
| maximumLabelOverrun | double | The maximum distance that a label is allowed to overrun the end of its feature. 
| maximumLabelOverrunUnit | [enumeration MaplexUnit](CIMLabelPlacement.md#enumeration-maplexunit) | The label overrun unit. 
| maximumWordSpacing | double | Maximum word spacing. The word spacing may be increased up to this limit. 
| minimumEndOfStreetClearance | double | Minimum clearance between street label and street end. 
| minimumFeatureSizeUnit | [enumeration MaplexUnit](CIMLabelPlacement.md#enumeration-maplexunit) | Minimum feature size unit. 
| minimumRepetitionInterval | double | The interval that must elapse before label is repeated. 
| minimumSizeForLabeling | double | The minimum size of a line or area feature for it to be labeled. 
| multiPartOption | [enumeration MaplexMultiPartOption](CIMLabelPlacement.md#enumeration-maplexmultipartoption) | The option for labeling multi-part shapes. 
| neverRemoveLabel | boolean | A value indicating whether to not remove the label if no position is found. 
| offsetAlongLineProperties | [CIMMaplexOffsetAlongLineProperties](CIMLabelPlacement.md#cimmaplexoffsetalonglineproperties) | The offset along line properties for a layer. 
| pointExternalZonePriorities | [CIMMaplexExternalZonePriorities](CIMLabelPlacement.md#cimmaplexexternalzonepriorities) | The properties which control placement of a label around point feature. 
| pointPlacementMethod | [enumeration MaplexPointPlacementMethod](CIMLabelPlacement.md#enumeration-maplexpointplacementmethod) | The point placement method. 
| polygonAnchorPointType | [enumeration MaplexAnchorPointType](CIMLabelPlacement.md#enumeration-maplexanchorpointtype) | The polygon anchor point type. 
| polygonBoundaryWeight | long | The feature weight for the boundary of the polygon. 
| polygonExternalZones | [CIMMaplexExternalZonePriorities](CIMLabelPlacement.md#cimmaplexexternalzonepriorities) | The placement priorities associated with zones external to the polygon. 
| polygonFeatureType | [enumeration MaplexPolygonFeatureType](CIMLabelPlacement.md#enumeration-maplexpolygonfeaturetype) | The polygon feature type. 
| polygonInternalZones | [CIMMaplexInternalZonePriorities](CIMLabelPlacement.md#cimmaplexinternalzonepriorities) | The placement priorities associated with zones internal to the polygon. 
| polygonPlacementMethod | [enumeration MaplexPolygonPlacementMethod](CIMLabelPlacement.md#enumeration-maplexpolygonplacementmethod) | The polygon placement method. 
| preferHorizontalPlacement | boolean | A value indicating whether there is a preference to place the label horizontally. 
| preferLabelNearJunction | boolean | A value indicating whether there is a preference for placing a line label near a junction. 
| preferLabelNearJunctionClearance | double | The preferred clearance for placing a line label near a junction. 
| preferLabelNearMapBorder | boolean | A value indicating whether there is a preference for placing a line label near the map border. 
| preferLabelNearMapBorderClearance | double | The preferred clearance for placing a line label near the map border. 
| preferredEndOfStreetClearance | double | The preferred clearance between street label and street end. 
| primaryOffset | double | The primary offset between label and symbol. 
| primaryOffsetUnit | [enumeration MaplexUnit](CIMLabelPlacement.md#enumeration-maplexunit) | The unit of the primary offset. 
| removeExtraLineBreaks | boolean | A value indicating whether extra line breaks are removed from the label text. 
| removeExtraWhiteSpace | boolean | A value indicating whether extra white space characters are removed from the label text. 
| repeatLabel | boolean | A value indicating whether to enable the repetition of label along line feature. 
| repetitionIntervalUnit | [enumeration MaplexUnit](CIMLabelPlacement.md#enumeration-maplexunit) | The label repetition interval unit. 
| rotationProperties | [CIMMaplexRotationProperties](CIMLabelPlacement.md#cimmaplexrotationproperties) | The label rotation properties. 
| secondaryOffset | double | The secondary offset between label and symbol. 
| secondaryOffsetMaximum | double | The secondary offset maximum. 
| secondaryOffsetMinimum | double | The secondary offset minimum. 
| spreadCharacters | boolean | A value indicating whether to spread label characters along line features. 
| spreadWords | boolean | A value indicating whether to whether to spread words along line features. 
| strategyPriorities | [CIMMaplexStrategyPriorities](CIMLabelPlacement.md#cimmaplexstrategypriorities) | The priority of a placement strategy when placing text. 
| thinDuplicateLabels | boolean | A value indicating whether to remove duplicate labels that lie within a specified distance of each other. 
| thinningDistance | double | The distance used to control the thinning of duplicate labels. 
| thinningDistanceUnit | [enumeration MaplexUnit](CIMLabelPlacement.md#enumeration-maplexunit) | The thinning distance unit. 
| truncationMarkerCharacter | string | The marker character used by the truncation strategy. 
| truncationMinimumLength | long | The minimum length of a label used by the truncation strategy. 
| truncationPreferredCharacters | string | The preferred characters used by the truncation strategy. These characters will be removed as needed. 
| useExactSymbolOutline | boolean | A value indicating whether to use the exact polygon outline of a symbol when measuring the label offset. 





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
| stackAlignment | [enumeration MaplexStackingAlignment](CIMLabelPlacement.md#enumeration-maplexstackingalignment) | The stacking alignment. 
| maximumNumberOfLines | long | The maximum number of lines. 
| minimumNumberOfCharsPerLine | long | The minimum number of characters per line. 
| maximumNumberOfCharsPerLine | long | The maximum number of characters per line. 
| separators | [CIMMaplexStackingSeparator](CIMLabelPlacement.md#cimmaplexstackingseparator) | The stacking separators. 





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
#### Maplex multipart options. 

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
| placementMethod | [enumeration MaplexOffsetAlongLineMethod](CIMLabelPlacement.md#enumeration-maplexoffsetalonglinemethod) | The placement method. 
| labelAnchorPoint | [enumeration MaplexLabelAnchorPoint](CIMLabelPlacement.md#enumeration-maplexlabelanchorpoint) | The label anchor point for positioning along the line. 
| distance | double | The distance along the line. 
| tolerance | double | The tolerance. 
| distanceUnit | [enumeration MaplexUnit](CIMLabelPlacement.md#enumeration-maplexunit) | The distance unit. 
| useLineDirection | boolean | A value indicating whether or not to use the line direction. 





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
| enable | boolean | A value indicating whether to enable rotation. 
| rotationType | [enumeration MaplexLabelRotationType](CIMLabelPlacement.md#enumeration-maplexlabelrotationtype) | The rotation type. 
| rotationField | string | The rotation field to get values from. 
| perpendicularToAngle | boolean | A value indicating whether to place the label perpendicular to the angle. 
| alignLabelToAngle | boolean | A value indicating whether or not to align the label to the angle. 
| alignmentType | [enumeration MaplexRotationAlignmentType](CIMLabelPlacement.md#enumeration-maplexrotationalignmenttype) | The alignment type. 
| additionalAngle | long | Additional angle to add to the data value. 
| rotationExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | ExpressionInfo that contains the Arcade expression that returns rotation as a number. When both RotationField and RotationExpressionInfo are present RotationExpressionInfo is used. 





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
| separator | string | The separator as a string of one character. 
| visible | boolean | A value indicating whether or not the separator should be visible after stacking. 
| splitForced | boolean | A value indicating whether or not to force a split at every instance of the separator. 
| splitAfter | boolean | A value indicating whether or not to split after the separator. 






## CIMMaplexStrategyPriorities
#### Represents Maplex strategy priorities. 


### CIMMaplexStrategyPriorities 

|Property | Type | Description | 
|---------|--------|--------|
| stacking | long | The priority for stacking. 
| overrun | long | The priority for overrun. 
| fontCompression | long | The priority for font compression. 
| fontReduction | long | The priority for font reduction. 
| abbreviation | long | The priority for abbreviation. 





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
| drawUnplacedLabels | boolean | A value indicating whether or not to draw unplaced labels. 
| invertedLabelTolerance | double | The inverted label tolerance which is the angle at which the label orientation is switched. 
| rotateLabelWithDisplay | boolean | A value indicating whether or not rotate labels when the display rotates. 
| unplacedLabelColor | [Color](Types.md#color) | The unplaced label color. 


### CIMStandardGeneralPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|






## CIMStandardLabelPlacementProperties
#### Represents standard label engine label placement properties. 


### CIMLabelPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| featureType | [enumeration LabelFeatureType](CIMLabelPlacement.md#enumeration-labelfeaturetype) | The feature type being labeled. 


### CIMStandardLabelPlacementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| featureWeight | [enumeration StandardFeatureWeight](CIMLabelPlacement.md#enumeration-standardfeatureweight) | The feature weight. 
| labelWeight | [enumeration StandardLabelWeight](CIMLabelPlacement.md#enumeration-standardlabelweight) | The label weight. 
| numLabelsOption | [enumeration StandardNumLabelsOption](CIMLabelPlacement.md#enumeration-standardnumlabelsoption) | The option for number of labels. 
| lineLabelPosition | [CIMStandardLineLabelPosition](CIMLabelPlacement.md#cimstandardlinelabelposition) | The line label position. 
| lineLabelPriorities | [CIMStandardLineLabelPriorities](CIMLabelPlacement.md#cimstandardlinelabelpriorities) | The line label priorities. 
| pointPlacementMethod | [enumeration StandardPointPlacementMethod](CIMLabelPlacement.md#enumeration-standardpointplacementmethod) | The point placement method. 
| pointPlacementPriorities | [CIMStandardPointPlacementPriorities](CIMLabelPlacement.md#cimstandardpointplacementpriorities) | The point placement priorities. 
| pointPlacementAngles | [double] | An array of point placement angles. 
| bufferRatio | double | The buffer ratio. 
| lineOffset | double | The line offset. 
| maxDistanceFromTarget | double | The maximum distance from target. 
| rotationType | [enumeration StandardLabelRotationType](CIMLabelPlacement.md#enumeration-standardlabelrotationtype) | The rotation type. 
| rotationField | string | The rotation field. 
| perpendicularToAngle | boolean | A value indicating whether or not to place the label perpendicular to the angle. 
| polygonPlacementMethod | [enumeration StandardPolygonPlacementMethod](CIMLabelPlacement.md#enumeration-standardpolygonplacementmethod) | The polygon placement method. 
| placeOnlyInsidePolygon | boolean | A value indicating whether or not to place the label only inside a polygon. 
| allowOverlappingLabels | boolean | A value indicating whether or not to allow overlapping labels. 





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
| produceCurvedLabels | boolean | A value indicating whether or not to produce curved labels. 
| above | boolean | A value indicating whether or not to allow placement above lines. 
| below | boolean | A value indicating whether or not to allow placement below lines. 
| onTop | boolean | A value indicating whether or not to allow placement on top of lines. 
| left | boolean | A value indicating whether or not to allow placement to the left of the line. 
| right | boolean | A value indicating whether or not to allow placement to the right of the line. 
| inLine | boolean | A value indicating whether or not to allow along lines at the best position. 
| atStart | boolean | A value indicating whether or not to allow placement at the start of lines. 
| atEnd | boolean | A value indicating whether or not to allow placement at the end of lines. 
| parallel | boolean | A value indicating whether or not to allow placement parallel to lines. 
| perpendicular | boolean | A value indicating whether or not to allow placement perpendicular to lines. 
| horizontal | boolean | A value indicating whether or not to allow placement horizontally. 
| offset | double | A the offset from the line. 






## CIMStandardLineLabelPriorities
#### Represents standard label engine line label priorities. 


### CIMStandardLineLabelPriorities 

|Property | Type | Description | 
|---------|--------|--------|
| aboveBefore | long | A the label position priority for above and before the line. 
| aboveStart | long | A the label position priority for above and at the start of the line. 
| aboveAlong | long | A the label position priority for above and along the line. 
| aboveEnd | long | A the label position priority for above and at the end of the line. 
| aboveAfter | long | A the label position priority for above and after the line. 
| centerBefore | long | A the label position priority for centered and before the line. 
| centerStart | long | A the label position priority for centered and at the start of the line. 
| centerAlong | long | A the label position priority for centered and along the line. 
| centerEnd | long | A the label position priority for centered and at the end of the line. 
| centerAfter | long | A the label position priority for centered and after the line. 
| belowBefore | long | A the label position priority for below and before the line. 
| belowStart | long | A the label position priority for below and at the start of the line. 
| belowAlong | long | A the label position priority for below and along the line. 
| belowEnd | long | A the label position priority for below and at the end of the line. 
| belowAfter | long | A the label position priority for below and after the line. 





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
| aboveLeft | long | A the label position priority for the above left position. 
| aboveCenter | long | A the label position priority for the above center position. 
| aboveRight | long | A the label position priority for the above right position. 
| centerLeft | long | A the label position priority for the center left position. 
| centerRight | long | A the label position priority for the center right position. 
| belowLeft | long | A the label position priority for the below left position. 
| belowCenter | long | A the label position priority for the below center position. 
| belowRight | long | A the label position priority for the below right position. 





### Enumeration: StandardPolygonPlacementMethod
#### Standard label engine polygon placement methods. 

|Property | Value | Description | 
|---------|--------|--------|
| AlwaysHorizontal| 0| Always horizontal. 
| AlwaysStraight| 1| Always straight. 
| MixedStrategy| 2| Mixed strategy, prefer horizontal before placing straight. 

