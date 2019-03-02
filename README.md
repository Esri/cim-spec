# Cartographic Information Model

This repository hosts the specification for the Cartographic Information Model (CIM) which is a map content specification used to persist and transfer cartographic descriptions of GIS datasets. Represented in JSON, the specification is used for maps, scenes, layouts, layers, symbols, and styles in ArcGIS applications and APIs.

Usage of the CIM primarily begins with an entry point through a primary object. These objects are:
- Layer files: [CIMLayerDocument](docs/v2/CIMDocument.md#cimlayerdocument): A JSON document containing one of more layers representing data such as features from a feature class or raster.
- Map files: [CIMMapDocument](docs/v2/CIMDocument.md#cimmapdocument): A JSON document containing a collection of layers and display properties for 2D maps or 3D scenes. Maps and scenes in the CIM are represented by the [CIMMap](docs/v2/CIMMap.md#CIMMap) object. There are not separate object types and maps and scenes are instead differentiated by the `mapType` property. Types of scenes, global and local, are differentiated by the `defaultViewingMode` property.
- Layout files: [CIMLayoutDocument](docs/v2/CIMDocument.md#cimlayoutdocument) : A JSON document with a representation of a page ([CIMLayout](docs/v2/CIMLayout.md#cimlayout)), its elements, and the maps and scenes on it for print of document export.
- Report files: [CIMReportDocument](docs/v2/CIMLayout.md#cimreportdocument): A JSON document representing a report ([CIMReport](docs/v2/CIMLayout.md#cimreport)), its elements, and the report specific
- Styles : A database with style items defining graphic objects like [colors](docs/v2/Types.md#color), [colors schemes](docs/v2/Types.md#colorramp), and [symbols](docs/v2/Types.md#symbol) used to draw a feature or layout graphic. These items are used in the definitions of layers, maps, scenes, and layouts but may also be stored on their own as items in styles where the JSON is written to a database field. See also [An overview of symbols in the CIM](docs/v2/Overview-Symbols.md).

## How this specification is formatted
This CIM specification is documented via Markdown documents that contain definitions for objects and their properties. JSON lacks an inheritance mechanism and CIM implementations often deal with many abstract types using inheritance. The formatting of the Markdown reflects these realities in the following ways:
1. Objects that can be thought of inheriting from a type list properties in a section for each inherited type. In some cases, the final type may inherit all properties from another type and have no unique properties for itself. See  [CIMRGBColor](CIMColor.md#CIMRGBColor) for an example.
2. The [Types](docs/v2/Types.md) document lists objects by their type for quick reference.

## Versioning

The Cartographic Information Model uses [Semantic Versioning](https://semver.org/) and this documentation corresponds to version 2.3.0.

## Licensing

See [License](License.md)

## Contributing

You are invited to fork this repository to a public or private repository and to send Pull Requests suggest improvements or notify us of errors or omissions in this documentation. Creating a fork solely for this purpose does not constitute the creation and distribution of a derivative work. Please see our [guidelines for  contributing](https://github.com/esri/contributing).
