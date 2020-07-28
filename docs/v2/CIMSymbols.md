


## CIM3DSymbolProperties
#### Represents 3D symbol properties, a collection of symbol properties that apply when the symbol is used in a 3D context. 


### CIM3DSymbolProperties 

|Property | Type | Description | 
|---------|--------|--------|
| dominantSizeAxis3D | [enumeration DominantSizeAxis](CIMEnumerations.md#enumeration-dominantsizeaxis) | The dominant size axis. 
| rotationOrder3D | [enumeration RotationOrder](CIMEnumerations.md#enumeration-rotationorder) | The rotation order 3D. 
| scaleZ | double | The scale Z. 
| scaleY | double | The scale Y. 





### Enumeration: AngleAlignment
#### Angle alignment types. 

|Property | Value | Description | 
|---------|--------|--------|
| Display| 0| Points remain aligned to the display when the map is rotated. 
| Map| 1| Points are rotated with the map. 




## CIMBackgroundCallout
#### Represents a background callout which draws a callout with an optional polygon background and leader line. 


### CIMCallout 

|Property | Type | Description | 
|---------|--------|--------|
| leaderTolerance | double | The leader tolerance which is the closest distance (in points) to the text the anchor point can be for the callout to draw. 
| leaderOffset | double | The leader offset which is an offset value defining the distance (in points) between the anchor point and the beginning of the drawn leader. 


### CIMLineCallout 

|Property | Type | Description | 
|---------|--------|--------|
| leaderLineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol) | The line symbol to draw leaders with. 
| gap | double | The gap (in points) between the point symbol and the beginning of the leader line. 
| lineStyle | [enumeration LeaderLineStyle](CIMSymbols.md#enumeration-leaderlinestyle) | The style of line to generate when a Point leader is drawn defined by an enumeration value. Line leaders will always be drawn with their own geometry. 


### CIMBackgroundCallout 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundSymbol | [CIMPolygonSymbol](CIMSymbols.md#cimpolygonsymbol) | The symbol used to draw the background. If null, the background doesn't draw. 
| accentBarSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol) | The symbol used to draw the accent bar. If null, the accent bar doesn't draw. 
| margin | [CIMTextMargin](CIMSymbols.md#cimtextmargin) | The text margin defining the space around the text that is accounted for in background creation. 






## CIMBalloonCallout
#### Represents a balloon callout. Balloon callouts are a filled background that is placed behind text. They may or may not have a leader line connecting the callout to an anchor point. 


### CIMCallout 

|Property | Type | Description | 
|---------|--------|--------|
| leaderTolerance | double | The leader tolerance which is the closest distance (in points) to the text the anchor point can be for the callout to draw. 
| leaderOffset | double | The leader offset which is an offset value defining the distance (in points) between the anchor point and the beginning of the drawn leader. 


### CIMBalloonCallout 

|Property | Type | Description | 
|---------|--------|--------|
| balloonStyle | [enumeration BalloonCalloutStyle](CIMSymbols.md#enumeration-ballooncalloutstyle) | The balloon style. 
| backgroundSymbol | [CIMPolygonSymbol](CIMSymbols.md#cimpolygonsymbol) | The symbol used to draw the background. 
| margin | [CIMTextMargin](CIMSymbols.md#cimtextmargin) | The text margin defining the space around the text that is accounted for in balloon creation. 
| useFixedDartWidth | boolean | A value indicating whether to use a fixed size when drawing the dart symbol. 
| fixedDartWidth | double | The dart width. 
| useDartSymbol | boolean | A value indicating whether the dart symbol is drawn differently to the background symbol. 
| dartSymbol | [CIMPolygonSymbol](CIMSymbols.md#cimpolygonsymbol) | A symbol used to draw the dart. 





### Enumeration: BalloonCalloutStyle
#### Balloon callout styles. 

|Property | Value | Description | 
|---------|--------|--------|
| Rectangle| 0| Rectangle style. 
| RoundedRectangle| 1| Rounded rectangle style. 
| Oval| 2| Oval style. 




## CIMBarChartMarker
#### Represents a bar chart marker, a chart made of vertical bars displaying values. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMMarker 

|Property | Type | Description | 
|---------|--------|--------|
| anchorPoint | [Point](ExternalReferences.md#point) | The specified location where all transformation property operations originate. 
| anchorPointUnits | [enumeration SymbolUnits](CIMSymbols.md#enumeration-symbolunits) | A value which specifies if the anchor point location is considered a percentage of the size or as an absolute distance. 
| angleX | double | The angle the marker is rotated around the X axis. This type of rotation is also referred to as tilt and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Tilt. 
| angleY | double | The angle the marker is rotated around the Y axis. This type of rotation is also referred to as roll and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Roll. 
| dominantSizeAxis3D | [enumeration DominantSizeAxis](CIMEnumerations.md#enumeration-dominantsizeaxis) | Which axis is considered as the Size in 3D. Only applicable when the marker layer is a 3DShapeMarker. 
| offsetX | double | The value the marker is moved along the X axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetY | double | The value the marker is moved along the Y axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetZ | double | The value the marker is moved along the Z axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| rotateClockwise | boolean | A value indicating whether the rotation is applied clockwise or counterclockwise to the marker layer. 
| rotation | double | The angle that the marker is rotated around the anchor point, in degrees. 
| size | double | The height of the marker. Modifying Size changes the marker's height to the specified size and the width is updated proportionally. 
| billboardMode3D | [enumeration BillboardMode](CIMEnumerations.md#enumeration-billboardmode) | The billboard mode of the marker. 
| markerPlacement | [MarkerPlacement](Types.md#markerplacement) | Marker placements which determine how markers are placed along a line or within a polygon. 


### CIMChartMarker 

|Property | Type | Description | 
|---------|--------|--------|
| display3D | boolean | A value indicating whether to draw the chart with a 3D perspective. 
| parts | [[CIMChartPart]](CIMSymbols.md#cimchartpart) | The individual components of the chart marker. 
| thickness3D | double | The thickness or depth of a chart. Only applied when Display3D is true. 
| tilt3D | double | The tilt (rotation around the X axis) of the chart. Only applied when Display3D is true. 


### CIMBarChartMarker 

|Property | Type | Description | 
|---------|--------|--------|
| axesSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol) | The axes symbol. 
| spacing | double | The spacing. 
| verticalBars | boolean | A value indicating whether this bar chart marker has vertical bars. 
| width | double | The width. 
| showAxes | boolean | A value indicating whether or not to show the axes symbol. 





### Enumeration: BlendingMode
#### Blending modes. Determines how the strokes with dash patterns and other patterns (tiled pictures, placement effects) are handled at the end points of the line geometry's segments. If more than one pattern exists (for example, a dashed simple stroke, a hash stroke, and a marker stroke) then the longest pattern's length is affected directly by this option and the rest of the stroke patterns are resized proportionately to match. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No blending. 
| Alpha| 1| Alpha blending. 
| Screen| 2| Screen. 
| Multiply| 3| Multiply. 
| Add| 4| Add. 



### Enumeration: BlockProgression
#### Block progressions. 

|Property | Value | Description | 
|---------|--------|--------|
| TTB| 0| Top To Bottom. 
| RTL| 1| Right To Left (vertical text). 
| BTT| 2| Bottom To Top. 




## CIMCGAAttribute
#### Represents a CGA attribute, the symbol attribute as specified by the CGA code in the rule package. 


### CIMCGAAttribute 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| CGAAttributeType | [enumeration CGAAttributeType](CIMSymbols.md#enumeration-cgaattributetype) | The CGA attribute type. 
| value | any | The value. 





### Enumeration: CGAAttributeType
#### CGA attribute type. 

|Property | Value | Description | 
|---------|--------|--------|
| Float| 0| Float - Attribute is a numeric attribute that is a float value 
| String| 1| String - Attribute is a string 
| Boolean| 2| Boolean - Attribute is a boolean 




## CIMCharacterMarker
#### Represents a character marker. The shape of a marker is defined by a glyph in a font. The marker is drawn using the specified size and color. Each marker has a defined frame around the glyph that is considered when the size is applied. As a result, character markers of the same size may appear different sizes if the glyphs frames are different sizes. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMMarker 

|Property | Type | Description | 
|---------|--------|--------|
| anchorPoint | [Point](ExternalReferences.md#point) | The specified location where all transformation property operations originate. 
| anchorPointUnits | [enumeration SymbolUnits](CIMSymbols.md#enumeration-symbolunits) | A value which specifies if the anchor point location is considered a percentage of the size or as an absolute distance. 
| angleX | double | The angle the marker is rotated around the X axis. This type of rotation is also referred to as tilt and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Tilt. 
| angleY | double | The angle the marker is rotated around the Y axis. This type of rotation is also referred to as roll and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Roll. 
| dominantSizeAxis3D | [enumeration DominantSizeAxis](CIMEnumerations.md#enumeration-dominantsizeaxis) | Which axis is considered as the Size in 3D. Only applicable when the marker layer is a 3DShapeMarker. 
| offsetX | double | The value the marker is moved along the X axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetY | double | The value the marker is moved along the Y axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetZ | double | The value the marker is moved along the Z axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| rotateClockwise | boolean | A value indicating whether the rotation is applied clockwise or counterclockwise to the marker layer. 
| rotation | double | The angle that the marker is rotated around the anchor point, in degrees. 
| size | double | The height of the marker. Modifying Size changes the marker's height to the specified size and the width is updated proportionally. 
| billboardMode3D | [enumeration BillboardMode](CIMEnumerations.md#enumeration-billboardmode) | The billboard mode of the marker. 
| markerPlacement | [MarkerPlacement](Types.md#markerplacement) | Marker placements which determine how markers are placed along a line or within a polygon. 


### CIMCharacterMarker 

|Property | Type | Description | 
|---------|--------|--------|
| characterIndex | long | The Unicode decimal value for the individual glyph of the font that defines the shape of the marker. 
| depth3D | double | The depth of the marker when drawn in 3D. 
| fontFamilyName | string | The font family name of the font. e.g. Comic Sans. 
| fontStyleName | string | The style name for the font family. e.g. Regular, Bold, or Italic. 
| fontType | [enumeration FontType](CIMSymbols.md#enumeration-fonttype) | The font type. 
| scaleX | double | The width of the symbol without changing the height (or depth in 3D), as a ratio. 
| symbol | [CIMPolygonSymbol](CIMSymbols.md#cimpolygonsymbol) | The polygon symbol that is used to renderer the marker. 
| verticalOrientation3D | boolean | A value indicating whether the marker stands a marker upright as though locked in place. The marker can be viewed from all angles. 
| scaleSymbolsProportionally | boolean | A value indicating whether the strokes and/or fills of a marker are scaled proportionally when the symbol size is changed. When enabled, the strokes for the outline or fill of the polygon symbol used to draw the marker will be scaled proportionally with changes to the symbol size. If this property is not enabled, the stroke will draw with the specified width regardless of the marker size. 
| respectFrame | boolean | A value indicating whether the frame of the character marker should be honored when transforming the marker. 






## CIMChartPart
#### Represents a chart part, individual components of the chart marker. 


### CIMChartPart 

|Property | Type | Description | 
|---------|--------|--------|
| value | double | The value of the chart part used to size the part. 
| polygonSymbol | [CIMPolygonSymbol](CIMSymbols.md#cimpolygonsymbol) | The polygon symbol used to draw the chart part. 






## CIMClippingPath
#### Represents a vector marker clipping path. 


### CIMClippingPath 

|Property | Type | Description | 
|---------|--------|--------|
| clippingType | [enumeration ClippingType](CIMSymbols.md#enumeration-clippingtype) | The clipping type. 
| path | [Polygon](ExternalReferences.md#polygon) | The clipping path. 





### Enumeration: ClippingType
#### Clipping types. 

|Property | Value | Description | 
|---------|--------|--------|
| Intersect| 0| Intersect. 
| Subtract| 1| Subtract. 




## CIMColorSubstitution
#### Represents color substitution, an ordered list of color substitutes. 


### CIMColorSubstitution 

|Property | Type | Description | 
|---------|--------|--------|
| oldColor | [Color](Types.md#color) | The old color (the color that will be substituted). 
| newColor | [Color](Types.md#color) | The new color that will replace the old color. 






## CIMCompositeCallout
#### Represents a composite callout. Composite callouts are a filled background along with an optional shadow, which is placed behind text. They may also have a leader line (consisting of one or both of a simple line, and filled dart) connecting the callout to an anchor point. Composite callouts may have additional surrounding text elements. The text representing these parts is specified in the text string using tags. Their relative position properties are specified in the CIMCompositeCallout through their corresponding CIMCompositeTextPartPosition elements specified below, but these properties can also be overridden with tag attributes. 


### CIMCallout 

|Property | Type | Description | 
|---------|--------|--------|
| leaderTolerance | double | The leader tolerance which is the closest distance (in points) to the text the anchor point can be for the callout to draw. 
| leaderOffset | double | The leader offset which is an offset value defining the distance (in points) between the anchor point and the beginning of the drawn leader. 


### CIMCompositeCallout 

|Property | Type | Description | 
|---------|--------|--------|
| cornerRadius | double | The callout corner radius in points. 0.0 corresponds to a rectangle corner. 
| backgroundSymbol | [CIMPolygonSymbol](CIMSymbols.md#cimpolygonsymbol) | The symbol used to draw the background. 
| margin | [CIMTextMargin](CIMSymbols.md#cimtextmargin) | The text margin defining the space around the text that is accounted for in balloon creation. 
| dartWidth | double | The dart width. 
| dartSymbol | [CIMPolygonSymbol](CIMSymbols.md#cimpolygonsymbol) | A symbol used to draw the dart. This is only used if LeaderLinePercentage is less than 100%. 
| snapLeaderToCornersOnly | boolean | A value indicating whether the leader line should snap only to corners. 
| leaderLinePercentage | double | The percentage of the leader line which is drawn as a line as opposed to a solid dart. 
| leaderLineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol) | The leader line symbol. This is only used if LeaderLinePercentage is greater than 0%. 
| shadowSymbol | [CIMPolygonSymbol](CIMSymbols.md#cimpolygonsymbol) | The shadow symbol for the callout. 
| shadowXOffset | double | The shadow offset from the callout symbol in the horizontal direction. If X and Y are zero, no shadow is drawn. 
| shadowYOffset | double | The shadow offset from the callout symbol in the vertical direction. If X and Y are zero, no shadow is drawn. 
| middle | [CIMCompositeTextPartPosition](CIMSymbols.md#cimcompositetextpartposition) | The text part position properties for the middle part of the callout text. This contains the relative positioning information. Split offset and box will have no effect on this text part, since it is required that that the middle part is in the center of the callout. 
| topLeft | [CIMCompositeTextPartPosition](CIMSymbols.md#cimcompositetextpartposition) | The text part position properties for the top left part of the callout text. This contains the relative positioning information, as well as split offset indicating the extent to which the callout part will mask the callout outline, and whether or not the part should be boxed in by the overall callout, or not. 
| top | [CIMCompositeTextPartPosition](CIMSymbols.md#cimcompositetextpartposition) | The text part position properties for the top part of the callout text. This contains the relative positioning information, as well as split offset indicating the extent to which the callout part will mask the callout outline, and whether or not the part should be boxed in by the overall callout, or not. 
| topRight | [CIMCompositeTextPartPosition](CIMSymbols.md#cimcompositetextpartposition) | The text part position properties for the top right part of the callout text. This contains the relative positioning information, as well as split offset indicating the extent to which the callout part will mask the callout outline, and whether or not the part should be boxed in by the overall callout, or not. 
| right | [CIMCompositeTextPartPosition](CIMSymbols.md#cimcompositetextpartposition) | The text part position properties for the right part of the callout text. This contains the relative positioning information, as well as split offset indicating the extent to which the callout part will mask the callout outline, and whether or not the part should be boxed in by the overall callout, or not. 
| left | [CIMCompositeTextPartPosition](CIMSymbols.md#cimcompositetextpartposition) | The text part position properties for the left part of the callout text. This contains the relative positioning information, as well as split offset indicating the extent to which the callout part will mask the callout outline, and whether or not the part should be boxed in by the overall callout, or not. 
| bottomLeft | [CIMCompositeTextPartPosition](CIMSymbols.md#cimcompositetextpartposition) | The text part position properties for the bottom left part of the callout text. This contains the relative positioning information, as well as split offset indicating the extent to which the callout part will mask the callout outline, and whether or not the part should be boxed in by the overall callout, or not. 
| bottom | [CIMCompositeTextPartPosition](CIMSymbols.md#cimcompositetextpartposition) | The text part position properties for the bottom part of the callout text. This contains the relative positioning information, as well as split offset indicating the extent to which the callout part will mask the callout outline, and whether or not the part should be boxed in by the overall callout, or not. 
| bottomRight | [CIMCompositeTextPartPosition](CIMSymbols.md#cimcompositetextpartposition) | The text part position properties for the bottom right part of the callout text. This contains the relative positioning information, as well as split offset indicating the extent to which the callout part will mask the callout outline, and whether or not the part should be boxed in by the overall callout, or not. 
| floating | [CIMCompositeTextPartPosition](CIMSymbols.md#cimcompositetextpartposition) | The text part position properties for the floating part of the callout text. This contains the relative positioning information, as well as split offset indicating the extent to which the callout part will mask the callout outline, and whether or not the part should be boxed in by the overall callout, or not. The floating part is anchored below the bottom text part. If there is no bottom text part it is anchored below the middle text part plus margins. 






## CIMCompositeTextPartPosition
#### Represents the text part position properties on a callout part. 


### CIMCompositeTextPartPosition 

|Property | Type | Description | 
|---------|--------|--------|
| horizontalAlignment | [enumeration HorizontalAlignment](CIMSymbols.md#enumeration-horizontalalignment) | The horizontal alignment of the text part. 
| verticalAlignment | [enumeration VerticalAlignment](CIMSymbols.md#enumeration-verticalalignment) | The vertical alignment of the text part. 
| XOffset | double | The X offset of the text part. 
| YOffset | double | The Y offset of the text part. 
| splitOffset | double | The split offset of the text part. This determines how much of a gap there is between the callout border and any part of the text part intersecting the border If this is set to wider than the callout width, none of the associated callout line will draw. 
| isPartWithinCalloutBox | boolean | A value indicating whether the text part will be contained within the main callout. If this is set to true, the main callout will expand to encompass this text part, and a line will be draw separating the part from the rest of the callout. This line will have the same symbol as the callout outline and will only draw if the text part is above or below the top and bottom margins of the middle text. 





### Enumeration: ExternalColorMixMode
#### Options to control how material combines with externally defined colors. 

|Property | Value | Description | 
|---------|--------|--------|
| Tint| 0| Tint using external color. 
| Ignore| 1| Ignore external color. 
| Multiply| 99| Multiply components by components of external color. 



### Enumeration: ExtremityPlacement
#### Extremity placement options which specify at which ends of the line a marker will be placed. 

|Property | Value | Description | 
|---------|--------|--------|
| Both| 0| Both - marker is placed at the beginning and end of the line. 
| JustBegin| 1| JustBegin - marker is placed at the beginning of the line, determined by the direction that the line was digitized. 
| JustEnd| 2| JustEnd - marker is placed at the end of the line, determined by the direction that the line was digitized. 
| None| 3| None - no marker is placed at either end of the marker. 



### Enumeration: FillMode
#### Fill modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Mosaic| 0| Mosaic fill. 
| Centered| 1| Centered fill. 



### Enumeration: FontEffects
#### Font effects. 

|Property | Value | Description | 
|---------|--------|--------|
| Normal| 0x00| Normal text. 
| Superscript| 0x01| Superscript text. 
| Subscript| 0x02| Subscript text 



### Enumeration: FontEncoding
#### Font encodings. 

|Property | Value | Description | 
|---------|--------|--------|
| MSSymbol| 0| Symbol encoding. 
| Unicode| 1| Unicode. 



### Enumeration: FontType
#### Font types. 

|Property | Value | Description | 
|---------|--------|--------|
| Unspecified| 0| Unspecified. 
| TrueType| 1| TrueType. 
| PSOpenType| 2| OpenType with CFF outlines. 
| TTOpenType| 3| OpenType with TrueType outlines. 
| Type1| 4| Adobe Type 1. 




## CIMGeometricEffectAddControlPoints
#### Represents the add control points geometric effect. Dynamically adds geometry control points to a feature to dictate the placement of markers or other effect properties that leverage control points. Control points are placed at angles or deflection based on the AngleTolerance value. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectAddControlPoints 

|Property | Type | Description | 
|---------|--------|--------|
| angleTolerance | double | The value below which a control point will be placed. The maximum amount of deflection from one segment to another at a vertex. Angle values between 180 and 360 are interpreted the same as values between 0 and 180. Angle values of 180 and 360 are the same as 0. 






## CIMGeometricEffectArrow
#### Represents the arrow geometric effect which creates a dynamic line along a line feature with an arrow of a specified arrow type and width. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectArrow 

|Property | Type | Description | 
|---------|--------|--------|
| geometricEffectArrowType | [enumeration GeometricEffectArrowType](CIMSymbols.md#enumeration-geometriceffectarrowtype) | The type of arrow to be displayed. 
| width | double | The distance between the lines that construct the body of the arrow. 





### Enumeration: GeometricEffectArrowType
#### Geometric effect arrow types. 

|Property | Value | Description | 
|---------|--------|--------|
| OpenEnded| 0| An open ended arrow. 
| Block| 1| A block arrow. 
| Crossed| 2| A crossed arrow. 




## CIMGeometricEffectBuffer
#### Represents the buffer geometric effect which creates a dynamic polygon with a specified distance around features. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectBuffer 

|Property | Type | Description | 
|---------|--------|--------|
| size | double | The distance from the feature. This distance is either from the edge of the marker, the edge of the stroke or the edge of the polygon outline. 






## CIMGeometricEffectCut
#### Represents the cut geometric effect which creates a dynamic line that is shorter on one or both ends than the line feature or polygon outline. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectCut 

|Property | Type | Description | 
|---------|--------|--------|
| beginCut | double | The distance from the beginning of a line that the display of the stroke starts. The beginning of the line is determined by the direction in which the line was digitized. 
| endCut | double | The distance from the end of a line that the display of the stroke ends. The end of the line is determined by the direction in which the line was digitized. 
| middleCut | double | The distance around the middle of a line that the display of the stroke is interrupted. 
| invert | boolean | A value indicating whether the effect should be applied in the opposite manner. This displays the stroke symbol only at the ends of the line and leaves the rest of the line unsymbolized. 






## CIMGeometricEffectDashes
#### Represents the dashes geometric effect which creates a dynamic multipart line geometry from a line feature or the outline of a polygon based on a template. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectDashes 

|Property | Type | Description | 
|---------|--------|--------|
| customEndingOffset | double | Where the pattern should end relative to the ending point of the geometry. Negative numbers indicate a shift to the left and positive numbers a shift to the right. This property is only applied if the LineDashEnding is set to Custom. 
| dashTemplate | [double] | The distance for each dash and gap. There can be multiple dash and gap values to form a complex pattern. 
| lineDashEnding | [enumeration LineDashEnding](CIMSymbols.md#enumeration-linedashending) | The setting which determines how the strokes with dash patterns and other patterns (pictures, placement effects) are handled at the end points of the line geometry's segments. 
| offsetAlongLine | double | The position where the pattern should begin relative to the starting point of the geometry. It shifts the entire pattern along the line the specified distance. Negative values indicate a shift to the left and positive numbers a shift to the right. This property is only applied if LineDashEnding is set to NoConstraint or Custom. 
| controlPointEnding | [enumeration LineDashEnding](CIMSymbols.md#enumeration-linedashending) | The line dash ending position. 






## CIMGeometricEffectDonut
#### Represents the donut geometric effect which creates a dynamic polygon ring of a specified width in relation to the outline of polygon features. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectDonut 

|Property | Type | Description | 
|---------|--------|--------|
| method | [enumeration GeometricEffectDonutMethod](CIMSymbols.md#enumeration-geometriceffectdonutmethod) | The method which specifies the way the strokes are displayed at convex corners of the polygon. 
| option | [enumeration GeometricEffectOffsetOption](CIMSymbols.md#enumeration-geometriceffectoffsetoption) | The option for the way the symbol handles complex geometries. 
| width | double | The distance from the edge of the polygon that the fill symbol is to be displayed. 





### Enumeration: GeometricEffectDonutMethod
#### Geometric effect donut methods. 

|Property | Value | Description | 
|---------|--------|--------|
| Mitered| 0| Mitered - matches the exact shape around a convex corner of the polygon. 
| Bevelled| 1| Bevelled - follows the shortest straight path across a convex corner of the polygon. 
| Rounded| 2| Rounded - follows a path of equal distance around a convex corner of the polygon. 
| Square| 3| Square - follows a straight path across the corner of a line or polygon. 
| TrueBuffer| 4| TrueBuffer - uses the buffer algorithm to follow a path around convex corners. 




## CIMGeometricEffectEnclosingPolygon
#### Represents the enclosing polygon geometric effect which creates a dynamic polygon from the spatial extent of a line or polygon feature. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectEnclosingPolygon 

|Property | Type | Description | 
|---------|--------|--------|
| method | [enumeration GeometricEffectEnclosingPolygonMethod](CIMSymbols.md#enumeration-geometriceffectenclosingpolygonmethod) | The method which specifies the way in which the polygon geometry is generated around the feature geometry. 





### Enumeration: GeometricEffectEnclosingPolygonMethod
#### Geometric effect enclosing polygon methods. 

|Property | Value | Description | 
|---------|--------|--------|
| ClosePath| 0| ClosePath - for polygon input, it generates a polygon that matches the geometry of a polygon feature. For line input, it generates a polygon that connects both ends of the line to each other. 
| ConvexHull| 1| ConvexHull - for polygon input, it generates a polygon with a minimum number of sides to surround the feature. For line input, it generates a polygon that approximates the shape of the line. 
| RectangularBox| 2| RectangularBox - generates a polygon equal to the spatial envelope of the feature. 




## CIMGeometricEffectExtension
#### Represents the extension geometric effect which creates a dynamic line that is extended from either the beginning or the end of the line feature at a specified deflection angle and length. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectExtension 

|Property | Type | Description | 
|---------|--------|--------|
| deflection | double | The deflection angle used for the extension. A value of 0 indicates no deflection. 
| origin | [enumeration GeometricEffectExtensionOrigin](CIMSymbols.md#enumeration-geometriceffectextensionorigin) | The origin of the extension to add to the line. The beginning and end of the line is defined by the direction the line was digitized. 
| length | double | The length of the extension that is dynamically created. 





### Enumeration: GeometricEffectExtensionOrigin
#### Geometric effect extension origins. Specifies the origin of the extension to add to the line. The beginning and end of the line is defined by the direction the line was digitized. 

|Property | Value | Description | 
|---------|--------|--------|
| BeginningOfLine| 0| BeginningOfLine - extension is added to the end of the line. 
| EndOfLine| 1| EndOfLine - extension is added to the end of the line. 




## CIMGeometricEffectJog
#### Represents the jog geometric effect which creates a dynamic line with a jog of a specified angle, position, and width in the line. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectJog 

|Property | Type | Description | 
|---------|--------|--------|
| angle | double | The angle of the jog in the line which is measured in degrees. 
| length | double | The length of the segment that forms the jog in the line. 
| position | double | The location of the center of the jog, as a percentage measured from the start of the input geometry. 






## CIMGeometricEffectLocalizerFeather
#### Represents a geometric effect which creates a localizer feather for aeronautical charts. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectLocalizerFeather 

|Property | Type | Description | 
|---------|--------|--------|
| style | [enumeration GeometricEffectLocalizerFeatherStyle](CIMSymbols.md#enumeration-geometriceffectlocalizerfeatherstyle) | The localizer feather style. 
| length | double | The length of the localizer feather. 
| width | double | The width of the localizer feather. 
| angle | double | The angle of the localizer feather. 





### Enumeration: GeometricEffectLocalizerFeatherStyle
#### Geometric effect localizer feather styles. 

|Property | Value | Description | 
|---------|--------|--------|
| Complete| 0| Displays a complete localizer feather. 
| Left| 1| Displays the left side of a localizer feather. 
| Right| 2| Displays the right side of a localizer feather. 




## CIMGeometricEffectMove
#### Represents the move geometric effect which creates a point, line or polygon that is offset a specified distance in X and Y. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectMove 

|Property | Type | Description | 
|---------|--------|--------|
| offsetX | double | The distance to move the symbol along the X-axis of the feature geometry. 
| offsetY | double | The distance to move the symbol along the Y-axis of the feature geometry. 






## CIMGeometricEffectOffset
#### Represents the offset geometric effect which creates a dynamic line or polygon offset at a specified distance perpendicularly from a feature. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectOffset 

|Property | Type | Description | 
|---------|--------|--------|
| method | [enumeration GeometricEffectOffsetMethod](CIMSymbols.md#enumeration-geometriceffectoffsetmethod) | The way the strokes or fills are displayed at corners. 
| offset | double | The distance of the symbol perpendicular to the feature geometry. 
| option | [enumeration GeometricEffectOffsetOption](CIMSymbols.md#enumeration-geometriceffectoffsetoption) | The way the symbol handles complex geometries. 






## CIMGeometricEffectOffsetHatch
#### Represents a geometric effect which creates a hatch pattern to depict special use airspace for aeronautical charts. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectOffsetHatch 

|Property | Type | Description | 
|---------|--------|--------|
| length | double | The length of the offset hatch. 
| spacing | double | The spacing of the offset hatch. 





### Enumeration: GeometricEffectOffsetMethod
#### Geometric effect offset method which specifies the way the strokes or fills are displayed at corners. 

|Property | Value | Description | 
|---------|--------|--------|
| Mitered| 0| Mitered - matches the exact shape around a corner of the line or polygon. 
| Bevelled| 1| Bevelled - follows the shortest straight path across a corner of the line or polygon. 
| Rounded| 2| Rounded - follows a path of equal distance around a corner of the line or polygon. 
| Square| 3| Square - follows a straight path across the corner of a line or polygon. 



### Enumeration: GeometricEffectOffsetOption
#### Geometric effect offset options which specify the way the symbol handles complex geometries. 

|Property | Value | Description | 
|---------|--------|--------|
| Fast| 0| Fast - ignores complex geometries and applies a best fit to the symbol. 
| Accurate| 1| Accurate - accommodates complex geometries and applied a true fit to the symbol. 




## CIMGeometricEffectOffsetTangent
#### Represents the offset tangent geometric effect which creates a dynamic line along a line feature offset in the direction defined by either the beginning or the end of the line. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectOffsetTangent 

|Property | Type | Description | 
|---------|--------|--------|
| method | [enumeration GeometricEffectOffsetTangentMethod](CIMSymbols.md#enumeration-geometriceffectoffsettangentmethod) | The origin of the tangent offset for the line. The beginning and end of the lines are defined by how the line was digitized. 
| offset | double | The distance the geometry is moved tangent. 





### Enumeration: GeometricEffectOffsetTangentMethod
#### Geometric effect offset tangent methods which specify the origin of the tangent offset for the line. The beginning and end of the lines are defined by how the line was digitized. 

|Property | Value | Description | 
|---------|--------|--------|
| BeginningOfLine| 0| BeginningOfLine - the tangent offset is applied from the beginning of the line. 
| EndOfLine| 1| EndOfLine - the tangent offset is applied from the end of the line. 




## CIMGeometricEffectRadial
#### Represents the radial geometric effect which creates a dynamic line of a specified length and angle originating from a point feature. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectRadial 

|Property | Type | Description | 
|---------|--------|--------|
| angle | double | The orientation of the line from the marker. The angle is calculated in a counterclockwise manner with 0 degrees equal to due east. 
| length | double | The distance of the line from end to end. 






## CIMGeometricEffectRegularPolygon
#### Represents the regular polygon geometric effect which creates a dynamic polygon around a point feature with a specified number of edges. All edges are equal in length and all angles are equal. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectRegularPolygon 

|Property | Type | Description | 
|---------|--------|--------|
| angle | double | The amount of rotation for the polygon. 
| edges | long | The number of sides for the polygon. Specifying a value less than 3 produces a circle. 
| radius | double | The distance from the center of the polygon. 






## CIMGeometricEffectReverse
#### Represents the reverse geometric effect which creates a dynamic polygon around a point feature with a specified number of edges. All edges are equal in length and all angles are equal. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectReverse 

|Property | Type | Description | 
|---------|--------|--------|
| reverse | boolean | A value indicating whether the dynamic output of a previous geometric effect is to be flipped or not. 






## CIMGeometricEffectRotate
#### Represents the rotate geometric effect which creates a dynamic line or polygon rotated a specified angle from the feature. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectRotate 

|Property | Type | Description | 
|---------|--------|--------|
| angle | double | The amount of rotation for the symbol. 






## CIMGeometricEffectScale
#### Represents the rotate geometric effect which creates a dynamic line or polygon scaled by a specified factor. Vertices are moved in relation to the center point of a feature envelope. Values greater than 1 move vertices away from the center point. Values between 0 and 1 move vertices toward the center point. Values less than 0 draw an inverse dynamic line or polygon where the vertices have crossed to the other side of the center point. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectScale 

|Property | Type | Description | 
|---------|--------|--------|
| XScaleFactor | double | The amount of change in size of a symbol in the x-axis. The value is expressed in terms of a ratio/percentage. 
| YScaleFactor | double | The amount of change in size of a symbol in the y-axis. The value is expressed in terms of a ratio/percentage. 






## CIMGeometricEffectSuppress
#### Represents the suppress geometric effect which creates a dynamic line that hides sections of a stroke between pairs control points. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectSuppress 

|Property | Type | Description | 
|---------|--------|--------|
| suppress | boolean | A value indicating whether the portion of the stroke symbol between control points should be suppressed. Sections that are suppressed draw with no symbol. 
| invert | boolean | A value indicating whether to invert the suppression process. If this value is true, portions of the stroke symbol between control points are kept and all other portions are suppressed. 






## CIMGeometricEffectTaperedPolygon
#### Represents the tapered polygon geometric effect which creates a dynamic polygon along a line feature, whose width varies by two specified amounts along its length, as defined by a percentage of the line feature's length. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectTaperedPolygon 

|Property | Type | Description | 
|---------|--------|--------|
| fromWidth | double | The width at the start of the line to be used to generate a polygon. 
| length | double | The distance along the line to be used to generate the polygon. 
| toWidth | double | The width at the end of the line to be used to generate the polygon. 






## CIMGeometricEffectWave
#### Represents the wave geometric effect which creates a dynamic line or polygon along a feature with a repeating wave pattern. 


### CIMGeometricEffect 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMGeometricEffectWave 

|Property | Type | Description | 
|---------|--------|--------|
| amplitude | double | The distance perpendicular to a feature to display the curves for the symbol. 
| period | double | The distance along the line or polygon to display the curves for the symbol. 
| seed | long | The staring value for generating a random number. This is only used when the Waveform is set to Random. 
| waveform | [enumeration GeometricEffectWaveform](CIMSymbols.md#enumeration-geometriceffectwaveform) | The shape of the curves to be displayed along the symbol. 





### Enumeration: GeometricEffectWaveform
#### Geometric effect offset waveforms. 

|Property | Value | Description | 
|---------|--------|--------|
| Sinus| 0| Sinus - displays a sinusoidal curve. 
| Square| 1| Square - displays a three-sided rectangular shape. 
| Triangle| 2| Triangle - displays a two-sided triangular shape. 
| Random| 3| Random - displays a sine curve with random variations in the period and amplitude 



### Enumeration: GlyphHinting
#### Glyph hinting options. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No glyph hinting. 
| Default| 1| Default glyph hinting according to the font's settings. 
| Force| 2| Force glyph hinting. 



### Enumeration: GradientAlignment
#### Gradient alignment types. 

|Property | Value | Description | 
|---------|--------|--------|
| Buffered| 0| Buffered - Distributes the color ramp along the line's geometry from the outside in (similar to the effect of creating a buffer of the line, then using the "buffer" fill type). 
| Left| 1| Left - Progresses the color ramp from the line's centerline to the outside edge on the left. The gradient will follow any curvature in the line's geometry. 
| Right| 2| Right - Progresses the color ramp from the line's centerline to the outside edge on the right. The gradient will follow any curvature in the line's geometry. 
| AlongLine| 3| Along line - Distributes the color ramp linearly along the line, following the curvature of the line. 




## CIMGradientFill
#### Represents a gradient fill which fills polygonal geometry with a specified color scheme. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMFill 

|Property | Type | Description | 
|---------|--------|--------|


### CIMGradientFill 

|Property | Type | Description | 
|---------|--------|--------|
| angle | double | The angle of the gradient when the GradientMethod is set to Linear or Rectangular. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color scheme that is applied to the fill. 
| gradientMethod | [enumeration GradientFillMethod](CIMSymbols.md#enumeration-gradientfillmethod) | A value which specifies how the gradient is applied within the fill. 
| gradientSize | double | A value which determines how much of the feature is covered by the color scheme. This is either a percentage of the total area which the color scheme spans or the number of page units from the starting point at which the gradient displays. 
| gradientSizeUnits | [enumeration SymbolUnits](CIMSymbols.md#enumeration-symbolunits) | A value which specifies whether GradientSize is applied with an absolute distance or a relative percentage. 
| gradientType | [enumeration GradientStrokeType](CIMSymbols.md#enumeration-gradientstroketype) | A value which specifies if the gradient is applied with discrete intervals or if it is continuous. 
| interval | long | How many bands draw when the GradientType is set to Discrete. 





### Enumeration: GradientFillMethod
#### Describes the gradient fill method which is how the gradient is applied. 

|Property | Value | Description | 
|---------|--------|--------|
| Linear| 0| Linear - Change from one color to the next is linear across the geometry. 
| Rectangular| 1| Rectangular - Change from one color to the next is rectangular, from the extent of the geometry. 
| Circular| 2| Circular - Change from one color to the next is circular, from the extent of the geometry 
| Buffered| 3| Buffered - Color changes based on an internal buffering of the geometry outline 




## CIMGradientStroke
#### Represents a gradient stroke which draws linear geometry with a specified color scheme. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMStroke 

|Property | Type | Description | 
|---------|--------|--------|
| capStyle | [enumeration LineCapStyle](CIMSymbols.md#enumeration-linecapstyle) | How the stroke should draw at the ends of the geometries. 
| joinStyle | [enumeration LineJoinStyle](CIMSymbols.md#enumeration-linejoinstyle) | How the symbol is drawn at the stroke segment connections. 
| lineStyle3D | [enumeration Simple3DLineStyle](CIMSymbols.md#enumeration-simple3dlinestyle) | How strokes will be rendered in 3D. 
| miterLimit | double | The maximum 'sharpness' that is allowed for Miter joins. If the spike created by the miter join exceeds the miter limit times the width of the stroke, the sharp angle will be clipped and rendered with a bevel join. This property is only applied to the symbol layer when the JoinType is set to Miter. 
| width | double | The width of the stroke. 
| closeCaps3D | boolean | A value indicating whether to close caps when drawing them in 3D. When set to false, the caps are hollow. 


### CIMGradientStroke 

|Property | Type | Description | 
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp) | The color scheme that is applied to the stroke. 
| gradientMethod | [enumeration GradientStrokeMethod](CIMEnumerations.md#enumeration-gradientstrokemethod) | How the gradient is applied along the stroke. 
| gradientSize | double | How much of the feature is covered by the color scheme. This is either a percentage of the total area which the color scheme spans or the number of page units from the starting point at which the gradient displays. 
| gradientSizeUnits | [enumeration SymbolUnits](CIMSymbols.md#enumeration-symbolunits) | Whether GradientSize is applied with an absolute distance or a relative percentage. 
| gradientType | [enumeration GradientStrokeType](CIMSymbols.md#enumeration-gradientstroketype) | Whether the gradient is applied with discrete or continuous intervals. 
| interval | long | How many bands draw when the GradientType is set to Discrete. 





### Enumeration: GradientStrokeType
#### Gradient stroke types. 

|Property | Value | Description | 
|---------|--------|--------|
| Discrete| 0| Discrete gradient types have distinct lines of separation between each color. 
| Continuous| 1| Continuous gradients vary continuously along the color change with no distinct boundary between the colors. 




## CIMHatchFill
#### Represents a hatch fill which fills polygonal geometry with a uniform series of parallel line symbols. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMFill 

|Property | Type | Description | 
|---------|--------|--------|


### CIMHatchFill 

|Property | Type | Description | 
|---------|--------|--------|
| lineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol) | The line symbol that is used to draw the hatch lines in the fill. 
| offsetX | double | How much to move the stroke to a new X-position. 
| rotation | double | The angle of rotation for all the strokes, in degrees. 
| separation | double | The distance between the line symbols in the hatch pattern. 
| offsetY | double | How much to move the stroke to a new Y-position. 





### Enumeration: HorizontalAlignment
#### Horizontal alignment types. 

|Property | Value | Description | 
|---------|--------|--------|
| Left| 0| Left aligned. 
| Right| 1| Right aligned. 
| Center| 2| Centered. 
| Justify| 3| Justified alignment. 



### Enumeration: LeaderLineStyle
#### The style of line to generate when a leader is drawn defined by an enumeration value. Line leaders will always be drawn with their own geometry. 

|Property | Value | Description | 
|---------|--------|--------|
| Base| 0| The line callout leader is a single line originating from the closest corner of the text box with the gap applied. If the callout has an accent bar it is connected to the closest point at the either top or bottom of the accent bar. 
| MidPoint| 1| The line callout leader is a single line originating from the midpoint of the left or right side of the text box with the gap applied or from the midpoint of the accent bar if the callout has one. 
| ThreePoint| 2| The line callout leader is a 3-point line originating from the midpoint of the left or right side of the text box with the gap applied or the midpoint of the accent bar if the callout has one. 
| FourPoint| 3| The line callout leader is a 4-point line originating from the midpoint of the left or right side of the text box with the gap applied or the midpoint of the accent bar if the callout has one. 
| Underline| 4| The line callout draws a line that connects to the closest of the four corners of the text with the gap applied. If the callout has an accent bar it is connected to the closest point at either the top or bottom of the accent bar. Additionally, either and underline or an "overline" is drawn along the closest side (bottom or top) of the text. 
| CircularCW| 5| The line callout leader is curved (clockwise) from the anchor point to the closest corner of the text box with the gap applied. If the callout has an accent bar it is connected to the closest point at the either top or bottom of the accent bar. 
| CircularCCW| 6| The line callout leader is curved (counter-clockwise) from the anchor point to the closest corner of the text box with the gap applied. If the callout has an accent bar it is connected to the closest point at the either top or bottom of the accent bar. 



### Enumeration: LineCapStyle
#### The style of stroke ending caps. 

|Property | Value | Description | 
|---------|--------|--------|
| Butt| 0| Stroke ends in butt caps. 
| Round| 1| Stroke ends in round caps. 
| Square| 2| Stroke ends in square caps. 



### Enumeration: LineDashEnding
#### Determines how the strokes with dash patterns and other patterns (tiled pictures, placement effects) are handled at the end points of the line geometry's segments. If more than one pattern exists (for example, a dashed simple stroke, a hash stroke, and a marker stroke) then the longest pattern's length is affected directly by this option and the rest of the stroke patterns are resized proportionately to match. 

|Property | Value | Description | 
|---------|--------|--------|
| NoConstraint| 0| No Constraint - no constraint is applied to how the dash is placed. 
| HalfPattern| 1| Half Pattern - a half dash will be placed on either side of control points. 
| HalfGap| 2| Half Gap - a space equal to the half the gap value will be placed on either side of control points. 
| FullPattern| 3| Full Pattern - a full dash will be placed on either side of control points. 
| FullGap| 4| Full Gap - a space equal to the gap value will be placed on either side of control points. 
| Custom| 5| Custom - the pattern is fit to the length of the feature by adjusting the gaps slightly. 



### Enumeration: LineDecorationStyle
#### Defines simple decorations for lines. 

|Property | Value | Description | 
|---------|--------|--------|
| None| -1| No decoration. 
| Custom| 0| The decoration is defined in the Layers property as a set of SymbolReferences. 
| Circle| 1| A circle is added at the end of the line. 
| OpenArrow| 2| An open arrow is added to the end of the line. 
| ClosedArrow| 3| A closed arrow is added to the end of the line. 
| Diamond| 4| A diamond is added at the end of the line. 



### Enumeration: LineGapType
#### Specifies the type of line gap (line spacing) that is applied. 

|Property | Value | Description | 
|---------|--------|--------|
| ExtraLeading| 0| Extra Leading - Adds the specified value to the line spacing that accommodates the largest font in the line 
| Multiple| 1| Multiple - Sets the line spacing based on a multiple of the line. 
| Exact| 2| Exact - Sets a fixed line spacing 



### Enumeration: LineJoinStyle
#### Specifies how the symbol is drawn at the stroke segment connections. 

|Property | Value | Description | 
|---------|--------|--------|
| Bevel| 0| The stroke join is beveled. 
| Round| 1| The line join is round. 
| Miter| 2| The line join is mitered. 




## CIMLineSymbol
#### Represents a line symbol which is used to draw polyline features or graphics. 


### CIMSymbol 

|Property | Type | Description | 
|---------|--------|--------|


### CIMMultiLayerSymbol 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | The geometric effects that are applied to the symbol. 
| symbolLayers | [[CIMSymbolLayer]](Types.md#cimsymbollayer) | The symbol layers. Symbol layers are the components that make up a symbol. A symbol layer is represented by a stroke, fill, marker, or procedural symbol layer. 
| thumbnailURI | string | The representative image of the symbol. 
| useRealWorldSymbolSizes | boolean | A value indicating whether the symbol size properties are rendered using real world units or page units. When set to true the symbol will draw using real world units (e.g. meters). 


### CIMLineSymbol 

|Property | Type | Description | 
|---------|--------|--------|






## CIMMarkerGraphic
#### Represents a marker graphic which is used to define vector graphics in a vector marker. 


### CIMMarkerGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| geometry | [Geometry](ExternalReferences.md#geometry) | The geometry of the marker. 
| symbol | [Symbol](Types.md#symbol) | The symbol used to draw the marker graphic, can be a point, line, polygon, or text symbol. 
| textString | string | The text that is defined within the marker if drawn with a text symbol. 
| primitiveName | string | The primitive name. 






## CIMMarkerPlacementAlongLineRandomSize
#### Represents marker placement along the line which places randomly sized markers evenly along a line or polygon outline. 


### CIMMarkerPlacement 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMMarkerStrokePlacement 

|Property | Type | Description | 
|---------|--------|--------|
| angleToLine | boolean | A value indicating whether to angle the marker to the line. 
| offset | double | The offset. 


### CIMMarkerPlacementAlongLine 

|Property | Type | Description | 
|---------|--------|--------|
| controlPointPlacement | [enumeration PlacementEndings](CIMSymbols.md#enumeration-placementendings) | How markers are placed at control points. 
| customEndingOffset | double | Where the pattern should end relative to the ending point of the geometry. The entire pattern is shifted along the line for the specified distance. Negative numbers shift to the left and positive numbers shift to the right. This is only applied if the Endings property is set to Custom. 
| endings | [enumeration PlacementEndings](CIMSymbols.md#enumeration-placementendings) | How markers are placed at the end points of a line. 
| offsetAlongLine | double | Where the pattern should begin relative to the starting point of the geometry. The entire pattern is shifted along the line for the specified distance. Negative numbers shift to the left and positive numbers shift to the right. This is only applied if the Endings property is set to No Constraint or Custom. 
| placementTemplate | [double] | The numeric pattern that defines the sequence of placed markers and the length of space between them. 


### CIMMarkerPlacementAlongLineRandomSize 

|Property | Type | Description | 
|---------|--------|--------|
| randomization | [enumeration PlacementRandomlyAlongLineRandomization](CIMSymbols.md#enumeration-placementrandomlyalonglinerandomization) | The amount of randomness to be used for the size and rotation of the markers on the line. The size and rotation of the marker will vary for individual markers. 
| seed | long | The starting value for generating a random number. This random number is used by the Randomization property to determine the marker shape. 






## CIMMarkerPlacementAlongLineSameSize
#### Represents marker placement along the line which places markers that are the same size evenly along a line or polygon outline. 


### CIMMarkerPlacement 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMMarkerStrokePlacement 

|Property | Type | Description | 
|---------|--------|--------|
| angleToLine | boolean | A value indicating whether to angle the marker to the line. 
| offset | double | The offset. 


### CIMMarkerPlacementAlongLine 

|Property | Type | Description | 
|---------|--------|--------|
| controlPointPlacement | [enumeration PlacementEndings](CIMSymbols.md#enumeration-placementendings) | How markers are placed at control points. 
| customEndingOffset | double | Where the pattern should end relative to the ending point of the geometry. The entire pattern is shifted along the line for the specified distance. Negative numbers shift to the left and positive numbers shift to the right. This is only applied if the Endings property is set to Custom. 
| endings | [enumeration PlacementEndings](CIMSymbols.md#enumeration-placementendings) | How markers are placed at the end points of a line. 
| offsetAlongLine | double | Where the pattern should begin relative to the starting point of the geometry. The entire pattern is shifted along the line for the specified distance. Negative numbers shift to the left and positive numbers shift to the right. This is only applied if the Endings property is set to No Constraint or Custom. 
| placementTemplate | [double] | The numeric pattern that defines the sequence of placed markers and the length of space between them. 


### CIMMarkerPlacementAlongLineSameSize 

|Property | Type | Description | 
|---------|--------|--------|






## CIMMarkerPlacementAlongLineVariableSize
#### Represents marker placement along the line which places markers in either increasing, decreasing or alternating gradations along a line or polygon outline. 


### CIMMarkerPlacement 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMMarkerStrokePlacement 

|Property | Type | Description | 
|---------|--------|--------|
| angleToLine | boolean | A value indicating whether to angle the marker to the line. 
| offset | double | The offset. 


### CIMMarkerPlacementAlongLine 

|Property | Type | Description | 
|---------|--------|--------|
| controlPointPlacement | [enumeration PlacementEndings](CIMSymbols.md#enumeration-placementendings) | How markers are placed at control points. 
| customEndingOffset | double | Where the pattern should end relative to the ending point of the geometry. The entire pattern is shifted along the line for the specified distance. Negative numbers shift to the left and positive numbers shift to the right. This is only applied if the Endings property is set to Custom. 
| endings | [enumeration PlacementEndings](CIMSymbols.md#enumeration-placementendings) | How markers are placed at the end points of a line. 
| offsetAlongLine | double | Where the pattern should begin relative to the starting point of the geometry. The entire pattern is shifted along the line for the specified distance. Negative numbers shift to the left and positive numbers shift to the right. This is only applied if the Endings property is set to No Constraint or Custom. 
| placementTemplate | [double] | The numeric pattern that defines the sequence of placed markers and the length of space between them. 


### CIMMarkerPlacementAlongLineVariableSize 

|Property | Type | Description | 
|---------|--------|--------|
| maxRandomOffset | double | The maximum random offset. 
| maxZoom | double | The largest size of the marker to be placed on the line. The value is expressed as a ratio. 
| minZoom | double | The smallest size of the marker to be placed on the line. The value is expressed as a ratio. 
| numberOfSizes | long | The number of different sizes of markers to be placed on the line. 
| seed | long | The starting value for generating a random number. This random number is used by the Randomization property to determine which size a marker will receive. This is only used if the VariationMethod is set to Random. 
| variationMethod | [enumeration SizeVariationMethod](CIMSymbols.md#enumeration-sizevariationmethod) | The order in which the change of size in the markers should occur. 






## CIMMarkerPlacementAtExtremities
#### Represents marker placement at extremities which places markers at only one or both endpoints of a line. 


### CIMMarkerPlacement 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMMarkerStrokePlacement 

|Property | Type | Description | 
|---------|--------|--------|
| angleToLine | boolean | A value indicating whether to angle the marker to the line. 
| offset | double | The offset. 


### CIMMarkerPlacementAtExtremities 

|Property | Type | Description | 
|---------|--------|--------|
| extremityPlacement | [enumeration ExtremityPlacement](CIMSymbols.md#enumeration-extremityplacement) | Which ends of the line a marker will be placed. 
| offsetAlongLine | double | The distance from the ends of a line that the marker will be placed. 






## CIMMarkerPlacementAtMeasuredUnits
#### Represents marker placement at geometry M values. 


### CIMMarkerPlacement 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMMarkerStrokePlacement 

|Property | Type | Description | 
|---------|--------|--------|
| angleToLine | boolean | A value indicating whether to angle the marker to the line. 
| offset | double | The offset. 


### CIMMarkerPlacementAtMeasuredUnits 

|Property | Type | Description | 
|---------|--------|--------|
| interval | double | The interval of measured units used to place markers. 
| skipMarkerRate | long | The rate of markers to skip. 
| placeAtExtremities | boolean | A value indicating whether markers should be placed at extremities. 






## CIMMarkerPlacementAtRatioPositions
#### Represents marker placement at ratio positions which places a set number of markers along the line or the outline of a polygon. 


### CIMMarkerPlacement 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMMarkerStrokePlacement 

|Property | Type | Description | 
|---------|--------|--------|
| angleToLine | boolean | A value indicating whether to angle the marker to the line. 
| offset | double | The offset. 


### CIMMarkerPlacementAtRatioPositions 

|Property | Type | Description | 
|---------|--------|--------|
| beginPosition | double | The distance from the beginning of a line that the marker will be placed. 
| endPosition | double | The distance from the end of a line that the marker will be placed. The ending of a line is determined by the direction in which the line was digitized. 
| flipFirst | boolean | A value indicating whether only the first marker will be rotated 180 degrees. 
| positionArray | [double] | The array of positions. 






## CIMMarkerPlacementInsidePolygon
#### Represents marker placement inside a polygon which defines how a polygon is filled with a pattern of markers. 


### CIMMarkerPlacement 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMMarkerFillPlacement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMMarkerPlacementInsidePolygon 

|Property | Type | Description | 
|---------|--------|--------|
| gridAngle | double | The orientation angle that the markers are placed on within the polygon. 
| gridType | [enumeration PlacementGridType](CIMSymbols.md#enumeration-placementgridtype) | The grid type which defines how markers are placed. 
| offsetX | double | The marker row offset horizontally. 
| randomness | double | The randomness of the pattern when markers are placed randomly in a polygon. 
| seed | long | The starting value for generating a random pattern. 
| shiftOddRows | boolean | A value indicating whether every other row of markers should be shifted to create an offset grid. 
| stepX | double | The distance between each marker on the X-axis of the grid. 
| stepY | double | The distance between each marker on the Y-axis of the grid. 
| offsetY | double | The marker row offset vertically. 
| clipping | [enumeration PlacementClip](CIMSymbols.md#enumeration-placementclip) | The clipping option which specifies how markers should be clipped at the polygon boundary. 






## CIMMarkerPlacementOnLine
#### Represents a marker placement on the line. 


### CIMMarkerPlacement 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMMarkerStrokePlacement 

|Property | Type | Description | 
|---------|--------|--------|
| angleToLine | boolean | A value indicating whether to angle the marker to the line. 
| offset | double | The offset. 


### CIMMarkerPlacementOnLine 

|Property | Type | Description | 
|---------|--------|--------|
| relativeTo | [enumeration PlacementOnLineRelativeTo](CIMSymbols.md#enumeration-placementonlinerelativeto) | The location on a line where a marker will be placed. The direction of the line is determined by the direction in which the line was digitized. 
| startPointOffset | double | The distances from a specified location on a line that a marker will be placed. 






## CIMMarkerPlacementOnVertices
#### Represents a marker placement on vertices which places a single marker on a line or polygon outline at a set distance from the middle or one of the endpoints. 


### CIMMarkerPlacement 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMMarkerStrokePlacement 

|Property | Type | Description | 
|---------|--------|--------|
| angleToLine | boolean | A value indicating whether to angle the marker to the line. 
| offset | double | The offset. 


### CIMMarkerPlacementOnVertices 

|Property | Type | Description | 
|---------|--------|--------|
| placeOnControlPoints | boolean | A value indicating whether a marker will be placed on the control points of the line. 
| placeOnEndPoints | boolean | A value indicating whether a marker will be placed on the endpoints of the line. 
| placeOnRegularVertices | boolean | A value indicating whether a marker will be placed on the vertices of the line. 






## CIMMarkerPlacementPolygonCenter
#### Represents marker placement polygon center which defines how a single marker will be placed within the polygon. 


### CIMMarkerPlacement 

|Property | Type | Description | 
|---------|--------|--------|
| primitiveName | string | The primitive name. 


### CIMMarkerFillPlacement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMMarkerPlacementPolygonCenter 

|Property | Type | Description | 
|---------|--------|--------|
| method | [enumeration PlacementPolygonCenterMethod](CIMSymbols.md#enumeration-placementpolygoncentermethod) | The method used to determine the polygon center. 
| offsetX | double | The value which offsets the marker horizontally from the center. 
| offsetY | double | The value which offsets the marker vertically from the center. 
| clipAtBoundary | boolean | A value indicating whether the marker should be clipped if it extends pasts the boundary of the polygon. 





### Enumeration: MarkerPlacementType
#### Marker placement types. 

|Property | Value | Description | 
|---------|--------|--------|
| InsidePolygon| 0| Place inside the polygon. 
| PolygonCenter| 1| Place inside the polygon at the center. 
| RandomlyInsidePolygon| 2| Place randomly inside the polygon. 



### Enumeration: MaterialMode
#### Material modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Tint| 0| Tint materials and textures with color property. 
| Replace| 1| Replace materials and textures with color property. 
| Multiply| 2| Multiply materials and textures with color property. 




## CIMMaterialProperties
#### Represents material properties. 


### CIMMaterialProperties 

|Property | Type | Description | 
|---------|--------|--------|
| specularColor | [Color](Types.md#color) | The specular color. 
| shininess | float | The shininess. 
| externalColorMixMode | [enumeration ExternalColorMixMode](CIMSymbols.md#enumeration-externalcolormixmode) | How this material combines with externally defined colors. 






## CIMMaterialSymbolLayer
#### Represents a material which defines how the multipatch or mesh is drawn. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMMaterialSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| color | [Color](Types.md#color) | The material color. 
| materialMode | [enumeration MaterialMode](CIMSymbols.md#enumeration-materialmode) | The mode in which the material is applied. 






## CIMMeshSymbol
#### Represents a mesh symbol which is used to draw multipatch features or mesh features. 


### CIMSymbol 

|Property | Type | Description | 
|---------|--------|--------|


### CIMMultiLayerSymbol 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | The geometric effects that are applied to the symbol. 
| symbolLayers | [[CIMSymbolLayer]](Types.md#cimsymbollayer) | The symbol layers. Symbol layers are the components that make up a symbol. A symbol layer is represented by a stroke, fill, marker, or procedural symbol layer. 
| thumbnailURI | string | The representative image of the symbol. 
| useRealWorldSymbolSizes | boolean | A value indicating whether the symbol size properties are rendered using real world units or page units. When set to true the symbol will draw using real world units (e.g. meters). 


### CIMMeshSymbol 

|Property | Type | Description | 
|---------|--------|--------|






## CIMObjectMarker3D
#### Represents a marker symbol for 3D objects. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMMarker 

|Property | Type | Description | 
|---------|--------|--------|
| anchorPoint | [Point](ExternalReferences.md#point) | The specified location where all transformation property operations originate. 
| anchorPointUnits | [enumeration SymbolUnits](CIMSymbols.md#enumeration-symbolunits) | A value which specifies if the anchor point location is considered a percentage of the size or as an absolute distance. 
| angleX | double | The angle the marker is rotated around the X axis. This type of rotation is also referred to as tilt and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Tilt. 
| angleY | double | The angle the marker is rotated around the Y axis. This type of rotation is also referred to as roll and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Roll. 
| dominantSizeAxis3D | [enumeration DominantSizeAxis](CIMEnumerations.md#enumeration-dominantsizeaxis) | Which axis is considered as the Size in 3D. Only applicable when the marker layer is a 3DShapeMarker. 
| offsetX | double | The value the marker is moved along the X axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetY | double | The value the marker is moved along the Y axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetZ | double | The value the marker is moved along the Z axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| rotateClockwise | boolean | A value indicating whether the rotation is applied clockwise or counterclockwise to the marker layer. 
| rotation | double | The angle that the marker is rotated around the anchor point, in degrees. 
| size | double | The height of the marker. Modifying Size changes the marker's height to the specified size and the width is updated proportionally. 
| billboardMode3D | [enumeration BillboardMode](CIMEnumerations.md#enumeration-billboardmode) | The billboard mode of the marker. 
| markerPlacement | [MarkerPlacement](Types.md#markerplacement) | Marker placements which determine how markers are placed along a line or within a polygon. 


### CIMObjectMarker3D 

|Property | Type | Description | 
|---------|--------|--------|
| modelURI | string | The URI of the binary reference containing the "web resource". 
| width | double | The marker width. 
| depth | double | The marker depth. 
| tintColor | [Color](Types.md#color) | The color which defines the color that is applied to the marker. 
| isRestricted | boolean | A value indicating whether the model can be exported. 
| thumbnail | string | The representative image of the marker. 
| useAnchorPoint | boolean | A value indicating whether or not to ignore the marker anchor point and insert the model directly at the data point. 
| LODs | [[CIMObjectMarker3DLOD]](CIMSymbols.md#cimobjectmarker3dlod) | The array of levels of detail. 






## CIMObjectMarker3DLOD
#### Represents a level of detail of an object marker 3D. 


### CIMObjectMarker3DLOD 

|Property | Type | Description | 
|---------|--------|--------|
| faceCount | long | The total number of triangles in the geometry of this level of detail. 
| modelURI | string | The URI of the binary reference containing the "web resource" for this level of detail. 






## CIMPictureFill
#### Represents a picture fill which fills polygonal geometry with a picture. Supported file types are .bmp, .jpg, .png, and .gif. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMFill 

|Property | Type | Description | 
|---------|--------|--------|


### CIMPictureFill 

|Property | Type | Description | 
|---------|--------|--------|
| URL | string | The URL of the image. Typically a base64 encoded image. 
| offsetX | double | The distance that the image is offset in the horizontal direction. 
| offsetY | double | The distance that the image is offset in the vertical direction. 
| rotation | double | Angle of the image within the fill. 
| scaleX | double | The width of the symbol without changing the height (or depth in 3D), as a ratio. 
| height | double | The height of the image. 
| textureFilter | [enumeration TextureFilter](CIMSymbols.md#enumeration-texturefilter) | How the image is resampled. 
| colorSubstitutions | [[CIMColorSubstitution]](CIMSymbols.md#cimcolorsubstitution) | The color substitutions which allows colors in the image to be substituted with a different color. 
| tintColor | [Color](Types.md#color) | The color that is applied as a tint to the image. The color is applied to the whole image. When the tint is set to white the image appears with its native colors. 






## CIMPictureMarker
#### Represents a picture marker created from a raster (bitmapped) image file. The image can have color substitutions to replace one or more colors in the image or it can have a tint applied to the whole image depending on the picture type. Supported formats are .bmp, .jpg, .png, and .gif. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMMarker 

|Property | Type | Description | 
|---------|--------|--------|
| anchorPoint | [Point](ExternalReferences.md#point) | The specified location where all transformation property operations originate. 
| anchorPointUnits | [enumeration SymbolUnits](CIMSymbols.md#enumeration-symbolunits) | A value which specifies if the anchor point location is considered a percentage of the size or as an absolute distance. 
| angleX | double | The angle the marker is rotated around the X axis. This type of rotation is also referred to as tilt and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Tilt. 
| angleY | double | The angle the marker is rotated around the Y axis. This type of rotation is also referred to as roll and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Roll. 
| dominantSizeAxis3D | [enumeration DominantSizeAxis](CIMEnumerations.md#enumeration-dominantsizeaxis) | Which axis is considered as the Size in 3D. Only applicable when the marker layer is a 3DShapeMarker. 
| offsetX | double | The value the marker is moved along the X axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetY | double | The value the marker is moved along the Y axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetZ | double | The value the marker is moved along the Z axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| rotateClockwise | boolean | A value indicating whether the rotation is applied clockwise or counterclockwise to the marker layer. 
| rotation | double | The angle that the marker is rotated around the anchor point, in degrees. 
| size | double | The height of the marker. Modifying Size changes the marker's height to the specified size and the width is updated proportionally. 
| billboardMode3D | [enumeration BillboardMode](CIMEnumerations.md#enumeration-billboardmode) | The billboard mode of the marker. 
| markerPlacement | [MarkerPlacement](Types.md#markerplacement) | Marker placements which determine how markers are placed along a line or within a polygon. 


### CIMPictureMarker 

|Property | Type | Description | 
|---------|--------|--------|
| colorSubstitutions | [[CIMColorSubstitution]](CIMSymbols.md#cimcolorsubstitution) | The color substitutions for the picture. 
| depth3D | double | The depth of the image when drawn in 3D. 
| invertBackfaceTexture | boolean | A value indicating whether the image is right-reading when viewed from behind. 
| scaleX | double | The scale X which changes the width of the symbol without changing the height (or depth in 3D), as a ratio. 
| textureFilter | [enumeration TextureFilter](CIMSymbols.md#enumeration-texturefilter) | How the image is resampled. 
| tintColor | [Color](Types.md#color) | The color that is applied as a tint to the image. The color is applied to the whole image. When the tint is set to white the image appears with its native colors. 
| URL | string | The image that is used in the symbol layer. Typically a base64 encoded image. 
| verticalOrientation3D | boolean | A value indicating whether the marker stands upright as though locked in place. The marker can be viewed from all angles. 






## CIMPictureStroke
#### Represents a picture stroke which draws linear geometry with a repeating image file. Supported file types are .bmp, .jpg, .png, and .gif. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMStroke 

|Property | Type | Description | 
|---------|--------|--------|
| capStyle | [enumeration LineCapStyle](CIMSymbols.md#enumeration-linecapstyle) | How the stroke should draw at the ends of the geometries. 
| joinStyle | [enumeration LineJoinStyle](CIMSymbols.md#enumeration-linejoinstyle) | How the symbol is drawn at the stroke segment connections. 
| lineStyle3D | [enumeration Simple3DLineStyle](CIMSymbols.md#enumeration-simple3dlinestyle) | How strokes will be rendered in 3D. 
| miterLimit | double | The maximum 'sharpness' that is allowed for Miter joins. If the spike created by the miter join exceeds the miter limit times the width of the stroke, the sharp angle will be clipped and rendered with a bevel join. This property is only applied to the symbol layer when the JoinType is set to Miter. 
| width | double | The width of the stroke. 
| closeCaps3D | boolean | A value indicating whether to close caps when drawing them in 3D. When set to false, the caps are hollow. 


### CIMPictureStroke 

|Property | Type | Description | 
|---------|--------|--------|
| colorSubstitutions | [[CIMColorSubstitution]](CIMSymbols.md#cimcolorsubstitution) | The color substitutions for the picture. 
| textureFilter | [enumeration TextureFilter](CIMSymbols.md#enumeration-texturefilter) | How the image is resampled. 
| URL | string | The image that is used in the symbol layer. Typically a base64 encoded image. 
| tintColor | [Color](Types.md#color) | The color that is applied as a tint to the image. The color is applied to the whole image. When the tint is set to white the image appears with its native colors. 






## CIMPieChartMarker
#### Represents a pie chart marker which is a marker that draws numeric values arranged in a circle. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMMarker 

|Property | Type | Description | 
|---------|--------|--------|
| anchorPoint | [Point](ExternalReferences.md#point) | The specified location where all transformation property operations originate. 
| anchorPointUnits | [enumeration SymbolUnits](CIMSymbols.md#enumeration-symbolunits) | A value which specifies if the anchor point location is considered a percentage of the size or as an absolute distance. 
| angleX | double | The angle the marker is rotated around the X axis. This type of rotation is also referred to as tilt and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Tilt. 
| angleY | double | The angle the marker is rotated around the Y axis. This type of rotation is also referred to as roll and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Roll. 
| dominantSizeAxis3D | [enumeration DominantSizeAxis](CIMEnumerations.md#enumeration-dominantsizeaxis) | Which axis is considered as the Size in 3D. Only applicable when the marker layer is a 3DShapeMarker. 
| offsetX | double | The value the marker is moved along the X axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetY | double | The value the marker is moved along the Y axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetZ | double | The value the marker is moved along the Z axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| rotateClockwise | boolean | A value indicating whether the rotation is applied clockwise or counterclockwise to the marker layer. 
| rotation | double | The angle that the marker is rotated around the anchor point, in degrees. 
| size | double | The height of the marker. Modifying Size changes the marker's height to the specified size and the width is updated proportionally. 
| billboardMode3D | [enumeration BillboardMode](CIMEnumerations.md#enumeration-billboardmode) | The billboard mode of the marker. 
| markerPlacement | [MarkerPlacement](Types.md#markerplacement) | Marker placements which determine how markers are placed along a line or within a polygon. 


### CIMChartMarker 

|Property | Type | Description | 
|---------|--------|--------|
| display3D | boolean | A value indicating whether to draw the chart with a 3D perspective. 
| parts | [[CIMChartPart]](CIMSymbols.md#cimchartpart) | The individual components of the chart marker. 
| thickness3D | double | The thickness or depth of a chart. Only applied when Display3D is true. 
| tilt3D | double | The tilt (rotation around the X axis) of the chart. Only applied when Display3D is true. 


### CIMPieChartMarker 

|Property | Type | Description | 
|---------|--------|--------|
| clockwise | boolean | A value indicating whether the orientation of the wedges of the pie chart are clockwise or counterclockwise. 
| showOutline | boolean | A value indicating whether or not to show the outline symbol. 
| outlineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol) | The line symbol that is applied to outline of the whole pie chart. 





### Enumeration: PlacementClip
#### Options for how the markers should be clipped at the polygon boundary. 

|Property | Value | Description | 
|---------|--------|--------|
| ClipAtBoundary| 0| Markers are clipped at the boundary of the polygon. 
| RemoveIfCenterOutsideBoundary| 1| Markers are not drawn if their center falls outside of the polygon. 
| DoNotTouchBoundary| 2| Markers are not drawn if they touch the boundary of the polygon. 
| DoNotClip| 3| Markers are not clipped and may extend past the boundary of the polygon. 



### Enumeration: PlacementEndings
#### Options for how markers are placed at control points. 

|Property | Value | Description | 
|---------|--------|--------|
| NoConstraint| 0| No constraint on how the markers are placed. 
| WithMarkers| 1| A marker is placed at the control point. 
| WithFullGap| 2| A space equal to the placement template will be placed at the control point. 
| WithHalfGap| 3| A space equal to half the placement template will be placed at the control point. 
| Custom| 4| Will fit the pattern to the length of the features by adjusting the gaps slightly. 



### Enumeration: PlacementGridType
#### Options for how markers are placed in a uniform grid or randomly. 

|Property | Value | Description | 
|---------|--------|--------|
| Fixed| 0| Markers are placed on a uniform grid. 
| Random| 1| Markers are placed randomly in the polygon. 
| RandomFixedQuantity| 2| Markers are placed randomly with a fixed quantity (dot density). 



### Enumeration: PlacementOnLineRelativeTo
#### Options for the location on a line where a marker will be placed. 

|Property | Value | Description | 
|---------|--------|--------|
| LineMiddle| 0| Marker is placed in the middle of the line. 
| LineBeginning| 1| Marker is placed at the beginning of the line. 
| LineEnd| 2| Marker is placed at the end of the line. 
| SegmentMidpoint| 3| Marker is at the midpoint of each segment in a line feature. 



### Enumeration: PlacementPolygonCenterMethod
#### Options for how a single marker will be placed within the polygon. 

|Property | Value | Description | 
|---------|--------|--------|
| OnPolygon| 0| Place on the polygon. 
| CenterOfMass| 1| The centroid of the polygon is used. 
| BoundingBoxCenter| 2| The bounding box of the polygon is used. 



### Enumeration: PlacementRandomlyAlongLineRandomization
#### Options for the amount of randomness to be used for the size and rotation of the markers on the line. 

|Property | Value | Description | 
|---------|--------|--------|
| Low| 0| A low amount of randomness is applied 
| Medium| 1| A medium amount of randomness is applied 
| High| 2| A high amount of randomness is applied 



### Enumeration: PlacementStepPosition
#### Options for the placement step position. 

|Property | Value | Description | 
|---------|--------|--------|
| MarkerCenter| 0| The marker center. 
| MarkerBounds| 1| The marker bounds. 




## CIMPointSymbol
#### Represents a point symbol used to draw point features and point graphics. 


### CIMSymbol 

|Property | Type | Description | 
|---------|--------|--------|


### CIMMultiLayerSymbol 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | The geometric effects that are applied to the symbol. 
| symbolLayers | [[CIMSymbolLayer]](Types.md#cimsymbollayer) | The symbol layers. Symbol layers are the components that make up a symbol. A symbol layer is represented by a stroke, fill, marker, or procedural symbol layer. 
| thumbnailURI | string | The representative image of the symbol. 
| useRealWorldSymbolSizes | boolean | A value indicating whether the symbol size properties are rendered using real world units or page units. When set to true the symbol will draw using real world units (e.g. meters). 


### CIMPointSymbol 

|Property | Type | Description | 
|---------|--------|--------|
| callout | [Callout](Types.md#callout) | The callout of the point symbol. 
| haloSize | double | The size of the halo that extends beyond the symbol shape. 
| haloSymbol | [CIMPolygonSymbol](CIMSymbols.md#cimpolygonsymbol) | The polygon symbol that is used to draw the halo for a point symbol. 
| primitiveName | string | The primitive name. 
| scaleX | double | The X scale which changes the width of the symbol without changing the height (or depth in 3D), as a ratio. 
| symbol3DProperties | [CIM3DSymbolProperties](CIMSymbols.md#cim3dsymbolproperties) | The collection of symbol properties that apply when the symbol is used in a 3D context. 
| angle | double | The amount of variation applied to the symbol, measured in degrees, propagated cumulatively to all marker symbols. 
| angleAlignment | [enumeration AngleAlignment](CIMSymbols.md#enumeration-anglealignment) | Whether point symbols align to the map or to the display when a rotation is applied to the map. 






## CIMPointSymbolCallout
#### Represents a point symbol callout which draws a point symbol as the background and a line symbol for leaders. Often used for highway shields. 


### CIMCallout 

|Property | Type | Description | 
|---------|--------|--------|
| leaderTolerance | double | The leader tolerance which is the closest distance (in points) to the text the anchor point can be for the callout to draw. 
| leaderOffset | double | The leader offset which is an offset value defining the distance (in points) between the anchor point and the beginning of the drawn leader. 


### CIMLineCallout 

|Property | Type | Description | 
|---------|--------|--------|
| leaderLineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol) | The line symbol to draw leaders with. 
| gap | double | The gap (in points) between the point symbol and the beginning of the leader line. 
| lineStyle | [enumeration LeaderLineStyle](CIMSymbols.md#enumeration-leaderlinestyle) | The style of line to generate when a Point leader is drawn defined by an enumeration value. Line leaders will always be drawn with their own geometry. 


### CIMPointSymbolCallout 

|Property | Type | Description | 
|---------|--------|--------|
| pointSymbol | [CIMPointSymbol](CIMSymbols.md#cimpointsymbol) | The symbol that will be drawn as the background behind the text. The most common use case for this type of symbol is a highway shield. When drawing a highway shield this property will be the shield itself without numbers. 
| backgroundScale | [enumeration PointSymbolCalloutScale](CIMSymbols.md#enumeration-pointsymbolcalloutscale) | An enumeration value that defines how the background is scaled to fit the dimensions of the symbol. 





### Enumeration: PointSymbolCalloutScale
#### An enumeration that defines how the background point symbol is scaled to fit the dimensions of the text. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No scaling. 
| PropUniform| 1| Uniform scaling. 
| PropNonuniform| 2| Non-uniform scaling. 
| DifUniform| 3| Uniform scaling. 
| DifNonuniform| 4| Non-uniform scaling. 




## CIMPolygonSymbol
#### Represents a polygon symbol which is used to draw polygon features or polygon graphics. 


### CIMSymbol 

|Property | Type | Description | 
|---------|--------|--------|


### CIMMultiLayerSymbol 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | The geometric effects that are applied to the symbol. 
| symbolLayers | [[CIMSymbolLayer]](Types.md#cimsymbollayer) | The symbol layers. Symbol layers are the components that make up a symbol. A symbol layer is represented by a stroke, fill, marker, or procedural symbol layer. 
| thumbnailURI | string | The representative image of the symbol. 
| useRealWorldSymbolSizes | boolean | A value indicating whether the symbol size properties are rendered using real world units or page units. When set to true the symbol will draw using real world units (e.g. meters). 


### CIMPolygonSymbol 

|Property | Type | Description | 
|---------|--------|--------|






## CIMProceduralSymbolLayer
#### Represents a procedural symbol layer which defines rendering using script-based logic to construct complex 3D objects and textures from simple geometries. Properties of the symbol are derived from a rule package (.rpk file). 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMProceduralSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| attributes | [[CIMCGAAttribute]](CIMSymbols.md#cimcgaattribute) | The symbol attributes as specified by the CGA code in the rule package. 
| rulePackage | string | The URI of the referenced rule package file. 
| rulePackageName | string | The name of the package displayed in the user interface. 






## CIMShapeVertex
#### Represents a shape vertex. Each Vertex in a 3DShapeGraphic is represented by three points, contained in a ShapeVertex. The first point is the actual position of the Vertex. The second represents the normalized vector that describes the orientation of the point. The last point is optional - it defines the coordinates of the texture that correspond with this point in the shape. In this case only x and y are used as the traditional texture coordinates S and T. 


### CIMShapeVertex 

|Property | Type | Description | 
|---------|--------|--------|
| position | [Point](ExternalReferences.md#point) | The position. 
| normalVector | [Point](ExternalReferences.md#point) | The normal vector. 
| textureCoordinate | [Point](ExternalReferences.md#point) | The texture coordinate. 






## CIMShapeVertices
#### Represents shape vertices. 


### CIMShapeVertices 

|Property | Type | Description | 
|---------|--------|--------|
| indices | long | The indices. 
| shapes | string | The shape. 





### Enumeration: Simple3DLineStyle
#### Simple 3D line styles which define how strokes will be rendered in 3D. 

|Property | Value | Description | 
|---------|--------|--------|
| Tube| 0| Stroke draws as a tube where the width determines the diameter of the tube. 
| Strip| 1| Stroke draws flat upon the surface. 
| Wall| 2| Stroke is vertically oriented where Width determines the height of the wall. 




## CIMSimpleLineCallout
#### Represents a simple line callout for drawing basic leader lines. 


### CIMCallout 

|Property | Type | Description | 
|---------|--------|--------|
| leaderTolerance | double | The leader tolerance which is the closest distance (in points) to the text the anchor point can be for the callout to draw. 
| leaderOffset | double | The leader offset which is an offset value defining the distance (in points) between the anchor point and the beginning of the drawn leader. 


### CIMSimpleLineCallout 

|Property | Type | Description | 
|---------|--------|--------|
| lineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol) | The line symbol used to draw leader lines. 
| autoSnap | boolean | A value indicating whether or not to auto-snap the line leaders to the text. 





### Enumeration: SizeVariationMethod
#### Size variation methods which define the order in which the change of size in the markers should occur. 

|Property | Value | Description | 
|---------|--------|--------|
| Random| 0| Change in size is applied randomly. 
| Increasing| 1| Markers are drawn with a pattern where the markers increase in size. 
| Decreasing| 2| Markers are drawn in a pattern where the markers decrease in size. 
| IncreasingThenDecreasing| 3| Markers are drawn in a pattern where the size increase and then decrease. 




## CIMSolidFill
#### Represents a solid fill which fills polygonal geometry with a single solid color. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMFill 

|Property | Type | Description | 
|---------|--------|--------|


### CIMSolidFill 

|Property | Type | Description | 
|---------|--------|--------|
| color | [Color](Types.md#color) | The color that is applied to the fill. 






## CIMSolidMeshEdge
#### Represents a stroke drawn at specified edges of a mesh using solid color. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMMeshEdge 

|Property | Type | Description | 
|---------|--------|--------|
| color | [Color](Types.md#color) | Color of the mesh stroke. 






## CIMSolidStroke
#### Represents a solid stroke which draws linear geometry with a single solid color. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMStroke 

|Property | Type | Description | 
|---------|--------|--------|
| capStyle | [enumeration LineCapStyle](CIMSymbols.md#enumeration-linecapstyle) | How the stroke should draw at the ends of the geometries. 
| joinStyle | [enumeration LineJoinStyle](CIMSymbols.md#enumeration-linejoinstyle) | How the symbol is drawn at the stroke segment connections. 
| lineStyle3D | [enumeration Simple3DLineStyle](CIMSymbols.md#enumeration-simple3dlinestyle) | How strokes will be rendered in 3D. 
| miterLimit | double | The maximum 'sharpness' that is allowed for Miter joins. If the spike created by the miter join exceeds the miter limit times the width of the stroke, the sharp angle will be clipped and rendered with a bevel join. This property is only applied to the symbol layer when the JoinType is set to Miter. 
| width | double | The width of the stroke. 
| closeCaps3D | boolean | A value indicating whether to close caps when drawing them in 3D. When set to false, the caps are hollow. 


### CIMSolidStroke 

|Property | Type | Description | 
|---------|--------|--------|
| color | [Color](Types.md#color) | The color that is applied to the stroke. 






## CIMStackedBarChartMarker
#### Represents a stacked bar chart marker which is a chart made of vertical stacked bars displaying values. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMMarker 

|Property | Type | Description | 
|---------|--------|--------|
| anchorPoint | [Point](ExternalReferences.md#point) | The specified location where all transformation property operations originate. 
| anchorPointUnits | [enumeration SymbolUnits](CIMSymbols.md#enumeration-symbolunits) | A value which specifies if the anchor point location is considered a percentage of the size or as an absolute distance. 
| angleX | double | The angle the marker is rotated around the X axis. This type of rotation is also referred to as tilt and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Tilt. 
| angleY | double | The angle the marker is rotated around the Y axis. This type of rotation is also referred to as roll and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Roll. 
| dominantSizeAxis3D | [enumeration DominantSizeAxis](CIMEnumerations.md#enumeration-dominantsizeaxis) | Which axis is considered as the Size in 3D. Only applicable when the marker layer is a 3DShapeMarker. 
| offsetX | double | The value the marker is moved along the X axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetY | double | The value the marker is moved along the Y axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetZ | double | The value the marker is moved along the Z axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| rotateClockwise | boolean | A value indicating whether the rotation is applied clockwise or counterclockwise to the marker layer. 
| rotation | double | The angle that the marker is rotated around the anchor point, in degrees. 
| size | double | The height of the marker. Modifying Size changes the marker's height to the specified size and the width is updated proportionally. 
| billboardMode3D | [enumeration BillboardMode](CIMEnumerations.md#enumeration-billboardmode) | The billboard mode of the marker. 
| markerPlacement | [MarkerPlacement](Types.md#markerplacement) | Marker placements which determine how markers are placed along a line or within a polygon. 


### CIMChartMarker 

|Property | Type | Description | 
|---------|--------|--------|
| display3D | boolean | A value indicating whether to draw the chart with a 3D perspective. 
| parts | [[CIMChartPart]](CIMSymbols.md#cimchartpart) | The individual components of the chart marker. 
| thickness3D | double | The thickness or depth of a chart. Only applied when Display3D is true. 
| tilt3D | double | The tilt (rotation around the X axis) of the chart. Only applied when Display3D is true. 


### CIMStackedBarChartMarker 

|Property | Type | Description | 
|---------|--------|--------|
| fixedLength | boolean | A value indicating whether this chart is a fixed length. 
| showOutline | boolean | A value indicating whether or not to show the outline symbol. 
| outlineSymbol | [CIMLineSymbol](CIMSymbols.md#cimlinesymbol) | The outline symbol. 
| verticalBar | boolean | A value indicating whether this chart has a vertical bar. 
| width | double | The width. 





### Enumeration: SymbolUnits
#### Symbol unit types. 

|Property | Value | Description | 
|---------|--------|--------|
| Relative| 0| Relative units. 
| Absolute| 1| Absolute units. 



### Enumeration: TextCase
#### The letter case used to draw text. 

|Property | Value | Description | 
|---------|--------|--------|
| Normal| 0| Text is proper/mixed case. 
| LowerCase| 1| Text is all lower case. 
| Allcaps| 2| Text is all upper case. 




## CIMTextMargin
#### Represents a text margin which defines the margin to apply around text. 


### CIMTextMargin 

|Property | Type | Description | 
|---------|--------|--------|
| left | double | The left margin. 
| right | double | The right margin. 
| top | double | The top margin. 
| bottom | double | The bottom margin. 





### Enumeration: TextReadingDirection
#### Text reading directions. 

|Property | Value | Description | 
|---------|--------|--------|
| LTR| 0| Text is drawn from left-to-right. 
| RTL| 1| Text is drawn from right-to-left. 




## CIMTextSymbol
#### Represents a text symbol which is used to draw text graphics, bleeds, and annotation. Text symbols do not contain any symbol layers but can have callouts. 


### CIMSymbol 

|Property | Type | Description | 
|---------|--------|--------|


### CIMTextSymbol 

|Property | Type | Description | 
|---------|--------|--------|
| angle | double | The amount of rotation applied to the text symbol, measured in degrees, around the geometry. 
| angleX | double | The amount of rotation of the text symbol around the X axis, measured in degrees, around the geometry. This type of rotation is also referred to as tilt. It is applied in 3D. 
| angleY | double | The amount of rotation of the text symbol around the Y axis, measured in degrees, around the geometry. This type of rotation is also referred to as roll. It is applied in 3D. 
| blockProgression | [enumeration BlockProgression](CIMSymbols.md#enumeration-blockprogression) | The direction in which multi-line text is stacked. 
| callout | [Callout](Types.md#callout) | The callout or background of the text with optional leader lines. 
| compatibilityMode | boolean | A value indicating whether to draw the text in a fashion compatible with ArcMap. 
| countryISO | string | The ISO code for the base country of the text. 
| depth3D | double | The depth of the glyph when drawn in 3D. This is an extrusion of the characters of the text in the Z axis. 
| drawGlyphsAsGeometry | boolean | A value indicating whether fonts that are drawn as rasters at some scales to draw as vectors instead. 
| drawSoftHyphen | boolean | A value indicating whether soft hyphens should be drawn. Soft hyphens are invisible markers that indicate where a hyphenated break is allowed within the text. They are only drawn if there is word wrapping at the end of a line. 
| extrapolateBaselines | boolean | A value indicating whether the baseline of the text geometry should be expanded in the same manner as the existing geometry if the text extends beyond the baseline. 
| flipAngle | double | The angle (in degrees from vertical) at which point rotated text is flipped (mirrored) in place. 
| fontEffects | [enumeration FontEffects](CIMSymbols.md#enumeration-fonteffects) | Whether the text is drawn as subscript or superscript. 
| fontEncoding | [enumeration FontEncoding](CIMSymbols.md#enumeration-fontencoding) | The font encoding. 
| fontFamilyName | string | The font family name of the font. e.g. Comic Sans. 
| fontStyleName | string | The style name for the font family. e.g. Regular, Bold, or Italic. 
| fontType | [enumeration FontType](CIMSymbols.md#enumeration-fonttype) | The type of font that the font family/style name reference. 
| glyphRotation | double | An additional rotation that is applied to the individual glyphs contained in the text. This is applied to the individual glyphs whereas Angle, AngleX and AngleY are affect how the entire text string is oriented. 
| haloSize | double | The size of the halo that extends beyond the symbol shape. 
| haloSymbol | [CIMPolygonSymbol](CIMSymbols.md#cimpolygonsymbol) | The polygon symbol that is used to draw the halo for a text symbol. 
| height | double | The size of the text in points. 
| hinting | [enumeration GlyphHinting](CIMSymbols.md#enumeration-glyphhinting) | If hinting from the font is used for text rendering. Hinting is information included with most fonts to effectively fit the vector glyphs of the font into the raster grid onto which they are displayed. 
| horizontalAlignment | [enumeration HorizontalAlignment](CIMSymbols.md#enumeration-horizontalalignment) | The alignment type used to align the text to the geometry horizontally. Affects which side of a point geometry the point text is drawn or which end of a line it is drawn close to. Commonly used to define how stacked text appears. 
| indentAfter | double | How many points to indent the text back from the end of the baseline. 
| indentBefore | double | How many points to indent the text from the beginning of the baseline. 
| indentFirstLine | double | How many points to indent the text from the beginning of the baseline for the first line only. 
| kerning | boolean | A value indicating whether the text is drawn with metric kerning, which adjusts the spacing between individual letter forms. 
| languageISO | string | Whether the ISO code for the base language of the text. 
| letterSpacing | double | The additional spacing that is added to each glyph beyond what is defined by its character box in the font. Value indicates the percentage of a glyph's width. Also known as tracking. 
| letterWidth | double | The width that is added to each glyph beyond what is defined by its character box in its font. This is a percentage of the original glyph. 
| ligatures | boolean | A value indicating whether text is to be drawn with ligatures, which occur when two or more letters or portions of letters are joined to form a single glyph. 
| lineGap | double | The spacing between lines of text. This is also known as leading or line spacing. 
| lineGapType | [enumeration LineGapType](CIMSymbols.md#enumeration-linegaptype) | The type of line gap that is applied. 
| offsetX | double | The X offset. 
| offsetY | double | The Y offset. 
| offsetZ | double | The Z offset. 
| shadowColor | [Color](Types.md#color) | The color of the shadow that is defined for the text symbol. The shadow is drawn as an offset copy of the text. 
| shadowOffsetX | double | The shadow offset from the text symbol in the horizontal direction. If X and Y are zero, no shadow is drawn. 
| shadowOffsetY | double | The shadow offset from the text symbol in the vertical direction. If X and Y are zero, no shadow is drawn. 
| smallCaps | boolean | A value indicating whether the text should be drawn as Small Capitals, where lower case text is converted to small caps and upper case text is left as upper case. 
| strikethrough | boolean | A value indicating whether to draw the text with a strike through it. 
| symbol | [CIMPolygonSymbol](CIMSymbols.md#cimpolygonsymbol) | The polygon symbol that is used to draw the glyphs of the text. 
| symbol3DProperties | [CIM3DSymbolProperties](CIMSymbols.md#cim3dsymbolproperties) | The collection of properties that are applied to the text symbol only in a 3D context. 
| textCase | [enumeration TextCase](CIMSymbols.md#enumeration-textcase) | The letter case used to draw the text. 
| textDirection | [enumeration TextReadingDirection](CIMSymbols.md#enumeration-textreadingdirection) | The base text direction to draw the text. 
| underline | boolean | A value indicating whether to draw the text with an underline. 
| verticalAlignment | [enumeration VerticalAlignment](CIMSymbols.md#enumeration-verticalalignment) | The vertical alignment of the text. 
| verticalGlyphOrientation | [enumeration VerticalGlyphOrientation](CIMSymbols.md#enumeration-verticalglyphorientation) | The orientation for the non-vertical text in a vertical layout. For example, an English fragment in a Japanese text. 
| wordSpacing | double | The additional spacing that is added to between the words of the text string. 100% indicates that regular spacing is used. 
| billboardMode3D | [enumeration BillboardMode](CIMEnumerations.md#enumeration-billboardmode) | The billboard mode of the text symbol. 
| overprint | boolean | A value indicating whether or not the symbol should overprint in press printing. 





### Enumeration: TextureFilter
#### Texture filter types. 

|Property | Value | Description | 
|---------|--------|--------|
| Draft| 0| Low draft quality. 
| Picture| 1| Higher quality, recommended for pictures. 
| Text| 2| Higher quality, recommended when it is important to preserve edges for zoomed in images. 




## CIMVectorMarker
#### Represents a vector marker which can represent vector graphics. It's constructed from MarkerGraphics which are geometries and symbols used as building blocks for the marker. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMMarker 

|Property | Type | Description | 
|---------|--------|--------|
| anchorPoint | [Point](ExternalReferences.md#point) | The specified location where all transformation property operations originate. 
| anchorPointUnits | [enumeration SymbolUnits](CIMSymbols.md#enumeration-symbolunits) | A value which specifies if the anchor point location is considered a percentage of the size or as an absolute distance. 
| angleX | double | The angle the marker is rotated around the X axis. This type of rotation is also referred to as tilt and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Tilt. 
| angleY | double | The angle the marker is rotated around the Y axis. This type of rotation is also referred to as roll and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Roll. 
| dominantSizeAxis3D | [enumeration DominantSizeAxis](CIMEnumerations.md#enumeration-dominantsizeaxis) | Which axis is considered as the Size in 3D. Only applicable when the marker layer is a 3DShapeMarker. 
| offsetX | double | The value the marker is moved along the X axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetY | double | The value the marker is moved along the Y axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetZ | double | The value the marker is moved along the Z axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| rotateClockwise | boolean | A value indicating whether the rotation is applied clockwise or counterclockwise to the marker layer. 
| rotation | double | The angle that the marker is rotated around the anchor point, in degrees. 
| size | double | The height of the marker. Modifying Size changes the marker's height to the specified size and the width is updated proportionally. 
| billboardMode3D | [enumeration BillboardMode](CIMEnumerations.md#enumeration-billboardmode) | The billboard mode of the marker. 
| markerPlacement | [MarkerPlacement](Types.md#markerplacement) | Marker placements which determine how markers are placed along a line or within a polygon. 


### CIMVectorMarker 

|Property | Type | Description | 
|---------|--------|--------|
| depth3D | double | The depth of the marker when drawn in 3D. 
| frame | [Envelope](ExternalReferences.md#envelope) | The outer boundary of the entire vector marker. 
| markerGraphics | [[CIMMarkerGraphic]](CIMSymbols.md#cimmarkergraphic) | The vector graphics that define the shape of the marker. 
| verticalOrientation3D | boolean | A value indicating whether the marker stands upright as though locked in place. The marker can be viewed from all angles. 
| scaleSymbolsProportionally | boolean | A value indicating whether the strokes and or fills of a marker are scaled proportionally when the symbol size is changed. When enabled, the strokes for the outline or fill of the polygon symbol used to draw the marker will be scaled proportionally with changes to the symbol size. If this property is not enabled, then the stroke will draw with the specified width regardless of the marker size. 
| respectFrame | boolean | A value indicating whether the frame of the vector marker should be honored when drawing the marker. 
| clippingPath | [CIMClippingPath](CIMSymbols.md#cimclippingpath) | A clipping path for the vector marker graphics. 





### Enumeration: VerticalAlignment
#### Vertical alignment types. 

|Property | Value | Description | 
|---------|--------|--------|
| Top| 0| Top of the highest ascender in the text symbol is used to align the text. 
| Center| 1| Text is centered on the geometry. 
| Baseline| 2| Text is aligned so that the geometry lines up with the baseline of the text symbol. Descenders will go past the baseline. 
| Bottom| 3| Bottom of the lowest descender is used to align the text. 



### Enumeration: VerticalGlyphOrientation
#### Vertical glyph orientation. 

|Property | Value | Description | 
|---------|--------|--------|
| Right| 0| Align right. 
| Upright| 1| Align upright. 




## CIMWaterFill
#### Represents a water fill which fills polygonal geometry with animated water. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMFill 

|Property | Type | Description | 
|---------|--------|--------|


### CIMWaterFill 

|Property | Type | Description | 
|---------|--------|--------|
| color | [Color](Types.md#color) | The intrinsic color of the water. 
| waveStrength | [enumeration WaveStrength](CIMSymbols.md#enumeration-wavestrength) | Strength of the waves. This property along with waterbody size are the parameters which drive the wave appearance. 
| waterbodySize | [enumeration WaterbodySize](CIMSymbols.md#enumeration-waterbodysize) | The waterbody size allowing for a range of sizes from small pools to oceans. This property along with wave strength are the parameters which drive the wave appearance. 
| waveHasDirection | boolean | A value indicating whether the waves are directionless (false), or if they have a dominant direction (true). 
| waveDirection | double | The azimuthal bearing for direction of the waves. Only has effect when WasHasDirection is true. 





### Enumeration: WaterbodySize
#### Waterbody size. 

|Property | Value | Description | 
|---------|--------|--------|
| Small| 0| Small water body. 
| Medium| 1| Medium water body. 
| Large| 2| Large water body. 



### Enumeration: WaveStrength
#### Strength of waves. 

|Property | Value | Description | 
|---------|--------|--------|
| Calm| 0| Calm glassy water with no waves. 
| Rippled| 1| Rippled water. 
| Slight| 2| Slightly wavy water. 
| Moderate| 3| Moderately wavy water. 




## CIMglTFMarker3D
#### Represents a marker symbol for 3D objects. 


### CIMSymbolLayer 

|Property | Type | Description | 
|---------|--------|--------|
| effects | [[CIMGeometricEffect]](Types.md#cimgeometriceffect) | Whether the geometric effects that are applied to the symbol layer. Effects dynamically alter the feature geometry when the symbology is applied. Multiple effects applied to a symbol layer are rendered sequentially. 
| enable | boolean | A value indicating whether the symbol layer is visible. The symbol layer draws only when enabled. Currently, an invisible layer is not considered in any transformations when in a 3D context. 
| name | string | The internal name of the symbol layer used for symbol level drawing. 
| colorLocked | boolean | A value indicating whether the color set at the basic properties level is applied to the symbol layer. If the symbol layer is color locked then changes made to the color in the basic properties will not be applied to the symbol layer. 
| primitiveName | string | The primitive name. 
| overprint | boolean | A value indicating whether or not the symbol layer should overprint in press printing. 


### CIMMarker 

|Property | Type | Description | 
|---------|--------|--------|
| anchorPoint | [Point](ExternalReferences.md#point) | The specified location where all transformation property operations originate. 
| anchorPointUnits | [enumeration SymbolUnits](CIMSymbols.md#enumeration-symbolunits) | A value which specifies if the anchor point location is considered a percentage of the size or as an absolute distance. 
| angleX | double | The angle the marker is rotated around the X axis. This type of rotation is also referred to as tilt and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Tilt. 
| angleY | double | The angle the marker is rotated around the Y axis. This type of rotation is also referred to as roll and is only applied in 3D. The order of how this is applied with respect to other rotations depends on the RotationOrder3D. The name in the user interface is Roll. 
| dominantSizeAxis3D | [enumeration DominantSizeAxis](CIMEnumerations.md#enumeration-dominantsizeaxis) | Which axis is considered as the Size in 3D. Only applicable when the marker layer is a 3DShapeMarker. 
| offsetX | double | The value the marker is moved along the X axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetY | double | The value the marker is moved along the Y axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| offsetZ | double | The value the marker is moved along the Z axis from the anchor point. This is applied after all rotation, as opposed to anchor point which is applied before the rotation. 
| rotateClockwise | boolean | A value indicating whether the rotation is applied clockwise or counterclockwise to the marker layer. 
| rotation | double | The angle that the marker is rotated around the anchor point, in degrees. 
| size | double | The height of the marker. Modifying Size changes the marker's height to the specified size and the width is updated proportionally. 
| billboardMode3D | [enumeration BillboardMode](CIMEnumerations.md#enumeration-billboardmode) | The billboard mode of the marker. 
| markerPlacement | [MarkerPlacement](Types.md#markerplacement) | Marker placements which determine how markers are placed along a line or within a polygon. 


### CIMglTFMarker3D 

|Property | Type | Description | 
|---------|--------|--------|
| modelURI | string | The URI of the binary reference containing the GLTF or GLB which contains the node structure. 
| additionalModelURIs | [string] | The URIs of additional binary references used by the model. 
| width | double | The marker width. 
| depth | double | The marker depth. 
| tintColor | [Color](Types.md#color) | The color which defines the color that is applied to the marker. 
| isRestricted | boolean | A value indicating whether the model can be exported. 
| thumbnail | string | The representative image of the marker. 
| useAnchorPoint | boolean | A value indicating whether or not to ignore the marker anchor point and insert the model directly at the data point. 



