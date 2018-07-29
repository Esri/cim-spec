# Symbols
Symbols graphically describe, categorize, or rank geographic features and labels to locate them and show qualitative and quantitative relationships. They display graphical elements on a layout. Symbols can be optionally stored, managed, and shared in collections called styles.

Examples of symbols can be found [here](Example-Symbols.md).
## Symbol layers
Symbols are classified by the type of geometry they depict: [CIMPointSymbol](CIMSymbols.md#CIMPointSymbol), [CIMLineSymbol](CIMSymbols.md#CIMLineSymbol), [CIMPolygonSymbol](CIMSymbols.md#CIMPolygonSymbol), [CIMMeshSymbol](CIMSymbols.md#cimmeshsymbol), and [CIMTextSymbol](CIMSymbols.md#CIMTextSymbol). Each symbol type has unique characteristics and properties. Symbols are built from component [CIMSymbolLayers](CIMSymbols.md#CIMSymbolLayer). These symbol layers are classified by their graphical structure—either [CIMMarker](CIMSymbols.md#CIMMarker), [CIMStroke](CIMSymbols.md#CIMStroke), or [CIMFill](CIMSymbols.md#CIMFill). These layers are the building blocks of symbols; they combine to make rich graphical depictions. [CIMTextSymbol](CIMSymbols.md#CIMTextSymbol) are an exception—they have native properties but no component layers.

[CIMFills](CIMSymbols.msd#CIMFill) symbol layers cover areal geometries with either a single solid color ([CIMSolidFill](CIMSymbols.md#CIMSolidFill)), a series of regularly spaced lines ([CIMHatchFill](CIMSymbols.md#CIMHatchFill)), a gradation from one color to another ([CIMGradientFill](CIMSymbols.md#CIMGradientFill)), an image or texture ([CIMPictureFill](CIMSymbols.md#CIMPictureFill)), or a reference to a procedural rule package ([CIMProceduralSymbolLayer](CIMSymbols.md#CIMProceduralSymbolLayer)).

[CIMStroke](CIMSymbols.md#CIMStroke) symbol layers can be of type [CIMSolidStroke](CIMSymbols.md#CIMSolidStroke), [CIMPictureStroke](CIMSymbols.md#CIMPictureStroke), or [CIMGradientStroke](CIMSymbols.md#CIMGradientStroke).

[CIMMarker](CIMSymbols.md#CIMMarker) symbol layer types include [CIMPictureMarker](CIMSymbols.md#CIMPictureMarker), [CIMObjectMarker3D](CIMSymbols.md#CIMObjectMarker3D) (which are true three-dimensional objects), [CIMCharacterMarker](CIMSymbols.md#CIMCharacterMarker) (which references a font glyph for its shape), [CIMVectorMarker](CIMSymbols.md#CIMVectorMarker), which are vector-based, and [CIMProceduralSymbolLayer](CIMSymbols.md#CIMProceduralSymbolLayer) (referencing a rule package).

Symbols have at least one symbol layer, but can have more, as outlined below:

[CIMPointSymbol](CIMSymbols.md#CIMPointSymbol)
* [CIMMarker](CIMSymbols.md#CIMMarker) layers: Draw relative to the point geometry

[CIMLineSymbol](CIMSymbols.md#CIMLineSymbol)
* [CIMMarker](CIMSymbols.md#CIMMarker) layers: Draw at specified locations relative to the line geometry
* [CIMStroke](CIMSymbols.md#CIMStroke) layers: Draw relative to the line geometry

[CIMPolygonSymbol](CIMSymbols.md#CIMPolygonSymbol)
* [CIMMarker](CIMSymbols.md#CIMMarker) layers: Draw relative to the polygon outline or within the polygon interior, dependent on the marker placement setting
* [CIMStroke](CIMSymbols.md#CIMStroke) layers: Draw relative to the polygon outline
* [CIMFill](CIMSymbols.md#CIMFill) layers: Draw relative to the polygon interior

[CIMMeshSymbol](MeshSymbol.md#cimmeshsymbol)
* [CIMFill](CIMSymbols.md#CIMFill) layers: Draw relative to the mesh interior and is limited to [CIMMaterialSymbolLayer](CIMSymbols.md#CIMMaterialSymbolLayer).

[CIMTextSymbol](CIMSymbols.md#CIMTextSymbol)
* Text symbols do not contain layers but use [CIMPolygonSymbol](CIMSymbols.md#CIMPolygonSymbol) and can use additional decorator objects like [CIMCallouts](CIMSymbols.md#CIMCallout)

## Symbol effects
In addition to these arrangements, you can add any symbol layer to any symbol when using a [GeometricEffect](CIMSymbols.md#GeometricEffect). Geometric effects dynamically alter symbol geometry to create different appearances. For instance, a (CIMSymbols.md#GeometricEffectBuffer) can be added to a [CIMLineSymbol](CIMSymbols.md#CIMLineSymbol) so that the symbol can be drawn with a [CIMFill](CIMSymbols.md#CIMFill).

## Marker placements
[CIMMarker](CIMSymbols.md#CIMMarker) layers are most commonly used in [CIMPointSymbols](CIMSymbols.md#CIMPointSymbol), usually placed directly on the point feature geometry. You can adjust the anchor points and offsets of a marker to customize their relative position. [CIMMarker](CIMSymbols.md#CIMMarker) layers are also used in [CIMLineSymbols](CIMSymbols.md#CIMLineSymbol) and [CIMPolygonSymbols](CIMSymbols.md#CIMPolygonSymbol), drawn along lines and outlines, at endpoints, or within polygon interiors. This is achieved by selecting a [CIMMarkerPlacement](CIMSymbols.md#CIMMarkerPlacement) that places the symbols where desired.

## Mobile symbols
For increased compatibility with mobile devices, a mobile profile of CIMSymbols is used.  Mobile versions of symbols differ is a few minor ways:
* All colors are written as arrays instead of Objects with assumed RGBA values. For example: `[0,0,0,255]` for a black color.
* All [Geometries](ExternalReferences.md#Geometry) are written with straight segments. No curved segments are allowed.
* No [CIMCharacterMarker](CIMSymbols.md#CIMCharacterMarker) symbol layers are allowed since the fonts are not easily transferable.
