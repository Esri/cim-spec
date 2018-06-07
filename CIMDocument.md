


## CIMBinaryReference
#### Represents a binary reference in a document. 


### CIMBinaryReference 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string|Gets and sets theURI of the binary reference. Typically set by the system but used as a reference path. 
| data | string|Gets and sets the base64 encoded data of the binary reference. 






## CIMDocumentInfo
#### Represents high level information for a document. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string|Gets and sets document version. Set by the system. 
| build | long|Gets and sets the build an item was created with. Set by the system. 


### CIMDocumentInfo 

|Property | Type | Description | 
|---------|--------|--------|
| documentTitle | string|Gets and sets the title of the document. 
| subject | string|Gets and sets the subject of the document. 
| author | string|Gets and sets the author of the document. 
| category | string|Gets and sets the category of the document. 
| comments | string|Gets and sets the comments of the document. 
| keywords | string|Gets and sets the keywords of the document. 
| credits | string|Gets and sets the credits of the document. 
| hyperlinkBase | string|Gets and sets the hyperlink base path of the document. 
| savePreview | boolean|Gets and sets a boolean indicating whether to save a preview image. 
| activeMapRepositoryPath | string|Gets and sets the path of the active map. 
| useRelativePath | boolean|Gets and sets a boolean indicating whether to save with relative paths. Currently overriden by the application which always uses relative paths. 
| antialiasing | [enumeration esriBGLAntialiasingMode](ExternalReferences.md#enumeration-esribglantialiasingmode)|Gets and sets the anti-aliasing properties. Currently overriden by application settings. 
| textAntialiasing | [enumeration esriBGLTextAAlias](ExternalReferences.md#enumeration-esribgltextaalias)|Gets and sets the text anti-aliasing properties. Currently overriden by application settings. 






## CIMExternalTableView
#### Represents an external table view. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
| viewXML | string|Gets and sets the view properties as XML. 
| viewableObjectPath | string|Gets and sets the path of the item in the view. 
| viewType | string|Gets and sets the view type as a string. 
| instanceID | long|Gets and sets the instance identifier of this view. 


### CIMTableView 

|Property | Type | Description | 
|---------|--------|--------|
| fieldOrder | string|Gets and sets the field order as a string of field names. 
| sortInformation | {JSON_object}|Gets and sets a property set containing sort information. 
| selectionMode | boolean|Gets and sets a boolean indicating whether to view the table in selection mode. 
| honorTime | boolean|Gets and sets a boolean indicating whether to honor time on the table view. 
| frozenFields | long|Gets and sets the index of the frozen field. 
| zoomLevel | long|Gets and sets the zoom level of the table view. 
| fieldWidth | {JSON_object}|Gets and sets a property set of field width information. 
| displaySubtypeDomainDescriptions | boolean|Gets and sets a boolean indicating whether to display subtype and domain descriptions. 
| qualifyJoinFieldNames | boolean|Gets and sets a boolean indicating whether to qualify field names when the table contains fields from a join. 
| time | [TimeValue](ExternalReferences.md#timevalue)|Gets and sets the current time of the table view. 
| honorRange | boolean|Gets and sets a boolean indicating whether to honor ranges on the table view. 
| ranges | [CIMLayerRange](CIMVectorLayers.md#cimlayerrange) |Gets and sets the ranges of the table view. 
| extent | [Envelope](ExternalReferences.md#envelope)|Gets and sets the extent of the table view. 
| timeRelation | [enumeration esriTimeRelation](ExternalReferences.md#enumeration-esritimerelation)|Allows the start and end times to be included or excluded in the time query. 


### CIMExternalTableView 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection)|Gets and sets the data connection for the table view's table. 






## CIMGISProject
#### Represents a project. 


### CIMGISProject 

|Property | Type | Description | 
|---------|--------|--------|
| views | [CIMView](Types.md#cimview) |Gets and sets the views of the project. 
| moduleSettings | [CIMModuleSettings](CIMDocument.md#cimmodulesettings) |Gets and sets the module settings of the project. 
| projectItems | [CIMProjectItem](CIMDocument.md#cimprojectitem) |Gets and sets the items of the project. 
| databaseConnections | [CIMWorkspaceConnection](CIMVectorLayers.md#cimworkspaceconnection) |Gets and sets the database connections of the project. 
| serverConnections | [CIMServerConnection](Types.md#cimserverconnection) |Gets and sets the service connections of the project. 
| folderConnections | [CIMFolderConnection](CIMVectorLayers.md#cimfolderconnection) |Gets and sets the folder connections of the project. 
| viewLayoutXML | string|Gets and sets an XML representation of the view layout used for the project. 
| defaultGeoDatabase | string|Gets and sets the path of the default geodatabase of the project. 
| defaultToolbox | string|Gets and sets the path of the default toolbox of the project. 
| defaultSpatialReference | string|Gets and sets a WKT string representation of the default spatial reference of the project. 
| defaultFolder | string|Gets and sets the default folder of the project. 
| projectMetadata | string|Gets and sets the metadata of the project. 
| sourceURI | string|Gets and sets the source URI of the project. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|Gets and sets the time the project was last modfied. 
| readOnly | boolean|Gets and sets the ReadOnly property for updatable projects. 
| forceUpdate | boolean|Gets and sets the ForceUpdate property for updatable projects. 






## CIMGenericView
#### Represents a generic view. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
| viewXML | string|Gets and sets the view properties as XML. 
| viewableObjectPath | string|Gets and sets the path of the item in the view. 
| viewType | string|Gets and sets the view type as a string. 
| instanceID | long|Gets and sets the instance identifier of this view. 


### CIMGenericView 

|Property | Type | Description | 
|---------|--------|--------|
| viewProperties | {JSON_object}|Gets and sets a property set containing properties of the generic view in the project. 






## CIMLayerDocument
#### Represents a layer document which is the document type used for saving .lyrx files. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string|Gets and sets document version. Set by the system. 
| build | long|Gets and sets the build an item was created with. Set by the system. 


### CIMLayerDocument 

|Property | Type | Description | 
|---------|--------|--------|
| layers | IStringArray|Gets and sets an array of layer URIs stored in this layer document. 
| layerDefinitions | [CIMDefinition](Types.md#cimdefinition) |Gets and sets the layer definitions in the layer document. 
| binaryReferences | [CIMBinaryReference](CIMDocument.md#cimbinaryreference) |Gets and sets the binary references of the document. 
| elevationSurfaces | [CIMMapElevationSurface](CIMMap.md#cimmapelevationsurface) |Gets and sets the elevation surfaces used by layer definitions in the layer document. 
| validationRules | [CIMValidationRule](Types.md#cimvalidationrule) |Gets and sets the validation rules used by layer definitions in the layer document. 






## CIMLayoutDocument
#### Represents a layout document which is the document type used for saving .pagx files. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string|Gets and sets document version. Set by the system. 
| build | long|Gets and sets the build an item was created with. Set by the system. 


### CIMLayoutDocument 

|Property | Type | Description | 
|---------|--------|--------|
| binaryReferences | [CIMBinaryReference](CIMDocument.md#cimbinaryreference) |Gets and sets the binary references of the document. 
| layerDefinitions | [CIMDefinition](Types.md#cimdefinition) |Gets and sets the layer definitions in the layout document. 
| mapDefinitions | [CIMDefinition](Types.md#cimdefinition) |Gets and sets the map definitions of the layout document. 
| tableDefinitions | [CIMDefinition](Types.md#cimdefinition) |Gets and sets the table definitions of the layout document. 
| layoutDefinition | [CIMLayout](CIMLayout.md#cimlayout)|Gets and sets the layout definition of the layout document. 






## CIMMapDocument
#### Represents a map document which is the document type used for saving .mapx files. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string|Gets and sets document version. Set by the system. 
| build | long|Gets and sets the build an item was created with. Set by the system. 


### CIMMapDocument 

|Property | Type | Description | 
|---------|--------|--------|
| mapDefinition | [CIMMap](CIMMap.md#cimmap)|Gets and sets the map definition of the map document. 
| layerDefinitions | [CIMDefinition](Types.md#cimdefinition) |Gets and sets the layer definitions of the map document. 
| binaryReferences | [CIMBinaryReference](CIMDocument.md#cimbinaryreference) |Gets and sets the binary references of the document. 
| tableDefinitions | [CIMDefinition](Types.md#cimdefinition) |Gets and sets the table definitions of the map document. 






## CIMMapTableView
#### Represents a map table view in the project. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
| viewXML | string|Gets and sets the view properties as XML. 
| viewableObjectPath | string|Gets and sets the path of the item in the view. 
| viewType | string|Gets and sets the view type as a string. 
| instanceID | long|Gets and sets the instance identifier of this view. 


### CIMTableView 

|Property | Type | Description | 
|---------|--------|--------|
| fieldOrder | string|Gets and sets the field order as a string of field names. 
| sortInformation | {JSON_object}|Gets and sets a property set containing sort information. 
| selectionMode | boolean|Gets and sets a boolean indicating whether to view the table in selection mode. 
| honorTime | boolean|Gets and sets a boolean indicating whether to honor time on the table view. 
| frozenFields | long|Gets and sets the index of the frozen field. 
| zoomLevel | long|Gets and sets the zoom level of the table view. 
| fieldWidth | {JSON_object}|Gets and sets a property set of field width information. 
| displaySubtypeDomainDescriptions | boolean|Gets and sets a boolean indicating whether to display subtype and domain descriptions. 
| qualifyJoinFieldNames | boolean|Gets and sets a boolean indicating whether to qualify field names when the table contains fields from a join. 
| time | [TimeValue](ExternalReferences.md#timevalue)|Gets and sets the current time of the table view. 
| honorRange | boolean|Gets and sets a boolean indicating whether to honor ranges on the table view. 
| ranges | [CIMLayerRange](CIMVectorLayers.md#cimlayerrange) |Gets and sets the ranges of the table view. 
| extent | [Envelope](ExternalReferences.md#envelope)|Gets and sets the extent of the table view. 
| timeRelation | [enumeration esriTimeRelation](ExternalReferences.md#enumeration-esritimerelation)|Allows the start and end times to be included or excluded in the time query. 


### CIMMapTableView 

|Property | Type | Description | 
|---------|--------|--------|






## CIMMapView
#### Represents a map view in the project. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
| viewXML | string|Gets and sets the view properties as XML. 
| viewableObjectPath | string|Gets and sets the path of the item in the view. 
| viewType | string|Gets and sets the view type as a string. 
| instanceID | long|Gets and sets the instance identifier of this view. 


### CIMMapView 

|Property | Type | Description | 
|---------|--------|--------|
| viewingMode | [enumeration MapViewingMode](CIMEnumerations.md#enumeration-mapviewingmode)|Gets and sets the map viewing mode of the view. 
| camera | [CIMViewCamera](CIMMap.md#cimviewcamera)|Gets and sets the camera of the view. 
| verticalExaggerationScaleFactor | double|Gets and sets the veritcal exaggeration of the view. 
| timeDisplay | [CIMMapTimeDisplay](CIMMap.md#cimmaptimedisplay)|Gets and sets the map time display of the view. 
| layerRanges | [CIMLayerRange](CIMVectorLayers.md#cimlayerrange) |Gets and sets the layer ranges of the view. 
| rangeSliderSettings | [CIMSliderSettings](CIMMap.md#cimslidersettings)|Gets and sets the range slider settings of the view. 
| timeSliderSettings | [CIMSliderSettings](CIMMap.md#cimslidersettings)|Gets and sets the time slider settings of the view. 
| sceneDrawingMode | [enumeration SceneDrawingMode](CIMDocument.md#enumeration-scenedrawingmode)|Gets and sets the scene's drawing mode. 
| fieldOfView | double|Gets and sets the scene's field-of-view in degrees (value must be between 35 and 70). Only used when the scene is in Perspective draw mode. 






## CIMModuleSettings
#### Represents module settings in the project. 


### CIMModuleSettings 

|Property | Type | Description | 
|---------|--------|--------|
| moduleName | string|Gets and sets the name of the module. 
| settingsXML | string|Gets and sets module settings as XML. 






## CIMProjectItem
#### Represents an item in the project. 


### CIMProjectItem 

|Property | Type | Description | 
|---------|--------|--------|
| catalogPath | string|Gets and sets the catalog path of the project item. 
| pathHint | string|Gets and sets the path hint of the project item. 
| itemType | string|Gets and sets the item type of the project item. 
| name | string|Gets and sets the name of the project item. 
| propertiesXML | string|Gets and sets properties of the item as XML. 
| sourceURI | string|Gets and sets the source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant)|Gets and sets modified time of the item as a time instant. 
| consolidatePath | bool|Gets and sets consolidate path of the project item. 
| consolidationResources | IStringArray|Gets and sets consolidation resources string array of the project item. 
| pathSaveRelative | bool|Gets and sets a boolean indicating whether the item is saved with relative paths. 
| metadataURI | string|Gets or sets the URI of the metadata. 





### Enumeration: SceneDrawingMode
#### Represents the drawing modes of a scene view. 

|Property | Value | Description | 
|---------|--------|--------|
| Perspective| 0| Draw scene using vanishing point technique. 
| Isometric| 1| Draw scene using parallel line technique. 

