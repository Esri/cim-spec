

### Enumeration: Anchor
A list of anchor positions for an element on a page layout.

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




## CIMAutoCamera
Represents the camera settings associated with a map frame on a page layout.


### CIMAutoCamera

|Property | Type | Description |
|---------|--------|--------|
| camera | [CIMViewCamera](CIMMap.md#cimviewcamera)|The camera associated with the map frame.
| autoCameraType | [enumeration AutoCameraType](CIMLayout.md#enumeration-autocameratype)|The camera type.
| extent | [Envelope](ExternalReferences.md#envelope)|The extent for a map frame when using the fixed constraint.
| intersectLayerPath | string|The layer being used to set the camera when using the map frame link constraint.
| mapFrameLinkName | string|The map frame name being used to set the camera when using the map frame link constraint.
| margin | number //double|The margin value for a map frame with a map frame link constraint.
| marginType | [enumeration UnitType](CIMLayout.md#enumeration-unittype)|The margin type for a map frame with a map frame link constraint.
| marginUnits | [Unit](ExternalReferences.md#unit)|The margin units for a map frame with a map frame link constraint.
| source | [enumeration AutoCameraSource](CIMLayout.md#enumeration-autocamerasource)|The extent constraint associated with the map frame.
| syncRotation | boolean|A boolean indicating if the map frame should rotate when using a map frame link constraint.





### Enumeration: AutoCameraSource
A list of the advanced map frame options that further controls the camera behavior.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| Use navigation tools to set the extent.
| Fixed| 1| The extent specified will not change.
| MapFrameLink| 2| Base the extent on another map frame.
| MapSeriesLink| 3| Future implementation



### Enumeration: AutoCameraType
A list of the options available when using a fixed constraint.

|Property | Value | Description |
|---------|--------|--------|
| Center| 0| Show the map at the specified center point.
| Scale| 1| Show the map at the specified scale.
| CenterAndScale| 2| Show the map at the specified center point and scale.
| Extent| 3| Show the map at a specified extent.




## CIMDeclination
Represents the properties of a declination calculated using World Magnetic Model.


### CIMDeclination

|Property | Type | Description |
|---------|--------|--------|
| direction | [enumeration DeclinationDirection](CIMLayout.md#enumeration-declinationdirection)|Direction the declination is reckoned from
| degrees | number //int32|The degrees of declination
| minutes | number //int32|The minutes of declination
| mils | number //double|The mil radians of declination





### Enumeration: DeclinationDirection
Defines which direction declination will be calculated from.

|Property | Value | Description |
|---------|--------|--------|
| West| 0| Declination reckoned West (counterclockwise)
| East| 1| Declination reckoned East (clockwise)




## CIMDoubleFillScaleBar
Represents a double filled alternating scale bar


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMMapSurround

|Property | Type | Description |
|---------|--------|--------|
| mapFrame | string|The map frame associated with the map surround.


### CIMScaleBar

|Property | Type | Description |
|---------|--------|--------|
| alignToZeroPoint | boolean|A boolean indicating if scale bar should align to zero.
| barHeight | number //double|The scale bar height.
| division | number //double|The division value
| divisions | number //int32|The number of divisions.
| divisionsBeforeZero | number //int32|The number of divisions before zero.
| fittingStrategy | [enumeration ScaleBarFittingStrategy](CIMLayout.md#enumeration-scalebarfittingstrategy)|The fitting strategy.
| labelFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency)|The label frequency.
| labelGap | number //double|The label gap value.
| labelPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition)|The label position.
| labelSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The label symbol.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format.
| subdivisions | number //int32|The number of subdivisions.
| unitLabel | string|The unit label.
| unitLabelGap | number //double|The unit label gap. Units set in points.
| unitLabelPosition | [enumeration ScaleBarLabelPosition](CIMLayout.md#enumeration-scalebarlabelposition)|The unit label position
| unitLabelSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The unit label symbol.
| units | [Unit](ExternalReferences.md#unit)|The units for the scale bar.
| useFractionCharacters | boolean|A boolean indicating if fractional characters should be used.
| zeroPoint | [Point](ExternalReferences.md#point)|The zero location for the scale bar.
| computeAtCenter | boolean|The flag that computes scale at map center.


### CIMScaleMarks

|Property | Type | Description |
|---------|--------|--------|
| divisionMarkHeight | number //double|The division marker height value.
| divisionMarkSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The division marker symbol.
| markFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency)|The division marker frequency.
| markPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition)|The division marker position.
| subdivisionMarkHeight | number //double|The subdivision marker height.
| subdivisionMarkSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The subdivision marker symbol


### CIMDoubleFillScaleBar

|Property | Type | Description |
|---------|--------|--------|
| fillSymbol1 | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The first symbol of an alternating scale bar.
| fillSymbol2 | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The second symbol of an alternating scale bar.
| style | [enumeration DoubleFillScaleBarStyle](CIMLayout.md#enumeration-doublefillscalebarstyle)|The style for the scale bar.





### Enumeration: DoubleFillScaleBarStyle
A list of the styles available for a double file scale bar.

|Property | Value | Description |
|---------|--------|--------|
| Hollow| 0| Hollow fill.
| Alternating| 1| Alternating fill.
| DoubleAlternating| 2| Double alternating fill.



### Enumeration: EndPointPosition
Enumerates which end a component is visible.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| No end point is selected
| FromPoint| 1| From point.
| ToPoint| 2| To point.



### Enumeration: EndPointSelection
Represents the selection of endPoints.

|Property | Value | Description |
|---------|--------|--------|
| First| 1| First point selection.
| Interior| 2| Interior point selection.
| Last| 4| Last point selection.



### Enumeration: ExtentFitType
Extent fit types.

|Property | Value | Description |
|---------|--------|--------|
| BestFit| 0| Best fit.
| ExtentCenter| 1| Center the extent.
| DataDriven| 2| Data driven.




## CIMExtentIndicator
Represents an extent indicator which is used to display the visible extent of other map frames in an associated map frame.


### CIMExtentIndicator

|Property | Type | Description |
|---------|--------|--------|
| sourceMapFrame | string|The source map frame's extent to be displayed.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The area symbol used to represent the extent indicator.
| leaderType | [enumeration LeaderType](CIMLayout.md#enumeration-leadertype)|The leader style used to connect the associated extents.
| leaderSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The leader symbol used to connect the associated extents.
| collapseSize | number //double|The minimum size of the extent indicator before symbolizing it as a point. Units in points.
| pointSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The point symbol used to symbolize an extent indicator.
| name | string|The name of the extent indicator.
| isVisible | boolean|The visibility of the extent indicator.
| avoidLabelConflict | boolean|Future implementation
| symbolizeExterior | boolean|A boolean indicating if the area symbol should be applied outside the extent.
| extentIndicatorType | [enumeration ExtentIndicatorType](CIMLayout.md#enumeration-extentindicatortype)|Future implementation





### Enumeration: ExtentIndicatorType
Future implementation

|Property | Value | Description |
|---------|--------|--------|
| Frame| 0| Future implementation
| Rectangle| 1| Future implementation
| IndexFeatureFromDDP| 2| Future implementation




## CIMExteriorTick
Class that represents an exterior tick for a grid.


### CIMTick

|Property | Type | Description |
|---------|--------|--------|
| length | number //double|The length of the tick in page units.
| offset | number //double|The offset of the tick in page units.
| isVisible | boolean|The flag that toggles the visibility of the tick.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the tick.
| gridEndpoint | [CIMGridEndpoint](CIMLayout.md#cimgridendpoint)|The end point for the tick.


### CIMExteriorTick

|Property | Type | Description |
|---------|--------|--------|





### Enumeration: FieldSortInfo
Represents the sort information for a field.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| Field is not sorted.
| Asc| 1| The field is sorted by case insensitive ascending order.
| AscCase| 2| The field is sorted by case sensitive ascending order.
| Desc| 4| The field is sorted by case insensitive descending order.
| DescCase| 8| The field is sorted by case sensitive descending order.



### Enumeration: FieldStatisticsFlag
Represents field statistics.

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




## CIMGraphicElement
Represents the CIM representation of an element on a page layout.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMGraphicElement

|Property | Type | Description |
|---------|--------|--------|
| graphic | [Graphic](Types.md#graphic)|The CIMGraphic for an element on a page layout.






## CIMGraticule
Represents a graticule for a map frame.


### CIMMapGrid

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name of the Grid or Graticule.
| isVisible | boolean|The visiblity of the Grid or Graticule.
| neatlineSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The neatline symbol of the Grid or Graticule.


### CIMGraticule

|Property | Type | Description |
|---------|--------|--------|
| customOrigin | [Point](ExternalReferences.md#point)|The custom origin of a graticule.
| geographicCoordinateSystem | [GeographicCoordinateSystem](ExternalReferences.md#geographiccoordinatesystem)|The spatial reference of a graticule.
| gridLines | [CIMGridLine](Types.md#cimgridline) |The collection of latitudes and longitudes for a graticule.
| isAutoScaled | boolean|The flag that automatically adjusts the interval of the graticules based on scale of the map.





### Enumeration: GridElementType
The type of component of the grid.

|Property | Value | Description |
|---------|--------|--------|
| Line| 0| Represents lines.
| Tick| 1| Represents ticks.
| Label| 2| Represents labels.
| Corner| 3| Represents the corner label.
| IntersectionPoint| 4| Represents a grid component used to show intersection points on a map grid.




## CIMGridEndpoint
Represents an end point of a component. For ex: The labels for ticks are defined using an endPoint object.


### CIMGridEndpoint

|Property | Type | Description |
|---------|--------|--------|
| gridLabelTemplate | [CIMGridLabelTemplate](CIMLayout.md#cimgridlabeltemplate)|The grid label template for each endpoint
| offset | number //double|The offset of the labels.
| position | number //int32|The position of the labels of the end points.
| lineSelection | number //int32|The end point selection.





### Enumeration: GridLadderLabelPosition
Represents the position at which the ladder labels are drawn.

|Property | Value | Description |
|---------|--------|--------|
| Half| 0| Represents the ladder label at half the value of visible extent.
| Third| 1| Represents the ladder label at third of the value of visible extent.
| Quarter| 2| Represents the ladder label at quarter the value of visible extent.




## CIMGridLine
Represents latitudes or longitudes for a graticule. Represents eastings or nothings for a grid.


### CIMGridLine

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name of the grid line.
| elementType | [enumeration GridElementType](CIMLayout.md#enumeration-gridelementtype)|The type of the graticule element.
| gridLineOrientation | [enumeration GridLineOrientation](CIMLayout.md#enumeration-gridlineorientation)|The orientation of the gridLine with reference to the coordinate sytem of the spatial reference. For graticules it is latitudes and longitudes. For grids it is eastings and northings.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol of the gridline.
| pattern | [CIMGridPattern](CIMLayout.md#cimgridpattern)|The pattern of the grid lines.
| fromTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick)|Wraps the properties of the tick that is at the start of the grid line it represents.
| toTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick)|Wraps the properties of the tick that is at the end of the grid line it represents.
| interiorTicks | [CIMInteriorTick](CIMLayout.md#ciminteriortick) |Wraps the properties of the interior ticks for a grid line.
| visibleIndices | [long]|Represents the visibility of the corner labels to edges.





### Enumeration: GridLineOrientation
Represents the orientation of the grid line.

|Property | Value | Description |
|---------|--------|--------|
| NorthSouth| 0| North-South
| EastWest| 1| East-West




## CIMGridPattern
Defines pattern for a component.


### CIMGridPattern

|Property | Type | Description |
|---------|--------|--------|
| interval | number //double|The interval of the component the pattern represents.
| start | number //double|The start pattern of the component.
| stop | number //double|The stop pattern of the component.
| gap | number //double|The gap pattern of the component.






## CIMGroupElement
Represents a collection of layout elements in a group element.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMGroupElement

|Property | Type | Description |
|---------|--------|--------|


### CIMElementContainer

|Property | Type | Description |
|---------|--------|--------|
| elements | [CIMElement](Types.md#cimelement) |A collection of layout elements.






## CIMGroupFooter
Represents a group footer section in a report.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMElementContainer

|Property | Type | Description |
|---------|--------|--------|
| elements | [CIMElement](Types.md#cimelement) |A collection of layout elements.


### CIMGroupElement

|Property | Type | Description |
|---------|--------|--------|


### CIMReportSectionElement

|Property | Type | Description |
|---------|--------|--------|
| autoSize | boolean|The value indicating the section height will grow and shrink to fit the content of the section.
| elementFieldProperties | [CIMReportElementFieldProperties](CIMLayout.md#cimreportelementfieldproperties) |The field properties that will be applied to the elements.
| excludePageNumberPages | string|The comma delimited list of pages to exclude the page number from.
| excludeSectionPages | string|The comma delimited list of pages to exclude the section from.
| startOnNewPage | boolean|The value indicating the section should start on a new page.


### CIMGroupFooter

|Property | Type | Description |
|---------|--------|--------|
| field | string|The grouping field for the section.






## CIMGroupHeader
Represents a group header section in a report.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMElementContainer

|Property | Type | Description |
|---------|--------|--------|
| elements | [CIMElement](Types.md#cimelement) |A collection of layout elements.


### CIMGroupElement

|Property | Type | Description |
|---------|--------|--------|


### CIMReportSectionElement

|Property | Type | Description |
|---------|--------|--------|
| autoSize | boolean|The value indicating the section height will grow and shrink to fit the content of the section.
| elementFieldProperties | [CIMReportElementFieldProperties](CIMLayout.md#cimreportelementfieldproperties) |The field properties that will be applied to the elements.
| excludePageNumberPages | string|The comma delimited list of pages to exclude the page number from.
| excludeSectionPages | string|The comma delimited list of pages to exclude the section from.
| startOnNewPage | boolean|The value indicating the section should start on a new page.


### CIMGroupHeader

|Property | Type | Description |
|---------|--------|--------|
| field | string|The grouping field for the section.






## CIMGuide
Represents a guide used to snap elements on a page layout.


### CIMGuide

|Property | Type | Description |
|---------|--------|--------|
| position | number //double|The position of the guide.
| orientation | [enumeration Orientation](CIMLayout.md#enumeration-orientation)|The horizontal or vertical orientation of the guide.






## CIMHorizontalBarLegendItem
Represents a horizontal bar legend item.


### CIMLegendItem

|Property | Type | Description |
|---------|--------|--------|
| name | string|The legend item name.
| newColumn | boolean|A boolean indicating if a legend item should be placed in a new column.
| layerNameSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item symbol.
| columns | number //int32|The number of columns for a legend item.
| keepTogether | boolean|A boolean indicating if the legend item should be kept together.
| showLayerName | boolean|A boolean indicating if the legend item layer name should be displayed.
| showHeading | boolean|A boolean indicating if the legend item heading should be displayed.
| headingSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item heading symbol.
| showLabels | boolean|A boolean indicating if legend item labels should be displayed.
| layer | string|The legend item layer's path.
| showDescription | boolean|A boolean indicating if a legend item description should be displayed.
| labelSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item label symbol.
| descriptionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item description symbol.
| patchWidth | number //double|The legend item patch width. Units in points.
| patchHeight | number //double|The legend item patch height. Units in points.
| autoVisibility | boolean|A boolean indicating if the legend item should be displayed if in the visible extent.
| useMapSeriesShape | boolean|A flag to use map series shape instead of map frame to find dynamic classes.
| classIndent | number //double|The distance from the class name to the edge of the legend.
| headingIndent | number //double|The distance from the heading to the edge of the legend.
| layerNameIndent | number //double|The distance of the layer name to the edge of the legend.
| showGroupLayerName | boolean|A flag to show the containing group layer name above the item.
| groupLayerNameSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol used to display the group layer name.
| scaleToPatch | boolean|The flag to scale the symbol to the specified patch size.
| showCounts | boolean|A boolean indicating if the legend should display count statistics.
| countFormat | [NumberFormat](Types.md#numberformat)|The feature count format.
| countPrefix | string|The feature count prefix.
| countSuffix | string|The feature count suffix.
| isVisible | boolean|The visibility of the legend item.


### CIMHorizontalBarLegendItem

|Property | Type | Description |
|---------|--------|--------|
| angleAbove | number //double|Future implementation
| angleBelow | number //double|Future implementation


### CIMVerticalLegendItem

|Property | Type | Description |
|---------|--------|--------|
| arrangement | [enumeration LegendItemArrangement](CIMLayout.md#enumeration-legenditemarrangement)|The arrangement.






## CIMHorizontalLegendItem
Represents a horizontal legend item.


### CIMLegendItem

|Property | Type | Description |
|---------|--------|--------|
| name | string|The legend item name.
| newColumn | boolean|A boolean indicating if a legend item should be placed in a new column.
| layerNameSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item symbol.
| columns | number //int32|The number of columns for a legend item.
| keepTogether | boolean|A boolean indicating if the legend item should be kept together.
| showLayerName | boolean|A boolean indicating if the legend item layer name should be displayed.
| showHeading | boolean|A boolean indicating if the legend item heading should be displayed.
| headingSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item heading symbol.
| showLabels | boolean|A boolean indicating if legend item labels should be displayed.
| layer | string|The legend item layer's path.
| showDescription | boolean|A boolean indicating if a legend item description should be displayed.
| labelSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item label symbol.
| descriptionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item description symbol.
| patchWidth | number //double|The legend item patch width. Units in points.
| patchHeight | number //double|The legend item patch height. Units in points.
| autoVisibility | boolean|A boolean indicating if the legend item should be displayed if in the visible extent.
| useMapSeriesShape | boolean|A flag to use map series shape instead of map frame to find dynamic classes.
| classIndent | number //double|The distance from the class name to the edge of the legend.
| headingIndent | number //double|The distance from the heading to the edge of the legend.
| layerNameIndent | number //double|The distance of the layer name to the edge of the legend.
| showGroupLayerName | boolean|A flag to show the containing group layer name above the item.
| groupLayerNameSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol used to display the group layer name.
| scaleToPatch | boolean|The flag to scale the symbol to the specified patch size.
| showCounts | boolean|A boolean indicating if the legend should display count statistics.
| countFormat | [NumberFormat](Types.md#numberformat)|The feature count format.
| countPrefix | string|The feature count prefix.
| countSuffix | string|The feature count suffix.
| isVisible | boolean|The visibility of the legend item.


### CIMHorizontalLegendItem

|Property | Type | Description |
|---------|--------|--------|
| arrangement | [enumeration LegendItemArrangement](CIMLayout.md#enumeration-legenditemarrangement)|The arrangement.






## CIMInteriorTick
Class that represents an interior tick for a grid.


### CIMTick

|Property | Type | Description |
|---------|--------|--------|
| length | number //double|The length of the tick in page units.
| offset | number //double|The offset of the tick in page units.
| isVisible | boolean|The flag that toggles the visibility of the tick.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the tick.
| gridEndpoint | [CIMGridEndpoint](CIMLayout.md#cimgridendpoint)|The end point for the tick.


### CIMInteriorTick

|Property | Type | Description |
|---------|--------|--------|
| pattern | [CIMGridPattern](CIMLayout.md#cimgridpattern)|Represents a pattern for the interior ticks.






## CIMLadderGridLine
Represents internal labels for a MapGrid.


### CIMGridLine

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name of the grid line.
| elementType | [enumeration GridElementType](CIMLayout.md#enumeration-gridelementtype)|The type of the graticule element.
| gridLineOrientation | [enumeration GridLineOrientation](CIMLayout.md#enumeration-gridlineorientation)|The orientation of the gridLine with reference to the coordinate sytem of the spatial reference. For graticules it is latitudes and longitudes. For grids it is eastings and northings.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol of the gridline.
| pattern | [CIMGridPattern](CIMLayout.md#cimgridpattern)|The pattern of the grid lines.
| fromTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick)|Wraps the properties of the tick that is at the start of the grid line it represents.
| toTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick)|Wraps the properties of the tick that is at the end of the grid line it represents.
| interiorTicks | [CIMInteriorTick](CIMLayout.md#ciminteriortick) |Wraps the properties of the interior ticks for a grid line.
| visibleIndices | [long]|Represents the visibility of the corner labels to edges.


### CIMLadderGridLine

|Property | Type | Description |
|---------|--------|--------|
| dynamicStringTemplate | string|Represents dynamic string used to represent the ladder label of the mapgrid.
| gapX | number //double|Represents the gap in the X-Coordinate direction between the label extent and grid components.
| gapY | number //double|Represents the gap in the Y-Coordinate direction between the label extent and grid components.
| position | [enumeration GridLadderLabelPosition](CIMLayout.md#enumeration-gridladderlabelposition)|Represents the position of the ladder labels.






## CIMLayout
Represents a layout in a project. A layout is a collection of visual elements arranged on a logical sheet of paper. A layout in a GIS is typically used to display one or more maps at a particular extent and scale. The layout is used to compose a presentation of data, describe the maps, and/or tell a story of the map data. A layout defines a logical sheet of paper. It has a height and a width, and also a linear unit used to display positions on the page. It can have a snapping grid and a set of guides to help users arrange its elements. The layout contains an ordered list of elements. When the layout draws, it tells each element to draw, in order.


### CIMDefinition

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| URI | string|The URI of the definition. Typically set by the system and used as an identifier.
| sourceURI | string|The source URI of the item. Set if sourced from an external item such as an item on a portal.
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|The time the definition was last modfied.
| metadataURI | string|The metadata URI.
| useSourceMetadata | boolean|A boolean indicating if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project.


### CIMLayoutDefinition

|Property | Type | Description |
|---------|--------|--------|
| page | [CIMPage](CIMLayout.md#cimpage)|The CIMPage for the layout.
| dateExported | [TimeInstant](ExternalReferences.md#timeinstant)|The date exported property for a layout.
| datePrinted | [TimeInstant](ExternalReferences.md#timeinstant)|The date printed property for a layout.
| mapSeries | [MapSeries](Types.md#mapseries)|The map series for a layout.
| colorModel | [enumeration ColorModel](CIMEnumerations.md#enumeration-colormodel)|The color model for a layout.


### CIMElementContainer

|Property | Type | Description |
|---------|--------|--------|
| elements | [CIMElement](Types.md#cimelement) |A collection of layout elements.






## CIMLayoutView
Represents a layout view in the project.


### CIMView

|Property | Type | Description |
|---------|--------|--------|
| viewXML | string|The view properties as XML.
| viewableObjectPath | string|The path of the item in the view.
| viewType | string|The view type as a string.
| instanceID | number //int32|The instance identifier of this view.


### CIMLayoutView

|Property | Type | Description |
|---------|--------|--------|
| extent | [Envelope](ExternalReferences.md#envelope)|The extent for the view.
| defaultMapFrameName | string|The default map for a view.





### Enumeration: LeaderType
A list of leader styles for extent indicators.

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
Represents a legend on a layout.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMMapSurround

|Property | Type | Description |
|---------|--------|--------|
| mapFrame | string|The map frame associated with the map surround.


### CIMLegend

|Property | Type | Description |
|---------|--------|--------|
| autoAdd | boolean|A boolean indicating if an items should automatically be added to the legend.
| autoFonts | boolean|A boolean indicating if the fonts should automatically be sized.
| autoReorder | boolean|A boolean indicating if the items should automatically be ordered when added.
| autoVisibility | boolean|A boolean indicating if the items should display when not in the visible extent.
| defaultPatchHeight | number //double|An items default patch height. Units in points.
| defaultPatchWidth | number //double|An items default patch width. Units in points.
| descriptionWidth | number //double|The description width threshold. Units in points.
| groupGap | number //double|The gap between groups. Units in points.
| headingGap | number //double|The heading gap. Units in points.
| horizontalItemGap | number //double|The gap between horizontal items. Units in points.
| horizontalPatchGap | number //double|The horizontal gap between patches. Units in points.
| items | [CIMLegendItem](Types.md#cimlegenditem) |A collection of items in a layout.
| labelWidth | number //double|The label width. Units in points.
| minFontSize | number //double|The minimum font size. Units in points.
| rightToLeft | boolean|A boolean indicating if right to left orientation should be applied.
| scaleSymbols | boolean|A boolean indicating if symbols should be scaled.
| showTitle | boolean|A boolean indicating if the legend title should be displayed.
| textGap | number //double|The gap between text. Units in points.
| title | string|The title for the legend.
| titleGap | number //double|The title gap. Units in points.
| titleSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the title.
| verticalItemGap | number //double|The vertical gap between items. Units in points,
| verticalPatchGap | number //double|The vertical gap between patches. Units in points.
| layerNameGap | number //double|The layer name gap. Units in points.
| featureCountPrefix | string|The feature count prefix. Deprecated in 1.4. Use count prefix in legend item instead.
| featureCountSuffix | string|The feature count suffix. Deprecated in 1.4. Use count suffix in legend item instead.
| fittingStrategy | [enumeration LegendFittingStrategy](CIMLayout.md#enumeration-legendfittingstrategy)|The legends fitting strategy.
| groupLayerNameGap | number //double|The gap following the group layer name.
| columns | number //int32|The number of legend columns when either of the following fitting strategies is in effect: SpecifyColumnsAndAdjustFrame or SpecifyColumnsAndAdjustSize
| makeColumnsSameWidth | boolean|The flag that ensures that all the columns are the same width.
| defaultLegendItem | [LegendItem](Types.md#legenditem)|The default legend item used as the basis for new legend item creation.





### Enumeration: LegendFittingStrategy
A list of legend fitting strategies.

|Property | Value | Description |
|---------|--------|--------|
| AdjustSize| 0| Adjust the size of the text.
| AdjustColumns| 1| Adjust the number of columns within the frame.
| AdjustColumnsAndSize| 2| Adjust the number of columns and size of the text.
| AdjustFrame| 3| Adjust the size of the legend frame.



### Enumeration: LegendItemArrangement
A list of legend item arrangement options.

|Property | Value | Description |
|---------|--------|--------|
| PatchLabelDescription| 0| Display patch, label, then description.
| PatchDescriptionLabel| 1| display patch, description, then label.
| LabelPatchDescription| 2| Display label, patch, then description.
| LabelDescriptionPatch| 3| Display label, description, then patch.
| DescriptionPatchLabel| 4| Display description, patch, then label.
| DescriptionLabelPatch| 5| Display description, label, then patch.




## CIMMGRSGridLine
Represents a gridLine to draw the 100,000 MGRS grids.


### CIMGridLine

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name of the grid line.
| elementType | [enumeration GridElementType](CIMLayout.md#enumeration-gridelementtype)|The type of the graticule element.
| gridLineOrientation | [enumeration GridLineOrientation](CIMLayout.md#enumeration-gridlineorientation)|The orientation of the gridLine with reference to the coordinate sytem of the spatial reference. For graticules it is latitudes and longitudes. For grids it is eastings and northings.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol of the gridline.
| pattern | [CIMGridPattern](CIMLayout.md#cimgridpattern)|The pattern of the grid lines.
| fromTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick)|Wraps the properties of the tick that is at the start of the grid line it represents.
| toTick | [CIMExteriorTick](CIMLayout.md#cimexteriortick)|Wraps the properties of the tick that is at the end of the grid line it represents.
| interiorTicks | [CIMInteriorTick](CIMLayout.md#ciminteriortick) |Wraps the properties of the interior ticks for a grid line.
| visibleIndices | [long]|Represents the visibility of the corner labels to edges.


### CIMMGRSGridLine

|Property | Type | Description |
|---------|--------|--------|
| XOffset | number //double|Represents the offset in the x-coordinate direction for the grid label
| YOffset | number //double|Represents the offset in the y-coordinate direction for the grid label
| labelPosition | [enumeration MGRSLabelPosition](CIMLayout.md#enumeration-mgrslabelposition)|Represents the position of the label in the 100,000m grid square.





### Enumeration: MGRSLabelPosition
Represents the position of the MGRS label in the 100,000m grid square

|Property | Value | Description |
|---------|--------|--------|
| Corner| 1| Represents the corner position of the label in the 100,000m grid square.
| Center| 2| Represents the center position of the label in the 100,000m grid square.




## CIMMapFrame
Represents a map frame on a page layout.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMMapFrame

|Property | Type | Description |
|---------|--------|--------|
| autoCamera | [CIMAutoCamera](CIMLayout.md#cimautocamera)|The camera associated with the map frame.
| URI | string|The path to the map frame in the project.
| view | [CIMMapView](CIMDocument.md#cimmapview)|The view associated with the map frame.
| extentIndicators | [CIMExtentIndicator](CIMLayout.md#cimextentindicator) |The extent indicators associated with the map frame.
| grids | [CIMMapGrid](Types.md#cimmapgrid) |The Grids and Graticules associated with the MapFrame.






## CIMMarkerNorthArrow
Represents a marker north arrow on a page layout.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMMapSurround

|Property | Type | Description |
|---------|--------|--------|
| mapFrame | string|The map frame associated with the map surround.


### CIMNorthArrow

|Property | Type | Description |
|---------|--------|--------|
| referenceLocation | [Point](ExternalReferences.md#point)|The reference location for a north arrow.
| calibrationAngle | number //double|The calibration angle for a north arrow.


### CIMMarkerNorthArrow

|Property | Type | Description |
|---------|--------|--------|
| pointSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The point symbol for a north arrow.
| northType | [enumeration NorthType](CIMLayout.md#enumeration-northtype)|The type of north arrow.






## CIMMeasuredGrid
Represents a measured grid of the mapFrame.


### CIMMapGrid

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name of the Grid or Graticule.
| isVisible | boolean|The visiblity of the Grid or Graticule.
| neatlineSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The neatline symbol of the Grid or Graticule.


### CIMMeasuredGrid

|Property | Type | Description |
|---------|--------|--------|
| customOrigin | [Point](ExternalReferences.md#point)|The custom origin of the measured grid.
| projectedCoordinateSystem | [ProjectedCoordinateSystem](ExternalReferences.md#projectedcoordinatesystem)|The projected coordinate system of the grid.
| gridLines | [CIMGridLine](Types.md#cimgridline) |The gridLines of the measured grid.
| isAutoScaled | boolean|The property to turn the auto-scaling on/off






## CIMMeterReferenceGuide
Provides a set of instructions and examples that enable users to compose standard grid reference.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMMapSurround

|Property | Type | Description |
|---------|--------|--------|
| mapFrame | string|The map frame associated with the map surround.


### CIMMeterReferenceGuide

|Property | Type | Description |
|---------|--------|--------|
| autoUpdate | boolean|A boolean indicating whether the properties of this element should update automatically based on the changes in the map
| specificationType | [enumeration MeterReferenceSpecType](CIMLayout.md#enumeration-meterreferencespectype)|The layout of the element components for the target map product.
| gridSquareType | [enumeration MeterReferenceSquareType](CIMLayout.md#enumeration-meterreferencesquaretype)|The type of the 100,000-Square identification area.
| isSingleGridZone | boolean|A boolean indicating whether the grid zone is using single or multiple designators.
| properties | [CIMMeterReferenceProperties](CIMLayout.md#cimmeterreferenceproperties)|The display properties of the meter reference guide.
| textSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol used for the text elements in the meter reference guide.
| lineSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol used for the grid lines in the meter reference guide.






## CIMMeterReferenceProperties
Defines the display properties of the meter reference guide.


### CIMMeterReferenceProperties

|Property | Type | Description |
|---------|--------|--------|
| gridSquareUpperLeft | string|The text displayed in the upper left corner of the square identification area.
| gridSquareUpperRight | string|The text displayed in the upper right corner of the square identification area.
| gridSquareLowerLeft | string|The text displayed in the lower left corner of the square identification area.
| gridSquareLowerRight | string|The text displayed in the lower right corner of the square identification area.
| gridSquareUpperLeftDual | string|The auxiliary text displayed in the upper left corner of the square identification area.
| gridSquareUpperRightDual | string|The auxiliary text displayed in the upper left corner of the square identification area.
| gridSquareLowerLeftDual | string|The auxiliary text displayed in the lower left corner of the square identification area.
| gridSquareLowerRightDual | string|The auxiliary text displayed in the lower right corner of the square identification area.
| gridSquareVerticalSeparator | number //int32|The vertical separator value of the square identification area.
| gridSquareHorizontalSeparator | number //int32|The horizontal separator value of the square identification area.
| gridSquareHorizontalSeparatorDual | number //int32|The horizontal auxiliary separator value of the square identification area.
| gridZoneUpperLeft | string|The text displayed in the upper left corner of the grid zone designation area.
| gridZoneUpperRight | string|The text displayed in the upper right corner of the grid zone designation area.
| gridZoneLowerLeft | string|The text displayed in the lower left corner of the grid zone designation area.
| gridZoneLowerRight | string|The text displayed in the lower right corner of the grid zone designation area.
| gridZoneLatitude | number //int32|The latitude of the grid zone.
| gridZoneLongitude | number //int32|The longitude of the grid zone.





### Enumeration: MeterReferenceSpecType
Defines the layout types that meet different map product specifications.

|Property | Value | Description |
|---------|--------|--------|
| TLM| 0| Topographic Line Map
| ICM| 1| Image City Map
| JOG| 2| Joint Operation Graphics



### Enumeration: MeterReferenceSquareType
Defines options for 100,000-Square identification area.

|Property | Value | Description |
|---------|--------|--------|
| Single| 0| Single location identifier
| Multiple| 1| Multiple location identifiers for additional information
| DualGrid| 2| Enables location identifiers across multiple UTM zones.




## CIMNestedLegendItem
Represents a nested legend item in a legend.


### CIMLegendItem

|Property | Type | Description |
|---------|--------|--------|
| name | string|The legend item name.
| newColumn | boolean|A boolean indicating if a legend item should be placed in a new column.
| layerNameSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item symbol.
| columns | number //int32|The number of columns for a legend item.
| keepTogether | boolean|A boolean indicating if the legend item should be kept together.
| showLayerName | boolean|A boolean indicating if the legend item layer name should be displayed.
| showHeading | boolean|A boolean indicating if the legend item heading should be displayed.
| headingSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item heading symbol.
| showLabels | boolean|A boolean indicating if legend item labels should be displayed.
| layer | string|The legend item layer's path.
| showDescription | boolean|A boolean indicating if a legend item description should be displayed.
| labelSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item label symbol.
| descriptionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item description symbol.
| patchWidth | number //double|The legend item patch width. Units in points.
| patchHeight | number //double|The legend item patch height. Units in points.
| autoVisibility | boolean|A boolean indicating if the legend item should be displayed if in the visible extent.
| useMapSeriesShape | boolean|A flag to use map series shape instead of map frame to find dynamic classes.
| classIndent | number //double|The distance from the class name to the edge of the legend.
| headingIndent | number //double|The distance from the heading to the edge of the legend.
| layerNameIndent | number //double|The distance of the layer name to the edge of the legend.
| showGroupLayerName | boolean|A flag to show the containing group layer name above the item.
| groupLayerNameSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol used to display the group layer name.
| scaleToPatch | boolean|The flag to scale the symbol to the specified patch size.
| showCounts | boolean|A boolean indicating if the legend should display count statistics.
| countFormat | [NumberFormat](Types.md#numberformat)|The feature count format.
| countPrefix | string|The feature count prefix.
| countSuffix | string|The feature count suffix.
| isVisible | boolean|The visibility of the legend item.


### CIMNestedLegendItem

|Property | Type | Description |
|---------|--------|--------|
| autoLayout | boolean|The option for automatic layout of the legend item.
| labelEnds | boolean|A boolean indicating if the ends of a nested legend item should be labeled.
| leaderSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The leader symbol.
| outlineSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The outline symbol for the nested legend item.
| leaderOverhang | number //double|The leader overhang value for a nested legend item.
| showOutlines | boolean|A boolean indicating if outlines should be displayed for a nested legend item.
| textHorizontalAlignment | [enumeration HorizontalAlignment](CIMSymbols.md#enumeration-horizontalalignment)|The horizontal text alignment for a nested legend item.


### CIMHorizontalLegendItem

|Property | Type | Description |
|---------|--------|--------|
| arrangement | [enumeration LegendItemArrangement](CIMLayout.md#enumeration-legenditemarrangement)|The arrangement.





### Enumeration: NorthType
A list of north arrows types.

|Property | Value | Description |
|---------|--------|--------|
| SimpleNorth| 0| Simple north arrow.
| TrueNorth| 1| True north arrow.
| GridNorth| 2| Grid north arrow.
| MagneticNorth| 3| Magnetic north arrow.



### Enumeration: Orientation
A list of orientation values.

|Property | Value | Description |
|---------|--------|--------|
| Horizontal| 0| Horizontal.
| Vertical| 1| Vertical.




## CIMPage
Represents the page information associated with a layout.


### CIMPage

|Property | Type | Description |
|---------|--------|--------|
| height | number //double|The height of the layout in page units.
| stretchElements | boolean|A boolean indicating if elements should be stretched when the page size is changed.
| width | number //double|The width of the layout in page units.
| printerPreferences | [CIMPrinterPreferences](CIMLayout.md#cimprinterpreferences)|The printer preferences for the page.
| units | [LinearUnit](ExternalReferences.md#linearunit)|The page units for the layout.
| guides | [CIMGuide](CIMLayout.md#cimguide) |The guides on a layout.
| showRulers | boolean|A boolean indicating if rulers should be displayed on the layout.
| showGuides | boolean|A boolean indicating if guides should be displayed on the layout.
| smallestRulerDivision | number //double|The smallest ruler division.





### Enumeration: PageOrientation
A list of page orientation values.

|Property | Value | Description |
|---------|--------|--------|
| Portrait| 0| Portrait orientation.
| Landscape| 1| Landscape orientation.




## CIMPrinterPreferences
Represents the printer preferences associated with a layout.


### CIMPrinterPreferences

|Property | Type | Description |
|---------|--------|--------|
| printerName | string|The printer name.
| paperName | string|The paper size name.
| paperSource | number //int32|The paper source.





### Enumeration: RectanglePosition
A list of rectangle position values.

|Property | Value | Description |
|---------|--------|--------|
| TopSide| 0| Top side.
| BottomSide| 1| Bottom side.
| LeftSide| 2| Left side.
| RightSide| 3| Right side.




## CIMReport
Represents a report in a project.


### CIMDefinition

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| URI | string|The URI of the definition. Typically set by the system and used as an identifier.
| sourceURI | string|The source URI of the item. Set if sourced from an external item such as an item on a portal.
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|The time the definition was last modfied.
| metadataURI | string|The metadata URI.
| useSourceMetadata | boolean|A boolean indicating if the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project.


### CIMElementContainer

|Property | Type | Description |
|---------|--------|--------|
| elements | [CIMElement](Types.md#cimelement) |A collection of layout elements.


### CIMLayoutDefinition

|Property | Type | Description |
|---------|--------|--------|
| page | [CIMPage](CIMLayout.md#cimpage)|The CIMPage for the layout.
| dateExported | [TimeInstant](ExternalReferences.md#timeinstant)|The date exported property for a layout.
| datePrinted | [TimeInstant](ExternalReferences.md#timeinstant)|The date printed property for a layout.
| mapSeries | [MapSeries](Types.md#mapseries)|The map series for a layout.
| colorModel | [enumeration ColorModel](CIMEnumerations.md#enumeration-colormodel)|The color model for a layout.


### CIMReport

|Property | Type | Description |
|---------|--------|--------|
| height | number //double|The Height of the report.
| startPage | number //int32|The starting page for the report.
| watermarks | [CIMReportWatermark](CIMLayout.md#cimreportwatermark) |A collection of watermark for the report.






## CIMReportDataSource
Represents the data source properties of a report. The data source can be a map member or external data.


### CIMReportDataSource

|Property | Type | Description |
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|The data connection to the source.
| definitionQuery | string|The definition query.
| fields | [CIMReportField](CIMLayout.md#cimreportfield) |The fields used by the report.
| mapMemberURI | string|The uri to a Layer or Standalone table in the project.
| useSelectionSet | boolean|The value indicating that the selection of the Layer or Table should be used for the report.






## CIMReportDetails
Represents a details section of a report.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMElementContainer

|Property | Type | Description |
|---------|--------|--------|
| elements | [CIMElement](Types.md#cimelement) |A collection of layout elements.


### CIMGroupElement

|Property | Type | Description |
|---------|--------|--------|


### CIMReportSectionElement

|Property | Type | Description |
|---------|--------|--------|
| autoSize | boolean|The value indicating the section height will grow and shrink to fit the content of the section.
| elementFieldProperties | [CIMReportElementFieldProperties](CIMLayout.md#cimreportelementfieldproperties) |The field properties that will be applied to the elements.
| excludePageNumberPages | string|The comma delimited list of pages to exclude the page number from.
| excludeSectionPages | string|The comma delimited list of pages to exclude the section from.
| startOnNewPage | boolean|The value indicating the section should start on a new page.


### CIMReportDetails

|Property | Type | Description |
|---------|--------|--------|
| columns | number //int32|The number of columns for the details section.
| rowBackgroundColors | [CIMColor](Types.md#cimcolor) |The collection of background colors for each of the repeating rows.
| rowBackgroundCount | number //int32|The number of consecutive rows for each background color.






## CIMReportDocument
Represents a report document which is the document type used for saving .rlfx files.


### CIMVersion

|Property | Type | Description |
|---------|--------|--------|
| version | string|The document version. Set by the system.
| build | number //int32|The build an item was created with. Set by the system.


### CIMReportDocument

|Property | Type | Description |
|---------|--------|--------|
| binaryReferences | [CIMBinaryReference](CIMDocument.md#cimbinaryreference) |The binary references of the document.
| layerDefinitions | [CIMDefinition](Types.md#cimdefinition) |The layer definitions in the report document.
| mapDefinitions | [CIMDefinition](Types.md#cimdefinition) |The map definitions of the report document.
| reportDefinition | [CIMReport](CIMLayout.md#cimreport)|The report definition of the report document.
| tableDefinitions | [CIMDefinition](Types.md#cimdefinition) |The table definitions of the report document.






## CIMReportElementFieldProperties
Represents field properties that will be applied to an element in a report.


### CIMReportElementFieldProperties

|Property | Type | Description |
|---------|--------|--------|
| element | string|The name of the target element.
| field | string|The name of the source field.
| format | [NumberFormat](Types.md#numberformat)|The format for the source field value.
| statistic | [enumeration FieldStatisticsFlag](CIMLayout.md#enumeration-fieldstatisticsflag)|The statistic to apply to the source field.






## CIMReportField
Represents a field in a report.


### CIMTableField

|Property | Type | Description |
|---------|--------|--------|
| name | string|Field name - unique identifier
| isVisible | boolean|Show or hide field.
| width | number //double|Width of field. A value of 0 indicates "auto size".
| sortInfo | [enumeration FieldSortInfo](CIMLayout.md#enumeration-fieldsortinfo)|Options when this field is used for sorting.
| sortOrder | number //int32|Zero based sort order. -1 indicates field isn't used for sorting.
| fieldOrder | number //int32|Zero based display order.
| group | boolean|The property indicating this is a grouping field.


### CIMReportField

|Property | Type | Description |
|---------|--------|--------|






## CIMReportFooter
Represents a report footer in a report.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMElementContainer

|Property | Type | Description |
|---------|--------|--------|
| elements | [CIMElement](Types.md#cimelement) |A collection of layout elements.


### CIMGroupElement

|Property | Type | Description |
|---------|--------|--------|


### CIMReportSectionElement

|Property | Type | Description |
|---------|--------|--------|
| autoSize | boolean|The value indicating the section height will grow and shrink to fit the content of the section.
| elementFieldProperties | [CIMReportElementFieldProperties](CIMLayout.md#cimreportelementfieldproperties) |The field properties that will be applied to the elements.
| excludePageNumberPages | string|The comma delimited list of pages to exclude the page number from.
| excludeSectionPages | string|The comma delimited list of pages to exclude the section from.
| startOnNewPage | boolean|The value indicating the section should start on a new page.


### CIMReportFooter

|Property | Type | Description |
|---------|--------|--------|






## CIMReportHeader
Represents a report header section in a report.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMElementContainer

|Property | Type | Description |
|---------|--------|--------|
| elements | [CIMElement](Types.md#cimelement) |A collection of layout elements.


### CIMGroupElement

|Property | Type | Description |
|---------|--------|--------|


### CIMReportSectionElement

|Property | Type | Description |
|---------|--------|--------|
| autoSize | boolean|The value indicating the section height will grow and shrink to fit the content of the section.
| elementFieldProperties | [CIMReportElementFieldProperties](CIMLayout.md#cimreportelementfieldproperties) |The field properties that will be applied to the elements.
| excludePageNumberPages | string|The comma delimited list of pages to exclude the page number from.
| excludeSectionPages | string|The comma delimited list of pages to exclude the section from.
| startOnNewPage | boolean|The value indicating the section should start on a new page.


### CIMReportHeader

|Property | Type | Description |
|---------|--------|--------|






## CIMReportPageFooter
Represents a page footer in a report.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMElementContainer

|Property | Type | Description |
|---------|--------|--------|
| elements | [CIMElement](Types.md#cimelement) |A collection of layout elements.


### CIMGroupElement

|Property | Type | Description |
|---------|--------|--------|


### CIMReportSectionElement

|Property | Type | Description |
|---------|--------|--------|
| autoSize | boolean|The value indicating the section height will grow and shrink to fit the content of the section.
| elementFieldProperties | [CIMReportElementFieldProperties](CIMLayout.md#cimreportelementfieldproperties) |The field properties that will be applied to the elements.
| excludePageNumberPages | string|The comma delimited list of pages to exclude the page number from.
| excludeSectionPages | string|The comma delimited list of pages to exclude the section from.
| startOnNewPage | boolean|The value indicating the section should start on a new page.


### CIMReportPageFooter

|Property | Type | Description |
|---------|--------|--------|






## CIMReportPageHeader
Represents a page header section in a report.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMElementContainer

|Property | Type | Description |
|---------|--------|--------|
| elements | [CIMElement](Types.md#cimelement) |A collection of layout elements.


### CIMGroupElement

|Property | Type | Description |
|---------|--------|--------|


### CIMReportSectionElement

|Property | Type | Description |
|---------|--------|--------|
| autoSize | boolean|The value indicating the section height will grow and shrink to fit the content of the section.
| elementFieldProperties | [CIMReportElementFieldProperties](CIMLayout.md#cimreportelementfieldproperties) |The field properties that will be applied to the elements.
| excludePageNumberPages | string|The comma delimited list of pages to exclude the page number from.
| excludeSectionPages | string|The comma delimited list of pages to exclude the section from.
| startOnNewPage | boolean|The value indicating the section should start on a new page.


### CIMReportPageHeader

|Property | Type | Description |
|---------|--------|--------|






## CIMReportSection
The data source for a report.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMElementContainer

|Property | Type | Description |
|---------|--------|--------|
| elements | [CIMElement](Types.md#cimelement) |A collection of layout elements.


### CIMGroupElement

|Property | Type | Description |
|---------|--------|--------|


### CIMReportSectionElement

|Property | Type | Description |
|---------|--------|--------|
| autoSize | boolean|The value indicating the section height will grow and shrink to fit the content of the section.
| elementFieldProperties | [CIMReportElementFieldProperties](CIMLayout.md#cimreportelementfieldproperties) |The field properties that will be applied to the elements.
| excludePageNumberPages | string|The comma delimited list of pages to exclude the page number from.
| excludeSectionPages | string|The comma delimited list of pages to exclude the section from.
| startOnNewPage | boolean|The value indicating the section should start on a new page.


### CIMReportSection

|Property | Type | Description |
|---------|--------|--------|
| dataSource | [CIMReportDataSource](CIMLayout.md#cimreportdatasource)|The data source for a report.






## CIMReportSectionElement
Represents a section of elements in a report.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMElementContainer

|Property | Type | Description |
|---------|--------|--------|
| elements | [CIMElement](Types.md#cimelement) |A collection of layout elements.


### CIMGroupElement

|Property | Type | Description |
|---------|--------|--------|


### CIMReportSectionElement

|Property | Type | Description |
|---------|--------|--------|
| autoSize | boolean|The value indicating the section height will grow and shrink to fit the content of the section.
| elementFieldProperties | [CIMReportElementFieldProperties](CIMLayout.md#cimreportelementfieldproperties) |The field properties that will be applied to the elements.
| excludePageNumberPages | string|The comma delimited list of pages to exclude the page number from.
| excludeSectionPages | string|The comma delimited list of pages to exclude the section from.
| startOnNewPage | boolean|The value indicating the section should start on a new page.






## CIMReportWatermark
Represents a watermark in a report.


### CIMReportWatermark

|Property | Type | Description |
|---------|--------|--------|
| element | [Element](Types.md#element)|The element for the watermark.
| excludePageNumbers | string|The comma delimited list of excluded page numbers.
| isBackground | boolean|The value indicating that the overlay draws in the background of the report, else it draws on the foreground.





### Enumeration: ScaleBarFittingStrategy
A list of scale bar fitting strategies.

|Property | Value | Description |
|---------|--------|--------|
| AdjustDivision| 0| Adjust the division value.
| AdjustDivisions| 1| Adjust the number of divisions.
| AdjustDivisionAndDivisions| 2| Adjust the division value and number of divisions.
| AdjustFrame| 3| Adjust the size of the scale bar frame.



### Enumeration: ScaleBarFrequency
Lists the options for the frequency marks appear on the scale bar.

|Property | Value | Description |
|---------|--------|--------|
| None| 0| None.
| One| 1| One.
| MajorDivisions| 2| Major divisions.
| Divisions| 3| Divisions.
| DivisionsAndFirstMidpoint| 4| Divisions and first mid point.
| DivisionsAndFirstSubdivisions| 5| Divisions and first subdivisions.
| DivisionsAndSubdivisions| 6| Divisions and subdivisions.



### Enumeration: ScaleBarLabelPosition
Lists the options for scale bar label positions.

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



### Enumeration: ScaleBarVerticalPosition
A list of scale bar vertical positions.

|Property | Value | Description |
|---------|--------|--------|
| Above| 0| Above.
| Top| 1| Top.
| On| 2| On.
| Bottom| 3| Bottom.
| Below| 4| Below.




## CIMScaleLine
Represents a Scale line on a page layout.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMMapSurround

|Property | Type | Description |
|---------|--------|--------|
| mapFrame | string|The map frame associated with the map surround.


### CIMScaleBar

|Property | Type | Description |
|---------|--------|--------|
| alignToZeroPoint | boolean|A boolean indicating if scale bar should align to zero.
| barHeight | number //double|The scale bar height.
| division | number //double|The division value
| divisions | number //int32|The number of divisions.
| divisionsBeforeZero | number //int32|The number of divisions before zero.
| fittingStrategy | [enumeration ScaleBarFittingStrategy](CIMLayout.md#enumeration-scalebarfittingstrategy)|The fitting strategy.
| labelFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency)|The label frequency.
| labelGap | number //double|The label gap value.
| labelPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition)|The label position.
| labelSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The label symbol.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format.
| subdivisions | number //int32|The number of subdivisions.
| unitLabel | string|The unit label.
| unitLabelGap | number //double|The unit label gap. Units set in points.
| unitLabelPosition | [enumeration ScaleBarLabelPosition](CIMLayout.md#enumeration-scalebarlabelposition)|The unit label position
| unitLabelSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The unit label symbol.
| units | [Unit](ExternalReferences.md#unit)|The units for the scale bar.
| useFractionCharacters | boolean|A boolean indicating if fractional characters should be used.
| zeroPoint | [Point](ExternalReferences.md#point)|The zero location for the scale bar.
| computeAtCenter | boolean|The flag that computes scale at map center.


### CIMScaleMarks

|Property | Type | Description |
|---------|--------|--------|
| divisionMarkHeight | number //double|The division marker height value.
| divisionMarkSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The division marker symbol.
| markFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency)|The division marker frequency.
| markPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition)|The division marker position.
| subdivisionMarkHeight | number //double|The subdivision marker height.
| subdivisionMarkSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The subdivision marker symbol


### CIMScaleLine

|Property | Type | Description |
|---------|--------|--------|
| lineSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The scale line line symbol.
| stepped | boolean|A boolean indicating if the scale line should be stepped.






## CIMSimpleGridLabelTemplate
Represents a simple format for a label.


### CIMGridLabelTemplate

|Property | Type | Description |
|---------|--------|--------|


### CIMSimpleGridLabelTemplate

|Property | Type | Description |
|---------|--------|--------|
| dynamicStringTemplate | string|The dynamict text as a template for labels.
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the text of labels.






## CIMSingleFillScaleBar
Represents and single fill scale bar on a page layout.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMMapSurround

|Property | Type | Description |
|---------|--------|--------|
| mapFrame | string|The map frame associated with the map surround.


### CIMScaleBar

|Property | Type | Description |
|---------|--------|--------|
| alignToZeroPoint | boolean|A boolean indicating if scale bar should align to zero.
| barHeight | number //double|The scale bar height.
| division | number //double|The division value
| divisions | number //int32|The number of divisions.
| divisionsBeforeZero | number //int32|The number of divisions before zero.
| fittingStrategy | [enumeration ScaleBarFittingStrategy](CIMLayout.md#enumeration-scalebarfittingstrategy)|The fitting strategy.
| labelFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency)|The label frequency.
| labelGap | number //double|The label gap value.
| labelPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition)|The label position.
| labelSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The label symbol.
| numberFormat | [NumberFormat](Types.md#numberformat)|The number format.
| subdivisions | number //int32|The number of subdivisions.
| unitLabel | string|The unit label.
| unitLabelGap | number //double|The unit label gap. Units set in points.
| unitLabelPosition | [enumeration ScaleBarLabelPosition](CIMLayout.md#enumeration-scalebarlabelposition)|The unit label position
| unitLabelSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The unit label symbol.
| units | [Unit](ExternalReferences.md#unit)|The units for the scale bar.
| useFractionCharacters | boolean|A boolean indicating if fractional characters should be used.
| zeroPoint | [Point](ExternalReferences.md#point)|The zero location for the scale bar.
| computeAtCenter | boolean|The flag that computes scale at map center.


### CIMScaleMarks

|Property | Type | Description |
|---------|--------|--------|
| divisionMarkHeight | number //double|The division marker height value.
| divisionMarkSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The division marker symbol.
| markFrequency | [enumeration ScaleBarFrequency](CIMLayout.md#enumeration-scalebarfrequency)|The division marker frequency.
| markPosition | [enumeration ScaleBarVerticalPosition](CIMLayout.md#enumeration-scalebarverticalposition)|The division marker position.
| subdivisionMarkHeight | number //double|The subdivision marker height.
| subdivisionMarkSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The subdivision marker symbol


### CIMSingleFillScaleBar

|Property | Type | Description |
|---------|--------|--------|
| fillSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The fill symbol for the scale bar.






## CIMSpatialMapSeries
Spatial Map Series is a means to create a series of map pages based off of spatial features.


### CIMMapSeries

|Property | Type | Description |
|---------|--------|--------|
| enabled | boolean|A boolean indicating if the Map Series is enabled on the layout.
| mapFrameName | string|The URI of the MapFrame to which MapSeries is linked.
| startingPageNumber | number //int32|The starting page number
| currentPageID | number //int32|The current page Id.


### CIMSpatialMapSeries

|Property | Type | Description |
|---------|--------|--------|
| indexLayerURI | string|
| nameField | string|The name of the specified page.
| numberField | string|The number of the specified page.
| categoryField | string|The category of the page.
| rotationField | string|The page specific rotation.
| sortField | string|The required field that specifies the field used to determine sort order.
| scaleField | string|The field that specifies the page specific scale.
| spatialReferenceField | string|The spatial reference of the page.
| sortAscending | boolean|The field indicating whether to sort in ascending or descending order.
| scaleRounding | number //double|The specified value to which the scale rounds to.
| extentOptions | [enumeration ExtentFitType](CIMLayout.md#enumeration-extentfittype)|The extent fitting options.
| marginType | [enumeration UnitType](CIMLayout.md#enumeration-unittype)|The type of margins.
| marginUnits | [LinearUnit](ExternalReferences.md#linearunit)|The units of the margin.
| margin | number //double|The value of the margin.






## CIMTMElevationGuideBarElement
Represents TM Elevation Guide Bar surround element.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMMapSurround

|Property | Type | Description |
|---------|--------|--------|
| mapFrame | string|The map frame associated with the map surround.


### CIMTMElevationGuideBarElement

|Property | Type | Description |
|---------|--------|--------|
| updateDynamically | boolean|A boolean indicating whether properties are automatically updated dynamically with the associated data frame.
| elevationBandLayerURI | string|The elevation bands feature class, the number of bands in the bar is dependent on the number of bands identified in feature class.
| numberOfBands | number //int32|The number of bands displayed in the Elevation Guide Bar, if data is from source that does not have Bands field.
| textSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol used for text elements in the elevation guide bar.
| lineSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol used for line elements in the elevation guide bar.
| highestBandSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The highest band symbol in the elevation guide bar.
| highBandSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The high band symbol in the elevation guide bar.
| mediumBandSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The medium band symbol in the elevation guide bar.
| lowBandSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The low band symbol in the elevation guide bar.






## CIMTableFrame
Layout element used to display tabular data


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMMapSurround

|Property | Type | Description |
|---------|--------|--------|
| mapFrame | string|The map frame associated with the map surround.


### CIMTableFrame

|Property | Type | Description |
|---------|--------|--------|
| fields | [CIMTableFrameField](CIMLayout.md#cimtableframefield) |Fields displayed by the table frame.
| mapMemberURI | string|Layer or standalone table that defines the data to display.
| fillingStrategy | [enumeration TableFrameFillingStrategy](CIMLayout.md#enumeration-tableframefillingstrategy)|Strategy used to query records.
| fittingStrategy | [enumeration TableFrameFittingStrategy](CIMLayout.md#enumeration-tableframefittingstrategy)|Strategy used to query records.
| columns | number //int32|
| minFontSize | number //double|Limit when reducing font sizes. Values is in points.
| verticalTextGap | number //double|Margin around field values.
| horizontalTextGap | number //double|Margin around field values.
| headingGap | number //double|Gap between field names and rows.
| rowGap | number //double|Gap between rows.
| fieldGap | number //double|Gap between fields.
| columnGap | number //double|Gap between table columns.
| headingBackgroundSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Field name/alias background style.
| headingBorderSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Field name/alias border style.
| headingLineSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Field name/alias underline style.
| columnBorderSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Column border style.
| alternate1RowBackgroundSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Second alternating data record background style.
| alternate1RowBackgroundCount | number //int32|Show even row background for this many rows before alternating.
| alternate2RowBackgroundSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|First alternating data record background style.
| alternate2RowBackgroundCount | number //int32|Show odd row background for this many rows before alternating.
| rowBorderSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Border style for row sections: data records, summary statistics, and statistics totals.






## CIMTableFrameField
Display properties for fields in a table frame.


### CIMTableField

|Property | Type | Description |
|---------|--------|--------|
| name | string|Field name - unique identifier
| isVisible | boolean|Show or hide field.
| width | number //double|Width of field. A value of 0 indicates "auto size".
| sortInfo | [enumeration FieldSortInfo](CIMLayout.md#enumeration-fieldsortinfo)|Options when this field is used for sorting.
| sortOrder | number //int32|Zero based sort order. -1 indicates field isn't used for sorting.
| fieldOrder | number //int32|Zero based display order.
| group | boolean|The property indicating this is a grouping field.


### CIMTableFrameField

|Property | Type | Description |
|---------|--------|--------|
| enableWordWrapping | boolean|Wrap field values that don't fit the width.
| headingTextSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Field name/alias text style.
| textSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Field value text style.
| backgroundSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Field background style.
| borderSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Field border style.
| verticalLineSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Style of vertical lines on sides of field.





### Enumeration: TableFrameFillingStrategy
####

|Property | Value | Description |
|---------|--------|--------|
| ShowAllRows| 0| Show all the rows.
| ShowVisibleRows| 1| Show the rows that are visible.
| ShowMapSeriesRows| 2| Show the rows that intersect the current map series shape.



### Enumeration: TableFrameFittingStrategy
Defines which table rows to display

|Property | Value | Description |
|---------|--------|--------|
| AdjustSize| 0| Reduce fonts sizes to make data fit.
| AdjustColumns| 1| Flow to multiple columns to make data fit.
| AdjustColumnsAndSize| 2| Reduce font sizes and flow to multiple columns to make data fit.
| AdjustFrame| 3| Adjust the frame to fit the specified font sizes and columns.




## CIMTemporalMapSeries
Temporal map series is a means to create a series of map pages based on time settings.


### CIMMapSeries

|Property | Type | Description |
|---------|--------|--------|
| enabled | boolean|A boolean indicating if the Map Series is enabled on the layout.
| mapFrameName | string|The URI of the MapFrame to which MapSeries is linked.
| startingPageNumber | number //int32|The starting page number
| currentPageID | number //int32|The current page Id.


### CIMTemporalMapSeries

|Property | Type | Description |
|---------|--------|--------|
| timeExtent | [TimeExtent](ExternalReferences.md#timeextent)|The time extent.
| interval | number //double|The time interval.
| intervalUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits)|The time interval units.






## CIMTopoNorthArrow
Represents a topographic north arrow which displays declination of true, grid and magnetic north.


### CIMElement

|Property | Type | Description |
|---------|--------|--------|
| anchor | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The anchor position of the element.
| locked | boolean|The locked property of the element. Each element in the TOC has a lock symbol.If the symbol is locked, you can not select that feature in the layout using the select tool.
| name | string|The name of the element.
| visible | boolean|The visibility of the element.
| rotation | number //double|The rotation of the element.
| rotationCenter | [Point](ExternalReferences.md#point)|The location of the anchor in page units.This is also the location the feature is rotated around.
| lockedAspectRatio | boolean|The locked aspect ratio for an element.If locked, the width and height values stretch proportionally.


### CIMFrameElement

|Property | Type | Description |
|---------|--------|--------|
| frame | [Polygon](ExternalReferences.md#polygon)|The geometry of a frame for an element.
| graphicFrame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic symbology of an element's frame.


### CIMMapSurround

|Property | Type | Description |
|---------|--------|--------|
| mapFrame | string|The map frame associated with the map surround.


### CIMNorthArrow

|Property | Type | Description |
|---------|--------|--------|
| referenceLocation | [Point](ExternalReferences.md#point)|The reference location for a north arrow.
| calibrationAngle | number //double|The calibration angle for a north arrow.


### CIMTopoNorthArrow

|Property | Type | Description |
|---------|--------|--------|
| date | [TimeInstant](ExternalReferences.md#timeinstant)|The date used when calculating declination using world magnetic model.
| zone | [SpatialReference](ExternalReferences.md#spatialreference)|The spatial reference used for calculating declination, typically a UTM zone.
| isPrimaryZone | boolean|A boolean indicating whether the Zone is the primary zone. Set to false when using 2nd north arrow for maps that extend across two UTM zones.
| GMAngle | [CIMDeclination](CIMLayout.md#cimdeclination)|The Grid Magnetic declination
| gridConvergence | [CIMDeclination](CIMLayout.md#cimdeclination)|The Grid Convergence declination
| directionalNotes | boolean|A boolean indicating whether directional notes are displayed on north arrow
| leadingZero | boolean|A boolean indicating whether a leading zero is displayed for minute coordinates of grid convergence.
| roundGMAngle | boolean|How GM angle is displayed. If true GM angle is displayed to nearest 1/2 degree, if false it is displayed as degrees and minutes.
| roundMils | boolean|How Mils are displayed. If true Mils for both GC and GM will be displayed rounded to nearest 10 Mils, otherwise to nearest 1 Mil. If RoundGMAngle is true, this property is ignored.
| autoUpdate | boolean|A boolean indicating whether the properties of the topographic north arrow should update automatically based on changes in the map
| largeSize | boolean|A boolean indicating whether the topographic north arrow is displayed in large size.
| topographicType | [enumeration TopoNorthArrowType](CIMLayout.md#enumeration-toponortharrowtype)|The type of topographic north arrow to display.
| textSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol used for text elements in topographic north arrow
| lineSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol used for line elements in the topographic north arrow
| trueNorthMarkerSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol displayed at top of true north line, default is a star.
| magneticNorthNegativeSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol displayed at top of magnetic north line when the gm-angle is negative.
| magneticNorthPositiveSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol displayed at top of magnetic north line when the gm-angle is positive.
| magneticNorthZeroSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol displayed at top of magnetic north line when the gm-angle is 0 degrees.
| declinationArcSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The line symbol used to display declination arc lines.





### Enumeration: TopoNorthArrowType
Defines a type of topographic north arrow.

|Property | Value | Description |
|---------|--------|--------|
| Standard| 0| Standard topographic north arrow
| TLM| 1| North Arrow for Topographic Line Map
| ICM| 2| North Arrow for Image City Map



### Enumeration: UnitType
Lists the unit type values.

|Property | Value | Description |
|---------|--------|--------|
| Percent| 0| Percent.
| MapUnits| 1| Map Units.
| PageUnits| 2| Page units.




## CIMVerticalLegendItem
Represents a vertical legend item in a legend.


### CIMLegendItem

|Property | Type | Description |
|---------|--------|--------|
| name | string|The legend item name.
| newColumn | boolean|A boolean indicating if a legend item should be placed in a new column.
| layerNameSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item symbol.
| columns | number //int32|The number of columns for a legend item.
| keepTogether | boolean|A boolean indicating if the legend item should be kept together.
| showLayerName | boolean|A boolean indicating if the legend item layer name should be displayed.
| showHeading | boolean|A boolean indicating if the legend item heading should be displayed.
| headingSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item heading symbol.
| showLabels | boolean|A boolean indicating if legend item labels should be displayed.
| layer | string|The legend item layer's path.
| showDescription | boolean|A boolean indicating if a legend item description should be displayed.
| labelSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item label symbol.
| descriptionSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The legend item description symbol.
| patchWidth | number //double|The legend item patch width. Units in points.
| patchHeight | number //double|The legend item patch height. Units in points.
| autoVisibility | boolean|A boolean indicating if the legend item should be displayed if in the visible extent.
| useMapSeriesShape | boolean|A flag to use map series shape instead of map frame to find dynamic classes.
| classIndent | number //double|The distance from the class name to the edge of the legend.
| headingIndent | number //double|The distance from the heading to the edge of the legend.
| layerNameIndent | number //double|The distance of the layer name to the edge of the legend.
| showGroupLayerName | boolean|A flag to show the containing group layer name above the item.
| groupLayerNameSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol used to display the group layer name.
| scaleToPatch | boolean|The flag to scale the symbol to the specified patch size.
| showCounts | boolean|A boolean indicating if the legend should display count statistics.
| countFormat | [NumberFormat](Types.md#numberformat)|The feature count format.
| countPrefix | string|The feature count prefix.
| countSuffix | string|The feature count suffix.
| isVisible | boolean|The visibility of the legend item.


### CIMVerticalLegendItem

|Property | Type | Description |
|---------|--------|--------|
| arrangement | [enumeration LegendItemArrangement](CIMLayout.md#enumeration-legenditemarrangement)|The arrangement.
