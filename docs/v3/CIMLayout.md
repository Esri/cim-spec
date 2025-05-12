

### Enumeration: Anchor
#### A list of anchor positions for an element on a page layout. 

|Property | Value | Description | 
|---------|--------|--------|
| Unspecified| 0| Unspecified. 
| TopLeftCorner| 1| Top, left corner. 
| TopMidPoint| 2| Top, middle location. 
| TopRightCorner| 3| Top, right corner. 
| LeftMidPoint| 4| Left, middle location. 
| CenterPoint| 5| Center location. 
| RightMidPoint| 6| Right, middle location. 
| BottomLeftCorner| 7| Bottom, left corner. 
| BottomMidPoint| 8| Bottom, middle location. 
| BottomRightCorner| 9| Bottom, right corner. 




## CIMAttachmentFrame
#### Represents an attachment graphic frame. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMAttachmentFrame 

|Property | Type | Description | 
|---------|--------|--------|
| maxImages | long | Maximum number of image attachments to display. If -1, all images attachments will be available. 
| sortFieldName | string | Field name to sort. 
| sortOrder | [enumeration FieldSortInfo](CIMLayout.md#enumeration-fieldsortinfo) | Sort order of image attachments. 
| imageFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of each attachment image frame. 
| gridRows | long | The number of attachment image rows. If less than 0, the number of rows is automatically calculated. 
| gridColumns | long | The number of attachment image columns. 
| gridRowDirection | boolean | A value indicating whether the grid layout is in row major order. 
| imageHeight | double | The height of each attachment image. 
| imageWidth | double | The width of each attachment image. 






## CIMAutoCamera
#### Represents the camera settings associated with a map frame on a page layout. 


### CIMAutoCamera 

|Property | Type | Description | 
|---------|--------|--------|
| camera | [CIMViewCamera](CIMMap.md#cimviewcamera) | The camera associated with the map frame. 
| autoCameraType | [enumeration AutoCameraType](CIMLayout.md#enumeration-autocameratype) | The camera type. 
| extent | [Envelope](ExternalReferences.md#envelope) | The extent for a map frame when using the fixed constraint. 
| intersectLayerPath | string | The layer being used to set the camera when using the map frame link constraint. 
| mapFrameLinkName | string | The map frame name being used to set the camera when using the map frame link constraint. 
| margin | double | The margin value for a map frame with a map frame link constraint. 
| marginType | [enumeration UnitType](CIMLayout.md#enumeration-unittype) | The margin type for a map frame with a map frame link constraint. 
| marginUnits | [Unit](ExternalReferences.md#unit) | The margin units for a map frame with a map frame link constraint. 
| source | [enumeration AutoCameraSource](CIMLayout.md#enumeration-autocamerasource) | The extent constraint associated with the map frame. 
| syncRotation | boolean | A value indicating whether the map frame should rotate when using a map frame link constraint. 





### Enumeration: AutoCameraSource
#### A list of the advanced map frame options that further controls the camera behavior. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Use navigation tools to set the extent. 
| Fixed| 1| The extent specified will not change. 
| MapFrameLink| 2| Base the extent on another map frame. 
| MapSeriesLink| 3| Base the extent on the extent of the index feature. 



### Enumeration: AutoCameraType
#### A list of the options available when using a fixed constraint. 

|Property | Value | Description | 
|---------|--------|--------|
| Center| 0| Show the map at the specified center point. 
| Scale| 1| Show the map at the specified scale. 
| CenterAndScale| 2| Show the map at the specified center point and scale. 
| Extent| 3| Show the map at a specified extent. 




## CIMAviationArrow
#### Represents an individual arrow in CIMAviationNorthArrow. 


### CIMAviationArrow 

|Property | Type | Description | 
|---------|--------|--------|
| lineIndicatorTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The indicator text symbol for the arrow. 
| lineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol for the arrow. 
| defaultPointSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The default point symbol for the arrow. 
| positivePointSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The positive point symbol for the arrow. 
| negativePointSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The negative point symbol for the arrow. 
| enableArrow | boolean | A value indicating whether the arrow is enabled. 
| enableLineIndicator | boolean | A value indicating whether the arrow's line indicator is enabled. 
| arrowLength | double | The line length for the arrow, internally units will always be of type points. 
| lineIndicatorText | string | The text for the line indicator text symbol. 






## CIMAviationNorthArrow
#### Represents a aviation north arrow which displays declination of true, grid and magnetic north. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMNorthArrow 

|Property | Type | Description | 
|---------|--------|--------|
| referenceLocation | [Point](ExternalReferences.md#point) | The reference location for a north arrow. 
| calibrationAngle | double | The calibration angle for a north arrow. 


### CIMAviationNorthArrow 

|Property | Type | Description | 
|---------|--------|--------|
| date | [TimeInstant](ExternalReferences.md#timeinstant) | The date used when calculating declination using world magnetic model. 
| declinationSpatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference used for calculating declination, typically a UTM zone. 
| GMAngle | [CIMDeclination](CIMLayout.md#cimdeclination) | The Grid Magnetic declination. 
| gridConvergence | [CIMDeclination](CIMLayout.md#cimdeclination) | The Grid Convergence declination. 
| trueNorthArrow | [CIMAviationArrow](CIMLayout.md#cimaviationarrow) | The true north arrow for aviation north arrow. 
| magneticNorthArrow | [CIMAviationArrow](CIMLayout.md#cimaviationarrow) | The magnetic north arrow for the aviation north arrow. 
| gridNorthArrow | [CIMAviationArrow](CIMLayout.md#cimaviationarrow) | The grid north arrow for the aviation north arrow. 
| variation | [CIMAviationVariation](CIMLayout.md#cimaviationvariation) | The variation for the aviation north arrow. 
| rateOfChangeTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The rate of change text symbol for the north arrow. 
| displayVariationDate | boolean | A value indicating whether to display the variation date. 
| displayRateOfChange | boolean | A value indicating whether to display the rate of change text. 
| autoUpdate | boolean | A value indicating whether the north arrow auto updates. 
| rateOfChangeText | string | The rate of change text displayed. 






## CIMAviationVariation
#### Represents the properties for the variation text which is displayed in aviation north arrow. 


### CIMAviationVariation 

|Property | Type | Description | 
|---------|--------|--------|
| variationTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol used for variation text in aviation north arrow. 
| alignVariationToLine | boolean | A value indicating whether to align text to line or display on side. 
| variationTextOnLeft | boolean | A value indicating whether the variation text will be displayed on the left side of aviation north arrow, if false will display on the right side. 
| showYear | boolean | A value indicating whether to show the variation year in the variation text. 
| showYearInParenthesis | boolean | A value indicating whether to show the variation year enclosed in parenthesis. 
| variationYearSeparator | string | The string separator that goes between the variation text and the variation year. 
| magneticVariationIdentifier | string | The magnetic north identifier for the variation text. 
| gridVariationIdentifier | string | The grid north identifier for the variation text. 






## CIMAviationVerticalScaleBar
#### Represents an aviation-specific Vertical Scale Bar. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMAviationVerticalScaleBar 

|Property | Type | Description | 
|---------|--------|--------|
| verticalLineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol for the vertical line of the scale bar. 
| feetScale | [CIMAviationVerticalScaleProperties](CIMLayout.md#cimaviationverticalscaleproperties) | The feet scale properties for the vertical scale bar. 
| meterScale | [CIMAviationVerticalScaleProperties](CIMLayout.md#cimaviationverticalscaleproperties) | The meters scale properties for the vertical scale bar. 
| divisionMarkHeight | double | The division marker's height. 
| divisionsBeforeZero | boolean | A value indicating whether to show division symbols before zero. 
| feetOnRight | boolean | A value indicating whether to show feet on the right, if false will show feet on the left and meters on the right. 






## CIMAviationVerticalScaleProperties
#### Represents a set of scale properties for aviation-specific Vertical Scale Bar, such as a feet scale or meter scale properties. 


### CIMAviationVerticalScaleProperties 

|Property | Type | Description | 
|---------|--------|--------|
| unitTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol used for the scale unit. 
| divisionMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol for the divisions. 
| subdivisionMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol for the subdivisions. 
| scaleTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for the scale values. 
| scaleBarHeight | double | The height for the scale bar. 
| divisionLineLength | double | The division line length for the scale bar. The units are in points. 
| subdivisionLineLength | double | The subdivision line length for the scale bar. The units are in points. 
| scaleUnitText | string | The string value for the scale unit text. 
| divisions | long | The division count for the scale. 
| subdivisions | long | The subdivision count for the scale. 
| visible | boolean | A value indicating whether to show this scale, if false no graphics will be shown. 






## CIMBookmarkMapSeries
#### Bookmark map series is a means to create a series of map pages based on saved bookmarks. 


### CIMMapSeries 

|Property | Type | Description | 
|---------|--------|--------|
| enabled | boolean | A value indicating whether the map series is enabled on the layout. 
| mapFrameName | string | The URI of the MapFrame to which MapSeries is linked. 
| startingPageNumber | long | The starting page number. 
| currentPageID | long long | The current page Id. 


### CIMBookmarkMapSeries 

|Property | Type | Description | 
|---------|--------|--------|
| pages | [[CIMBookmarkMapSeriesPage]](CIMLayout.md#cimbookmarkmapseriespage) | The pages. 
| scaleRounding | double | The specified value to which the scale rounds. 
| extentOptions | [enumeration ExtentFitType](CIMLayout.md#enumeration-extentfittype) | The extent fitting options. 
| marginType | [enumeration UnitType](CIMLayout.md#enumeration-unittype) | The type of margin. 
| marginUnits | [LinearUnit](ExternalReferences.md#linearunit) | The units of the margin. 
| margin | double | The value of the margin. 






## CIMBookmarkMapSeriesPage
#### A map series page based on a bookmark. 


### CIMBookmarkMapSeriesPage 

|Property | Type | Description | 
|---------|--------|--------|
| bookmarkName | string | The bookmark. 
| mapURI | string | The map. 
| category | string | The category. Category lets you organize your pages into groups. 






## CIMChartFrame
#### Layout element used to display a chart. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMChartFrame 

|Property | Type | Description | 
|---------|--------|--------|
| mapMemberURI | string | The layer or standalone table that defines the data to display. 
| chartName | string | The chart to display. 
| isDynamic | boolean | A value indicating whether the chart is dynamic. 
| useMapSeriesShape | boolean | A value indicating whether the chart uses the map series shape. 






## CIMCondensedTabGridLine
#### Defines a condensed tab. 


### CIMGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | Name of the grid line. 
| elementType | [enumeration GridElementType](CIMLayout.md#enumeration-gridelementtype) | The type of the graticule element. 
| gridLineOrientation | [enumeration GridLineOrientation](CIMLayout.md#enumeration-gridlineorientation) | The orientation of the gridLine with reference to the coordinate system of the spatial reference. For graticules it is latitudes and longitudes. For grids it is eastings and northings. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | Symbol of the grid line. 
| pattern | [CIMGridPattern](CIMLayout.md#cimgridpattern) | The pattern of the grid lines. 
| fromTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick) | The properties of the tick that is at the start of the grid line it represents. 
| toTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick) | The properties of the tick that is at the end of the grid line it represents. 
| interiorTicks | [[CIMInteriorTick]](CIMLayout.md#ciminteriortick) | The properties of the interior ticks for a grid line. 
| visibleIndices | [long] | The visibility of the corner labels to edges by index. 


### CIMTabGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| alternatingSymbols | boolean | A value indicating whether symbols for the tab are alternating. 
| alternatingSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The alternating symbol. 
| height | double | The height of the tab. The height in defined in page units. 


### CIMCondensedTabGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| width | double | The width of the tab. The width is in page units. 
| condensedTab | [enumeration CondensedTabType](CIMLayout.md#enumeration-condensedtabtype) | The type of condensed tab. 





### Enumeration: CondensedTabType
#### Defines the type of condensed tab. 

|Property | Value | Description | 
|---------|--------|--------|
| Round| 0| Defines a rounded condensed tab. 
| Rectangle| 1| Defines a rectangular condensed tab. 
| RoundedRectangle| 2| Defines a rounded rectangle condensed tab. 




## CIMContiguousTabGridLine
#### Defines a contiguous tab for a referenced grid. 


### CIMGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | Name of the grid line. 
| elementType | [enumeration GridElementType](CIMLayout.md#enumeration-gridelementtype) | The type of the graticule element. 
| gridLineOrientation | [enumeration GridLineOrientation](CIMLayout.md#enumeration-gridlineorientation) | The orientation of the gridLine with reference to the coordinate system of the spatial reference. For graticules it is latitudes and longitudes. For grids it is eastings and northings. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | Symbol of the grid line. 
| pattern | [CIMGridPattern](CIMLayout.md#cimgridpattern) | The pattern of the grid lines. 
| fromTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick) | The properties of the tick that is at the start of the grid line it represents. 
| toTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick) | The properties of the tick that is at the end of the grid line it represents. 
| interiorTicks | [[CIMInteriorTick]](CIMLayout.md#ciminteriortick) | The properties of the interior ticks for a grid line. 
| visibleIndices | [long] | The visibility of the corner labels to edges by index. 


### CIMTabGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| alternatingSymbols | boolean | A value indicating whether symbols for the tab are alternating. 
| alternatingSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The alternating symbol. 
| height | double | The height of the tab. The height in defined in page units. 


### CIMContiguousTabGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| contiguousTab | [enumeration ContiguousTabType](CIMLayout.md#enumeration-contiguoustabtype) | The contiguous tab type. 





### Enumeration: ContiguousTabType
#### Represents a type of contiguous tabs. 

|Property | Value | Description | 
|---------|--------|--------|
| Continuous| 0| Represents a continuous tab. 
| Rounded| 1| Represents a rounded tab. 
| Squared| 2| Represents a squared tab. 




## CIMCruisingAltitudeDiagram
#### Represents a Cruising Altitude Diagram. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMCruisingAltitudeDiagram 

|Property | Type | Description | 
|---------|--------|--------|
| diagramType | [enumeration CruisingAltitudeDiagramType](CIMLayout.md#enumeration-cruisingaltitudediagramtype) | The diagram type which should be created. 
| altitudeTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol used for the altitude values on the diagram. 
| bearingTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol used for the bearing values for each part of the diagram. 
| titleTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol used for the diagram title, which appears above the element. 
| bearingArrowLineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol used for the arrow that leads from the starting bearing to the ending bearing for a part of the diagram. 
| lineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol used for the outline of the circle sections on the diagram. 
| diameterUnits | [LinearUnit](ExternalReferences.md#linearunit) | The page units used to determine the diameter of the cruising altitude diagram. 
| diagramDiameter | double | The diameter of the cruising altitude diagram in page units. 
| diagramTitle | string | The text for the diagram title. 
| verticalLeftText | string | The text for the left side of the vertical diagram. 
| verticalRightText | string | The text for the right side of the vertical diagram. 
| horizontalTopText | string | The text for the top of the horizontal diagram. 
| horizontalBottomText | string | The text for the bottom of the horizontal diagram. 
| quadrantalTopLeftText | string | The text for the top left of the quadrantal diagram. 
| quadrantalTopRightText | string | The text for the top right of the quadrantal diagram. 
| quadrantalBottomLeftText | string | The text for the bottom left of the quadrantal diagram. 
| quadrantalBottomRightText | string | The text for the bottom right of the quadrantal diagram. 
| autoResizeText | boolean | A value indicating whether to auto resize the text. 





### Enumeration: CruisingAltitudeDiagramType
#### A list of Cruising Altitude Diagram types. 

|Property | Value | Description | 
|---------|--------|--------|
| Vertical| 1| Vertical. 
| Horizontal| 2| Horizontal. 
| Quadrantal| 3| Quadrantal. 




## CIMCustomGrid
#### Represents a custom grid of the mapFrame. 


### CIMMapGrid 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the Grid or Graticule. 
| isVisible | boolean | A value indicating whether the grid or graticule is visible. 
| neatlineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The neat line symbol of the Grid or Graticule. 
| maxInteriorAngle | double | The maximum value of the interior angle that determines the edge of the mapFrame polygon. The angle is defined in degrees. 
| edgeMinimumLength | double | The minimum length of the edge of the mapFrame polygon in page units. 
| mapGridEdges | [[CIMMapGridEdge]](CIMLayout.md#cimmapgridedge) | The map grid edges. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMCustomGrid 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string | The path to the layer used to define the grid lines. 
| gridLines | [[CIMGridLine]](Types.md#gridline) | The gridLines of the custom grid. These are limited to ticks, labels, and tabs. 
| useMapClipShape | boolean | A value indicating whether to use the clip shape of the map (if set) as the grid boundary. 






## CIMCustomGridLabelTemplate
#### Defines the label template for custom grids. 


### CIMGridLabelTemplate 

|Property | Type | Description | 
|---------|--------|--------|


### CIMCustomGridLabelTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| labelExpressionInfo | [CIMExpressionInfo](CIMRenderers.md#cimexpressioninfo) | The label expression. Either a simple field name or an Arcade expression. 
| edgeLabelAngles | [double] | The list of label angles to set the text symbol angle for each grid edge. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol of the label. 






## CIMDeclination
#### Represents the properties of a declination calculated using World Magnetic Model. 


### CIMDeclination 

|Property | Type | Description | 
|---------|--------|--------|
| direction | [enumeration DeclinationDirection](CIMLayout.md#enumeration-declinationdirection) | The direction the declination is reckoned from. 
| degrees | long | The degrees of declination. 
| minutes | long | The minutes of declination. 
| mils | double | The mil radians of declination. 





### Enumeration: DeclinationDirection
#### Defines which direction declination will be calculated from. 

|Property | Value | Description | 
|---------|--------|--------|
| West| 0| Declination reckoned West (counterclockwise) 
| East| 1| Declination reckoned East (clockwise) 




## CIMDoubleFillScaleBar
#### Represents a double filled alternating scale bar. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMScaleBar 

|Property | Type | Description | 
|---------|--------|--------|
| alignToZeroPoint | boolean | A value indicating whether the scale bar should align to zero. 
| barHeight | double | The scale bar height. 
| division | double | The division value. 
| divisions | long | The number of divisions. 
| divisionsBeforeZero | long | The number of divisions before zero. 
| fittingStrategy | [enumeration ScaleBarFittingStrategy](CIMLayout.md#enumeration-scalebarfittingstrategy) | The fitting strategy. 
| labelFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency) | The label frequency. 
| labelGap | double | The label gap value. 
| labelPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition) | The label position. 
| labelSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | Label symbol. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| subdivisions | long | The number of subdivisions. 
| unitLabel | string | The unit label. 
| unitLabelGap | double | The unit label gap. Units set in points. 
| unitLabelPosition | [enumeration ScaleBarLabelPosition](CIMLayout.md#enumeration-scalebarlabelposition) | The unit label position. 
| unitLabelSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The unit label symbol. 
| units | [Unit](ExternalReferences.md#unit) | The units for the scale bar. 
| useFractionCharacters | boolean | A value indicating whether fractional characters should be used. 
| zeroPoint | [Point](ExternalReferences.md#point) | The zero location for the scale bar. 
| computeAtCenter | boolean | A value indicating whether to compute the scale at map center. 
| displayFirstOutside | boolean | A value indicating whether to display the first numeric value outside the bar. 
| displayLastOutside | boolean | A value indicating whether to display the last numeric value outside the bar. 
| barWidth | double | The width of the scalebar. 


### CIMScaleMarks 

|Property | Type | Description | 
|---------|--------|--------|
| divisionMarkHeight | double | The division mark height value. 
| divisionMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The division mark line symbol. 
| markFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency) | The division mark frequency. 
| markPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition) | The division mark position. 
| subdivisionMarkHeight | double | The subdivision mark height. 
| subdivisionMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The subdivision mark line symbol. 
| midpointMarkHeight | double | The midpoint mark height. 
| midpointMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The midpoint mark line symbol. 


### CIMDoubleFillScaleBar 

|Property | Type | Description | 
|---------|--------|--------|
| fillSymbol1 | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The first symbol of an alternating scale bar. 
| fillSymbol2 | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The second symbol of an alternating scale bar. 
| style | [enumeration DoubleFillScaleBarStyle](CIMLayout.md#enumeration-doublefillscalebarstyle) | The style for the scale bar. 





### Enumeration: DoubleFillScaleBarStyle
#### A list of the styles available for a double file scale bar. 

|Property | Value | Description | 
|---------|--------|--------|
| Hollow| 0| Hollow fill. 
| Alternating| 1| Alternating fill. 
| DoubleAlternating| 2| Double alternating fill. 




## CIMDualScaleBar
#### Represents a dual scale bar on a page layout. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMScaleBar 

|Property | Type | Description | 
|---------|--------|--------|
| alignToZeroPoint | boolean | A value indicating whether the scale bar should align to zero. 
| barHeight | double | The scale bar height. 
| division | double | The division value. 
| divisions | long | The number of divisions. 
| divisionsBeforeZero | long | The number of divisions before zero. 
| fittingStrategy | [enumeration ScaleBarFittingStrategy](CIMLayout.md#enumeration-scalebarfittingstrategy) | The fitting strategy. 
| labelFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency) | The label frequency. 
| labelGap | double | The label gap value. 
| labelPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition) | The label position. 
| labelSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | Label symbol. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| subdivisions | long | The number of subdivisions. 
| unitLabel | string | The unit label. 
| unitLabelGap | double | The unit label gap. Units set in points. 
| unitLabelPosition | [enumeration ScaleBarLabelPosition](CIMLayout.md#enumeration-scalebarlabelposition) | The unit label position. 
| unitLabelSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The unit label symbol. 
| units | [Unit](ExternalReferences.md#unit) | The units for the scale bar. 
| useFractionCharacters | boolean | A value indicating whether fractional characters should be used. 
| zeroPoint | [Point](ExternalReferences.md#point) | The zero location for the scale bar. 
| computeAtCenter | boolean | A value indicating whether to compute the scale at map center. 
| displayFirstOutside | boolean | A value indicating whether to display the first numeric value outside the bar. 
| displayLastOutside | boolean | A value indicating whether to display the last numeric value outside the bar. 
| barWidth | double | The width of the scalebar. 


### CIMScaleMarks 

|Property | Type | Description | 
|---------|--------|--------|
| divisionMarkHeight | double | The division mark height value. 
| divisionMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The division mark line symbol. 
| markFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency) | The division mark frequency. 
| markPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition) | The division mark position. 
| subdivisionMarkHeight | double | The subdivision mark height. 
| subdivisionMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The subdivision mark line symbol. 
| midpointMarkHeight | double | The midpoint mark height. 
| midpointMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The midpoint mark line symbol. 


### CIMDualScaleBar 

|Property | Type | Description | 
|---------|--------|--------|
| upperScaleBar | [ScaleBar](Types.md#scalebar) | The upper scale bar of the dual scale bar. 
| lowerScaleBar | [ScaleBar](Types.md#scalebar) | The lower scale bar of the dual scale bar. 
| unitLabelVerticalGap | double | The unit label vertical gap. Units set in points. 





### Enumeration: EndPointPosition
#### Enumerates which end a component is visible. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No end point is selected 
| FromPoint| 1| From point. 
| ToPoint| 2| To point. 



### Enumeration: EndPointSelection
#### Represents the selection of endPoints. 

|Property | Value | Description | 
|---------|--------|--------|
| First| 1| First point selection. 
| Interior| 2| Interior point selection. 
| Last| 4| Last point selection. 



### Enumeration: ExtentFitType
#### Extent fit types. 

|Property | Value | Description | 
|---------|--------|--------|
| BestFit| 0| Best fit. 
| ExtentCenter| 1| Center the extent. 
| DataDriven| 2| Data driven. 




## CIMExtentIndicator
#### Represents an extent indicator which is used to display the visible extent of other map frames in an associated map frame. 


### CIMExtentIndicator 

|Property | Type | Description | 
|---------|--------|--------|
| sourceMapFrame | string | The source map frame's extent to be displayed. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The area symbol used to represent the extent indicator. 
| leaderType | [enumeration LeaderType](CIMLayout.md#enumeration-leadertype) | The leader style used to connect the associated extents. 
| leaderSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The leader symbol used to connect the associated extents. 
| collapseSize | double | The minimum size of the extent indicator before symbolizing it as a point. Units in points. 
| pointSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The point symbol used to symbolize an extent indicator. 
| name | string | The name of the extent indicator. 
| isVisible | boolean | A value indicating whether the extent indicator is visible. 
| avoidLabelConflict | boolean | A value indicating whether to avoid label conflict. Reserved for future implementation. 
| symbolizeExterior | boolean | A value indicating whether the area symbol should be applied outside the extent. 
| extentIndicatorType | [enumeration ExtentIndicatorType](CIMLayout.md#enumeration-extentindicatortype) | The extent indicator type. Reserved for future implementation at this time. 





### Enumeration: ExtentIndicatorType
#### Future implementation. 

|Property | Value | Description | 
|---------|--------|--------|
| Frame| 0| Future implementation 
| Rectangle| 1| Future implementation 
| IndexFeatureFromDDP| 2| Future implementation 




## CIMExteriorTick
#### Class that represents an exterior tick for a grid. 


### CIMTick 

|Property | Type | Description | 
|---------|--------|--------|
| length | double | The length of the tick in page units. 
| offset | double | The offset of the tick in page units. 
| isVisible | boolean | A value indicating whether the tick is visible. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol for the tick. 
| gridEndpoint | [CIMGridEndpoint](CIMLayout.md#cimgridendpoint) | The end point for the tick. 


### CIMExteriorTick 

|Property | Type | Description | 
|---------|--------|--------|
| edgeAffinity | [long] | The collection of edges the ticks or the labels draw on. If the collection is empty, the drawing is made on the entire area of interest. 
| drawPerpendicular | boolean | A value indicating whether to the draw the ticks perpendicular to the map grid edges. 





### Enumeration: FieldSortInfo
#### Represents the sort information for a field. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Field is not sorted. 
| Asc| 1| The field is sorted by case insensitive ascending order. 
| AscCase| 2| The field is sorted by case sensitive ascending order. 
| Desc| 4| The field is sorted by case insensitive descending order. 
| DescCase| 8| The field is sorted by case sensitive descending order. 



### Enumeration: FieldStatisticsFlag
#### Represents field statistics. 

|Property | Value | Description | 
|---------|--------|--------|
| NoStatistics| 0| No statistics calculated. 
| Count| 1| The count of all field values. 
| Minimum| 2| The maximum field value. 
| Maximum| 4| The minimum field value. 
| Range| 8| The difference between the maximum and minimum field values. 
| Sum| 16| The sum of all field values. 
| Mean| 32| The average of all field values. 
| Median| 64| The middle value of all field values. 
| Mode| 128| The most common value of all field values. 
| StandardDeviation| 256| The standard deviation of the field values. 




## CIMGZDLabelGridLine
#### Represents a UTM Grid Zone Designator Label definition for a MapGrid. 


### CIMGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | Name of the grid line. 
| elementType | [enumeration GridElementType](CIMLayout.md#enumeration-gridelementtype) | The type of the graticule element. 
| gridLineOrientation | [enumeration GridLineOrientation](CIMLayout.md#enumeration-gridlineorientation) | The orientation of the gridLine with reference to the coordinate system of the spatial reference. For graticules it is latitudes and longitudes. For grids it is eastings and northings. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | Symbol of the grid line. 
| pattern | [CIMGridPattern](CIMLayout.md#cimgridpattern) | The pattern of the grid lines. 
| fromTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick) | The properties of the tick that is at the start of the grid line it represents. 
| toTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick) | The properties of the tick that is at the end of the grid line it represents. 
| interiorTicks | [[CIMInteriorTick]](CIMLayout.md#ciminteriortick) | The properties of the interior ticks for a grid line. 
| visibleIndices | [long] | The visibility of the corner labels to edges by index. 


### CIMGZDLabelGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| dynamicStringTemplate | string | The dynamic string used to represent the GZD label of the map grid. 
| verticalTopPosition | [CIMGridZoneLabelPosition](CIMLayout.md#cimgridzonelabelposition) | The vertical position of the GZD label at the top of each UTM grid zone. 
| verticalCenterPosition | [CIMGridZoneLabelPosition](CIMLayout.md#cimgridzonelabelposition) | The vertical position of the GZD label at the center of each UTM grid zone. 
| verticalBottomPosition | [CIMGridZoneLabelPosition](CIMLayout.md#cimgridzonelabelposition) | The vertical position of the GZD label at the bottom of each UTM grid zone. 
| horizontalLeftPosition | [CIMGridZoneLabelPosition](CIMLayout.md#cimgridzonelabelposition) | The horizontal position of the GZD label at the left of each UTM grid zone. 
| horizontalCenterPosition | [CIMGridZoneLabelPosition](CIMLayout.md#cimgridzonelabelposition) | The horizontal position of the GZD label at the center of each UTM grid zone. 
| horizontalRightPosition | [CIMGridZoneLabelPosition](CIMLayout.md#cimgridzonelabelposition) | The horizontal position of the GZD label at the right of each UTM grid zone. 






## CIMGlossaryTable
#### Represents a glossary table for map product surround elements. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMMapProductSurround 

|Property | Type | Description | 
|---------|--------|--------|
| autoUpdate | boolean | A value indicating whether properties of the surround should update automatically based on changes in the map. 
| productSpecification | [enumeration MapProductSpecType](CIMLayout.md#enumeration-mapproductspectype) | The map product specification type of the surround. 
| drawToSpecification | boolean | A value indicating whether to draw the element to specification size or allow user to manually resize element. 


### CIMGlossaryTable 

|Property | Type | Description | 
|---------|--------|--------|
| fittingStrategy | [enumeration TableFrameFittingStrategy](CIMLayout.md#enumeration-tableframefittingstrategy) | The fitting strategy. 
| mapMemberURI | string | The URI to a Layer or Standalone table in the project. 
| fields | [[CIMTableFrameField]](CIMLayout.md#cimtableframefield) | The fields displayed in the glossary table. 
| title | string | The title of the element. 
| titleTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for title text. 
| rightToLeft | boolean | A value indicating whether right to left orientation should be applied. 
| minFontSize | double | The limit when reducing font sizes. Values are in points. 
| titleGap | double | The gap between title and column headings. Values are in points. 
| headingGap | double | The gap between column headings and rows. Values are in points. 
| rowGap | double | The gap between rows. Values are in points. 
| horizontalTextGap | double | The horizontal gap around field values. Values are in points. 
| verticalTextGap | double | The vertical gap around field values. Values are in points. 
| delimiterCharacter | string | The delimiter character that is displayed between columns. 
| delimiterTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for the delimiter displayed between columns. 






## CIMGraphicElement
#### Represents the CIM representation of an element on a page layout. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMGraphicElement 

|Property | Type | Description | 
|---------|--------|--------|
| graphic | [Graphic](Types.md#graphic) | The CIMGraphic for an element on a page layout. 






## CIMGraticule
#### Represents a graticule for a map frame. 


### CIMMapGrid 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the Grid or Graticule. 
| isVisible | boolean | A value indicating whether the grid or graticule is visible. 
| neatlineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The neat line symbol of the Grid or Graticule. 
| maxInteriorAngle | double | The maximum value of the interior angle that determines the edge of the mapFrame polygon. The angle is defined in degrees. 
| edgeMinimumLength | double | The minimum length of the edge of the mapFrame polygon in page units. 
| mapGridEdges | [[CIMMapGridEdge]](CIMLayout.md#cimmapgridedge) | The map grid edges. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMGraticule 

|Property | Type | Description | 
|---------|--------|--------|
| customOrigin | [Point](ExternalReferences.md#point) | The custom origin of a graticule. 
| geographicCoordinateSystem | [GeographicCoordinateSystem](ExternalReferences.md#geographiccoordinatesystem) | The spatial reference of a graticule. 
| gridLines | [[CIMGridLine]](Types.md#gridline) | The collection of latitudes and longitudes for a graticule. 
| isAutoScaled | boolean | A value indicating whether to automatically adjust the interval of the graticules based on scale of the map. 
| useMapClipShape | boolean | A value indicating whether to use the clip shape of the map (if set) as the grid boundary. 





### Enumeration: GridElementType
#### The type of component of the grid. 

|Property | Value | Description | 
|---------|--------|--------|
| Line| 0| Represents lines. 
| Tick| 1| Represents ticks. 
| Label| 2| Represents labels. 
| Corner| 3| Represents the corner label. 
| IntersectionPoint| 4| Represents a grid component used to show intersection points on a map grid. 




## CIMGridEndpoint
#### Represents an end point of a component. For ex: The labels for ticks are defined using an endPoint object. 


### CIMGridEndpoint 

|Property | Type | Description | 
|---------|--------|--------|
| gridLabelTemplate | [GridLabelTemplate](Types.md#gridlabeltemplate) | The grid label template for each endpoint. 
| offset | double | The offset of the labels. 
| position | long | The position of the labels of the end points. 
| lineSelection | long | The end point selection. 
| drawLabelsParallel | boolean | A value indicating whether to draw the labels parallel to the map grid edges. 





### Enumeration: GridLadderLabelPosition
#### Represents the position at which the ladder labels are drawn. 

|Property | Value | Description | 
|---------|--------|--------|
| Half| 0| Represents the ladder label at half the value of visible extent. 
| Third| 1| Represents the ladder label at third of the value of visible extent. 
| Quarter| 2| Represents the ladder label at quarter the value of visible extent. 




## CIMGridLine
#### Represents latitudes or longitudes for a graticule. Represents eastings or nothings for a grid. 


### CIMGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | Name of the grid line. 
| elementType | [enumeration GridElementType](CIMLayout.md#enumeration-gridelementtype) | The type of the graticule element. 
| gridLineOrientation | [enumeration GridLineOrientation](CIMLayout.md#enumeration-gridlineorientation) | The orientation of the gridLine with reference to the coordinate system of the spatial reference. For graticules it is latitudes and longitudes. For grids it is eastings and northings. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | Symbol of the grid line. 
| pattern | [CIMGridPattern](CIMLayout.md#cimgridpattern) | The pattern of the grid lines. 
| fromTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick) | The properties of the tick that is at the start of the grid line it represents. 
| toTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick) | The properties of the tick that is at the end of the grid line it represents. 
| interiorTicks | [[CIMInteriorTick]](CIMLayout.md#ciminteriortick) | The properties of the interior ticks for a grid line. 
| visibleIndices | [long] | The visibility of the corner labels to edges by index. 





### Enumeration: GridLineOrientation
#### Represents the orientation of the grid line. 

|Property | Value | Description | 
|---------|--------|--------|
| NorthSouth| 0| North-South 
| EastWest| 1| East-West 




## CIMGridPattern
#### Defines pattern for a component. 


### CIMGridPattern 

|Property | Type | Description | 
|---------|--------|--------|
| interval | double | The interval of the component the pattern represents. 
| start | double | The start pattern of the component. 
| stop | double | The stop pattern of the component. 
| gap | double | The gap pattern of the component. 





### Enumeration: GridReferencePrecisionLevel
#### List of precision levels for Military Grid Reference System (MGRS). 

|Property | Value | Description | 
|---------|--------|--------|
| GridZoneDesignator| 0| Grid zone designator. 
| PrecisionLevel100km| 1| Precision level 100 km. 
| PrecisionLevel10km| 2| Precision level 10 km. 
| PrecisionLevel1km| 3| Precision level 1 km. 
| PrecisionLevel100m| 4| Precision level 100 m. 
| PrecisionLevel10m| 5| Precision level 10 m. 
| PrecisionLevel1m| 6| Precision level 1 m. 
| ICM| 7| Custom MGRS precision for Image City Map(ICM). 




## CIMGridZoneLabelPosition
#### Represents the state of a label at a given position on a MapGrid. 


### CIMGridZoneLabelPosition 

|Property | Type | Description | 
|---------|--------|--------|
| visible | boolean | A value indicating whether the label at this position is visible. 
| offsetX | double | The offset in the X-Coordinate direction between the label and grid components. 
| offsetY | double | The offset in the Y-Coordinate direction between the label and grid components. 






## CIMGroupElement
#### Represents a collection of layout elements in a group element. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 






## CIMGroupFooter
#### Represents a group footer section in a report. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReportSectionElement 

|Property | Type | Description | 
|---------|--------|--------|
| autoSize | boolean | A value indicating whether the section height will grow and shrink to fit the content of the section. 
| elementFieldProperties | [[CIMReportElementFieldProperties]](Types.md#reportelementfieldproperties) | The field properties that will be applied to the elements. 
| excludePageNumberPages | string | The comma delimited list of pages to exclude the page number from. 
| excludeSectionPages | string | The comma delimited list of pages to exclude the section from. 
| startOnNewPage | boolean | A value indicating whether the section should start on a new page. 
| autoGrowTextElements | boolean | A value indicating whether the height of Text elements in sections will grow based on their content. 


### CIMGroupFooter 

|Property | Type | Description | 
|---------|--------|--------|
| field | string | The grouping field for the section. 
| alignSubsectionToBottom | boolean | A value indicating whether to force the subsection to export at the bottom of the page. 






## CIMGroupHeader
#### Represents a group header section in a report. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReportSectionElement 

|Property | Type | Description | 
|---------|--------|--------|
| autoSize | boolean | A value indicating whether the section height will grow and shrink to fit the content of the section. 
| elementFieldProperties | [[CIMReportElementFieldProperties]](Types.md#reportelementfieldproperties) | The field properties that will be applied to the elements. 
| excludePageNumberPages | string | The comma delimited list of pages to exclude the page number from. 
| excludeSectionPages | string | The comma delimited list of pages to exclude the section from. 
| startOnNewPage | boolean | A value indicating whether the section should start on a new page. 
| autoGrowTextElements | boolean | A value indicating whether the height of Text elements in sections will grow based on their content. 


### CIMGroupHeader 

|Property | Type | Description | 
|---------|--------|--------|
| field | string | The grouping field for the section. 
| repeatOnEveryPage | boolean | A value indicating whether the section should be displayed on every page. 






## CIMGuide
#### Represents a guide used to snap elements on a page layout. 


### CIMGuide 

|Property | Type | Description | 
|---------|--------|--------|
| position | double | The position of the guide. 
| orientation | [enumeration Orientation](CIMLayout.md#enumeration-orientation) | The horizontal or vertical orientation of the guide. 






## CIMHorizontalBarLegendItem
#### Represents a horizontal bar legend item. 


### CIMLegendItem 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The legend item name. 
| newColumn | boolean | A value indicating whether a legend item should be placed in a new column. 
| layerNameSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item symbol. 
| manualColumn | long | The manual column assignment for a legend item. 
| keepTogetherOption | [enumeration LegendKeepTogetherOption](CIMLayout.md#enumeration-legendkeeptogetheroption) | A value indicating whether the legend item or group should be kept together. 
| showLayerName | boolean | A value indicating whether the legend item layer name should be displayed. 
| showHeading | boolean | A value indicating whether the legend item heading should be displayed. 
| headingSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item heading symbol. 
| showLabels | boolean | A value indicating whether the legend item labels should be displayed. 
| layer | string | The legend item layer's path. 
| showDescription | boolean | A value indicating whether a legend item description should be displayed. 
| labelSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item label symbol. 
| descriptionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item description symbol. 
| patchWidth | double | The legend item patch width. Units in points. 
| patchHeight | double | The legend item patch height. Units in points. 
| autoVisibility | boolean | A value indicating whether the legend item should be displayed if in the visible extent. 
| useMapSeriesShape | boolean | A value indicating whether to use map series shape instead of map frame to find dynamic classes. 
| classIndent | double | Distance from the class name to the edge of the legend. 
| headingIndent | double | Distance from the heading to the edge of the legend. 
| layerNameIndent | double | Distance of the layer name to the edge of the legend. 
| showGroupLayerName | boolean | A value indicating whether to show the containing group layer name above the item. 
| groupLayerNameSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used to display the group layer name. 
| scaleToPatch | boolean | A value indicating whether to scale the symbol to the specified patch size. 
| showCounts | boolean | A value indicating whether the legend should display count statistics. 
| countFormat | [NumberFormat](Types.md#numberformat) | The feature count format. 
| countPrefix | string | The feature count prefix. 
| countSuffix | string | The feature count suffix. 
| isVisible | boolean | A value indicating whether the legend item is visible. 
| groupFilter | [long] | A value specifying which legend groups are displayed. 


### CIMLegendItemArrangement 

|Property | Type | Description | 
|---------|--------|--------|
| arrangement | [enumeration LegendItemArrangement](Types.md#enumeration-legenditemarrangement) | The Arrangement. 


### CIMHorizontalBarLegendItem 

|Property | Type | Description | 
|---------|--------|--------|
| angleAbove | double | The angle above. Reserved for future implementation. 
| angleBelow | double | The angle below. Reserved for future implementation. 
| patchAlignment | [enumeration VerticalAlignment](CIMSymbols.md#enumeration-verticalalignment) | A value that allows alignment of graduated symbols to be specified. 


### CIMLegendItemLeader 

|Property | Type | Description | 
|---------|--------|--------|
| lineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol for a legend item leader. 
| lineLength | double | The line length for a legend item leader. 






## CIMHorizontalLegendItem
#### Represents a horizontal legend item. 


### CIMLegendItem 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The legend item name. 
| newColumn | boolean | A value indicating whether a legend item should be placed in a new column. 
| layerNameSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item symbol. 
| manualColumn | long | The manual column assignment for a legend item. 
| keepTogetherOption | [enumeration LegendKeepTogetherOption](CIMLayout.md#enumeration-legendkeeptogetheroption) | A value indicating whether the legend item or group should be kept together. 
| showLayerName | boolean | A value indicating whether the legend item layer name should be displayed. 
| showHeading | boolean | A value indicating whether the legend item heading should be displayed. 
| headingSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item heading symbol. 
| showLabels | boolean | A value indicating whether the legend item labels should be displayed. 
| layer | string | The legend item layer's path. 
| showDescription | boolean | A value indicating whether a legend item description should be displayed. 
| labelSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item label symbol. 
| descriptionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item description symbol. 
| patchWidth | double | The legend item patch width. Units in points. 
| patchHeight | double | The legend item patch height. Units in points. 
| autoVisibility | boolean | A value indicating whether the legend item should be displayed if in the visible extent. 
| useMapSeriesShape | boolean | A value indicating whether to use map series shape instead of map frame to find dynamic classes. 
| classIndent | double | Distance from the class name to the edge of the legend. 
| headingIndent | double | Distance from the heading to the edge of the legend. 
| layerNameIndent | double | Distance of the layer name to the edge of the legend. 
| showGroupLayerName | boolean | A value indicating whether to show the containing group layer name above the item. 
| groupLayerNameSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used to display the group layer name. 
| scaleToPatch | boolean | A value indicating whether to scale the symbol to the specified patch size. 
| showCounts | boolean | A value indicating whether the legend should display count statistics. 
| countFormat | [NumberFormat](Types.md#numberformat) | The feature count format. 
| countPrefix | string | The feature count prefix. 
| countSuffix | string | The feature count suffix. 
| isVisible | boolean | A value indicating whether the legend item is visible. 
| groupFilter | [long] | A value specifying which legend groups are displayed. 


### CIMLegendItemArrangement 

|Property | Type | Description | 
|---------|--------|--------|
| arrangement | [enumeration LegendItemArrangement](Types.md#enumeration-legenditemarrangement) | The Arrangement. 


### CIMHorizontalLegendItem 

|Property | Type | Description | 
|---------|--------|--------|






## CIMInteriorTick
#### Class that represents an interior tick for a grid. 


### CIMTick 

|Property | Type | Description | 
|---------|--------|--------|
| length | double | The length of the tick in page units. 
| offset | double | The offset of the tick in page units. 
| isVisible | boolean | A value indicating whether the tick is visible. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol for the tick. 
| gridEndpoint | [CIMGridEndpoint](CIMLayout.md#cimgridendpoint) | The end point for the tick. 


### CIMInteriorTick 

|Property | Type | Description | 
|---------|--------|--------|
| pattern | [CIMGridPattern](CIMLayout.md#cimgridpattern) | The pattern for the interior ticks. 
| indicateDirection | boolean | A value indicating whether the ticks show the direction away from the origin. If false, the ticks bisect the center of the grid line. 






## CIMLadderGridLine
#### Represents internal labels for a MapGrid. 


### CIMGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | Name of the grid line. 
| elementType | [enumeration GridElementType](CIMLayout.md#enumeration-gridelementtype) | The type of the graticule element. 
| gridLineOrientation | [enumeration GridLineOrientation](CIMLayout.md#enumeration-gridlineorientation) | The orientation of the gridLine with reference to the coordinate system of the spatial reference. For graticules it is latitudes and longitudes. For grids it is eastings and northings. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | Symbol of the grid line. 
| pattern | [CIMGridPattern](CIMLayout.md#cimgridpattern) | The pattern of the grid lines. 
| fromTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick) | The properties of the tick that is at the start of the grid line it represents. 
| toTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick) | The properties of the tick that is at the end of the grid line it represents. 
| interiorTicks | [[CIMInteriorTick]](CIMLayout.md#ciminteriortick) | The properties of the interior ticks for a grid line. 
| visibleIndices | [long] | The visibility of the corner labels to edges by index. 


### CIMLadderGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| dynamicStringTemplate | string | The dynamic string used to represent the ladder label of the map grid. 
| gapX | double | The gap in the X-Coordinate direction between the label extent and grid components. 
| gapY | double | The gap in the Y-Coordinate direction between the label extent and grid components. 
| position | [enumeration GridLadderLabelPosition](CIMLayout.md#enumeration-gridladderlabelposition) | The position of the ladder labels. 






## CIMLayerOverrideSet
#### Represents a layer property override set. 


### CIMLayerOverrideSet 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string | The path to the associated map layer. 
| value | boolean | A value indicating whether this flag is set. It overrides some arbitrary property on the associated map layer. 






## CIMLayout
#### Represents a layout in a project. A layout is a collection of visual elements arranged on a logical sheet of paper. A layout in a GIS is typically used to display one or more maps at a particular extent and scale. The layout is used to compose a presentation of data, describe the maps, and/or tell a story of the map data. A layout defines a logical sheet of paper. It has a height and a width, and also a linear unit used to display positions on the page. It can have a snapping grid and a set of guides to help users arrange its elements. The layout contains an ordered list of elements. When the layout draws, it tells each element to draw, in order. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the source was last modified, as of the last sync. Used to detect when another sync is needed. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 
| sourcePortalUrl | string | The source portal URI of the item. Set if sourced from an external item such as an item on a portal. 


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMLayoutDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| page | [CIMPage](CIMLayout.md#cimpage) | The CIMPage for the layout. 
| dateExported | [TimeInstant](ExternalReferences.md#timeinstant) | The date exported property for a layout. 
| datePrinted | [TimeInstant](ExternalReferences.md#timeinstant) | The date printed property for a layout. 
| mapSeries | [MapSeries](Types.md#mapseries) | The map series for a layout. 
| colorModel | [enumeration ColorModel](CIMEnumerations.md#enumeration-colormodel) | The color model for a layout. 
| RGBColorProfile | string | The name of the RGB color profile for a layout. 
| CMYKColorProfile | string | The name of the CMYK color profile for a layout. 
| simulateOverprint | boolean | A value indicating whether to simulate overprint for a layout. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layout. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| defaultColorVisionDeficiencyMode | [enumeration ColorVisionDeficiencyType](CIMEnumerations.md#enumeration-colorvisiondeficiencytype) | The color vision deficiency mode that new views of this layout are opened with. 






## CIMLayoutView
#### Represents a layout view in the project. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
| viewableObjectPath | string | The path of the item in the view. 
| viewType | string | The view type as a string. 
| instanceID | long | The instance identifier of this view. 


### CIMLayoutView 

|Property | Type | Description | 
|---------|--------|--------|
| extent | [Envelope](ExternalReferences.md#envelope) | The extent for the view. 
| defaultMapFrameName | string | The default map for a view. 
| pauseDrawing | boolean | A value indicating whether drawing is in the paused state for the view. 
| colorVisionDeficiencyMode | [enumeration ColorVisionDeficiencyType](CIMEnumerations.md#enumeration-colorvisiondeficiencytype) | The color vision deficiency mode of the view. 





### Enumeration: LeaderType
#### A list of leader types for extent indicators. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No leader line. 
| LineToNearestPoint| 1| Shortest line 
| LineToMidpoint| 2| Line to mid-point of the frame. 
| LineThroughCenters| 3| Line from center to center of each extent. 
| CalloutToCenter| 4| Callout to center. 
| CalloutToEdge| 5| Callout to edge. 
| CalloutToEdges| 6| Callout to edges. 




## CIMLegend
#### Represents a legend on a layout. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMLegend 

|Property | Type | Description | 
|---------|--------|--------|
| autoAdd | boolean | A value indicating whether items should automatically be added to the legend. 
| autoFonts | boolean | A value indicating whether legend fonts should automatically be sized. 
| autoReorder | boolean | A value indicating whether the items should automatically be ordered when added. 
| autoVisibility | boolean | A value indicating whether the items should display when not in the visible extent. 
| defaultPatchHeight | double | An items default patch height. Units in points. 
| defaultPatchWidth | double | An items default patch width. Units in points. 
| descriptionWidth | double | The description width threshold. Units in points. 
| groupGap | double | The gap between groups. Units in points. 
| headingGap | double | The heading gap. Units in points. 
| horizontalItemGap | double | The gap between horizontal items. Units in points. 
| patchGap | double | The gap between patches. Units in points. 
| items | [[CIMLegendItem]](Types.md#legenditem) | A collection of items in a layout. 
| labelWidth | double | The label width. Units in points. 
| minFontSize | double | The minimum font size. Units in points. 
| rightToLeft | boolean | A value indicating whether right to left orientation should be applied. 
| scaleSymbols | boolean | A value indicating whether symbols should be scaled. 
| showTitle | boolean | A value indicating whether the legend title should be displayed. 
| textGap | double | The gap between text. Units in points. 
| title | string | The title for the legend. 
| titleGap | double | The title gap. Units in points. 
| titleSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol for the title. 
| itemGap | double | The gap between items. Units in points,. 
| classGap | double | The gap between classes. Units in points. 
| layerNameGap | double | The layer name gap. Units in points. 
| featureCountPrefix | string | The feature count prefix. Deprecated in 1.4. Use count prefix in legend item instead. 
| featureCountSuffix | string | The feature count suffix. Deprecated in 1.4. Use count suffix in legend item instead. 
| fittingStrategy | [enumeration LegendFittingStrategy](CIMLayout.md#enumeration-legendfittingstrategy) | The legends fitting strategy. 
| groupLayerNameGap | double | The gap following the group layer name. 
| columns | long | The number of legend columns when either of the following fitting strategies is in effect: SpecifyColumnsAndAdjustFrame or SpecifyColumnsAndAdjustSize. 
| makeColumnsSameWidth | boolean | A value indicating whether to ensure all the columns are the same width. 
| defaultLegendItem | [LegendItem](Types.md#legenditem) | The default legend item used as the basis for new legend item creation. 
| excludedLayers | [string] | A collection of layer URIs from the associated map that are explicitly excluded from the legend. 
| balanceColumns | boolean | A value indicating whether to balance the columns or simply "pour" the text into each column. 





### Enumeration: LegendFittingStrategy
#### A list of legend fitting strategies. 

|Property | Value | Description | 
|---------|--------|--------|
| AdjustSize| 0| Adjust the size of the text. 
| AdjustColumns| 1| Adjust the number of columns within the frame. 
| AdjustColumnsAndSize| 2| Adjust the number of columns and size of the text. 
| AdjustFrame| 3| Adjust the size of the legend frame. 
| ManualColumns| 4| Adjust the columns manually. 



### Enumeration: LegendItemArrangement
#### A list of legend item arrangement options. 

|Property | Value | Description | 
|---------|--------|--------|
| PatchLabelDescription| 0| Display patch, label, then description. 
| PatchDescriptionLabel| 1| display patch, description, then label. 
| LabelPatchDescription| 2| Display label, patch, then description. 
| LabelDescriptionPatch| 3| Display label, description, then patch. 
| DescriptionPatchLabel| 4| Display description, patch, then label. 
| DescriptionLabelPatch| 5| Display description, label, then patch. 



### Enumeration: LegendKeepTogetherOption
#### A list of choices for keeping legend parts together. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| Don't try to keep parts together. 
| Items| 1| Keep legend items together. 
| Groups| 2| Keep legend groups together. 




## CIMMGRSGridLine
#### Represents a gridLine to draw the 100,000 MGRS grids. 


### CIMGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | Name of the grid line. 
| elementType | [enumeration GridElementType](CIMLayout.md#enumeration-gridelementtype) | The type of the graticule element. 
| gridLineOrientation | [enumeration GridLineOrientation](CIMLayout.md#enumeration-gridlineorientation) | The orientation of the gridLine with reference to the coordinate system of the spatial reference. For graticules it is latitudes and longitudes. For grids it is eastings and northings. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | Symbol of the grid line. 
| pattern | [CIMGridPattern](CIMLayout.md#cimgridpattern) | The pattern of the grid lines. 
| fromTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick) | The properties of the tick that is at the start of the grid line it represents. 
| toTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick) | The properties of the tick that is at the end of the grid line it represents. 
| interiorTicks | [[CIMInteriorTick]](CIMLayout.md#ciminteriortick) | The properties of the interior ticks for a grid line. 
| visibleIndices | [long] | The visibility of the corner labels to edges by index. 


### CIMMGRSGridLine 

|Property | Type | Description | 
|---------|--------|--------|
| XOffset | double | The offset in the x-coordinate direction for the grid label. 
| YOffset | double | The offset in the y-coordinate direction for the grid label. 
| labelPosition | [enumeration MGRSLabelPosition](CIMLayout.md#enumeration-mgrslabelposition) | The position of the label in the 100,000m grid square. 





### Enumeration: MGRSLabelPosition
#### Represents the position of the MGRS label in the 100,000m grid square. 

|Property | Value | Description | 
|---------|--------|--------|
| Corner| 1| Represents the corner position of the label in the 100,000m grid square. 
| Center| 2| Represents the center position of the label in the 100,000m grid square. 




## CIMMapFrame
#### Represents a map frame on a page layout. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapFrame 

|Property | Type | Description | 
|---------|--------|--------|
| autoCamera | [CIMAutoCamera](CIMLayout.md#cimautocamera) | The camera associated with the map frame. 
| URI | string | The path to the map in the project. 
| view | [CIMMapView](CIMDocument.md#cimmapview) | The view associated with the map frame. 
| extentIndicators | [[CIMExtentIndicator]](CIMLayout.md#cimextentindicator) | The extent indicators associated with the map frame. 
| grids | [[CIMMapGrid]](Types.md#mapgrid) | The Grids and Graticules associated with the MapFrame. 
| useMapBackgroundColor | boolean | A value indicating whether the MapFrame should use the Map background color. 
| extentIndicatorsExpanded | boolean | A value indicating whether the map frame extent indicators are expanded in the contents pane. 
| mapGridsExpanded | boolean | A value indicating whether the map frame grids are expanded in the contents pane. 
| overrideLayerVisibility | boolean | A value indicating whether LayerVisibilityOverrides are used to override layer visibility. 
| layerVisibilityOverrides | [[CIMLayerOverrideSet]](CIMLayout.md#cimlayeroverrideset) | The array of layer visibility overrides. 






## CIMMapGridEdge
#### Represents a map grid edge. 


### CIMMapGridEdge 

|Property | Type | Description | 
|---------|--------|--------|
| partIndex | long | The part index of the map grid edge. 
| segmentIndices | [long] | The segment indices of the segments making up the edge. 






## CIMMapProductFeatureGuide
#### Represents the Guide to Numbered (GNF) surround element. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMBaseStreetIndex 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string | The path to the layer containing the features to be indexed. 
| fields | [[CIMTableField]](Types.md#tablefield) | The fields displayed in the street index. 
| titleText | string | The title of the element. 
| titleTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for title text. 
| headerTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for header text. 
| textSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for the features. 
| fittingStrategy | [enumeration TableFrameFittingStrategy](CIMLayout.md#enumeration-tableframefittingstrategy) | The fitting strategy. 
| wrapMethod | [enumeration StreetIndexWrapMethod](CIMLayout.md#enumeration-streetindexwrapmethod) | How the data should wrap across multiple columns. 
| minFontSize | double | The minimum font size. Units in points. 
| headerGap | double | The spacing between headers and data. 
| groupTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for a field that is grouped. 
| groupGap | double | The spacing between group and headers. 
| columns | long | The number of columns allowed to display. 
| indexDelimiter | [enumeration StreetIndexDelimiter](CIMLayout.md#enumeration-streetindexdelimiter) | The delimiter that is displayed between columns. 


### CIMMapProductSurround 

|Property | Type | Description | 
|---------|--------|--------|
| autoUpdate | boolean | A value indicating whether properties of the surround should update automatically based on changes in the map. 
| productSpecification | [enumeration MapProductSpecType](CIMLayout.md#enumeration-mapproductspectype) | The map product specification type of the surround. 
| drawToSpecification | boolean | A value indicating whether to draw the element to specification size or allow user to manually resize element. 


### CIMMapProductFeatureGuide 

|Property | Type | Description | 
|---------|--------|--------|
| gridReference | [CIMMapProductGridReference](CIMLayout.md#cimmapproductgridreference) | The grid reference field name. 
| IDNumberFieldName | string | The Identification Number field name. 
| categoryCodeFieldName | string | The Category Code field name. 






## CIMMapProductGridReference
#### Represents how a grid reference (MGRS) should be displayed within CIMMapProductGridStreetIndex. 


### CIMMapProductGridReference 

|Property | Type | Description | 
|---------|--------|--------|
| gridReferenceFieldName | string | The grid reference field name. 
| precisionLevel | [enumeration GridReferencePrecisionLevel](CIMLayout.md#enumeration-gridreferenceprecisionlevel) | Grid reference resolution. 






## CIMMapProductGridStreetIndex
#### Represents a street index that calculates the grid reference (MGRS) of each street in surround element. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMBaseStreetIndex 

|Property | Type | Description | 
|---------|--------|--------|
| layerURI | string | The path to the layer containing the features to be indexed. 
| fields | [[CIMTableField]](Types.md#tablefield) | The fields displayed in the street index. 
| titleText | string | The title of the element. 
| titleTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for title text. 
| headerTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for header text. 
| textSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for the features. 
| fittingStrategy | [enumeration TableFrameFittingStrategy](CIMLayout.md#enumeration-tableframefittingstrategy) | The fitting strategy. 
| wrapMethod | [enumeration StreetIndexWrapMethod](CIMLayout.md#enumeration-streetindexwrapmethod) | How the data should wrap across multiple columns. 
| minFontSize | double | The minimum font size. Units in points. 
| headerGap | double | The spacing between headers and data. 
| groupTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for a field that is grouped. 
| groupGap | double | The spacing between group and headers. 
| columns | long | The number of columns allowed to display. 
| indexDelimiter | [enumeration StreetIndexDelimiter](CIMLayout.md#enumeration-streetindexdelimiter) | The delimiter that is displayed between columns. 


### CIMMapProductSurround 

|Property | Type | Description | 
|---------|--------|--------|
| autoUpdate | boolean | A value indicating whether properties of the surround should update automatically based on changes in the map. 
| productSpecification | [enumeration MapProductSpecType](CIMLayout.md#enumeration-mapproductspectype) | The map product specification type of the surround. 
| drawToSpecification | boolean | A value indicating whether to draw the element to specification size or allow user to manually resize element. 


### CIMMapProductGridStreetIndex 

|Property | Type | Description | 
|---------|--------|--------|
| gridReference | [CIMMapProductGridReference](CIMLayout.md#cimmapproductgridreference) | The grid reference field name. 





### Enumeration: MapProductSpecType
#### Defines the layout types that meet different map product specifications. 

|Property | Value | Description | 
|---------|--------|--------|
| Unset| -1| Unset product specification 
| TLM| 0| Topographic Line Map, a.k.a. Topographic Map 
| ICM| 1| Image City Map 
| JOG| 2| Joint Operation Graphics 
| USTOPO| 3| United States Topographic Maps 
| GNC| 4| Global Navigation and Planning Chart 
| JNC| 5| Jet Navigation Chart 
| ONC| 6| Operational Navigation Chart 
| TPC| 7| Tactical Pilotage Chart 
| EVC| 8| Escape Evasion Chart 




## CIMMargin
#### Represents a margin to apply around the page. 


### CIMMargin 

|Property | Type | Description | 
|---------|--------|--------|
| left | double | The left margin. 
| right | double | The right margin. 
| top | double | The top margin. 
| bottom | double | The bottom margin. 






## CIMMarkerNorthArrow
#### Represents a marker north arrow on a page layout. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMNorthArrow 

|Property | Type | Description | 
|---------|--------|--------|
| referenceLocation | [Point](ExternalReferences.md#point) | The reference location for a north arrow. 
| calibrationAngle | double | The calibration angle for a north arrow. 


### CIMMarkerNorthArrow 

|Property | Type | Description | 
|---------|--------|--------|
| pointSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The point symbol for a north arrow. 
| northType | [enumeration NorthType](CIMLayout.md#enumeration-northtype) | The type of north arrow. 






## CIMMeasuredGrid
#### Represents a measured grid of the mapFrame. 


### CIMMapGrid 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the Grid or Graticule. 
| isVisible | boolean | A value indicating whether the grid or graticule is visible. 
| neatlineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The neat line symbol of the Grid or Graticule. 
| maxInteriorAngle | double | The maximum value of the interior angle that determines the edge of the mapFrame polygon. The angle is defined in degrees. 
| edgeMinimumLength | double | The minimum length of the edge of the mapFrame polygon in page units. 
| mapGridEdges | [[CIMMapGridEdge]](CIMLayout.md#cimmapgridedge) | The map grid edges. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMMeasuredGrid 

|Property | Type | Description | 
|---------|--------|--------|
| customOrigin | [Point](ExternalReferences.md#point) | The custom origin of the measured grid. 
| projectedCoordinateSystem | [ProjectedCoordinateSystem](ExternalReferences.md#projectedcoordinatesystem) | The projected coordinate system of the grid. 
| gridLines | [[CIMGridLine]](Types.md#gridline) | The gridLines of the measured grid. 
| isAutoScaled | boolean | A value indicating whether to auto-scale the grid. 
| clipUTMZone | boolean | A value indicating whether to clip the grid to the UTM zone. If the measured grid is not defined in one of the UTM coordinates, then this property is irrelevant. 
| useMapClipShape | boolean | A value indicating whether to use the clip shape of the map (if set) as the grid boundary. 






## CIMMeterReferenceGuide
#### Provides a set of instructions and examples that enable users to compose standard grid reference. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMMapProductSurround 

|Property | Type | Description | 
|---------|--------|--------|
| autoUpdate | boolean | A value indicating whether properties of the surround should update automatically based on changes in the map. 
| productSpecification | [enumeration MapProductSpecType](CIMLayout.md#enumeration-mapproductspectype) | The map product specification type of the surround. 
| drawToSpecification | boolean | A value indicating whether to draw the element to specification size or allow user to manually resize element. 


### CIMMeterReferenceGuide 

|Property | Type | Description | 
|---------|--------|--------|
| gridSquareType | [enumeration MeterReferenceSquareType](CIMLayout.md#enumeration-meterreferencesquaretype) | The type of the 100,000-Square identification area. 
| isSingleGridZone | boolean | A value indicating whether the grid zone is using single (true) or multiple (false) designators. 
| properties | [CIMMeterReferenceProperties](CIMLayout.md#cimmeterreferenceproperties) | The display properties of the meter reference guide. 
| textSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for the text elements in the meter reference guide. 
| lineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for the grid lines in the meter reference guide. 






## CIMMeterReferenceProperties
#### Defines the display properties of the meter reference guide. 


### CIMMeterReferenceProperties 

|Property | Type | Description | 
|---------|--------|--------|
| gridSquareUpperLeft | string | The text displayed in the upper left corner of the square identification area. 
| gridSquareUpperRight | string | The text displayed in the upper right corner of the square identification area. 
| gridSquareLowerLeft | string | The text displayed in the lower left corner of the square identification area. 
| gridSquareLowerRight | string | The text displayed in the lower right corner of the square identification area. 
| gridSquareUpperLeftDual | string | The auxiliary text displayed in the upper left corner of the square identification area. 
| gridSquareUpperRightDual | string | The auxiliary text displayed in the upper left corner of the square identification area. 
| gridSquareLowerLeftDual | string | The auxiliary text displayed in the lower left corner of the square identification area. 
| gridSquareLowerRightDual | string | The auxiliary text displayed in the lower right corner of the square identification area. 
| gridSquareVerticalSeparator | long | The vertical separator value of the square identification area. 
| gridSquareHorizontalSeparator | long | The horizontal separator value of the square identification area. 
| gridSquareHorizontalSeparatorDual | long | The horizontal auxiliary separator value of the square identification area. 
| gridZoneUpperLeft | string | The text displayed in the upper left corner of the grid zone designation area. 
| gridZoneUpperRight | string | The text displayed in the upper right corner of the grid zone designation area. 
| gridZoneLowerLeft | string | The text displayed in the lower left corner of the grid zone designation area. 
| gridZoneLowerRight | string | The text displayed in the lower right corner of the grid zone designation area. 
| gridZoneLatitude | long | The latitude of the grid zone. 
| gridZoneLongitude | long | The longitude of the grid zone. 





### Enumeration: MeterReferenceSquareType
#### Defines options for 100,000-Square identification area. 

|Property | Value | Description | 
|---------|--------|--------|
| Single| 0| Single location identifier 
| Multiple| 1| Multiple location identifiers for additional information 
| DualGrid| 2| Enables location identifiers across multiple UTM zones. 




## CIMNestedLegendItem
#### Represents a nested legend item in a legend. 


### CIMLegendItem 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The legend item name. 
| newColumn | boolean | A value indicating whether a legend item should be placed in a new column. 
| layerNameSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item symbol. 
| manualColumn | long | The manual column assignment for a legend item. 
| keepTogetherOption | [enumeration LegendKeepTogetherOption](CIMLayout.md#enumeration-legendkeeptogetheroption) | A value indicating whether the legend item or group should be kept together. 
| showLayerName | boolean | A value indicating whether the legend item layer name should be displayed. 
| showHeading | boolean | A value indicating whether the legend item heading should be displayed. 
| headingSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item heading symbol. 
| showLabels | boolean | A value indicating whether the legend item labels should be displayed. 
| layer | string | The legend item layer's path. 
| showDescription | boolean | A value indicating whether a legend item description should be displayed. 
| labelSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item label symbol. 
| descriptionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item description symbol. 
| patchWidth | double | The legend item patch width. Units in points. 
| patchHeight | double | The legend item patch height. Units in points. 
| autoVisibility | boolean | A value indicating whether the legend item should be displayed if in the visible extent. 
| useMapSeriesShape | boolean | A value indicating whether to use map series shape instead of map frame to find dynamic classes. 
| classIndent | double | Distance from the class name to the edge of the legend. 
| headingIndent | double | Distance from the heading to the edge of the legend. 
| layerNameIndent | double | Distance of the layer name to the edge of the legend. 
| showGroupLayerName | boolean | A value indicating whether to show the containing group layer name above the item. 
| groupLayerNameSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used to display the group layer name. 
| scaleToPatch | boolean | A value indicating whether to scale the symbol to the specified patch size. 
| showCounts | boolean | A value indicating whether the legend should display count statistics. 
| countFormat | [NumberFormat](Types.md#numberformat) | The feature count format. 
| countPrefix | string | The feature count prefix. 
| countSuffix | string | The feature count suffix. 
| isVisible | boolean | A value indicating whether the legend item is visible. 
| groupFilter | [long] | A value specifying which legend groups are displayed. 


### CIMLegendItemLeader 

|Property | Type | Description | 
|---------|--------|--------|
| lineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol for a legend item leader. 
| lineLength | double | The line length for a legend item leader. 


### CIMLegendItemArrangement 

|Property | Type | Description | 
|---------|--------|--------|
| arrangement | [enumeration LegendItemArrangement](Types.md#enumeration-legenditemarrangement) | The Arrangement. 


### CIMNestedLegendItem 

|Property | Type | Description | 
|---------|--------|--------|
| autoLayout | boolean | A value indicating whether to automatically layout the legend item. 
| labelEnds | boolean | A value indicating whether the ends of a nested legend item should be labeled. 
| outlineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The outline symbol for the nested legend item. 
| showOutlines | boolean | A value indicating whether outlines should be displayed for a nested legend item. 
| patchAlignment | [enumeration HorizontalAlignment](CIMSymbols.md#enumeration-horizontalalignment) | The patch alignment for a nested legend item. 





### Enumeration: NorthType
#### A list of north arrows types. 

|Property | Value | Description | 
|---------|--------|--------|
| SimpleNorth| 0| Simple north arrow. 
| TrueNorth| 1| True north arrow. 
| GridNorth| 2| Grid north arrow. 
| MagneticNorth| 3| Magnetic north arrow. 



### Enumeration: Orientation
#### A list of orientation values. 

|Property | Value | Description | 
|---------|--------|--------|
| Horizontal| 0| Horizontal. 
| Vertical| 1| Vertical. 




## CIMPage
#### Represents the page information associated with a layout. 


### CIMPage 

|Property | Type | Description | 
|---------|--------|--------|
| height | double | The height of the layout in page units. 
| stretchElements | boolean | A value indicating whether elements should be stretched when the page size is changed. 
| width | double | The width of the layout in page units. 
| printerPreferences | [CIMPrinterPreferences](CIMLayout.md#cimprinterpreferences) | The printer preferences for the page. 
| units | [LinearUnit](ExternalReferences.md#linearunit) | The page units for the layout. 
| guides | [[CIMGuide]](CIMLayout.md#cimguide) | The guides on a layout. 
| showRulers | boolean | A value indicating whether rulers should be displayed on the layout. 
| showGuides | boolean | A value indicating whether guides should be displayed on the layout. 
| smallestRulerDivision | double | The smallest ruler division. 
| margin | [CIMMargin](CIMLayout.md#cimmargin) | The margin for the page. 
| showMargin | boolean | A value indicating whether the printer margin should be displayed on the layout. 





### Enumeration: PageOrientation
#### A list of page orientation values. 

|Property | Value | Description | 
|---------|--------|--------|
| Portrait| 0| Portrait orientation. 
| Landscape| 1| Landscape orientation. 




## CIMPrinterPreferences
#### Represents the printer preferences associated with a layout. 


### CIMPrinterPreferences 

|Property | Type | Description | 
|---------|--------|--------|
| printerName | string | The printer name. 
| paperName | string | The paper size name. 
| paperSource | long | The paper source. 






## CIMProfileFrame
#### Layout element used to draw Profile view of Runway, Terrain, obstacles and Obstruction Identification Surfaces (OIS). 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMProfileFrame 

|Property | Type | Description | 
|---------|--------|--------|
| heightOption | [enumeration ProfileFrameHeightOption](CIMLayout.md#enumeration-profileframeheightoption) | The option to control the height of profile. 
| height | double | The height of the profile, used if the height option is set to ConstantHeight. 
| heightUnits | [LinearUnit](ExternalReferences.md#linearunit) | The height units of the profile, used if the height option is set to ConstantHeight. 
| ratio | double | The ratio between width and height scale. 
| runwayDesignator | string | The runway designator for which profile is created. 
| primaryOISDescription | string | The primary OIS surface for which profile is created. 
| secondaryOISDescription | string | The secondary OIS description for cases where different classifications were used for the ends of runway user can choose secondary classification. 
| OISLayerURI | string | The URI of the layer of the OIS feature which defines the data for which profile is drawn. 
| grid | [CIMProfileGrid](CIMLayout.md#cimprofilegrid) | The display options for the grid. 
| terrain | [CIMProfileTerrain](CIMLayout.md#cimprofileterrain) | Display options for terrain. 
| runway | [CIMProfileRunway](CIMLayout.md#cimprofilerunway) | The text symbol for runway elevation. 
| OISSurfaces | [[CIMProfileOIS]](CIMLayout.md#cimprofileois) | The display option for all the OIS surfaces shown in the profile. 
| obstacles | [[CIMProfileObstacle]](Types.md#profileobstacle) | The display option for all the point obstacles shown in the profile. 
| profileType | [enumeration ProfileFrameType](CIMLayout.md#enumeration-profileframetype) | The option for profile type. 
| profileStyle | [enumeration ProfileFrameStyle](CIMLayout.md#enumeration-profileframestyle) | The style of the profile frame. 
| runwayEndLeftAsReference | boolean | A value indicating whether to use left end of runway as base elevation. 





### Enumeration: ProfileFrameHeightOption
#### Options for controlling the height of the profile element. 

|Property | Value | Description | 
|---------|--------|--------|
| ConstantHeight| 0| Adjust the cell height based on the overall height of element 
| ConstantRatio| 1| Keeps a constant ratio between width to height of each cell 



### Enumeration: ProfileFrameStyle
#### Available styles for profile frames. 

|Property | Value | Description | 
|---------|--------|--------|
| AOC| 0| Aerodrome Obstacle Chart style. 
| PATC| 1| Precision Approach Terrain Chart style. 



### Enumeration: ProfileFrameType
#### Options to specify if profile is displaying straight or curved approach. 

|Property | Value | Description | 
|---------|--------|--------|
| Straight| 0| Default option for straight approach profile 
| Curved| 1| option for a curved approach profile 




## CIMProfileGrid
#### Grid shown for the profile. 


### CIMProfileGrid 

|Property | Type | Description | 
|---------|--------|--------|
| horizontalScale | double | The horizontal scale for the profile. 
| horizontalScaleUnits | [LinearUnit](ExternalReferences.md#linearunit) | The horizontal scale units for the profile. 
| verticalScale | double | The vertical scale for the profile. 
| verticalScaleUnits | [LinearUnit](ExternalReferences.md#linearunit) | The vertical scale units for the profile. 
| autoGridExtent | boolean | A value indicating whether to calculate the start and stop of grid automatically If set to false user will set the minimum and maximum based on requirements. 
| YMin | double | The vertical scale minimum value. 
| YMax | double | The vertical scale maximum value. 
| subDivisionsX | long | The number of subdivisions in horizontal direction. 
| subDivisionsY | long | The number of divisions in vertical direction. 
| gridSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line Symbol for the major grid lines. 
| subDivisionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol for the subdivision. 
| horizontalScaleTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for the horizontal scale. 
| verticalScaleLeftTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for the vertical scale left. 
| verticalScaleRightTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for the vertical scale right. 
| showEntireApproach | boolean | A value indicating whether to show the entire length of curved approach, or just show up to a particular distance. 
| XMax | double | The horizontal length maximum value. 
| verticalIntervalInMeters | long | The vertical interval for scale in meters. 
| verticalIntervalInFeet | long | The vertical interval for scale in feet. 
| showAbsoluteHorizontalScale | boolean | A value indicating whether to display absolute or relative grid text automatically. 






## CIMProfileOIS
#### Defines the properties for OIS features. 


### CIMProfileOIS 

|Property | Type | Description | 
|---------|--------|--------|
| OISDescription | string | The description of OIS surface read only. 
| OISLabel | string | The label to be displayed for OIS. 
| showOIS | boolean | A value indicating whether to show OIS surface. 
| isPrimary | boolean | A value indicating whether the surface is primary. If surface is primary it can't be hidden and terrain and obstacles will be drawn based on the primary surface. 
| displayOrder | long | The zero based index to control the display order. 
| OISSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line Symbol used to draw the OIS Surface. 
| OISTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol used to draw the label of OIS Surface. 






## CIMProfileObstacle
#### Represents common properties for all the obstacles. 


### CIMProfileObstacle 

|Property | Type | Description | 
|---------|--------|--------|
| showPenetrating | boolean | A value indicating whether to the obstacle only if it penetrates OIS Surface. 
| obstacleLayerName | string | The name connecting display options to obstacle layers coming from Obstacle JSON (read only). 
| symbolSubstitutionType | [enumeration ProfileObstacleSymbolSubstitutionType](CIMLayout.md#enumeration-profileobstaclesymbolsubstitutiontype) | The type of substitution applied to the obstacle symbol. 





### Enumeration: ProfileObstacleGroundDisplayOption
#### Options for displaying the base of polygon/polyline obstacles. 

|Property | Value | Description | 
|---------|--------|--------|
| Actual| 0| Show the actual ground elevation of each vertex 
| Max| 1| Show the maximum ground elevation for all the vertices 
| Min| 2| Show the minimum ground elevation for all the vertices 
| Average| 3| Show the average ground elevation for all the vertices 



### Enumeration: ProfileObstacleMarkerLocation
#### Marker display location options. 

|Property | Value | Description | 
|---------|--------|--------|
| Surface| 0| Show marker at the OIS surface 
| Top| 1| Show marker at the top of obstacle 
| Base| 2| Show marker at the base of obstacle 



### Enumeration: ProfileObstacleSymbolSubstitutionType
#### Types of symbol substitution used to display obstacles. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No substitute symbols used to display obstacles 
| Penetrating| 1| Penetrating obstacles are displayed with substitute symbols 
| Protruding| 2| Protruding portion of penetrating obstacles is displayed with substitute symbols 




## CIMProfilePointObstacle
#### Defines the properties for a Point obstacle. 


### CIMProfileObstacle 

|Property | Type | Description | 
|---------|--------|--------|
| showPenetrating | boolean | A value indicating whether to the obstacle only if it penetrates OIS Surface. 
| obstacleLayerName | string | The name connecting display options to obstacle layers coming from Obstacle JSON (read only). 
| symbolSubstitutionType | [enumeration ProfileObstacleSymbolSubstitutionType](CIMLayout.md#enumeration-profileobstaclesymbolsubstitutiontype) | The type of substitution applied to the obstacle symbol. 


### CIMProfilePointObstacle 

|Property | Type | Description | 
|---------|--------|--------|
| markerLocation | [enumeration ProfileObstacleMarkerLocation](CIMLayout.md#enumeration-profileobstaclemarkerlocation) | The location of marker symbol for obstacle. 
| obstacleBaseSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol to connect from base of the grid to base of the obstacle. 
| obstacleHeightSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol to display the height of the obstacle (base to top of obstacle). 
| obstacleMarkerSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The point symbol displayed based in the marker location. 
| obstacleTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol to display the number of obstacle at the marker location. 
| showOnlyShadowingObstacles | boolean | A value indicating whether only shadowing obstacles are displayed. 
| substituteObstacleBaseSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The substitute base symbol. 
| substituteObstacleHeightSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The substitute height symbol. 
| substituteObstacleMarkerSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The substitute marker symbol. 
| substituteObstacleTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The substitute text symbol. 






## CIMProfilePolyObstacle
#### Represents a profile poly obstacle. 


### CIMProfileObstacle 

|Property | Type | Description | 
|---------|--------|--------|
| showPenetrating | boolean | A value indicating whether to the obstacle only if it penetrates OIS Surface. 
| obstacleLayerName | string | The name connecting display options to obstacle layers coming from Obstacle JSON (read only). 
| symbolSubstitutionType | [enumeration ProfileObstacleSymbolSubstitutionType](CIMLayout.md#enumeration-profileobstaclesymbolsubstitutiontype) | The type of substitution applied to the obstacle symbol. 


### CIMProfilePolyObstacle 

|Property | Type | Description | 
|---------|--------|--------|
| groundDisplayOption | [enumeration ProfileObstacleGroundDisplayOption](CIMLayout.md#enumeration-profileobstaclegrounddisplayoption) | The option to display how the base of obstacle is shown. 
| obstacleSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used to draw the obstacle. 
| substituteObstacleSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The substitute obstacle symbol. 






## CIMProfileRunway
#### Display properties for Runway. 


### CIMProfileRunway 

|Property | Type | Description | 
|---------|--------|--------|
| precision | long | The number of decimal places for runway elevation. 
| elevationChangeThreshold | double | The percentage change between two elevation values when we can show the text symbol. Range is calculated by maximum and minimum elevation of the runway. 
| runwayLineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The display symbol for runway. 
| runwayTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The text symbol for runway elevation. 






## CIMProfileTerrain
#### Display properties for Terrain. 


### CIMProfileTerrain 

|Property | Type | Description | 
|---------|--------|--------|
| showOutline | boolean | A value indicating whether to show only the outline of terrain. 
| maxTerrain | [CIMProfileTerrainDisplay](CIMLayout.md#cimprofileterraindisplay) | The display settings for maximum elevation of terrain. 
| minTerrain | [CIMProfileTerrainDisplay](CIMLayout.md#cimprofileterraindisplay) | The display settings for minimum elevation of terrain. 
| centerLineTerrain | [CIMProfileTerrainDisplay](CIMLayout.md#cimprofileterraindisplay) | The display settings for CenterLine elevation of terrain. 






## CIMProfileTerrainDisplay
#### Settings to control how the terrain information is being displayed in the profile. 


### CIMProfileTerrainDisplay 

|Property | Type | Description | 
|---------|--------|--------|
| displayOption | [enumeration ProfileTerrainDisplayOption](CIMLayout.md#enumeration-profileterraindisplayoption) | The display option for terrain. 
| terrainSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The display Symbol for the entire terrain or terrain below OIS surface. 
| penetratingTerrainSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The display Symbol for the penetrating terrain or terrain above OIS surface. 





### Enumeration: ProfileTerrainDisplayOption
#### Options to control how terrain data is displayed. 

|Property | Value | Description | 
|---------|--------|--------|
| All| 0| Show the entire terrain using single symbol 
| PenetratingOnly| 1| Show only the terrain that is above the OIS surface 
| Highlight| 2| Use two different symbols to display the terrain above and below the OIS surface 
| None| 3| Terrain is not displayed 



### Enumeration: RectanglePosition
#### A list of rectangle position values. 

|Property | Value | Description | 
|---------|--------|--------|
| TopSide| 0| Top side. 
| BottomSide| 1| Bottom side. 
| LeftSide| 2| Left side. 
| RightSide| 3| Right side. 




## CIMReferenceGrid
#### Defines a reference grid. 


### CIMMapGrid 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the Grid or Graticule. 
| isVisible | boolean | A value indicating whether the grid or graticule is visible. 
| neatlineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The neat line symbol of the Grid or Graticule. 
| maxInteriorAngle | double | The maximum value of the interior angle that determines the edge of the mapFrame polygon. The angle is defined in degrees. 
| edgeMinimumLength | double | The minimum length of the edge of the mapFrame polygon in page units. 
| mapGridEdges | [[CIMMapGridEdge]](CIMLayout.md#cimmapgridedge) | The map grid edges. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMReferenceGrid 

|Property | Type | Description | 
|---------|--------|--------|
| isAutoScaled | boolean | A value indicating whether to auto-adjust the grid according to the size of the map frame. 
| rowCount | long | The number of rows for the reference grids. 
| columnCount | long | The number of columns for the reference grids. 
| gridLines | [[CIMGridLine]](Types.md#gridline) | The collection of the grid lines. 






## CIMReferenceGridLabelTemplate
#### Defines the label template for the reference grids. 


### CIMGridLabelTemplate 

|Property | Type | Description | 
|---------|--------|--------|


### CIMReferenceGridLabelTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the label scheme. 
| values | [string] | The list of values to label the grid. 
| delimiter | string | The delimiter for the list of labels. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol of the label. 






## CIMRelatedReportSection
#### Represents a Related Report section of a report. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReportSectionElement 

|Property | Type | Description | 
|---------|--------|--------|
| autoSize | boolean | A value indicating whether the section height will grow and shrink to fit the content of the section. 
| elementFieldProperties | [[CIMReportElementFieldProperties]](Types.md#reportelementfieldproperties) | The field properties that will be applied to the elements. 
| excludePageNumberPages | string | The comma delimited list of pages to exclude the page number from. 
| excludeSectionPages | string | The comma delimited list of pages to exclude the section from. 
| startOnNewPage | boolean | A value indicating whether the section should start on a new page. 
| autoGrowTextElements | boolean | A value indicating whether the height of Text elements in sections will grow based on their content. 


### CIMRelatedReportSection 

|Property | Type | Description | 
|---------|--------|--------|
| dataSource | [CIMReportDataSource](CIMLayout.md#cimreportdatasource) | The data source for a Related Report. 
| relateName | string | The relate or relationship class name. 
| expressions | [[CIMExpressionInfo]](CIMRenderers.md#cimexpressioninfo) | The expressions used by the related report. 






## CIMReport
#### Represents a report in a project. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the source was last modified, as of the last sync. Used to detect when another sync is needed. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 
| sourcePortalUrl | string | The source portal URI of the item. Set if sourced from an external item such as an item on a portal. 


### CIMLayoutDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| page | [CIMPage](CIMLayout.md#cimpage) | The CIMPage for the layout. 
| dateExported | [TimeInstant](ExternalReferences.md#timeinstant) | The date exported property for a layout. 
| datePrinted | [TimeInstant](ExternalReferences.md#timeinstant) | The date printed property for a layout. 
| mapSeries | [MapSeries](Types.md#mapseries) | The map series for a layout. 
| colorModel | [enumeration ColorModel](CIMEnumerations.md#enumeration-colormodel) | The color model for a layout. 
| RGBColorProfile | string | The name of the RGB color profile for a layout. 
| CMYKColorProfile | string | The name of the CMYK color profile for a layout. 
| simulateOverprint | boolean | A value indicating whether to simulate overprint for a layout. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layout. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| defaultColorVisionDeficiencyMode | [enumeration ColorVisionDeficiencyType](CIMEnumerations.md#enumeration-colorvisiondeficiencytype) | The color vision deficiency mode that new views of this layout are opened with. 


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReport 

|Property | Type | Description | 
|---------|--------|--------|
| height | double | The Height of the report. 
| startPage | long | The starting page for the report. 
| watermarks | [[CIMReportWatermark]](CIMLayout.md#cimreportwatermark) | A collection of watermark for the report. 






## CIMReportDataSource
#### Represents the data source properties of a report. The data source can be a map member or external data. 


### CIMReportDataSource 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection to the source. 
| definitionQuery | string | The definition query. 
| fields | [[CIMReportField]](CIMLayout.md#cimreportfield) | The fields used by the report. 
| mapMemberURI | string | The URI to a Layer or Standalone table in the project. 
| useSelectionSet | boolean | A value indicating whether the selection of the layer or table should be used for the report. 






## CIMReportDetails
#### Represents a details section of a report. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReportSectionElement 

|Property | Type | Description | 
|---------|--------|--------|
| autoSize | boolean | A value indicating whether the section height will grow and shrink to fit the content of the section. 
| elementFieldProperties | [[CIMReportElementFieldProperties]](Types.md#reportelementfieldproperties) | The field properties that will be applied to the elements. 
| excludePageNumberPages | string | The comma delimited list of pages to exclude the page number from. 
| excludeSectionPages | string | The comma delimited list of pages to exclude the section from. 
| startOnNewPage | boolean | A value indicating whether the section should start on a new page. 
| autoGrowTextElements | boolean | A value indicating whether the height of Text elements in sections will grow based on their content. 


### CIMReportDetails 

|Property | Type | Description | 
|---------|--------|--------|
| columns | long | The number of columns for the details section. 
| rowBackgroundColors | [[CIMColor]](Types.md#color) | The collection of background colors for each of the repeating rows. 
| rowBackgroundCount | long | The number of consecutive rows for each background color. 
| keepRecordTogether | boolean | A value indicating whether to prevent a page break for a record in the Details subsection. 






## CIMReportDocument
#### Represents a report document which is the document type used for saving .rlfx files. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMReportDocument 

|Property | Type | Description | 
|---------|--------|--------|
| binaryReferences | [[CIMBinaryReference]](CIMDocument.md#cimbinaryreference) | The binary references of the document. 
| layerDefinitions | [[CIMDefinition]](Types.md#definition) | The layer definitions in the report document. 
| mapDefinitions | [[CIMDefinition]](Types.md#definition) | The map definitions of the report document. 
| reportDefinition | [CIMReport](CIMLayout.md#cimreport) | The report definition of the report document. 
| tableDefinitions | [[CIMDefinition]](Types.md#definition) | The table definitions of the report document. 
| layoutDefinitions | [[CIMDefinition]](Types.md#definition) | The layout definitions referenced by supplemental pages of the report document. 
| linkChartDefinitions | [[CIMDefinition]](Types.md#definition) | The link chart definitions of the report document. 
| timelineDefinitions | [[CIMDefinition]](Types.md#definition) | The timeline definitions of the report document. 
| videoDefinitions | [[CIMDefinition]](Types.md#definition) | The video definitions of the report document. 
| elevationSurfaceLayerDefinitions | [[CIMDefinition]](Types.md#definition) | The elevation surface layer definitions. 






## CIMReportElementFieldProperties
#### Represents field properties that will be applied to an element in a report. 


### CIMReportElementFieldProperties 

|Property | Type | Description | 
|---------|--------|--------|
| element | string | The name of the target element. 
| field | string | The name of the source field. 
| format | [NumberFormat](Types.md#numberformat) | The format for the source field value. 
| statistic | [enumeration FieldStatisticsFlag](CIMLayout.md#enumeration-fieldstatisticsflag) | The statistic to apply to the source field. 






## CIMReportField
#### Represents a field in a report. 


### CIMTableField 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The field name and unique identifier. 
| isVisible | boolean | A value indicating whether the field is visible. 
| width | double | The width of field. A value of 0 indicates "auto size". 
| sortInfo | [enumeration FieldSortInfo](CIMLayout.md#enumeration-fieldsortinfo) | The options when this field is used for sorting. 
| sortOrder | long | The zero based sort order. -1 indicates field isn't used for sorting. 
| fieldOrder | long | The zero based display order. 
| group | boolean | A value indicating whether this is a grouping field. 
| displayName | string | The display name for the field. 


### CIMReportField 

|Property | Type | Description | 
|---------|--------|--------|






## CIMReportFooter
#### Represents a report footer in a report. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReportSectionElement 

|Property | Type | Description | 
|---------|--------|--------|
| autoSize | boolean | A value indicating whether the section height will grow and shrink to fit the content of the section. 
| elementFieldProperties | [[CIMReportElementFieldProperties]](Types.md#reportelementfieldproperties) | The field properties that will be applied to the elements. 
| excludePageNumberPages | string | The comma delimited list of pages to exclude the page number from. 
| excludeSectionPages | string | The comma delimited list of pages to exclude the section from. 
| startOnNewPage | boolean | A value indicating whether the section should start on a new page. 
| autoGrowTextElements | boolean | A value indicating whether the height of Text elements in sections will grow based on their content. 


### CIMReportFooter 

|Property | Type | Description | 
|---------|--------|--------|
| alignSubsectionToBottom | boolean | A value indicating whether to force the subsection to export at the bottom of the page. 






## CIMReportHeader
#### Represents a report header section in a report. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReportSectionElement 

|Property | Type | Description | 
|---------|--------|--------|
| autoSize | boolean | A value indicating whether the section height will grow and shrink to fit the content of the section. 
| elementFieldProperties | [[CIMReportElementFieldProperties]](Types.md#reportelementfieldproperties) | The field properties that will be applied to the elements. 
| excludePageNumberPages | string | The comma delimited list of pages to exclude the page number from. 
| excludeSectionPages | string | The comma delimited list of pages to exclude the section from. 
| startOnNewPage | boolean | A value indicating whether the section should start on a new page. 
| autoGrowTextElements | boolean | A value indicating whether the height of Text elements in sections will grow based on their content. 


### CIMReportHeader 

|Property | Type | Description | 
|---------|--------|--------|
| coverPage | boolean | A value indicating whether the report header is a cover page. 






## CIMReportLayoutPageSection
#### Represents a layout supplemental page section of a report. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReportSectionElement 

|Property | Type | Description | 
|---------|--------|--------|
| autoSize | boolean | A value indicating whether the section height will grow and shrink to fit the content of the section. 
| elementFieldProperties | [[CIMReportElementFieldProperties]](Types.md#reportelementfieldproperties) | The field properties that will be applied to the elements. 
| excludePageNumberPages | string | The comma delimited list of pages to exclude the page number from. 
| excludeSectionPages | string | The comma delimited list of pages to exclude the section from. 
| startOnNewPage | boolean | A value indicating whether the section should start on a new page. 
| autoGrowTextElements | boolean | A value indicating whether the height of Text elements in sections will grow based on their content. 


### CIMReportPageSection 

|Property | Type | Description | 
|---------|--------|--------|
| includePageNumber | boolean | A value indicating whether to include page number elements. 


### CIMReportLayoutPageSection 

|Property | Type | Description | 
|---------|--------|--------|
| layoutURI | string | The layout URI. 






## CIMReportMapFrameElementProperties
#### Represents properties that will be applied to a map frame element in a report. 


### CIMReportElementFieldProperties 

|Property | Type | Description | 
|---------|--------|--------|
| element | string | The name of the target element. 
| field | string | The name of the source field. 
| format | [NumberFormat](Types.md#numberformat) | The format for the source field value. 
| statistic | [enumeration FieldStatisticsFlag](CIMLayout.md#enumeration-fieldstatisticsflag) | The statistic to apply to the source field. 


### CIMReportMapFrameElementProperties 

|Property | Type | Description | 
|---------|--------|--------|
| spatialMapSeries | [CIMSpatialMapSeries](CIMLayout.md#cimspatialmapseries) | The spatial map series properties for a map frame element. 






## CIMReportPageFooter
#### Represents a page footer in a report. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReportSectionElement 

|Property | Type | Description | 
|---------|--------|--------|
| autoSize | boolean | A value indicating whether the section height will grow and shrink to fit the content of the section. 
| elementFieldProperties | [[CIMReportElementFieldProperties]](Types.md#reportelementfieldproperties) | The field properties that will be applied to the elements. 
| excludePageNumberPages | string | The comma delimited list of pages to exclude the page number from. 
| excludeSectionPages | string | The comma delimited list of pages to exclude the section from. 
| startOnNewPage | boolean | A value indicating whether the section should start on a new page. 
| autoGrowTextElements | boolean | A value indicating whether the height of Text elements in sections will grow based on their content. 


### CIMReportPageFooter 

|Property | Type | Description | 
|---------|--------|--------|






## CIMReportPageHeader
#### Represents a page header section in a report. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReportSectionElement 

|Property | Type | Description | 
|---------|--------|--------|
| autoSize | boolean | A value indicating whether the section height will grow and shrink to fit the content of the section. 
| elementFieldProperties | [[CIMReportElementFieldProperties]](Types.md#reportelementfieldproperties) | The field properties that will be applied to the elements. 
| excludePageNumberPages | string | The comma delimited list of pages to exclude the page number from. 
| excludeSectionPages | string | The comma delimited list of pages to exclude the section from. 
| startOnNewPage | boolean | A value indicating whether the section should start on a new page. 
| autoGrowTextElements | boolean | A value indicating whether the height of Text elements in sections will grow based on their content. 


### CIMReportPageHeader 

|Property | Type | Description | 
|---------|--------|--------|






## CIMReportPageSection
#### Represents a supplemental page section of a report. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReportSectionElement 

|Property | Type | Description | 
|---------|--------|--------|
| autoSize | boolean | A value indicating whether the section height will grow and shrink to fit the content of the section. 
| elementFieldProperties | [[CIMReportElementFieldProperties]](Types.md#reportelementfieldproperties) | The field properties that will be applied to the elements. 
| excludePageNumberPages | string | The comma delimited list of pages to exclude the page number from. 
| excludeSectionPages | string | The comma delimited list of pages to exclude the section from. 
| startOnNewPage | boolean | A value indicating whether the section should start on a new page. 
| autoGrowTextElements | boolean | A value indicating whether the height of Text elements in sections will grow based on their content. 


### CIMReportPageSection 

|Property | Type | Description | 
|---------|--------|--------|
| includePageNumber | boolean | A value indicating whether to include page number elements. 






## CIMReportSection
#### Gets or sets the data source for a report. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReportSectionElement 

|Property | Type | Description | 
|---------|--------|--------|
| autoSize | boolean | A value indicating whether the section height will grow and shrink to fit the content of the section. 
| elementFieldProperties | [[CIMReportElementFieldProperties]](Types.md#reportelementfieldproperties) | The field properties that will be applied to the elements. 
| excludePageNumberPages | string | The comma delimited list of pages to exclude the page number from. 
| excludeSectionPages | string | The comma delimited list of pages to exclude the section from. 
| startOnNewPage | boolean | A value indicating whether the section should start on a new page. 
| autoGrowTextElements | boolean | A value indicating whether the height of Text elements in sections will grow based on their content. 


### CIMReportSection 

|Property | Type | Description | 
|---------|--------|--------|
| dataSource | [CIMReportDataSource](CIMLayout.md#cimreportdatasource) | The data source for a report. 
| expressions | [[CIMExpressionInfo]](CIMRenderers.md#cimexpressioninfo) | The expressions used by the report. 






## CIMReportSectionElement
#### Represents a section of elements in a report. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMGroupElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMElementContainer 

|Property | Type | Description | 
|---------|--------|--------|
| elements | [[CIMElement]](Types.md#element) | A collection of elements. 


### CIMReportSectionElement 

|Property | Type | Description | 
|---------|--------|--------|
| autoSize | boolean | A value indicating whether the section height will grow and shrink to fit the content of the section. 
| elementFieldProperties | [[CIMReportElementFieldProperties]](Types.md#reportelementfieldproperties) | The field properties that will be applied to the elements. 
| excludePageNumberPages | string | The comma delimited list of pages to exclude the page number from. 
| excludeSectionPages | string | The comma delimited list of pages to exclude the section from. 
| startOnNewPage | boolean | A value indicating whether the section should start on a new page. 
| autoGrowTextElements | boolean | A value indicating whether the height of Text elements in sections will grow based on their content. 






## CIMReportWatermark
#### Represents a watermark in a report. 


### CIMReportWatermark 

|Property | Type | Description | 
|---------|--------|--------|
| element | [Element](Types.md#element) | The element for the watermark. 
| excludePageNumbers | string | The comma delimited list of excluded page numbers. 
| isBackground | boolean | A value indicating whether the overlay draws in the background of the report, else it draws on the foreground. 





### Enumeration: ScaleBarFittingStrategy
#### A list of scale bar fitting strategies. 

|Property | Value | Description | 
|---------|--------|--------|
| AdjustDivision| 0| Adjust the division value. 
| AdjustDivisions| 1| Adjust the number of divisions. 
| AdjustDivisionAndDivisions| 2| Adjust the division value and number of divisions. 
| AdjustFrame| 3| Adjust the size of the scale bar frame. 
| FixedWidth| 4| Preserve the width of the scale bar in page units. Deprecated in 3.4. Use FixedBarWidth instead. 
| FixedHeight| 5| Preserve the total distance shown in the scale bar. Deprecated in 3.4. 
| FixedBarWidth| 6| Preserve the width of the scale bar in page units. 



### Enumeration: ScaleBarFrequency
#### Lists the options for the frequency marks appear on the scale bar. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| None. 
| One| 1| One. 
| MajorDivisions| 2| Major divisions. 
| Divisions| 3| Divisions. 
| DivisionsAndFirstMidpoint| 4| Divisions and first mid point. 
| DivisionsAndFirstSubdivisions| 5| Divisions and first subdivisions. 
| DivisionsAndSubdivisions| 6| Divisions and subdivisions. 
| DivisionsFirstSubdivisionFirstMidpoint| 7| Divisions first subdivision and first midpoint. 



### Enumeration: ScaleBarLabelPosition
#### Lists the options for scale bar label positions. 

|Property | Value | Description | 
|---------|--------|--------|
| Above| 0| Above the scale bar. 
| BeforeLabels| 1| Before the labels. 
| AfterLabels| 2| After labels. 
| BeforeBar| 3| Before the scale bar. 
| AfterBar| 4| After the scale bar. 
| Below| 5| Below the scale bar. 
| AboveLeft| 6| Above the scale bar and to the left. 
| AboveRight| 7| Above the scale bar and to the right. 
| AboveEnds| 8| Above the ends of the scale bar. 
| BeforeAndAfterLabels| 9| Before and after labels. 
| BeforeAndAfterBar| 10| Before and after the scale bar. 
| BelowLeft| 11| Below the scale bar and to the left. 
| BelowRight| 12| Below the scale bar and to the right. 
| BelowEnds| 13| Below the scale bar and on the ends. 
| OnBarAfterFirstDivision| 14| On the scale bar after the first division. 



### Enumeration: ScaleBarVerticalPosition
#### A list of scale bar vertical positions. 

|Property | Value | Description | 
|---------|--------|--------|
| Above| 0| Above. 
| Top| 1| Top. 
| On| 2| On. 
| Bottom| 3| Bottom. 
| Below| 4| Below. 
| OnRight| 5| On right. 
| OnLeft| 6| On left. 




## CIMScaleLine
#### Represents a Scale line on a page layout. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMScaleBar 

|Property | Type | Description | 
|---------|--------|--------|
| alignToZeroPoint | boolean | A value indicating whether the scale bar should align to zero. 
| barHeight | double | The scale bar height. 
| division | double | The division value. 
| divisions | long | The number of divisions. 
| divisionsBeforeZero | long | The number of divisions before zero. 
| fittingStrategy | [enumeration ScaleBarFittingStrategy](CIMLayout.md#enumeration-scalebarfittingstrategy) | The fitting strategy. 
| labelFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency) | The label frequency. 
| labelGap | double | The label gap value. 
| labelPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition) | The label position. 
| labelSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | Label symbol. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| subdivisions | long | The number of subdivisions. 
| unitLabel | string | The unit label. 
| unitLabelGap | double | The unit label gap. Units set in points. 
| unitLabelPosition | [enumeration ScaleBarLabelPosition](CIMLayout.md#enumeration-scalebarlabelposition) | The unit label position. 
| unitLabelSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The unit label symbol. 
| units | [Unit](ExternalReferences.md#unit) | The units for the scale bar. 
| useFractionCharacters | boolean | A value indicating whether fractional characters should be used. 
| zeroPoint | [Point](ExternalReferences.md#point) | The zero location for the scale bar. 
| computeAtCenter | boolean | A value indicating whether to compute the scale at map center. 
| displayFirstOutside | boolean | A value indicating whether to display the first numeric value outside the bar. 
| displayLastOutside | boolean | A value indicating whether to display the last numeric value outside the bar. 
| barWidth | double | The width of the scalebar. 


### CIMScaleMarks 

|Property | Type | Description | 
|---------|--------|--------|
| divisionMarkHeight | double | The division mark height value. 
| divisionMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The division mark line symbol. 
| markFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency) | The division mark frequency. 
| markPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition) | The division mark position. 
| subdivisionMarkHeight | double | The subdivision mark height. 
| subdivisionMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The subdivision mark line symbol. 
| midpointMarkHeight | double | The midpoint mark height. 
| midpointMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The midpoint mark line symbol. 


### CIMScaleLine 

|Property | Type | Description | 
|---------|--------|--------|
| lineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The scale line symbol. 
| stepped | boolean | A value indicating whether the scale line should be stepped. 






## CIMSimpleGridLabelTemplate
#### Represents a simple format for a label. 


### CIMGridLabelTemplate 

|Property | Type | Description | 
|---------|--------|--------|


### CIMSimpleGridLabelTemplate 

|Property | Type | Description | 
|---------|--------|--------|
| dynamicStringTemplate | string | The dynamic text as a template for labels. 
| symbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol for the text of labels. 






## CIMSingleFillScaleBar
#### Represents and single fill scale bar on a page layout. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMScaleBar 

|Property | Type | Description | 
|---------|--------|--------|
| alignToZeroPoint | boolean | A value indicating whether the scale bar should align to zero. 
| barHeight | double | The scale bar height. 
| division | double | The division value. 
| divisions | long | The number of divisions. 
| divisionsBeforeZero | long | The number of divisions before zero. 
| fittingStrategy | [enumeration ScaleBarFittingStrategy](CIMLayout.md#enumeration-scalebarfittingstrategy) | The fitting strategy. 
| labelFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency) | The label frequency. 
| labelGap | double | The label gap value. 
| labelPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition) | The label position. 
| labelSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | Label symbol. 
| numberFormat | [NumberFormat](Types.md#numberformat) | The number format. 
| subdivisions | long | The number of subdivisions. 
| unitLabel | string | The unit label. 
| unitLabelGap | double | The unit label gap. Units set in points. 
| unitLabelPosition | [enumeration ScaleBarLabelPosition](CIMLayout.md#enumeration-scalebarlabelposition) | The unit label position. 
| unitLabelSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The unit label symbol. 
| units | [Unit](ExternalReferences.md#unit) | The units for the scale bar. 
| useFractionCharacters | boolean | A value indicating whether fractional characters should be used. 
| zeroPoint | [Point](ExternalReferences.md#point) | The zero location for the scale bar. 
| computeAtCenter | boolean | A value indicating whether to compute the scale at map center. 
| displayFirstOutside | boolean | A value indicating whether to display the first numeric value outside the bar. 
| displayLastOutside | boolean | A value indicating whether to display the last numeric value outside the bar. 
| barWidth | double | The width of the scalebar. 


### CIMScaleMarks 

|Property | Type | Description | 
|---------|--------|--------|
| divisionMarkHeight | double | The division mark height value. 
| divisionMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The division mark line symbol. 
| markFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency) | The division mark frequency. 
| markPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition) | The division mark position. 
| subdivisionMarkHeight | double | The subdivision mark height. 
| subdivisionMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The subdivision mark line symbol. 
| midpointMarkHeight | double | The midpoint mark height. 
| midpointMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The midpoint mark line symbol. 


### CIMSingleFillScaleBar 

|Property | Type | Description | 
|---------|--------|--------|
| fillSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The fill symbol for the scale bar. 






## CIMSlopeGuide
#### A slope guide surround element which is used to ascertaining terrain slope graphically as a percentage and a gradient (degree). 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMMapProductSurround 

|Property | Type | Description | 
|---------|--------|--------|
| autoUpdate | boolean | A value indicating whether properties of the surround should update automatically based on changes in the map. 
| productSpecification | [enumeration MapProductSpecType](CIMLayout.md#enumeration-mapproductspectype) | The map product specification type of the surround. 
| drawToSpecification | boolean | A value indicating whether to draw the element to specification size or allow user to manually resize element. 


### CIMSlopeGuide 

|Property | Type | Description | 
|---------|--------|--------|
| slopeGuideLayerURI | string | The layer used to calculate slope guide. 
| contourIntervalField | string | The name of the contour interval field. 
| mapScale | long | The map scale the slope guide will be based on. 
| contourInterval | long | The contour interval. 
| titleTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for title of element. 
| slopeUnitTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for text identifying slope as percentage or degree. 
| slopeTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for labeling slope values. 
| footnoteTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for footnote at bottom of slope guide. 
| verticalLineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for vertical lines in slope guide. 
| horizontalLineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for horizontal lines in slope guide. 
| tickLineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for dashed lines in slope guide. 






## CIMSpatialMapSeries
#### Spatial Map Series is a means to create a series of map pages based off of spatial features. 


### CIMMapSeries 

|Property | Type | Description | 
|---------|--------|--------|
| enabled | boolean | A value indicating whether the map series is enabled on the layout. 
| mapFrameName | string | The URI of the MapFrame to which MapSeries is linked. 
| startingPageNumber | long | The starting page number. 
| currentPageID | long long | The current page Id. 


### CIMSpatialMapSeries 

|Property | Type | Description | 
|---------|--------|--------|
| indexLayerURI | string | The URI of the index layer. 
| nameField | string | The name of the specified page. 
| numberField | string | The number of the specified page. 
| categoryField | string | The category of the page. 
| rotationField | string | The page specific rotation. 
| sortField | string | The required field that specifies the field used to determine sort order. 
| scaleField | string | Field that specifies the page specific scale. 
| spatialReferenceField | string | The spatial reference of the page. 
| sortAscending | boolean | A value indicating whether to sort in ascending or descending order. 
| scaleRounding | double | The specified value to which the scale rounds to. 
| extentOptions | [enumeration ExtentFitType](CIMLayout.md#enumeration-extentfittype) | The extent fitting options. 
| marginType | [enumeration UnitType](CIMLayout.md#enumeration-unittype) | The type of margins. 
| marginUnits | [LinearUnit](ExternalReferences.md#linearunit) | The units of the margin. 
| margin | double | The value of the margin. 
| clipMapToIndexFeature | boolean | A value indicating whether map clipping is synchronized with the current series index feature. 





### Enumeration: StreetIndexDelimiter
#### List of delimiters for column separation. 

|Property | Value | Description | 
|---------|--------|--------|
| Period| 0| Period delimiter. 
| Space| 1| Space delimiter. 
| Hyphen| 2| Hyphen delimiter. 
| Underscore| 3| Underscore delimiter. 



### Enumeration: StreetIndexWrapMethod
#### A list of ways to wrap data across multiple columns in CIMMapProductBaseStreetIndex. 

|Property | Value | Description | 
|---------|--------|--------|
| Wrap| 0| Wrap text based on height of frame across multiple columns. Text will continue at top of next column. 
| GroupWrap| 1| Wrap text based on a grouped field across multiple columns. Text will continue at top of next column if group does not fit in current column. 




## CIMTMElevationGuideBarElement
#### Represents TM Elevation Guide Bar surround element. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMMapProductSurround 

|Property | Type | Description | 
|---------|--------|--------|
| autoUpdate | boolean | A value indicating whether properties of the surround should update automatically based on changes in the map. 
| productSpecification | [enumeration MapProductSpecType](CIMLayout.md#enumeration-mapproductspectype) | The map product specification type of the surround. 
| drawToSpecification | boolean | A value indicating whether to draw the element to specification size or allow user to manually resize element. 


### CIMTMElevationGuideBarElement 

|Property | Type | Description | 
|---------|--------|--------|
| elevationBandLayerURI | string | Elevation bands feature class, the number of bands in the bar is dependent on the number of bands identified in feature class. 
| numberOfBands | long | The number of bands displayed in the Elevation Guide Bar, if data is from source that does not have Bands field. 
| textSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for text elements in the elevation guide bar. 
| lineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for line elements in the elevation guide bar. 
| highestBandSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The highest band symbol in the elevation guide bar. 
| highBandSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The high band symbol in the elevation guide bar. 
| mediumBandSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The medium band symbol in the elevation guide bar. 
| lowBandSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The low band symbol in the elevation guide bar. 






## CIMTableFrame
#### Layout element used to display tabular data. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMTableFrame 

|Property | Type | Description | 
|---------|--------|--------|
| fields | [[CIMTableFrameField]](CIMLayout.md#cimtableframefield) | The fields displayed by the table frame. 
| mapMemberURI | string | The layer or standalone table that defines the data to display. 
| fillingStrategy | [enumeration TableFrameFillingStrategy](CIMLayout.md#enumeration-tableframefillingstrategy) | The strategy used to query records. 
| fittingStrategy | [enumeration TableFrameFittingStrategy](CIMLayout.md#enumeration-tableframefittingstrategy) | The strategy used to query records. 
| columns | long | The number of columns. 
| minFontSize | double | The limit when reducing font sizes. Values is in points. 
| verticalTextGap | double | The vertical gap around field values. 
| horizontalTextGap | double | The horizontal gap around field values. 
| headingGap | double | The gap between field names and rows. 
| rowGap | double | The gap between rows. 
| fieldGap | double | The gap between fields. 
| columnGap | double | The gap between table columns. 
| headingBackgroundSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The field name/alias background symbol. 
| headingBorderSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The field name/alias border symbol. 
| headingLineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The field name/alias underline symbol. 
| columnBorderSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The column border symbol. 
| alternate1RowBackgroundSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The second alternating data record background symbol. 
| alternate1RowBackgroundCount | long | The alternate 1 row background count. Show even row background for this many rows before alternating. 
| alternate2RowBackgroundSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The first alternating data record background symbol. 
| alternate2RowBackgroundCount | long | The alternate 2 row background count. Show odd row background for this many rows before alternating. 
| rowBorderSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The border symbol for row sections: data records, summary statistics, and statistics totals. 
| customWhereClause | string | The custom where clause. Show rows that match custom where clause when FillingStrategy is set to esriCIMTableFrameFillingStrategy_CustomWhereClause. 
| defaultTableFrameField | [CIMTableFrameField](CIMLayout.md#cimtableframefield) | The default table frame field used when creating new table frames. 
| balanceColumns | boolean | A value indicating whether to balance the columns of the table. 
| rowLimit | long | The maximum number of rows the table frame will show. 0 Indicates "no limit". 
| showHeadings | boolean | A value indicating whether to show the headings. 






## CIMTableFrameField
#### Display properties for fields in a table frame. 


### CIMTableField 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The field name and unique identifier. 
| isVisible | boolean | A value indicating whether the field is visible. 
| width | double | The width of field. A value of 0 indicates "auto size". 
| sortInfo | [enumeration FieldSortInfo](CIMLayout.md#enumeration-fieldsortinfo) | The options when this field is used for sorting. 
| sortOrder | long | The zero based sort order. -1 indicates field isn't used for sorting. 
| fieldOrder | long | The zero based display order. 
| group | boolean | A value indicating whether this is a grouping field. 
| displayName | string | The display name for the field. 


### CIMTableFrameField 

|Property | Type | Description | 
|---------|--------|--------|
| enableWordWrapping | boolean | A value indicating whether to wrap field values that don't fit the width. 
| headingTextSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The field name/alias text symbol. 
| textSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The field value text symbol. 
| backgroundSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The field background symbol. 
| borderSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The field border symbol. 
| verticalLineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol for vertical lines on sides of field. 





### Enumeration: TableFrameFillingStrategy
#### Table frame fitting strategies. 

|Property | Value | Description | 
|---------|--------|--------|
| ShowAllRows| 0| Show all the rows. 
| ShowVisibleRows| 1| Show the rows that are visible. 
| ShowMapSeriesRows| 2| Show the rows that intersect the current map series shape. 
| CustomWhereClause| 3| Show rows that match a custom query. 



### Enumeration: TableFrameFittingStrategy
#### Defines which table rows to display. 

|Property | Value | Description | 
|---------|--------|--------|
| AdjustSize| 0| Reduce fonts sizes to make data fit. 
| AdjustColumns| 1| Flow to multiple columns to make data fit. 
| AdjustColumnsAndSize| 2| Reduce font sizes and flow to multiple columns to make data fit. 
| AdjustFrame| 3| Adjust the frame to fit the specified font sizes and columns. 




## CIMTopoCompassRose
#### Represents a compass rose north arrow which displays declination with a compass dial. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMNorthArrow 

|Property | Type | Description | 
|---------|--------|--------|
| referenceLocation | [Point](ExternalReferences.md#point) | The reference location for a north arrow. 
| calibrationAngle | double | The calibration angle for a north arrow. 


### CIMTopoNorthArrow 

|Property | Type | Description | 
|---------|--------|--------|
| date | [TimeInstant](ExternalReferences.md#timeinstant) | The date used when calculating declination using world magnetic model. 
| zone | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference used for calculating declination, typically a UTM zone. 
| isPrimaryZone | boolean | A value indicating whether the zone is the primary zone. Set to false when using 2nd north arrow for maps that extend across two UTM zones. 
| GMAngle | [CIMDeclination](CIMLayout.md#cimdeclination) | The Grid Magnetic declination. 
| gridConvergence | [CIMDeclination](CIMLayout.md#cimdeclination) | The Grid Convergence declination. 
| directionalNotes | boolean | A value indicating whether the directional notes are displayed on the north arrow. 
| leadingZero | boolean | A value indicating whether a leading zero is displayed for minute coordinates of grid convergence. 
| roundGMAngle | boolean | A value indicating whether GM angle is rounded for display. If true GM angle is displayed to nearest 1/2 degree, if false it is displayed as degrees and minutes. 
| roundMils | boolean | A value indicating whether Mils rounded for display. If true Mils for both GC and GM will be displayed rounded to nearest 10 Mils, otherwise to nearest 1 Mil. If RoundGMAngle is true, this property is ignored. 
| autoUpdate | boolean | A value indicating whether the properties of the topographic north arrow should update automatically based on changes in the map. 
| largeSize | boolean | A value indicating whether the topographic north arrow is displayed in large size. 
| textSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for text elements in topographic north arrow. 
| lineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for line elements in the topographic north arrow. 
| trueNorthMarkerSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol displayed at top of true north line, default is a star. 
| magneticNorthNegativeSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol displayed at top of magnetic north line when the gm-angle is negative. 
| magneticNorthPositiveSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol displayed at top of magnetic north line when the gm-angle is positive. 
| magneticNorthZeroSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol displayed at top of magnetic north line when the gm-angle is 0 degrees. 
| declinationArcSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol used to display declination arc lines. 
| productSpecification | [enumeration MapProductSpecType](CIMLayout.md#enumeration-mapproductspectype) | The map product specification type of topographic north arrow. 
| drawToSpecification | boolean | A value indicating whether to draw the element to specification size or allow user to manually resize element. 
| dateInterval | long | A value indicating the date interval used to calculate declination. The default value is 5 which is based on the interval used by the World Magnetic Model. A value of zero indicates the current date should be used. 


### CIMTopoCompassRose 

|Property | Type | Description | 
|---------|--------|--------|
| degreeLabelFrequency | long | The frequency in which a degree label is displayed. Valid values are 0 to 359. 
| divisionMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol used to draw the division marks on compass dial. 
| subdivisionMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol used to draw the sub division marks on compass dial. 
| degreeMarkSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol used to draw the degree marks on compass dial. 
| divisions | long | The frequency of divisions on the compass dial. Valid values are 0 to 359. 
| subdivisions | long | The frequency of subdivisions on the compass dial. Valid values are 0 to 359. 






## CIMTopoNorthArrow
#### Represents a topographic north arrow which displays declination of true, grid and magnetic north. 


### CIMElement 

|Property | Type | Description | 
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor) | The anchor position of the element. 
| locked | boolean | A value indicating whether the element is locked. Each element in the contents pane has a lock icon. If the icon is shown as locked, you can not select that feature in the layout using the select tool. 
| name | string | The name of the element. 
| visible | boolean | A value indicating whether the element is visible. 
| rotation | double | The rotation of the element. 
| rotationCenter | [Point](ExternalReferences.md#point) | The location of the anchor in page units.This is also the location the feature is rotated around. 
| lockedAspectRatio | boolean | A value indicating whether the aspect ratio for an element is locked. If locked, the width and height values stretch proportionally. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the element. 
| expanded | boolean | A value indicating whether this element is expanded in the contents pane. 


### CIMFrameElement 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon) | The geometry of a frame for an element. 
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe) | The graphic symbology of an element's frame. 


### CIMMapSurround 

|Property | Type | Description | 
|---------|--------|--------|
| mapFrame | string | The map frame associated with the map surround. 
| minScale | double | The minimum scale. 
| maxScale | double | The maximum scale. 


### CIMNorthArrow 

|Property | Type | Description | 
|---------|--------|--------|
| referenceLocation | [Point](ExternalReferences.md#point) | The reference location for a north arrow. 
| calibrationAngle | double | The calibration angle for a north arrow. 


### CIMTopoNorthArrow 

|Property | Type | Description | 
|---------|--------|--------|
| date | [TimeInstant](ExternalReferences.md#timeinstant) | The date used when calculating declination using world magnetic model. 
| zone | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference used for calculating declination, typically a UTM zone. 
| isPrimaryZone | boolean | A value indicating whether the zone is the primary zone. Set to false when using 2nd north arrow for maps that extend across two UTM zones. 
| GMAngle | [CIMDeclination](CIMLayout.md#cimdeclination) | The Grid Magnetic declination. 
| gridConvergence | [CIMDeclination](CIMLayout.md#cimdeclination) | The Grid Convergence declination. 
| directionalNotes | boolean | A value indicating whether the directional notes are displayed on the north arrow. 
| leadingZero | boolean | A value indicating whether a leading zero is displayed for minute coordinates of grid convergence. 
| roundGMAngle | boolean | A value indicating whether GM angle is rounded for display. If true GM angle is displayed to nearest 1/2 degree, if false it is displayed as degrees and minutes. 
| roundMils | boolean | A value indicating whether Mils rounded for display. If true Mils for both GC and GM will be displayed rounded to nearest 10 Mils, otherwise to nearest 1 Mil. If RoundGMAngle is true, this property is ignored. 
| autoUpdate | boolean | A value indicating whether the properties of the topographic north arrow should update automatically based on changes in the map. 
| largeSize | boolean | A value indicating whether the topographic north arrow is displayed in large size. 
| textSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for text elements in topographic north arrow. 
| lineSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used for line elements in the topographic north arrow. 
| trueNorthMarkerSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol displayed at top of true north line, default is a star. 
| magneticNorthNegativeSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol displayed at top of magnetic north line when the gm-angle is negative. 
| magneticNorthPositiveSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol displayed at top of magnetic north line when the gm-angle is positive. 
| magneticNorthZeroSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol displayed at top of magnetic north line when the gm-angle is 0 degrees. 
| declinationArcSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The line symbol used to display declination arc lines. 
| productSpecification | [enumeration MapProductSpecType](CIMLayout.md#enumeration-mapproductspectype) | The map product specification type of topographic north arrow. 
| drawToSpecification | boolean | A value indicating whether to draw the element to specification size or allow user to manually resize element. 
| dateInterval | long | A value indicating the date interval used to calculate declination. The default value is 5 which is based on the interval used by the World Magnetic Model. A value of zero indicates the current date should be used. 





### Enumeration: UnitType
#### Lists the unit type values. 

|Property | Value | Description | 
|---------|--------|--------|
| Percent| 0| Percent. 
| MapUnits| 1| Map Units. 
| PageUnits| 2| Page units. 




## CIMVerticalLegendItem
#### Represents a vertical legend item in a legend. 


### CIMLegendItem 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The legend item name. 
| newColumn | boolean | A value indicating whether a legend item should be placed in a new column. 
| layerNameSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item symbol. 
| manualColumn | long | The manual column assignment for a legend item. 
| keepTogetherOption | [enumeration LegendKeepTogetherOption](CIMLayout.md#enumeration-legendkeeptogetheroption) | A value indicating whether the legend item or group should be kept together. 
| showLayerName | boolean | A value indicating whether the legend item layer name should be displayed. 
| showHeading | boolean | A value indicating whether the legend item heading should be displayed. 
| headingSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item heading symbol. 
| showLabels | boolean | A value indicating whether the legend item labels should be displayed. 
| layer | string | The legend item layer's path. 
| showDescription | boolean | A value indicating whether a legend item description should be displayed. 
| labelSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item label symbol. 
| descriptionSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The legend item description symbol. 
| patchWidth | double | The legend item patch width. Units in points. 
| patchHeight | double | The legend item patch height. Units in points. 
| autoVisibility | boolean | A value indicating whether the legend item should be displayed if in the visible extent. 
| useMapSeriesShape | boolean | A value indicating whether to use map series shape instead of map frame to find dynamic classes. 
| classIndent | double | Distance from the class name to the edge of the legend. 
| headingIndent | double | Distance from the heading to the edge of the legend. 
| layerNameIndent | double | Distance of the layer name to the edge of the legend. 
| showGroupLayerName | boolean | A value indicating whether to show the containing group layer name above the item. 
| groupLayerNameSymbol | [CIMSymbolReference](CIMRenderers.md#cimsymbolreference) | The symbol used to display the group layer name. 
| scaleToPatch | boolean | A value indicating whether to scale the symbol to the specified patch size. 
| showCounts | boolean | A value indicating whether the legend should display count statistics. 
| countFormat | [NumberFormat](Types.md#numberformat) | The feature count format. 
| countPrefix | string | The feature count prefix. 
| countSuffix | string | The feature count suffix. 
| isVisible | boolean | A value indicating whether the legend item is visible. 
| groupFilter | [long] | A value specifying which legend groups are displayed. 


### CIMLegendItemArrangement 

|Property | Type | Description | 
|---------|--------|--------|
| arrangement | [enumeration LegendItemArrangement](Types.md#enumeration-legenditemarrangement) | The Arrangement. 


### CIMVerticalLegendItem 

|Property | Type | Description | 
|---------|--------|--------|
| patchAlignment | [enumeration HorizontalAlignment](CIMSymbols.md#enumeration-horizontalalignment) | A value to allow alignment of graduated symbols to be specified. 



