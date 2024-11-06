

### Enumeration: AltitudeMode
#### Relative to the ground. 

|Property | Value | Description | 
|---------|--------|--------|
| ClampToGround| 0| Indicates to ignore an altitude specification and draw the graphic directly on the surface of the earth. 
| RelativeToGround| 1| Sets the altitude of the graphic relative to the actual ground elevation of a particular location. 
| Absolute| 2| Sets the altitude of the coordinate relative to sea level, regardless of the actual elevation of the terrain beneath the element. 



### Enumeration: AnimationTransition
#### Specifies the method of transition for a value in a keyframe. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| The keyframe value is ignored. 
| Linear| 1| Value changes at a constant (linear) rate to the end state. 
| Stepped| 2| Value switches to the end state at a specified point along the transition. 
| Hop| 3| Value increases, using a parabolic curve, beyond the end state before returning back to it. The height of the curve can be configured. 
| FixedArc| 4| Value changes along a tightly controlled curve to the end state. 
| AdjustableArc| 5| Value changes along a smooth curve to the end state. The tightness of the curve can be configured. 
| Hold| 6| Value remains constant, equaling the previous keyframe's value. 



### Enumeration: BaseElevationType
#### A list of base elevation types. 

|Property | Value | Description | 
|---------|--------|--------|
| Expression| 0| Elevation defined by an expression. 
| Surface| 1| Elevation defined by a surface. 
| Shape| 2| Elevation defined by a shape. 



### Enumeration: BillboardMode
#### A list of different billboard modes. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Not billboarded. 
| SignPost| 1| The symbol always faces toward the viewer as though spinning on a vertical signpost. Viewed from above, the symbol does not face you; you see the top of the symbol. 
| FaceNearPlane| 2| The symbol always faces the viewer directly, regardless of view angle. 



### Enumeration: ColorModel
#### Specifies color model used for maps and layouts. 

|Property | Value | Description | 
|---------|--------|--------|
| RGB| 0| The RGB (red, green, blue) color space. 
| CMYK| 1| The CMYK (cyan, magenta, yellow, black) color space. 



### Enumeration: ColorVisionDeficiencyType
#### Color vision deficiency types. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No color vision deficiency. 
| Deuteranopia| 1| Green color vision deficiency. 
| Protanopia| 2| Red color vision deficiency. 
| Tritanopia| 3| Blue color vision deficiency. 
| Achromatopsia| 4| Monochromatic vision. 



### Enumeration: DominantSizeAxis
#### Specifies the dominant size axis types. 

|Property | Value | Description | 
|---------|--------|--------|
| Z| 0| Dominant on the Z axis. 
| X| 1| Dominant on the X axis. 
| Y| 2| Dominant on the Y axis. 



### Enumeration: ElevationMode
#### Specifies the types of elevation surfaces. 

|Property | Value | Description | 
|---------|--------|--------|
| BaseGlobeSurface| 0| The ground or base surface. Only one ground per map or scene. 
| CustomSurface| 1| A custom surface. 
| None| 2| Not a surface. 



### Enumeration: ExtrusionType
#### The types of extrusion. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No extrusion. 
| MinZ| 1| Add an extrusion to each feature's minimum height. 
| MaxZ| 2| Add an extrusion to each feature's maximum height. 
| Base| 3| Add an extrusion to each feature's base height. 
| Absolute| 4| Add an extrusion by using it as an absolute value features are extruded to. 



### Enumeration: FaceCulling3D
#### The types of face culling. 

|Property | Value | Description | 
|---------|--------|--------|
| Backface| 0| Turns on back-face culling, eliminating those objects from view that face away from you. 
| Frontface| 1| Turns on front-face culling, eliminating those objects from view that face you. Use this option to see through the front of an object. 
| None| 2| Turns off culling so you view both sides. 
| FromGeometry| 3| Turns on the feature's built-in face culling. This option is only applicable for multipatch features. 



### Enumeration: GradientStrokeMethod
#### The different methods of gradient strokes. 

|Property | Value | Description | 
|---------|--------|--------|
| AcrossLine| 0| A gradient across the line. 
| AlongLine| 1| A gradient along the line. 



### Enumeration: MapLayerType
#### The types of map layers by use in the map or scene. 

|Property | Value | Description | 
|---------|--------|--------|
| Operational| 0| An operational layer. This is the most common layer type. 
| BasemapBackground| 1| An basemap layer used a background information. This is the basic basemap layer type. 
| BasemapTopReference| 2| An basemap layer used for top reference information. This is the basemap layer type used for overlay of information like text. 
| MapNotes| 3| An layer containing map notes. Primarily used to identify how the layer will be shared to WebMaps. 



### Enumeration: MapViewingMode
#### The map viewing modes. 

|Property | Value | Description | 
|---------|--------|--------|
| Map| 0| A 2D map. 
| SceneLocal| 1| A scene (3D map) in local view mode. 
| SceneGlobal| 2| A scene (3D map) in global view mode. 
| MapStereo| 3| A 2D map in stereo mode. Applicable if map is configured for stereo mode. 



### Enumeration: OffsetCurveMethod
#### Indicates the way the strokes will display at corners. 

|Property | Value | Description | 
|---------|--------|--------|
| Square| 0| Indicates the stroke will follow a straight path across the corner of a line. 
| Mitered| 1| Indicates the stroke will match the exact shape around a corner of the line. 
| Bevelled| 2| Indicates the stroke will follow the shortest straight path across a corner of the line. 
| Rounded| 3| Indicates the stroke will follow a path of equal distance around a corner of the line. 



### Enumeration: OffsetCurveOption
#### Indicates the way strokes will handle complex geometries. 

|Property | Value | Description | 
|---------|--------|--------|
| Fast| 0| Ignores complex geometries and applies a best fit to the stroke symbol. 
| Accurate| 1| Accommodates complex geometries and applies a true fit to the stroke symbol. 



### Enumeration: PrimitiveShapeType
#### Indicates the types of primitive shapes. 

|Property | Value | Description | 
|---------|--------|--------|
| Unknown| 0| Unknown. 
| Cone| 1| A cone. 
| Cube| 2| A cube. 
| Cylinder| 3| A cylinder. 
| Diamond| 4| A diamond. 
| Sphere| 5| A sphere. 
| Tetrahedron| 6| A tetrahedron. 



### Enumeration: PrimitiveType3D
#### Indicates the types of 3D primitives. 

|Property | Value | Description | 
|---------|--------|--------|
| TriangleStrip| 0| A triangle strip. 
| TriangleFan| 1| A triangle fan. 
| TriangleList| 2| A triangle list. 
| PointList| 3| A point list. 
| LineList| 4| A line list. 



### Enumeration: RangeRelation
#### Range relation types. 

|Property | Value | Description | 
|---------|--------|--------|
| Overlaps| 0| Include values equal to the start or end and values that are between the start and end. 
| OverlapsStartWithinEnd| 1| Include values equal to the start and values that are between the start and end. 
| AfterStartOverlapsEnd| 2| Include values equal to the end and values that are between the start and end. 
| Within| 3| Include values that are between the start and end but not equal to either. 



### Enumeration: RasterResamplingType
#### Raster resampling types. 

|Property | Value | Description | 
|---------|--------|--------|
| NearestNeighbor| 0| Nearest neighbor. 
| BilinearInterpolation| 1| Bilinear interpolation. 
| CubicConvolution| 2| Cubic convolution. 
| Majority| 3| Majority. 
| BilinearInterpolationPlus| 4| Bilinear interpolation plus. 
| BilinearGaussianBlur| 5| Bilinear Gaussian blur. 
| BilinearGaussianBlurPlus| 6| Bilinear Gaussian blur plus. 
| Average| 7| Average. 
| Minimum| 8| Minimum. 
| Maximum| 9| Maximum. 
| VectorAverage| 10| Vector average. 



### Enumeration: RasterStretchStatsType
#### Raster stretch statistics types. 

|Property | Value | Description | 
|---------|--------|--------|
| AreaOfView| 0| Stretch stats from current area of view. 
| Dataset| 1| Stretch stats from current dataset being rendered. 
| GlobalStats| 2| Stretch stats from global stats definition. 



### Enumeration: RasterStretchType
#### Raster stretch types. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No raster stretch. 
| DefaultFromSource| 1| Default stretch from source. 
| Custom| 2| Custom stretch. 
| StandardDeviations| 3| Stretch by standard deviation. 
| HistogramEqualize| 4| Stretch histogram equalization. 
| MinimumMaximum| 5| Stretch by minimum and maximum. 
| HistogramSpecification| 6| Stretch by histogram specification. 
| PercentMinimumMaximum| 7| Stretch by percent minimum and maximum. 
| Count| 8| Stretch by count. 
| ESRI| 9| Esri's stretch. 
| SquareRoot| 10| Square root stretch. 
| Logarithm| 11| Logarithmic stretch. 



### Enumeration: RotationOrder
#### Rotation order modes. 

|Property | Value | Description | 
|---------|--------|--------|
| XYZ| 0| Rotate in XYZ order. 
| ZXY| 1| Rotate in ZYX order. 
| YXZ| 2| Rotate in YXZ order. 

