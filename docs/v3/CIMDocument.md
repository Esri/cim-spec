


## CIMBinaryReference
#### Represents a binary reference in a document. 


### CIMBinaryReference 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string | The URI of the binary reference. Typically set by the system but used as a reference path. 
| data | string | The base64 encoded data of the binary reference. 
| object | [CIMObject](ExternalReferences.md#cimobject) | The stored CIM object. This property is meant to be used as an alternative to the Data property. 






## CIMBookmarkDocument
#### Represents a bookmark document which is the document type used for saving .bkmx files. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMBookmarkDocument 

|Property | Type | Description | 
|---------|--------|--------|
| spatialReference | [SpatialReference](ExternalReferences.md#spatialreference) | The spatial reference. 
| bookmarks | [[CIMBookmark]](CIMMap.md#cimbookmark) | The bookmarks. 






## CIMColorReplacementDocument
#### Represents list of color replacement rules. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMColorReplacementDocument 

|Property | Type | Description | 
|---------|--------|--------|
| replacementRules | [[CIMColorReplacementRule]](CIMDocument.md#cimcolorreplacementrule) | The list of color replacement rules. 






## CIMColorReplacementRule
#### Represents a color replacement rule. 


### CIMColorReplacementRule 

|Property | Type | Description | 
|---------|--------|--------|
| inputColor | [Color](Types.md#color) | The color that needs to be replaced. 
| outputColor | [Color](Types.md#color) | The color that will replace the input color. 






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
| useRelativePath | boolean | A value indicating whether to save with relative paths. In typical Pro usage (e.g. saving projects or .lyrx files) this is set to true. 
| antialiasing | [enumeration esriBGLAntialiasingMode](ExternalReferences.md#enumeration-esribglantialiasingmode) | The anti-aliasing properties. Currently overridden by application settings. 
| textAntialiasing | [enumeration esriBGLTextAAlias](ExternalReferences.md#enumeration-esribgltextaalias) | The text anti-aliasing properties. Currently overridden by application settings. 






## CIMExternalTableView
#### Represents an external table view. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
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
| frozenFields | long | The count of frozen fields. 
| zoomLevel | long | The zoom level of the table view. 
| fieldWidth | {JSON_object}| A property set of field width information. 
| displaySubtypeDomainDescriptions | boolean | A value indicating whether to display subtype and domain descriptions. 
| qualifyJoinFieldNames | boolean | A value indicating whether to qualify field names when the table contains fields from a join. 
| time | [TimeValue](ExternalReferences.md#timevalue) | The current time of the table view. 
| honorRange | boolean | A value indicating whether to honor ranges on the table view. 
| ranges | [[CIMLayerRange]](CIMVectorLayers.md#cimlayerrange) | The ranges of the table view. 
| extent | [Envelope](ExternalReferences.md#envelope) | The extent of the table view. 
| timeRelation | [enumeration esriTimeRelation](ExternalReferences.md#enumeration-esritimerelation) | A time relation which allows the start and end times to be included or excluded in the time query. 
| showOnlyContingentValueFields | boolean | A value indicating whether the table field visibility settings should be overridden to only show fields that are part of one or more contingent value field groups. 
| highlightInvalidContingentValueFields | boolean | A value indicating whether invalid contingent value fields should be highlighted in the table. 
| autoPopulateContingentValueFields | boolean | A value indicating whether other contingent value fields should be automatically populated after a value is changed when only one match is valid. 
| columnHeaderRowHeight | [enumeration TableRowHeightType](CIMDocument.md#enumeration-tablerowheighttype) | A value indicating the height for the column header row in the table. 
| rowHeight | [enumeration TableRowHeightType](CIMDocument.md#enumeration-tablerowheighttype) | A value indicating the height for the rows in the table. 


### CIMExternalTableView 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection for the table view's table. 






## CIMGISProject
#### Represents a project. 


### CIMGISProject 

|Property | Type | Description | 
|---------|--------|--------|
| views | [[CIMView]](Types.md#view) | The views of the project. 
| moduleSettings | [[CIMModuleSettings]](CIMDocument.md#cimmodulesettings) | The module settings of the project. 
| projectItems | [[CIMProjectItem]](CIMDocument.md#cimprojectitem) | The items of the project. 
| databaseConnections | [[CIMWorkspaceConnection]](CIMVectorLayers.md#cimworkspaceconnection) | The database connections of the project. 
| serverConnections | [[CIMServerConnection]](Types.md#serverconnection) | The service connections of the project. 
| folderConnections | [[CIMFolderConnection]](CIMVectorLayers.md#cimfolderconnection) | The folder connections of the project. 
| viewLayoutXML | string | An XML representation of the view layout used for the project. 
| defaultGeoDatabase | string | The path of the default geodatabase of the project. 
| defaultToolbox | string | The path of the default toolbox of the project. 
| defaultSpatialReference | string | A WKT string representation of the default spatial reference of the project. 
| defaultFolder | string | The default folder of the project. 
| projectMetadata | string | The path to an XML file in the same folder as the APRX that contains metadata about the project. 
| sourceURI | string | The source URI of the project. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the project was last modified. 
| readOnly | boolean | A value indicating whether the project is read only for updatable projects. 
| forceUpdate | boolean | A value indicating whether to force update an updatable project. 
| thumbnailOptions | [CIMProjectThumbnailOptions](CIMDocument.md#cimprojectthumbnailoptions) | The thumbnail generation options for the project. 






## CIMGenericView
#### Represents a generic view. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
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
| tables | [string] | An array of table URIs stored in this layer document. 
| layerDefinitions | [[CIMDefinition]](Types.md#definition) | The layer definitions in the layer document. 
| binaryReferences | [[CIMBinaryReference]](CIMDocument.md#cimbinaryreference) | The binary references of the document. 
| tableDefinitions | [[CIMDefinition]](Types.md#definition) | The table definitions in the layer document. 
| RGBColorProfile | string | The name of the RGB color profile of this layer's source map. If the target map has color management enabled, this value will be used to transform the layer's RGB colors as it is imported into that map. 
| CMYKColorProfile | string | The name of the CMYK color profile of this layer's source map. If the target map has color management enabled, this value will be used to transform the layer's CMYK colors as it is imported into that map. 
| elevationSurfaceLayerDefinitions | [[CIMDefinition]](Types.md#definition) | The elevation surface layer definitions. 






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
| binaryReferences | [[CIMBinaryReference]](CIMDocument.md#cimbinaryreference) | The binary references of the document. 
| layerDefinitions | [[CIMDefinition]](Types.md#definition) | The layer definitions in the layout document. 
| mapDefinitions | [[CIMDefinition]](Types.md#definition) | The map definitions of the layout document. 
| tableDefinitions | [[CIMDefinition]](Types.md#definition) | The table definitions of the layout document. 
| layoutDefinition | [CIMLayout](CIMLayout.md#cimlayout) | The layout definition of the layout document. 
| linkChartDefinitions | [[CIMDefinition]](Types.md#definition) | The link chart definitions of the layout document. 
| timelineDefinitions | [[CIMDefinition]](Types.md#definition) | The timeline definitions of the layout document. 
| videoDefinitions | [[CIMDefinition]](Types.md#definition) | The video definitions of the layout document. 
| elevationSurfaceLayerDefinitions | [[CIMDefinition]](Types.md#definition) | The elevation surface layer definitions of the layout document. 






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
| layerDefinitions | [[CIMDefinition]](Types.md#definition) | The layer definitions of the map document. 
| binaryReferences | [[CIMBinaryReference]](CIMDocument.md#cimbinaryreference) | The binary references of the document. 
| tableDefinitions | [[CIMDefinition]](Types.md#definition) | The table definitions of the map document. 
| linkChartDefinitions | [[CIMDefinition]](Types.md#definition) | The link chart definitions of the map document. 
| timelineDefinitions | [[CIMDefinition]](Types.md#definition) | The timeline definitions of the map document. 
| videoDefinitions | [[CIMDefinition]](Types.md#definition) | The video definitions of the map document. 
| elevationSurfaceLayerDefinitions | [[CIMDefinition]](Types.md#definition) | The elevation surface layer definitions of the map document. 






## CIMMapTableView
#### Represents a map table view in the project. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
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
| frozenFields | long | The count of frozen fields. 
| zoomLevel | long | The zoom level of the table view. 
| fieldWidth | {JSON_object}| A property set of field width information. 
| displaySubtypeDomainDescriptions | boolean | A value indicating whether to display subtype and domain descriptions. 
| qualifyJoinFieldNames | boolean | A value indicating whether to qualify field names when the table contains fields from a join. 
| time | [TimeValue](ExternalReferences.md#timevalue) | The current time of the table view. 
| honorRange | boolean | A value indicating whether to honor ranges on the table view. 
| ranges | [[CIMLayerRange]](CIMVectorLayers.md#cimlayerrange) | The ranges of the table view. 
| extent | [Envelope](ExternalReferences.md#envelope) | The extent of the table view. 
| timeRelation | [enumeration esriTimeRelation](ExternalReferences.md#enumeration-esritimerelation) | A time relation which allows the start and end times to be included or excluded in the time query. 
| showOnlyContingentValueFields | boolean | A value indicating whether the table field visibility settings should be overridden to only show fields that are part of one or more contingent value field groups. 
| highlightInvalidContingentValueFields | boolean | A value indicating whether invalid contingent value fields should be highlighted in the table. 
| autoPopulateContingentValueFields | boolean | A value indicating whether other contingent value fields should be automatically populated after a value is changed when only one match is valid. 
| columnHeaderRowHeight | [enumeration TableRowHeightType](CIMDocument.md#enumeration-tablerowheighttype) | A value indicating the height for the column header row in the table. 
| rowHeight | [enumeration TableRowHeightType](CIMDocument.md#enumeration-tablerowheighttype) | A value indicating the height for the rows in the table. 


### CIMMapTableView 

|Property | Type | Description | 
|---------|--------|--------|
| mapURI | string | The path of the Map for the item in the view. 






## CIMMapView
#### Represents a map view in the project. 


### CIMView 

|Property | Type | Description | 
|---------|--------|--------|
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
| layerRanges | [[CIMLayerRange]](CIMVectorLayers.md#cimlayerrange) | The layer ranges of the view. 
| rangeSliderSettings | [CIMSliderSettings](CIMMap.md#cimslidersettings) | The range slider settings of the view. 
| timeSliderSettings | [CIMSliderSettings](CIMMap.md#cimslidersettings) | The time slider settings of the view. 
| floorFilterSettings | [CIMFloorFilterSettings](CIMMap.md#cimfloorfiltersettings) | The floor filter settings of the view. 
| sceneDrawingMode | [enumeration SceneDrawingMode](CIMDocument.md#enumeration-scenedrawingmode) | The scene's drawing mode. 
| fieldOfView | double | The scene's field-of-view in degrees (value must be between 35 and 70). Only used when the scene is in Perspective draw mode. 
| pauseDrawing | boolean | A value indicating whether drawing is in paused state for the view. 
| pauseAnimatedSymbols | boolean | A value indicating whether all animated symbol playback is in paused state for the view. 
| exploratoryAnalysis | [[CIMExploratoryAnalysisDefinition]](Types.md#exploratoryanalysisdefinition) | The exploratory analysis definitions for the view. 
| visualEffect | [VisualEffect](Types.md#visualeffect) | The visual effect definition for the scene. 
| cameraEffect | [CameraEffect](Types.md#cameraeffect) | The camera effect definition for the scene. 
| postprocessingEffects | [[CIMPostprocessingEffect]](Types.md#postprocessingeffect) | The post-processing effect definitions for the scene. 
| colorVisionDeficiencyMode | [enumeration ColorVisionDeficiencyType](CIMEnumerations.md#enumeration-colorvisiondeficiencytype) | The color vision deficiency mode of the view. 






## CIMModuleSettings
#### Represents module settings in the project. 


### CIMModuleSettings 

|Property | Type | Description | 
|---------|--------|--------|
| moduleName | string | The name of the module. 
| settingsXML | string | Module settings as XML. 






## CIMPresentationDocument
#### Represents a presentation document which is the document type used for saving .prsx files. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMPresentationDocument 

|Property | Type | Description | 
|---------|--------|--------|
| presentationDefinition | [CIMPresentation](CIMPresentation.md#cimpresentation) | The presentation definition in the document. 
| binaryReferences | [[CIMBinaryReference]](CIMDocument.md#cimbinaryreference) | The binary references in the document. 
| layerDefinitions | [[CIMDefinition]](Types.md#definition) | The layer definitions in the document. 
| mapDefinitions | [[CIMDefinition]](Types.md#definition) | The map definitions in the document. 
| tableDefinitions | [[CIMDefinition]](Types.md#definition) | The table definitions in the document. 
| linkChartDefinitions | [[CIMDefinition]](Types.md#definition) | The link chart definitions in the document. 
| timelineDefinitions | [[CIMDefinition]](Types.md#definition) | The timeline definitions in the document. 
| videoDefinitions | [[CIMDefinition]](Types.md#definition) | The video definitions in the document. 
| elevationSurfaceLayerDefinitions | [[CIMDefinition]](Types.md#definition) | The elevation surface layer definitions in the document. 






## CIMProjectItem
#### Represents an item in the project. 


### CIMProjectItem 

|Property | Type | Description | 
|---------|--------|--------|
| alias | string | An identifier for this item that the user provides and can be displayed instead of the Name. 
| ID | string | The system assigned unique identifier of the project item. 
| catalogPath | string | The catalog path of the project item. 
| pathHint | string | The path hint of the project item. Contains the absolute path of the item. Used as a fallback in case the relative path cannot be resolved. 
| itemType | string | The item type of the project item. 
| name | string | The name of the project item. 
| propertiesXML | string | Properties of the item as XML. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | Modified time of the item as a time instant. 
| consolidatePath | boolean | A value indicating whether to consolidate the path of the project item. 
| consolidationResources | [string] | Consolidation resources string array of the project item. 
| pathSaveRelative | boolean | A value indicating whether the item is saved with relative paths. 
| metadataURI | string | The URI of the binary reference containing the metadata. This property is only used for project items representing tasks. 





### Enumeration: ProjectThumbnailAutomaticGenerationSource
#### Represents the sources for automatic project thumbnail generation. 

|Property | Value | Description | 
|---------|--------|--------|
| ActiveMap| 0| Thumbnail is generated from the active map on save. 
| SpecifiedMap| 1| Thumbnail is generated from a specified map on save. 



### Enumeration: ProjectThumbnailGenerationMethod
#### Represents the types of project thumbnail generation. 

|Property | Value | Description | 
|---------|--------|--------|
| Manual| 0| Thumbnail is set manually in the UI by the user. 
| Automatic| 1| Thumbnail is set using the specified automatic generation source. 




## CIMProjectThumbnailOptions
#### A collection of options governing project thumbnail generation. 


### CIMProjectThumbnailOptions 

|Property | Type | Description | 
|---------|--------|--------|
| generationMethod | [enumeration ProjectThumbnailGenerationMethod](CIMDocument.md#enumeration-projectthumbnailgenerationmethod) | A value indicating how a thumbnail should be generated for a project. 
| automaticGenerationSource | [enumeration ProjectThumbnailAutomaticGenerationSource](CIMDocument.md#enumeration-projectthumbnailautomaticgenerationsource) | A value indicating how an automatically generated thumbnail is created. 
| mapURI | string | A value indicating the path of a map to be used in the automatic generation of a project thumbnail. 





### Enumeration: SceneDrawingMode
#### Represents the drawing modes of a scene view. 

|Property | Value | Description | 
|---------|--------|--------|
| Perspective| 0| Draw scene using vanishing point technique. 
| Isometric| 1| Draw scene using parallel line technique. 




## CIMStatisticalDataCollection
#### A statistical data collection is used by the Business Analyst to organize and present data that can be aggregated by the enrich functionality. This is not the storage of the data, it is metadata about the data that describes how data will be aggregated by Business Analyst. Currently, data can be calculated by defining what data collections and analysis variables are needed in the output for a given input features. 


### CIMStatisticalDataCollection 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The Name of the data collection. 
| shortDescription | string | Short description of the data collection. 
| longDescription | string | Long description of the data collection. 
| keywords | [string] | Keywords for the data collection. 
| countries | [string] | List of countries for data collection. Use to filter data collections by country. 
| categories | [string] | Levels of categories the data collection. Used to show the data collection in the Data Browser. 
| author | string | Author of the data collection. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant) | Creation date of the data collection. 
| lastRevisionDate | [TimeInstant](ExternalReferences.md#timeinstant) | Last revision date of the data collection. 
| calculators | [[CIMStatisticalDataCollectionCalculator]](Types.md#statisticaldatacollectioncalculator) | The Calculators of the data collection. 
| dataVintage | string | Vintage of used data (for example, "Q3_2018"). 
| dataVintageDescription | string | Description of used data ("2018 US Data Update"). 
| icon | string | Data collection image. 






## CIMStatisticalDataCollectionDocument
#### Represents a document used for saving statistical data collections. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMStatisticalDataCollectionDocument 

|Property | Type | Description | 
|---------|--------|--------|
| statisticalDataCollection | [CIMStatisticalDataCollection](CIMDocument.md#cimstatisticaldatacollection) | The Statistical Data Collection. 






## CIMStatisticalDataCollectionFeatureLayerCalculator
#### Statistical data collection calculator based on a feature layer. 


### CIMStatisticalDataCollectionCalculator 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The Name of the calculator. 


### CIMStatisticalDataCollectionFeatureLayerCalculator 

|Property | Type | Description | 
|---------|--------|--------|
| datasetID | string | The DatasetID which is used for getting the information about which points layer will be available and which apportionment methods will be used. If DatasetID is empty, only Area Apportionment method is available. 
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection to the source. 
| fields | [[CIMStatisticalDataCollectionField]](CIMDocument.md#cimstatisticaldatacollectionfield) | The regular fields of the calculator. 
| apportionmentDatasetConnection | [DataConnection](Types.md#dataconnection) | The data connection to apportionment dataset. This property is optional. 






## CIMStatisticalDataCollectionField
#### Represents a field of a statistical data collection that matches to existing field in referenced feature dataset. 


### CIMStatisticalDataCollectionField 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The field name from the data. 
| alias | string | The alias of the field. 
| category | string | The category of the field. 
| apportionmentMethod | string | How the values from the feature service are apportioned. For local data it should be one of the apportionment method from default hierarchy of the specified dataset. Use ?GEOM? for Area apportionment. 
| summaryType | [enumeration StatisticalDataCollectionSummaryType](CIMDocument.md#enumeration-statisticaldatacollectionsummarytype) | The summary type how apportioned values are summarized to produce the final result. 
| weightFieldName | string | The additional attribute for 'Average' summary type that defines which field should be used to get weighted sum. 
| precision | long | The number of digits in a number. For example, the number 56.78 has a precision of 4. Precision is only valid for fields that are numeric. 
| fieldFormat | [enumeration StatisticalReportFieldFormat](CIMDocument.md#enumeration-statisticalreportfieldformat) | How to display values of the field in reports. 
| vintage | string | The description of vintage of the data (For example, "US2018 Q4"). 
| script | string | The additional attribute for 'Script' summary type that defines script which should be calculated. 
| scriptLanguage | [enumeration LabelExpressionEngine](CIMLabelPlacement.md#enumeration-labelexpressionengine) | The additional attribute for 'Script' summary type that defines script language used by 'Script' attribute. Currently only Python is supported. 
| usedFields | [string] | The additional attribute for 'Script' summary type that defines another fields used by script. These may include featureclass fields (even non-existing in calculator?) and another scripts. 
| showInDataBrowser | boolean | A value indicating whether the field will be shown in the Data Browser control in ArcGIS Pro. 
| outputFieldType | [enumeration esriFieldType](ExternalReferences.md#enumeration-esrifieldtype) | The type of the field for enrich output. For example, if we want to have a script variable returning String type values (like TLIFENAME variable in US dataset), or when the input (SDCX layer) fields are Integers we want to have integer output too. 






## CIMStatisticalDataCollectionInputAreaProperty
#### Represents the property used to calculate the geodesic area of the input feature. 


### CIMStatisticalDataCollectionInputProperty 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the property. 
| alias | string | The alias of the property. 
| propertyType | [enumeration esriFieldType](ExternalReferences.md#enumeration-esrifieldtype) | The type of the property. 


### CIMStatisticalDataCollectionInputAreaProperty 

|Property | Type | Description | 
|---------|--------|--------|
| units | [AreaUnit](ExternalReferences.md#areaunit) | The area units. 






## CIMStatisticalDataCollectionInputPropertiesCalculator
#### Statistical Data Collection calculator for accessing properties of input features, e.g. Area of polygonal input. 


### CIMStatisticalDataCollectionCalculator 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The Name of the calculator. 


### CIMStatisticalDataCollectionInputPropertiesCalculator 

|Property | Type | Description | 
|---------|--------|--------|
| area | [CIMStatisticalDataCollectionInputAreaProperty](CIMDocument.md#cimstatisticaldatacollectioninputareaproperty) | The area property. If this property is not null, the geodesic area of the input feature will be calculated. 






## CIMStatisticalDataCollectionInputProperty
#### Represents a property of an input feature. 


### CIMStatisticalDataCollectionInputProperty 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the property. 
| alias | string | The alias of the property. 
| propertyType | [enumeration esriFieldType](ExternalReferences.md#enumeration-esrifieldtype) | The type of the property. 






## CIMStatisticalDataCollectionScriptCalculator
#### Statistical data collection calculator based on a scripts that use fields from other calculators. 


### CIMStatisticalDataCollectionCalculator 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The Name of the calculator. 


### CIMStatisticalDataCollectionScriptCalculator 

|Property | Type | Description | 
|---------|--------|--------|
| scripts | [[CIMStatisticalDataCollectionField]](CIMDocument.md#cimstatisticaldatacollectionfield) | The scripts of the calculator. 






## CIMStatisticalDataCollectionStandardDataCalculator
#### Statistical data collection calculator based on a standard local data. 


### CIMStatisticalDataCollectionCalculator 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The Name of the calculator. 


### CIMStatisticalDataCollectionStandardDataCalculator 

|Property | Type | Description | 
|---------|--------|--------|
| datasetID | string | The DatasetID which is used for getting the information about which points layer will be available and which apportionment methods will be used. For example, for US 2019 dataset it will be ID of the dataset: "USA_ESRI_2019". 
| variables | [[CIMStatisticalDataCollectionStandardVariable]](CIMDocument.md#cimstatisticaldatacollectionstandardvariable) | The variables of the calculator. 






## CIMStatisticalDataCollectionStandardVariable
#### Represents a field of a statistical data collection that matches to an existing variable in referenced feature dataset. 


### CIMStatisticalDataCollectionStandardVariable 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the variable. 
| showInDataBrowser | boolean | A value indicating whether the variable will be shown in the Data Browser control in ArcGIS Pro. 





### Enumeration: StatisticalDataCollectionSummaryType
#### Represents the script language used by the statistical data collection. 

|Property | Value | Description | 
|---------|--------|--------|
| Sum| 0| Sum 
| Avg| 1| Average 
| Min| 2| Minimum 
| Max| 3| Maximum 
| Script| 4| Script/Calculated variable 



### Enumeration: StatisticalReportFieldFormat
#### How to display values of the field in reports. 

|Property | Value | Description | 
|---------|--------|--------|
| Count| 0| Regular value (numeric or text). 
| Percent| 1| It is a percentage value and it should displayed using the rules for percentage values. 
| Currency| 2| The value is a currency and should be displayed using the rules for currencies. 



### Enumeration: TableRowHeightType
#### Represents the height of rows in the table view. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| No row height. 
| Single| 1| The row will display one line of text. 
| Double| 2| The row will display two lines of text. 
| Triple| 3| The row will display three lines of text. 

