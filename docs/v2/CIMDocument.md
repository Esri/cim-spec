


## CIMBinaryReference
#### Represents a binary reference in a document. 


### CIMBinaryReference 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string | The URI or the binary reference. Typically set by the system but used as a reference path. 
| data | string | The base64 encoded data of the binary reference. 






## CIMDocumentInfo
#### Represents high level information for a document. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMDocumentInfo 

|Property | Type | Description | 
|---------|--------|--------|
| documentTitle | string | The title of the document. 
| subject | string | The subject of the document. 
| author | string | The author of the document. 
| category | string | The category of the document. 
| comments | string | The comments of the document. 
| keywords | string | The keywords of the document. 
| credits | string | The credits of the document. 
| hyperlinkBase | string | The hyperlink base path of the document. 
| savePreview | boolean | A value indicating whether to save a preview image. 
| activeMapRepositoryPath | string | The path of the active map. 
| useRelativePath | boolean | A value indicating whether to save with relative paths. Currently overridden by the application which always uses relative paths. 
| antialiasing | [enumeration esriBGLAntialiasingMode](ExternalReferences.md#enumeration-esribglantialiasingmode) | The anti-aliasing properties. Currently overridden by application settings. 
| textAntialiasing | [enumeration esriBGLTextAAlias](ExternalReferences.md#enumeration-esribgltextaalias) | The text anti-aliasing properties. Currently overridden by application settings. 






## CIMExternalTableView
#### Represents an external table view. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
| viewXML | string | The view properties as XML. 
| viewableObjectPath | string | The path of the item in the view. 
| viewType | string | The view type as a string. 
| instanceID | long | The instance identifier of this view. 


### CIMTableView 

|Property | Type | Description | 
|---------|--------|--------|
| fieldOrder | string | The field order as a string of field names. 
| sortInformation | {JSON_object}| A property set containing sort information. 
| selectionMode | boolean | A value indicating whether to view the table in selection mode. 
| honorTime | boolean | A value indicating whether to honor time on the table view. 
| frozenFields | long | The index of the frozen field. 
| zoomLevel | long | The zoom level of the table view. 
| fieldWidth | {JSON_object}| A property set of field width information. 
| displaySubtypeDomainDescriptions | boolean | A value indicating whether to display subtype and domain descriptions. 
| qualifyJoinFieldNames | boolean | A value indicating whether to qualify field names when the table contains fields from a join. 
| time | [TimeValue](ExternalReferences.md#timevalue) | The current time of the table view. 
| honorRange | boolean | A value indicating whether to honor ranges on the table view. 
| ranges | [CIMLayerRange](CIMVectorLayers.md#cimlayerrange) | The ranges of the table view. 
| extent | [Envelope](ExternalReferences.md#envelope) | The extent of the table view. 
| timeRelation | [enumeration esriTimeRelation](ExternalReferences.md#enumeration-esritimerelation) | A time relation which allows the start and end times to be included or excluded in the time query. 


### CIMExternalTableView 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection for the table view's table. 






## CIMGISProject
#### Represents a project. 


### CIMGISProject 

|Property | Type | Description | 
|---------|--------|--------|
| views | [CIMView](Types.md#view) | The views of the project. 
| moduleSettings | [CIMModuleSettings](CIMDocument.md#cimmodulesettings) | The module settings of the project. 
| projectItems | [CIMProjectItem](CIMDocument.md#cimprojectitem) | The items of the project. 
| databaseConnections | [CIMWorkspaceConnection](CIMVectorLayers.md#cimworkspaceconnection) | The database connections of the project. 
| serverConnections | [CIMServerConnection](Types.md#serverconnection) | The service connections of the project. 
| folderConnections | [CIMFolderConnection](CIMVectorLayers.md#cimfolderconnection) | The folder connections of the project. 
| viewLayoutXML | string | An XML representation of the view layout used for the project. 
| defaultGeoDatabase | string | The path of the default geodatabase of the project. 
| defaultToolbox | string | The path of the default toolbox of the project. 
| defaultSpatialReference | string | A WKT string representation of the default spatial reference of the project. 
| defaultFolder | string | The default folder of the project. 
| projectMetadata | string | The metadata of the project. 
| sourceURI | string | The source URI of the project. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the project was last modified. 
| readOnly | boolean | A value indicating whether the project is read only for updatable projects. 
| forceUpdate | boolean | A value indicating whether to force update an updatable project. 






## CIMGenericView
#### Represents a generic view. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
| viewXML | string | The view properties as XML. 
| viewableObjectPath | string | The path of the item in the view. 
| viewType | string | The view type as a string. 
| instanceID | long | The instance identifier of this view. 


### CIMGenericView 

|Property | Type | Description | 
|---------|--------|--------|
| viewProperties | {JSON_object}| A property set containing properties of the generic view in the project. 






## CIMLayerDocument
#### Represents a layer document which is the document type used for saving .lyrx files. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMLayerDocument 

|Property | Type | Description | 
|---------|--------|--------|
| layers | [string] | An array of layer URIs stored in this layer document. 
| layerDefinitions | [CIMDefinition](Types.md#definition) | The layer definitions in the layer document. 
| binaryReferences | [CIMBinaryReference](CIMDocument.md#cimbinaryreference) | The binary references of the document. 
| elevationSurfaces | [CIMMapElevationSurface](CIMMap.md#cimmapelevationsurface) | The elevation surfaces used by layer definitions in the layer document. 






## CIMLayoutDocument
#### Represents a layout document which is the document type used for saving .pagx files. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMLayoutDocument 

|Property | Type | Description | 
|---------|--------|--------|
| binaryReferences | [CIMBinaryReference](CIMDocument.md#cimbinaryreference) | The binary references of the document. 
| layerDefinitions | [CIMDefinition](Types.md#definition) | The layer definitions in the layout document. 
| mapDefinitions | [CIMDefinition](Types.md#definition) | The map definitions of the layout document. 
| tableDefinitions | [CIMDefinition](Types.md#definition) | The table definitions of the layout document. 
| layoutDefinition | [CIMLayout](CIMLayout.md#cimlayout) | The layout definition of the layout document. 






## CIMMapDocument
#### Represents a map document which is the document type used for saving .mapx files. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMMapDocument 

|Property | Type | Description | 
|---------|--------|--------|
| mapDefinition | [CIMMap](CIMMap.md#cimmap) | The map definition of the map document. 
| layerDefinitions | [CIMDefinition](Types.md#definition) | The layer definitions of the map document. 
| binaryReferences | [CIMBinaryReference](CIMDocument.md#cimbinaryreference) | The binary references of the document. 
| tableDefinitions | [CIMDefinition](Types.md#definition) | The table definitions of the map document. 






## CIMMapTableView
#### Represents a map table view in the project. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
| viewXML | string | The view properties as XML. 
| viewableObjectPath | string | The path of the item in the view. 
| viewType | string | The view type as a string. 
| instanceID | long | The instance identifier of this view. 


### CIMTableView 

|Property | Type | Description | 
|---------|--------|--------|
| fieldOrder | string | The field order as a string of field names. 
| sortInformation | {JSON_object}| A property set containing sort information. 
| selectionMode | boolean | A value indicating whether to view the table in selection mode. 
| honorTime | boolean | A value indicating whether to honor time on the table view. 
| frozenFields | long | The index of the frozen field. 
| zoomLevel | long | The zoom level of the table view. 
| fieldWidth | {JSON_object}| A property set of field width information. 
| displaySubtypeDomainDescriptions | boolean | A value indicating whether to display subtype and domain descriptions. 
| qualifyJoinFieldNames | boolean | A value indicating whether to qualify field names when the table contains fields from a join. 
| time | [TimeValue](ExternalReferences.md#timevalue) | The current time of the table view. 
| honorRange | boolean | A value indicating whether to honor ranges on the table view. 
| ranges | [CIMLayerRange](CIMVectorLayers.md#cimlayerrange) | The ranges of the table view. 
| extent | [Envelope](ExternalReferences.md#envelope) | The extent of the table view. 
| timeRelation | [enumeration esriTimeRelation](ExternalReferences.md#enumeration-esritimerelation) | A time relation which allows the start and end times to be included or excluded in the time query. 


### CIMMapTableView 

|Property | Type | Description | 
|---------|--------|--------|






## CIMMapView
#### Represents a map view in the project. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
| viewXML | string | The view properties as XML. 
| viewableObjectPath | string | The path of the item in the view. 
| viewType | string | The view type as a string. 
| instanceID | long | The instance identifier of this view. 


### CIMMapView 

|Property | Type | Description | 
|---------|--------|--------|
| viewingMode | [enumeration MapViewingMode](CIMEnumerations.md#enumeration-mapviewingmode) | The map viewing mode of the view. 
| camera | [CIMViewCamera](CIMMap.md#cimviewcamera) | The camera of the view. 
| verticalExaggerationScaleFactor | double | The vertical exaggeration of the view. 
| timeDisplay | [CIMMapTimeDisplay](CIMMap.md#cimmaptimedisplay) | The map time display of the view. 
| layerRanges | [CIMLayerRange](CIMVectorLayers.md#cimlayerrange) | The layer ranges of the view. 
| rangeSliderSettings | [CIMSliderSettings](CIMMap.md#cimslidersettings) | The range slider settings of the view. 
| timeSliderSettings | [CIMSliderSettings](CIMMap.md#cimslidersettings) | The time slider settings of the view. 
| sceneDrawingMode | [enumeration SceneDrawingMode](CIMDocument.md#enumeration-scenedrawingmode) | The scene's drawing mode. 
| fieldOfView | double | The scene's field-of-view in degrees (value must be between 35 and 70). Only used when the scene is in Perspective draw mode. 
| pauseDrawing | boolean | A value indicating whether drawing is in paused state for the view. 






## CIMModuleSettings
#### Represents module settings in the project. 


### CIMModuleSettings 

|Property | Type | Description | 
|---------|--------|--------|
| moduleName | string | The name of the module. 
| settingsXML | string | Module settings as XML. 






## CIMProjectItem
#### Represents an item in the project. 


### CIMProjectItem 

|Property | Type | Description | 
|---------|--------|--------|
| catalogPath | string | Catalog path of the project item. 
| pathHint | string | The path hint of the project item. 
| itemType | string | The item type of the project item. 
| name | string | The name of the project item. 
| propertiesXML | string | Properties of the item as XML. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | Modified time of the item as a time instant. 
| consolidatePath | boolean | A value indicating whether to consolidate the path of the project item. 
| consolidationResources | [string] | Consolidation resources string array of the project item. 
| pathSaveRelative | boolean | A value indicating whether the item is saved with relative paths. 
| metadataURI | string | The URI of the metadata. 





### Enumeration: SceneDrawingMode
#### Represents the drawing modes of a scene view. 

|Property | Value | Description | 
|---------|--------|--------|
| Perspective| 0| Draw scene using vanishing point technique. 
| Isometric| 1| Draw scene using parallel line technique. 

