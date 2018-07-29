


## CIMGraphicFrame
Represents a graphic frame.


### CIMGraphicFrame

|Property | Type | Description |
|---------|--------|--------|
| backgroundSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The background symbol of the graphic frame.
| borderSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The border symbol of the graphic frame.
| shadowSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The shadow symbol of the graphic frame.
| backgroundGapX | number //double|The background X gap.
| backgroundGapY | number //double|The background Y gap.
| backgroundCornerRounding | number //double|The background corner rounding. 0 = fully square. 100 = fully round.
| borderGapX | number //double|The border X gap.
| borderGapY | number //double|The border Y gap.
| borderCornerRounding | number //double|The border corner rounding. 0 = fully square. 100 = fully round.
| shadowOffsetX | number //double|The shadow X offset.
| shadowOffsetY | number //double|The shadow Y offset.
| shadowCornerRounding | number //double|The shadow corner rounding. 0 = fully square. 100 = fully round.






## CIMInkGraphic
Represents an ink graphic.


### CIMGraphic

|Property | Type | Description |
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the graphic.
| transparency | number //double|The transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes.
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|The blending mode of the graphic. Typically set by the layer or element during draw.
| masks | [Object]|An array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon.
| referenceScale | number //double|The reference scale of the graphic. Typically set by the layer or element during draw.
| attributes | Object|A property set of attributes. Typically set by the layer or element during draw.
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The placement anchor of the graphic.


### CIMInkGraphic

|Property | Type | Description |
|---------|--------|--------|
| bounds | [Envelope](ExternalReferences.md#envelope)|The bounds of the ink graphic.
| inkData | string|The ink data as a string.
| roughSketch | [Polyline](ExternalReferences.md#polyline)|A polyline used to define a rough sketch of the ink data.






## CIMLeaderLine
Represents a leader line.


### CIMLeader

|Property | Type | Description |
|---------|--------|--------|


### CIMLeaderLine

|Property | Type | Description |
|---------|--------|--------|
| line | [Polyline](ExternalReferences.md#polyline)|The leader line drawn from the graphic.






## CIMLeaderPoint
Represents a leader point.


### CIMLeader

|Property | Type | Description |
|---------|--------|--------|


### CIMLeaderPoint

|Property | Type | Description |
|---------|--------|--------|
| point | [Point](ExternalReferences.md#point)|The anchor point for the leader.






## CIMLineGraphic
Represents a line graphic.


### CIMGraphic

|Property | Type | Description |
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the graphic.
| transparency | number //double|The transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes.
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|The blending mode of the graphic. Typically set by the layer or element during draw.
| masks | [Object]|An array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon.
| referenceScale | number //double|The reference scale of the graphic. Typically set by the layer or element during draw.
| attributes | Object|A property set of attributes. Typically set by the layer or element during draw.
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The placement anchor of the graphic.


### CIMShapeGraphic

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| popupHtmlText | string|The popup HTML text.


### CIMLineGraphic

|Property | Type | Description |
|---------|--------|--------|
| line | [Polyline](ExternalReferences.md#polyline)|The polyline of the line graphic






## CIMMultiPatchGraphic
Represents a shape graphic with a MultiPatch geometry.


### CIMGraphic

|Property | Type | Description |
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the graphic.
| transparency | number //double|The transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes.
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|The blending mode of the graphic. Typically set by the layer or element during draw.
| masks | [Object]|An array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon.
| referenceScale | number //double|The reference scale of the graphic. Typically set by the layer or element during draw.
| attributes | Object|A property set of attributes. Typically set by the layer or element during draw.
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The placement anchor of the graphic.


### CIMShapeGraphic

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| popupHtmlText | string|The popup HTML text.


### CIMMultiPatchGraphic

|Property | Type | Description |
|---------|--------|--------|
| multiPatch | [MultiPatch](ExternalReferences.md#multipatch)|The graphic's MultiPatch geometry.






## CIMMultipointGraphic
Represents a shape graphic with a Multipoint geometry.


### CIMGraphic

|Property | Type | Description |
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the graphic.
| transparency | number //double|The transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes.
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|The blending mode of the graphic. Typically set by the layer or element during draw.
| masks | [Object]|An array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon.
| referenceScale | number //double|The reference scale of the graphic. Typically set by the layer or element during draw.
| attributes | Object|A property set of attributes. Typically set by the layer or element during draw.
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The placement anchor of the graphic.


### CIMShapeGraphic

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| popupHtmlText | string|The popup HTML text.


### CIMMultipointGraphic

|Property | Type | Description |
|---------|--------|--------|
| multipoint | [Multipoint](ExternalReferences.md#multipoint)|The graphic's Multipoint geometry.






## CIMParagraphTextGraphic
Represents a paragraph text graphic.


### CIMGraphic

|Property | Type | Description |
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the graphic.
| transparency | number //double|The transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes.
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|The blending mode of the graphic. Typically set by the layer or element during draw.
| masks | [Object]|An array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon.
| referenceScale | number //double|The reference scale of the graphic. Typically set by the layer or element during draw.
| attributes | Object|A property set of attributes. Typically set by the layer or element during draw.
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The placement anchor of the graphic.


### CIMTextGraphic

|Property | Type | Description |
|---------|--------|--------|
| text | string|The text string of the text graphic.
| shape | [Geometry](ExternalReferences.md#geometry)|The geometry of the text graphic.
| leaders | [CIMLeader](Types.md#cimleader) |A collection of leaders coming off of the graphic.


### CIMParagraphTextGraphic

|Property | Type | Description |
|---------|--------|--------|
| frame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic frame of the paragraph text graphic.
| columnCount | number //int32|The number of columns in the paragraphic text graphic.
| columnGap | number //double|The gap between columns.
| margin | number //double|The margin of the paragraph text graphic.






## CIMPictureGraphic
Represents a picture graphic.


### CIMGraphic

|Property | Type | Description |
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the graphic.
| transparency | number //double|The transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes.
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|The blending mode of the graphic. Typically set by the layer or element during draw.
| masks | [Object]|An array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon.
| referenceScale | number //double|The reference scale of the graphic. Typically set by the layer or element during draw.
| attributes | Object|A property set of attributes. Typically set by the layer or element during draw.
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The placement anchor of the graphic.


### CIMPictureGraphic

|Property | Type | Description |
|---------|--------|--------|
| pictureURL | string|The URL of the picture graphic. Typically a base64 encoded representation of the picture.
| box | [Envelope](ExternalReferences.md#envelope)|The bounding box of the picture graphic.
| frame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|The graphic frame of the picture graphic.
| sourceURL | string|The source URL of the picture graphic. Typically the source of the image copied into the PictureURL.






## CIMPointGraphic
Represents a point graphic.


### CIMGraphic

|Property | Type | Description |
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the graphic.
| transparency | number //double|The transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes.
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|The blending mode of the graphic. Typically set by the layer or element during draw.
| masks | [Object]|An array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon.
| referenceScale | number //double|The reference scale of the graphic. Typically set by the layer or element during draw.
| attributes | Object|A property set of attributes. Typically set by the layer or element during draw.
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The placement anchor of the graphic.


### CIMShapeGraphic

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| popupHtmlText | string|The popup HTML text.


### CIMPointGraphic

|Property | Type | Description |
|---------|--------|--------|
| location | [Point](ExternalReferences.md#point)|The location of the point graphic.
| leaders | [CIMLeader](Types.md#cimleader) |A collection of leaders coming off of the graphic.






## CIMPolygonGraphic
Represents a polygon graphic.


### CIMGraphic

|Property | Type | Description |
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the graphic.
| transparency | number //double|The transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes.
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|The blending mode of the graphic. Typically set by the layer or element during draw.
| masks | [Object]|An array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon.
| referenceScale | number //double|The reference scale of the graphic. Typically set by the layer or element during draw.
| attributes | Object|A property set of attributes. Typically set by the layer or element during draw.
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The placement anchor of the graphic.


### CIMShapeGraphic

|Property | Type | Description |
|---------|--------|--------|
| name | string|The name.
| popupHtmlText | string|The popup HTML text.


### CIMPolygonGraphic

|Property | Type | Description |
|---------|--------|--------|
| polygon | [Polygon](ExternalReferences.md#polygon)|The polygon of the polygon graphic.






## CIMTextGraphic
Represents a text graphic.


### CIMGraphic

|Property | Type | Description |
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|The symbol for the graphic.
| transparency | number //double|The transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes.
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|The blending mode of the graphic. Typically set by the layer or element during draw.
| masks | [Object]|An array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon.
| referenceScale | number //double|The reference scale of the graphic. Typically set by the layer or element during draw.
| attributes | Object|A property set of attributes. Typically set by the layer or element during draw.
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|The placement anchor of the graphic.


### CIMTextGraphic

|Property | Type | Description |
|---------|--------|--------|
| text | string|The text string of the text graphic.
| shape | [Geometry](ExternalReferences.md#geometry)|The geometry of the text graphic.
| leaders | [CIMLeader](Types.md#cimleader) |A collection of leaders coming off of the graphic.
