### Enumeration: esriTimeUnits
#### Time units. 

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
#### Number format alignment options. 

|Property | Value | Description | 
|---------|--------|--------|
| esriAlignRight| 0|Right-justify formatted numbers within the AlignmentWidth.
| esriAlignLeft| 1|Left-justify formatted numbers.


### Enumeration: esriRoundingOptionEnum
#### Number format rounding options. 

|Property | Value | Description | 
|---------|--------|--------|
| esriRoundNumberOfDecimals| 0|Specify the number of decimal places.
| esriRoundNumberOfSignificantDigits| 1| Specify the number of significant digits.

### Enumeration: esriGeometryType
#### The available kinds of geometry objects. 

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
#### Dataset type constants. 

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
#### Antialiasing modes. 

|Property | Value | Description | 
|---------|--------|--------|
| esriBGLAntialiasingNone| 0|No antialiasing.
| esriBGLAntialiasingFastest| 1|Fastest antialiasing.
| esriBGLAntialiasingFast| 3|Fast antialiasing.
| esriBGLAntialiasingNormal| 6|Normal antialiasing.
| esriBGLAntialiasingBest| 8|Best antialiasing.

### Enumeration: esriBGLTextAAlias
#### Text antialiasing modes. 

|Property | Value | Description | 
|---------|--------|--------|
| esriBGLTextAAliasNone| 0|No text antialiasing.
| esriBGLTextAAliasDefault| 1|Default antialiasing.
| esriBGLTextAAliasForce| 2|Forced antialiasing.
| esriBGLTextAAliasForceForTransformed| 3|Forced antialiasing for rotated and curved text.

### Enumeration: esriAnimationTransitionMode
#### Define the type of algorithm used to calculate transitions between animation camera keyframes.

|Property | Value | Description | 
|---------|--------|--------|
| esriAnimationTransitionModeAuto| 0|Calculate the path between camera keyframes using a geodesic algorithm in global scene views and a cartesian algorithm in all other views.
| esriAnimationTransitionModeCartesian| 1|Calculate the path between camera keyframes using a cartesian algorithm.
| esriAnimationTransitionModeGeodesic| 2|Calculate the path between camera keyframes using a geodesic algorithm.

### Enumeration: esriTimeRelation 
#### Time relation types.

|Property | Value | Description | 
|---------|--------|--------|
| esriTimeRelationOverlaps| 0|Overlaps.
| esriTimeRelationOverlapsStartWithinEnd| 1|Overlaps start within end.
| esriTimeRelationAfterStartOverlapsEnd| 2|After start, overlaps end.
| esriTimeRelationWithin| 3|After start, within end.

### Enumeration: esriSpatialRelEnum 
#### Queryable spatial relationships.

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
#### Join types.

|Property | Value | Description | 
|---------|--------|--------|
| esriLeftOuterJoin| 0|Left outer join.
| esriLeftInnerJoin| 1|Left inner join.

### Enumeration: esriDiagramDatasetFeatureClass 
#### Diagram feature class types.

|Property | Value | Description | 
|---------|--------|--------|
| esriDiagramEdgeFeatureClass| 0|Edge feature class.
| esriDiagramJunctionFeatureClass| 1|Junction feature class.
| esriDiagramContainerFeatureClass| 2|Container feature class.
| esriTemporaryDiagramEdgeFeatureClass| 3|Temporary Edge feature class.
| esriTemporaryDiagramJunctionFeatureClass| 4|Temporary Junction feature class.
| esriTemporaryDiagramContainerFeatureClass| 5|Temporary Container feature class.

### Enumeration: esriImageFormat 
#### Image formats.

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
#### Spatial Filter Search Order.

|Property | Value | Description | 
|---------|--------|--------|
| esriSearchOrderSpatial| 0|Spatial query is applied first.
| esriSearchOrderAttribute| 1|Attribute query is applied first.

### Enumeration: esriRelCardinality 
#### Relationship Cardinality.

|Property | Value | Description | 
|---------|--------|--------|
| esriRelCardinalityOneToOne| 0|One To One.
| esriRelCardinalityOneToMany| 1|One To Many.
| esriRelCardinalityManyToMany| 2|Many To Many.

###Geometry

[Point](ExternalReferences.md#point)

[Polyline](ExternalReferences.md#polyline)

[Polygon](ExternalReferences.md#polygon)

[Envelope](ExternalReferences.md#envelope)

###Unit

[LinearUnit](ExternalReferences.md#linearunit)

[AngularUnit] ExternalReferences.md#angularunit)

### SpatialReference

## LasFilter
#### Las filter.


### LasFilter

|Property | Type | Description | 
|---------|--------|--------|
| areOfInterest | [Envelope] (ExternalReferences.md#envelope)|Gets and sets the area of interest. 
| classCodes | long|Gets and sets the class codes. 
| classFlags | long|Gets and sets the class flags. 
| returns | long|Gets and sets the returns. 
| surfaceConstraints | string|Gets and sets the surface constraints. 
