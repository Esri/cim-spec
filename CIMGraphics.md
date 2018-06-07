


## CIMGraphicFrame
#### Represents a graphic frame. 


### CIMGraphicFrame 

|Property | Type | Description | 
|---------|--------|--------|
| backgroundSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the background symbol of the graphic frame. 
| borderSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the border symbol of the graphic frame. 
| shadowSymbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the shadow symbol of the graphic frame. 
| backgroundGapX | double|Gets and sets the background X gap. 
| backgroundGapY | double|Gets and sets the background Y gap. 
| backgroundCornerRounding | double|Gets and sets the background corner rounding. 0 = fully square. 100 = fully round. 
| borderGapX | double|Gets and sets the border X gap. 
| borderGapY | double|Gets and sets the border Y gap. 
| borderCornerRounding | double|Gets and sets the border corner rounding. 0 = fully square. 100 = fully round. 
| shadowOffsetX | double|Gets and sets the shadow X offset. 
| shadowOffsetY | double|Gets and sets the shadow Y offset. 
| shadowCornerRounding | double|Gets and sets the shadow corner rounding. 0 = fully square. 100 = fully round. 






## CIMInkGraphic
#### Represents an ink graphic. 


### CIMGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol for the graphic. 
| transparency | double|Gets and sets the transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|Gets and sets the blending mode of the graphic. Typically set by the layer or element during draw. 
| masks | [{JSON_object}]|Gets and sets an array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon. 
| referenceScale | double|Gets and sets the reference scale of the graphic. Typically set by the layer or element during draw. 
| attributes | {JSON_object}|Gets and sets a property set of attributes. Typically set by the layer or element during draw. 
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|Gets and sets the placement anchor of the graphic. 


### CIMInkGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| bounds | [Envelope](ExternalReferences.md#envelope)|Gets and sets the bounds of the ink graphic. 
| inkData | string|Gets and sets the ink data as a string. 
| roughSketch | [Polyline](ExternalReferences.md#polyline)|Gets and sets a polyline used to define a rough sketch of the ink data. 






## CIMLeaderLine
#### Represents a leader line. 


### CIMLeader 

|Property | Type | Description | 
|---------|--------|--------|


### CIMLeaderLine 

|Property | Type | Description | 
|---------|--------|--------|
| line | [Polyline](ExternalReferences.md#polyline)|Gets and sets the leader line drawn from the graphic. 






## CIMLeaderPoint
#### Represents a leader point. 


### CIMLeader 

|Property | Type | Description | 
|---------|--------|--------|


### CIMLeaderPoint 

|Property | Type | Description | 
|---------|--------|--------|
| point | [Point](ExternalReferences.md#point)|Gets and sets the anchor point for the leader. 






## CIMLineGraphic
#### Represents a line graphic. 


### CIMGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol for the graphic. 
| transparency | double|Gets and sets the transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|Gets and sets the blending mode of the graphic. Typically set by the layer or element during draw. 
| masks | [{JSON_object}]|Gets and sets an array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon. 
| referenceScale | double|Gets and sets the reference scale of the graphic. Typically set by the layer or element during draw. 
| attributes | {JSON_object}|Gets and sets a property set of attributes. Typically set by the layer or element during draw. 
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|Gets and sets the placement anchor of the graphic. 


### CIMShapeGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| popupHtmlText | string|Gets and sets the popup HTML text. 


### CIMLineGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| line | [Polyline](ExternalReferences.md#polyline)|Gets and sets the polyline of the line graphic 






## CIMMultiPatchGraphic
#### Represents a shape graphic with a MultiPatch geometry. 


### CIMGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol for the graphic. 
| transparency | double|Gets and sets the transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|Gets and sets the blending mode of the graphic. Typically set by the layer or element during draw. 
| masks | [{JSON_object}]|Gets and sets an array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon. 
| referenceScale | double|Gets and sets the reference scale of the graphic. Typically set by the layer or element during draw. 
| attributes | {JSON_object}|Gets and sets a property set of attributes. Typically set by the layer or element during draw. 
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|Gets and sets the placement anchor of the graphic. 


### CIMShapeGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| popupHtmlText | string|Gets and sets the popup HTML text. 


### CIMMultiPatchGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| multiPatch | [MultiPatch](ExternalReferences.md#multipatch)|Gets/sets the graphic's MultiPatch geometry. 






## CIMMultipointGraphic
#### Represents a shape graphic with a Multipoint geometry. 


### CIMGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol for the graphic. 
| transparency | double|Gets and sets the transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|Gets and sets the blending mode of the graphic. Typically set by the layer or element during draw. 
| masks | [{JSON_object}]|Gets and sets an array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon. 
| referenceScale | double|Gets and sets the reference scale of the graphic. Typically set by the layer or element during draw. 
| attributes | {JSON_object}|Gets and sets a property set of attributes. Typically set by the layer or element during draw. 
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|Gets and sets the placement anchor of the graphic. 


### CIMShapeGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| popupHtmlText | string|Gets and sets the popup HTML text. 


### CIMMultipointGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| multipoint | [Multipoint](ExternalReferences.md#multipoint)|Gets/sets the graphic's Multipoint geometry. 






## CIMParagraphTextGraphic
#### Represents a paragraph text graphic. 


### CIMGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol for the graphic. 
| transparency | double|Gets and sets the transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|Gets and sets the blending mode of the graphic. Typically set by the layer or element during draw. 
| masks | [{JSON_object}]|Gets and sets an array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon. 
| referenceScale | double|Gets and sets the reference scale of the graphic. Typically set by the layer or element during draw. 
| attributes | {JSON_object}|Gets and sets a property set of attributes. Typically set by the layer or element during draw. 
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|Gets and sets the placement anchor of the graphic. 


### CIMTextGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| text | string|Gets and sets the text string of the text graphic. 
| shape | [Geometry](ExternalReferences.md#geometry)|Gets and sets the geometry of the text graphic. 
| leaders | [CIMLeader](Types.md#cimleader) |Gets and sets a collection of leaders coming off of the graphic. 


### CIMParagraphTextGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| frame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|Gets and sets the graphic frame of the paragraph text graphic. 
| columnCount | long|Gets and sets number of columns in the paragraphic text graphic. 
| columnGap | double|Gets and sets the gap between columns. 
| margin | double|Gets and sets the margin of the paragraph text graphic. 






## CIMPictureGraphic
#### Represents a picture graphic. 


### CIMGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol for the graphic. 
| transparency | double|Gets and sets the transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|Gets and sets the blending mode of the graphic. Typically set by the layer or element during draw. 
| masks | [{JSON_object}]|Gets and sets an array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon. 
| referenceScale | double|Gets and sets the reference scale of the graphic. Typically set by the layer or element during draw. 
| attributes | {JSON_object}|Gets and sets a property set of attributes. Typically set by the layer or element during draw. 
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|Gets and sets the placement anchor of the graphic. 


### CIMPictureGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| pictureURL | string|Gets and sets the URL of the picture graphic. Typically a base64 encoded representation of the picture. 
| box | [Envelope](ExternalReferences.md#envelope)|Gets and sets the bounding box of the picture graphic. 
| frame | [CIMGraphicFrame](CIMGraphics.md#cimgraphicframe)|Gets and sets the graphic frame of the picture graphic. 
| sourceURL | string|Gets and sets the source URL of the picture graphic. Typically the source of the image copied into the PictureURL. 






## CIMPointGraphic
#### Represents a point graphic. 


### CIMGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol for the graphic. 
| transparency | double|Gets and sets the transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|Gets and sets the blending mode of the graphic. Typically set by the layer or element during draw. 
| masks | [{JSON_object}]|Gets and sets an array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon. 
| referenceScale | double|Gets and sets the reference scale of the graphic. Typically set by the layer or element during draw. 
| attributes | {JSON_object}|Gets and sets a property set of attributes. Typically set by the layer or element during draw. 
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|Gets and sets the placement anchor of the graphic. 


### CIMShapeGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| popupHtmlText | string|Gets and sets the popup HTML text. 


### CIMPointGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| location | [Point](ExternalReferences.md#point)|Gets and sets the location of the point graphic. 
| leaders | [CIMLeader](Types.md#cimleader) |Gets and sets a collection of leaders coming off of the graphic. 






## CIMPolygonGraphic
#### Represents a polygon graphic. 


### CIMGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol for the graphic. 
| transparency | double|Gets and sets the transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|Gets and sets the blending mode of the graphic. Typically set by the layer or element during draw. 
| masks | [{JSON_object}]|Gets and sets an array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon. 
| referenceScale | double|Gets and sets the reference scale of the graphic. Typically set by the layer or element during draw. 
| attributes | {JSON_object}|Gets and sets a property set of attributes. Typically set by the layer or element during draw. 
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|Gets and sets the placement anchor of the graphic. 


### CIMShapeGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| name | string|Gets and sets the name. 
| popupHtmlText | string|Gets and sets the popup HTML text. 


### CIMPolygonGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| polygon | [Polygon](ExternalReferences.md#polygon)|Gets and sets the polygon of the polygon graphic. 






## CIMTextGraphic
#### Represents a text graphic. 


### CIMGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| symbol | [CIMSymbolReference](CIMSymbolizers.md#cimsymbolreference)|Gets and sets the symbol for the graphic. 
| transparency | double|Gets and sets the transparency of the graphic. Typically set by the layer or element during draw. Change the transparency of layers in the symbol for persistent changes. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode)|Gets and sets the blending mode of the graphic. Typically set by the layer or element during draw. 
| masks | [{JSON_object}]|Gets and sets an array of masks for the graphic. Typically set by the layer or element during draw. The per-feature masks which defines an area where the CIMGraphic should NOT draw. Every element in the array should support be a Polygon. 
| referenceScale | double|Gets and sets the reference scale of the graphic. Typically set by the layer or element during draw. 
| attributes | {JSON_object}|Gets and sets a property set of attributes. Typically set by the layer or element during draw. 
| placement | [enumeration Anchor](CIMLayout.md#enumeration-anchor)|Gets and sets the placement anchor of the graphic. 


### CIMTextGraphic 

|Property | Type | Description | 
|---------|--------|--------|
| text | string|Gets and sets the text string of the text graphic. 
| shape | [Geometry](ExternalReferences.md#geometry)|Gets and sets the geometry of the text graphic. 
| leaders | [CIMLeader](Types.md#cimleader) |Gets and sets a collection of leaders coming off of the graphic. 



