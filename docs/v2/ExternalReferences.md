### Enumeration: esriTimeUnits
Time units.

|Property | Value | Description |
|---------|--------|--------|
| esriTimeUnitsUnknown| 0| Unknown.
| esriTimeUnitsMilliseconds| 1| Milliseconds.
| esriTimeUnitsSeconds| 2| Seconds.
| esriTimeUnitsMinutes| 3| Minutes.
| esriTimeUnitsHours| 4| Hours.
| esriTimeUnitsDays| 5| Days.
| esriTimeUnitsWeeks| 6| Weeks.
| esriTimeUnitsMonths| 7| Months.
| esriTimeUnitsYears| 8| Years.
| esriTimeUnitsDecades| 9| Decades.
| esriTimeUnitsCenturies| 10| Centuries

### Enumeration: esriNumericAlignmentEnum
Number format alignment options.

|Property | Value | Description |
|---------|--------|--------|
| esriAlignRight| 0|Right-justify formatted numbers within the AlignmentWidth.
| esriAlignLeft| 1|Left-justify formatted numbers.


### Enumeration: esriRoundingOptionEnum
Number format rounding options.

|Property | Value | Description |
|---------|--------|--------|
| esriRoundNumberOfDecimals| 0|Specify the number of decimal places.
| esriRoundNumberOfSignificantDigits| 1| Specify the number of significant digits.

### Enumeration: esriGeometryType
The available kinds of geometry objects.

|Property | Value | Description |
|---------|--------|--------|
| esriGeometryNull| 0|A geometry of unknown type.
| esriGeometryPoint| 1|A single zero dimensional geometry.
| esriGeometryMultipoint| 2|An ordered collection of points.
| esriGeometryPolyline| 3|An ordered collection of paths.
| esriGeometryPolygon| 4|A collection of rings ordered by their containment relationship.
| esriGeometryEnvelope| 5|A rectangle indicating the spatial extent of another geometry.
| esriGeometryPath| 6|A connected sequence of segments.
| esriGeometryAny| 7|Any of the geometry types.
| esriGeometryMultiPatch| 9|A collection of surface patches.
| esriGeometryRing| 11|An area bounded by one closed path.
| esriGeometryLine| 13|A straight line segment between two points.
| esriGeometryCircularArc| 14|A portion of the boundary of a circle.
| esriGeometryBezier3Curve| 15|A third degree bezier curve (four control points).
| esriGeometryEllipticArc| 16|A portion of the boundary of an ellipse.
| esriGeometryBag| 17|A collection of geometries of arbitrary type.
| esriGeometryTriangleStrip| 18|A surface patch of triangles defined by three consecutive points.
| esriGeometryTriangleFan| 19|A surface patch of triangles defined by the first point and two consecutive points.
| esriGeometryRay| 20|An infinite, one-directional line extending from an origin point.
| esriGeometrySphere| 21|A complete 3 dimensional sphere.
| esriGeometryTriangles| 22|A surface patch of triangles defined by non-overlapping sets of three consecutive points each.

### Enumeration: esriDatasetType
Dataset type constants.

|Property | Value | Description |
|---------|--------|--------|
| esriDTAny| 0|Any Dataset.
| esriDTContainer| 1|Any Container Dataset.
| esriDTGeo| 2|Any Geo Dataset.
| esriDTFeatureDataset| 3|Feature Dataset.
| esriDTFeatureClass| 4|Feature Class.
| esriDTPlanarGraph| 5|Planar Graph.
| esriDTGeometricNetwork| 6|Geometric Network.
| esriDTText| 7|Text Dataset.
| esriDTTable| 8|Table Dataset.
| esriDTRelationshipClass| 9|Relationship Class.
| esriDTRasterDataset| 10|Raster Dataset.
| esriDTRasterBand| 11|Raster Band.
| esriDTTin| 12|Tin Dataset.
| esriDTCadDrawing| 13|CadDrawing Dataset.
| esriDTRasterCatalog| 14|Raster Catalog.
| esriDTTopology| 15|Topology.
| esriDTToolbox| 16|Toolbox.
| esriDTTool| 17|Tool.
| esriDTNetworkDataset| 18|Network Dataset.
| esriDTTerrain| 19|Terrain dataset.
| esriDTRepresentationClass| 20|Feature Class Representation.
| esriDTCadastralFabric| 21|Cadastral Fabric.
| esriDTSchematicDataset| 22|Schematic Dataset.
| esriDTLocator| 23|Address Locator.
| esriDTMap| 24|Map.
| esriDTLayer| 25|Layer.
| esriDTStyle| 26|Style.
| esriDTMosaicDataset| 27|Mosaic Dataset.
| esriDTLasDataset| 28|Las Dataset.
| esriDTLayout| 29|Layout.
| esriDTStandaloneTable| 30|Standalone Table.
| esriDTUtilityNetwork| 31|Utility Network.
| esriDTDiagramDataset| 32|Diagram Dataset.
| esriDTDiagramFolder| 33|Diagram Folder.
| esriDTNetworkDiagram| 34|Network Diagram.
| esriDTParcelDataset| 35|Parcel Dataset.
| esriDTStandaloneVideo| 36|Standalone Video.
| esriDTReport| 37|Report.

### Enumeration: esriBGLAntialiasingMode
Antialiasing modes.

|Property | Value | Description |
|---------|--------|--------|
| esriBGLAntialiasingNone| 0|No antialiasing.
| esriBGLAntialiasingFastest| 1|Fastest antialiasing.
| esriBGLAntialiasingFast| 3|Fast antialiasing.
| esriBGLAntialiasingNormal| 6|Normal antialiasing.
| esriBGLAntialiasingBest| 8|Best antialiasing.

### Enumeration: esriBGLTextAAlias
Text antialiasing modes.

|Property | Value | Description |
|---------|--------|--------|
| esriBGLTextAAliasNone| 0|No text antialiasing.
| esriBGLTextAAliasDefault| 1|Default antialiasing.
| esriBGLTextAAliasForce| 2|Forced antialiasing.
| esriBGLTextAAliasForceForTransformed| 3|Forced antialiasing for rotated and curved text.

### Enumeration: esriAnimationTransitionMode
Define the type of algorithm used to calculate transitions between animation camera keyframes.

|Property | Value | Description |
|---------|--------|--------|
| esriAnimationTransitionModeAuto| 0|Calculate the path between camera keyframes using a geodesic algorithm in global scene views and a cartesian algorithm in all other views.
| esriAnimationTransitionModeCartesian| 1|Calculate the path between camera keyframes using a cartesian algorithm.
| esriAnimationTransitionModeGeodesic| 2|Calculate the path between camera keyframes using a geodesic algorithm.

### Enumeration: esriTimeRelation
Time relation types.

|Property | Value | Description |
|---------|--------|--------|
| esriTimeRelationOverlaps| 0|Overlaps.
| esriTimeRelationOverlapsStartWithinEnd| 1|Overlaps start within end.
| esriTimeRelationAfterStartOverlapsEnd| 2|After start, overlaps end.
| esriTimeRelationWithin| 3|After start, within end.

### Enumeration: esriSpatialRelEnum
Queryable spatial relationships.

|Property | Value | Description |
|---------|--------|--------|
| esriSpatialRelUndefined| 0|No Defined Spatial Relationship.
| esriSpatialRelIntersects| 1|Query Geometry Intersects Target Geometry.
| esriSpatialRelEnvelopeIntersects| 2|Envelope of Query Geometry Intersects Envelope of Target Geometry.
| esriSpatialRelIndexIntersects| 3|Query Geometry Intersects Index entry for Target Geometry (Primary Index Filter).
| esriSpatialRelTouches| 4|Query Geometry Touches Target Geometry.
| esriSpatialRelOverlaps| 5|Query Geometry Overlaps Target Geometry.
| esriSpatialRelCrosses| 6|Query Geometry Crosses Target Geometry.
| esriSpatialRelWithin| 7|Query Geometry is Within Target Geometry.
| esriSpatialRelContains| 8|Query Geometry Contains Target Geometry.
| esriSpatialRelRelation| 9|Query geometry IBE(Interior-Boundary-Exterior) relationship with target geometry.

### Enumeration: esriJoinType
Join types.

|Property | Value | Description |
|---------|--------|--------|
| esriLeftOuterJoin| 0|Left outer join.
| esriLeftInnerJoin| 1|Left inner join.

### Enumeration: esriDiagramDatasetFeatureClass
Diagram feature class types.

|Property | Value | Description |
|---------|--------|--------|
| esriDiagramEdgeFeatureClass| 0|Edge feature class.
| esriDiagramJunctionFeatureClass| 1|Junction feature class.
| esriDiagramContainerFeatureClass| 2|Container feature class.
| esriTemporaryDiagramEdgeFeatureClass| 3|Temporary Edge feature class.
| esriTemporaryDiagramJunctionFeatureClass| 4|Temporary Junction feature class.
| esriTemporaryDiagramContainerFeatureClass| 5|Temporary Container feature class.
| esriNetworkDiagramFeatureClass | 6|Diagram feature class.

### Enumeration: esriImageFormat
Image formats.

|Property | Value | Description |
|---------|--------|--------|
| esriImageNone| -1|None.
| esriImageBMP| 0|BMP.
| esriImageJPG| 1|JPEG.
| esriImageDIB| 2|DIB.
| esriImageTIFF| 3|TIFF.
| esriImagePNG| 4|PNG.
| esriImagePNG24| 5|PNG24.
| esriImageEMF| 6|Windows Enhanced Metafile.
| esriImagePS| 7|PostScript.
| esriImagePDF| 8|PDF.
| esriImageAI| 9|Adobe Illustrator.
| esriImageGIF| 10|GIF.
| esriImageSVG| 11|SVG.
| esriImageSVGZ| 12|Compressed SVG.
| esriImagePNG32| 13|PNG32.
| esriImageJPGPNG| 14|JPEG or PNG if containing transparent pixels.
| esriImageOptimalPNG| 15|Optimal PNG bit depth based on content.
| esriImageLERC| 16|Limted error raster compression.
| esriImageRaw| 17|Raw.
| esriImageBSQ| 18|Band sequential.
| esriImageBIP| 19|Band interleaved by pixel.

### Enumeration: esriSearchOrder
Spatial Filter Search Order.

|Property | Value | Description |
|---------|--------|--------|
| esriSearchOrderSpatial| 0|Spatial query is applied first.
| esriSearchOrderAttribute| 1|Attribute query is applied first.

### Enumeration: esriRelCardinality
Relationship Cardinality.

|Property | Value | Description |
|---------|--------|--------|
| esriRelCardinalityOneToOne| 0|One To One.
| esriRelCardinalityOneToMany| 1|One To Many.
| esriRelCardinalityManyToMany| 2|Many To Many.

### Geometry

### Point
Defines the JSON formats of the point and spatial reference objects.

|Property | Type | Description |
|---------|--------|--------|
| m | double | M coordinate which contains measures used for linear referencing.
|spatialReference| [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference can be defined using a well-known ID (WKID) or well-known text (WKT).
| x | double | X coordinate which is measured along the east/west axis.<br>Must be one of the following values:<ul><li>`Number`</li><li>`Null`</li><li>`String`</li></ul>
| y | double | Y coordinate which is measured along the north/south axis.
| z | double | Z coordinate which measures height or elevation.

### Multipoint
A Multipoint is a collection of Points.  A multipoint is a one-dimensional geometry object.  Multipoints can be used to store a collection of Point-based information where the order and individual identity of each point is not an essential characteristic of the Point set.  Functions that return multiple point results simultaneously return the result as a single Multipoint.

|Property | Type | Description |
|---------|--------|--------|
| hasM | boolean |Indicates whether the geometry contains M coordinate values.
| hasZ | boolean |Indicates whether the geometry contains Z coordinate values.
| points |[[Point](ExternalReferences.md#point)]| Array of [Points](ExternalReferences.md#point)
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference can be defined using a well-known ID (WKID) or well-known text (WKT).

### Multipatch

|Property | Type | Description |
|---------|--------|--------|
| hasM | boolean |Indicates whether the geometry contains M coordinate values.
| hasZ | boolean |Indicates whether the geometry contains Z coordinate values.
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference can be defined using a well-known ID (WKID) or well-known text (WKT).
| binaryPatches | string |Contains a zip-compressed and base64 encoded ESRI shape without materials.
| materials     |[[Material](ExternalReferences.md#material)] |This is an ordered Array contains MultiPatch materials and must have exactly same number of materials as the MultiPatch encoded in the binaryPatches.

### Material

|Property | Type | Description |
|---------|--------|--------|
|name     | string | Name that identifies the material.|
|color    | [Color](CIMColor.md#CIMColor)| Color of the material.|
|shininess| short | Shininess of the material ranging from 0 to 255 inclusive.|
|transparency| double | Transparency of the material ranging from 0 and 100 inclusive.|
|cull| boolean | Indicates the
|edgeColor| [Color](CIMColor.md#CIMColor)| Edge color.|
|edgeWidth| short | Width of the edge ranging from 0 and 255 inclusive.|
|texture| string | base64 encoded texture image.|
|textureUrl| string | URL of texture image.|
|sharedTexture| string | Name of the material that contains the actual texture.|

### Polyline

A polyline contains an array of paths or curvePaths and a spatialReference. For polylines with curvePaths, see the sections on JSON curve object and Polyline with curve. Each path is represented as an array of points, and each point in the path is represented as an array of numbers. A polyline can also have valued hasM and hasZ as boolean fields.

See the description of multipoints for details on how the point arrays are interpreted.

An empty polyline is represented with an empty array for the paths field. Nulls and/or NaNs embedded in an otherwise defined coordinate stream for polylines/polygons is a syntax error.

|Property | Type | Description |
|---------|--------|--------|
| hasM | boolean |Indicates whether the geometry contains M coordinate values.
| hasZ | boolean |Indicates whether the geometry contains Z coordinate values.
| paths |[[path](ExternalReferences.md#path)]| Ordered array of paths. Each path represented as ordered array of [Points](ExternalReferences.md#point)
| curvePaths |[[CurvePath](ExternalReferences.md#curvepath)]| Ordered array of curved paths. Each curve path is ordered array of [Points](ExternalReferences.md#point) and [Curves](ExternalReferences.md#curves)
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference can be defined using a well-known ID (WKID) or well-known text (WKT).

### Polygon

A polygon contains an array of rings or curveRings and a spatialReference. For polygons with curveRings, see the sections on JSON curve object and Polygon with curve. Each ring is represented as an array of points. The first point of each ring is always the same as the last point. Each point in the ring is represented as an array of numbers. A polygon can also have Boolean-valued hasM and hasZ fields.

See the description of multipoints for details on how the point arrays are interpreted.

An empty polygon is represented with an empty array for the rings field. Nulls and/or NaNs embedded in an otherwise defined coordinate stream for polylines/polygons is a syntax error.

Polygons should be topologically simple. Exterior rings are oriented clockwise, while holes are oriented counter-clockwise. Rings can touch at a vertex or self-touch at a vertex, but there should be no other intersections. Polygons returned by services are topologically simple.

When drawing a polygon, use the even-odd fill rule. The even-odd fill rule will guarantee that the polygon will draw correctly even if the ring orientation is not as described above.

|Property | Type | Description |
|---------|--------|--------|
| hasM | boolean |Indicates whether the geometry contains M coordinate values.
| hasZ | boolean |Indicates whether the geometry contains Z coordinate values.
| rings |[[Ring](ExternalReferences.md#ring)]| Ordered array of rings. Each ring is an array of [points](ExternalReferences.md#point).
| curveRings |[[CurveRing](ExternalReferences.md#curvering)]|  Ordered array of curved rings. Each curve ring is  ordered array of [Points](ExternalReferences.md#point) and [Curves](ExternalReferences.md#curves)
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference can be defined using a well-known ID (WKID) or well-known text (WKT).

### Envelope

An envelope is a rectangle defined by a range of values for each coordinate and attribute. It also has a spatialReference field. The fields for the z and m ranges are optional. An empty envelope has no location in space and is defined by the presence of an xmin field, a null value, or a "NaN" string.

|Property | Type | Description |
|---------|--------|--------|
| mmax | double | The maximum measure value in the area of the envelope.
| mmin | double | The minimum measure value in the area of the envelope.
|spatialReference | [SpatialReference](spatialReference.md) | The spatial reference can be defined using a well-known ID (wkid) or well-known text (wkt)
| xmax | double | The maximum X value in the area of the envelope.
| xmin | number or string ("NaN") | The minimum X value in the area of the envelope.
| ymax | double | The maximum Y value in the area of the envelope.
| ymin | double | The minimum Y value in the area of the envelope.
| zmax | double | The maximum Z value in the area of the envelope.
| zmin | double | The minimum Z value in the area of the envelope.

### GeometryBag
A GeometryBag is a heterogeneous collection of references to geometry objects.

When adding elements to a GeometryBag, keep in mind that the elements acquire the spatial reference of the bag. If the spatial reference of the bag is null, for example, and the element references a well-defined spatial reference, then the element will lose that reference when it is added to the bag.

|Property | Type | Description |
|---------|--------|--------|
| hasM | boolean |Indicates whether the geometry contains M coordinate values.
| hasZ | boolean |Indicates whether the geometry contains Z coordinate values.
| points |[[Geometry](ExternalReferences.md#point)]| Array of [Geometry](ExternalReferences.md#geometry)
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference can be defined using a well-known ID (WKID) or well-known text (WKT).

### Area
Area represents the type of geometries that have area. It can be one of these:
* [Envelope](ExternalReferences.md#envelope)
* [Polygon](ExternalReferences.md#polygon)

### Path
A path is a sequence of connected segments represented by an array of [points](ExternalReferences.md#point).

|Property | Type | Description |
|---------|--------|--------|
| - | [[point](ExternalReferences.md#point)] |Ordered array of [points](ExternalReferences.md#point)|

### CurvePath
A curve path is a sequence of connected segments represented by an array of [points](ExternalReferences.md#point) and [curves](ExternalReferences.md#curves).

|Property | Type | Description |
|---------|--------|--------|
| - | [[point](ExternalReferences.md#point)] |Ordered array of [points](ExternalReferences.md#point)|

### Ring
A ring is an area bounded by one, closed sequence of connected segments represented by array of [points](ExternalReferences.md#point).

|Property | Type | Description |
|---------|--------|--------|
| - | [[point](ExternalReferences.md#point)] |Ordered array of [points](ExternalReferences.md#point)|

### CurveRing
A curve ring is an area bounded by one, closed sequence of connected segments represented by array of [points](ExternalReferences.md#point) and [curves](ExternalReferences.md#curves).

|Property | Type | Description |
|---------|--------|--------|
| - | [[point](ExternalReferences.md#point)] |Ordered array of [points](ExternalReferences.md#point)|

### Curves
A curve object is a segment in a polyline or polygon. It cannot be used as a stand-alone object.

A curve object is given in a compact "curve to" manner with the first element representing the "to" point or end point. The "from" point is derived from the previous segment or curve object.

The supported curve objects are as follows:
  * [Circular Arc](ExternalReferences.md#circulararc)
  * [Elliptic Arc](ExternalReferences.md#ellipticarc)
  * [Bézier Curve](ExternalReferences.md#béziercurve)

### CircularArc
A Circular Arc is an object that describes any portion of a circle. A CircularArc differs from an EllipticArc in that every point along the CircularArc must be a fixed distance (the Radius) from the center.

Circular Arc is defined by an end point and an interior point. It is identified by the member "c" and can be represented in JSON as
{"c": [[x, y, <z>, <m>],[interior_x, interior_y]]}

|Property | Type | Description |
|---------|--------|--------|
|c|[[Point](ExternalReferences.md#point)]|In the array, first element represents end point and the second element represents interior point|

### EllipticArc
An Elliptic Arc is an object that describes any portion of an ellipse.  

Elliptic Arc is defined by end point, center point, axis, arc orientation, angle from major axis in radians, length of semi major axis and ratio of the minor axis to the major axis and can be represented in JSON as follows: {"a": [[x, y, <z>, <m>],[center_x, center_y], minor, clockwise, rotation, axis, ratio]}

|Property | Type | Description |
|---------|--------|--------|
|a|[[Point](ExternalReferences.md#point)(end point), [Point](ExternalReferences.md#point)(center point), number(minor), number(clockwise), number(rotation), number(semi major axis),number(ratio)]| <br>Array elements should be in the following order : <ul><li>`End point`</li><li>`Center Point`</li><li>`minor` (0: major, 1: minor)</li><li>arc orientation` (0: counter clockwise, 1: clockwise)</li><li>`rotation` (angle from major axis)</li><li>`axis`: length of the semi-major axis</li><li>`ratio`: ratio of the minor axis to major axis</li></ul>|

### BézierCurve

A cubic Bézier Curve is a non-linear Segment defined by four control points.  The Bézier curve starts at control point 0 and ends at control point 3.  Control points 0 and 1 define the tangent at the from point and control points 2 and 3 define the tangent at the to point.  The length of these tangent lines and position of the control points determines the shape of the created bézier curve.

|Property | Type | Description |
|---------|--------|--------|
|b|[[Point](ExternalReferences.md#point)(end point), [Point](ExternalReferences.md#point)(control point), [Point](ExternalReferences.md#point)(control point)]| <br>Array elements should be in the following order : <ul><li>`End point`</li><li>`Control Point`</li><li>`Control Point`</li></ul>|

### Unit

Represents a linear unit or angular unit of measure.

|Property | Type | Description |
|---------|--------|--------|
| uwkid | long | Well-known identifier representing the specific unit type.


### LinearUnit

Represents a linear unit of measure.

|Property | Type | Description |
|---------|--------|--------|
| uwkid | long| Well-known identifier representing the specific unit. Refer to the [list of units](http://desktop.arcgis.com/en/arcmap/latest/map/projections/pdf/projected_coordinate_systems.pdf) for well-known IDs and conversion values for Linear Units.

### AngularUnit

Represents a angular unit of measure.

|Property | Type | Description |
|---------|--------|--------|
| uwkid | long| Well-known identifier representing the specific unit. Refer to the [list of units](http://desktop.arcgis.com/en/arcmap/latest/map/projections/pdf/geographic_coordinate_systems.pdf) for well-known IDs and conversion values for angular Units.

### SpatialReference

A spatial reference is the georeferencing and coordinate system assigned to any geographic data.

|Property | Type | Description |
|---------|--------|--------|
| wkid | long| Well-known identifier representing the specific geographic or projected coordinate system. Refer to the list for well known identifiers:<ul><li>[Projected Coordinate Systems Listing](https://developers.arcgis.com/rest/services-reference/projected-coordinate-systems.htm)</li><li>[Geographic Coordinate Systems Listing](https://developers.arcgis.com/rest/services-reference/geographic-coordinate-systems.htm)</li></ul>
| latestWkid | long| Represents is an more resent version of an identifier for a wkid. when this value is different from wkid, wkid is considered the originally introduced identifier and latestWkid is the more resent one that should be preferred.|
| vcsWkid | long| Well-known identifier representing the specific geographic or projected coordinate system. Refer to the list for well known identifiers:<ul><li>[Vertical Coordinate Systems Listing](https://developers.arcgis.com/rest/services-reference/vertical-coordinate-systems.htm)</li></ul>
| latestVcsWkid | long| Represents is an more resent version of an identifier for a wkid. when this value is different from wkid, wkid is considered the originally introduced identifier and latestWkid is the more resent one that should be preferred.|

### GeoTransformation

 Geographic transformations translate coordinates from one geographic coordinate system to another. A geographic transformation can be a single transformation with properties as described below or a [CompositeGeoTransformation](ExternalReferences.md#compositegeotransformation) object.

|Property | Type | Description |
|---------|--------|--------|
| wkid | long| Well-known identifier representing the specific transformation. Refer to the list for well known identifiers:<ul><li>[Datum transformations](https://developers.arcgis.com/rest/services-reference/datum-transformations.htm)</li></ul>
| latestWkid | long | Represents is an more resent version of an identifier for a wkid. when this value is different from wkid, wkid is considered the originally introduced identifier and latestWkid is the more resent one that should be preferred.|
|transformForward|boolean|The direction (forward/reverse) of a geographic transformation.|
|name     | string | Name of the geographic transformation.|

### CompositeGeoTransformation

A composite geotransformation allows you to create a 'chain' of existing or custom transformations. Each transformation in the set must have its transformForward properly.

|Property | Type | Description |
|---------|--------|--------|
|geoTransforms | [[GeoTransformation](ExternalReferences.md#geotransformation)] | Ordererd array of the geographic transformation.|

## StatsHistogram
 A raster statistics and histogram used for statistics-based rendering of raster layers

|Property | Type | Description |
|---------|--------|--------|
| min | double |The minimum value of the histogram.|
| max | double |The maximum value of the histogram.|
| mean | double |The mean value of the histogram.|
| stddev | double |The standard deviation of the histogram.|
| limitMin | double |The minimum limit of the range.|
| limitMax | double |The maximum limit of the range.|
| histogram | [double] |The histogram values of the statistics.|
| nsamples | double |The number of samples.|
| resolution | double |The resolution.|
| nBands | long |The number of bands.|
| covariances | [double] |The covariances.|

## RasterColormap
A container for a colormap used to display a raster band.

|Property | Type | Description |
|---------|--------|--------|
| Values| [long] |An array of values of the colormap.|
| Colors| [long] |An array of colors corresponding to the values. Colors are represented as RGB stored as a long integer.|

## TimeReference
The Time Reference contains information about time zone and daylight savings time rules.  It is used to integrate different data sets that have time stamps from different time zones, or using different daylight savings time rules.

|Property | Type | Description |
|---------|--------|--------|
| timeZone | string |The time zone for this time reference.|
| respectsDaylightSaving | boolean |A boolean which indicates whether the time reference respects daylight saving time. |
| respectsDynamicAdjustmentRules | boolean|Aboolean which indicates whether the time reference respects dynamic adjustment rules.|

### TimeValue
TimeValue represents either a instance of time or an extent of time. It can either be a [TimeInstant](ExternalReferences.md#timeinstant) or a [TimeExtent](ExternalReferences.md#timeextent)

|Property | Type | Description |
|---------|--------|--------|
| TimeReference | [TimeReference](ExternalReferences.md#timereference) |The time reference for the time value.

## TimeExtent
A [TimeValue](ExternalReferences.md#timevalue) object that represents a time-referenced range of time with a beginning and end.

### TimeExtent
|Property | Type | Description |
|---------|--------|--------|
| type | string | The value for this will always be "TimeExtent"
| start | double |The time extent's start time.
| end | double |The time extent's end time.
| empty | boolean |A boolean indicating whether the time extent is empty.
| TimeReference | [TimeReference](ExternalReferences.md#timereference) |The time reference for the time value.

## TimeInstant
An [TimeValue](ExternalReferences.md#timevalue) object that represents a time-referenced instant of time.

### TimeInstant
|Property | Type | Description |
|---------|--------|--------|
| type  | string| The value for this will always be "TimeInstant"
| start | double |The time value of the time instant.
| TimeReference | [TimeReference](ExternalReferences.md#timereference) |The time reference for the time value.

## LasFilter
An object defining LAS filtering

|Property | Type | Description |
|---------|--------|--------|
| type  | string | The value for this will always be "LasFilter"|
| areaOfInterest | [geometry](ExternalReferences.md#geometry) |The area of interest.|
| classCodes     | [long] |An array of class codes each number ranging from 0-255. |
| classFlags     | long |	The number that is the bitwise OR of several values indicating. the class flags. Here are the values:<br><ul><li>0x00000001 - None</li><li>0x00000002 - LAS synthetic-point flag.</li><li>0x00000004 - LAS key-point flag.</li><li>0x00000002 - LAS synthetic-point flag.</li><li>0x00000008 - LAS withheld-point flag.</li><li>0x000000010 - LAS overlap-point flag.</li></ul>|
| Returns        | [long] |An arrayof LAS return numbers. |
| SurfaceConstraints|	[string] |The array of surface constraints.|
