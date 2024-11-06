


## CIMBAAreaOfInterest
#### Represents Business Analyst Color Coded Layer Area Of Interest properties. 


### CIMBAAreaOfInterest 

|Property | Type | Description | 
|---------|--------|--------|
| areaOfInterestDataConnection | [CIMStandardDataConnection](CIMVectorLayers.md#cimstandarddataconnection) | The area of interest data connection. 
| areaOfInterestItems | [[CIMBAAreaOfInterestItem]](Types.md#baareaofinterestitem) | The area of interest items. 






## CIMBAAreaOfInterestItem
#### Represents Business Analyst Color Coded Layer area of interest item. 


### CIMBAAreaOfInterestItem 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The area of interest item name. 






## CIMBABenchmarkComparisonsProperties
#### Benchmark Comparisons properties. 


### CIMBABenchmarkComparisonsProperties 

|Property | Type | Description | 
|---------|--------|--------|
| nameField | string | The Name field which is required. 
| siteAttributes | [string] | The fields in the input features layer containing site-specific attributes. 
| variables | [string] | The variables from the data browser, such as income, population, or spending, used to enrich the input features. 
| addDifferenceField | boolean | A value indicating whether to add difference benchmark field. 
| addPercentDifferenceField | boolean | A value indicating whether to add % difference benchmark field. 
| benchmarkMethod | [enumeration BABenchmarkMethod](CIMBusinessAnalyst.md#enumeration-babenchmarkmethod) | The benchmark method. 
| benchmarkFeatureID | string | Benchmark feature ID. 
| benchmarkStyle | [enumeration BABenchmarkStyle](CIMBusinessAnalyst.md#enumeration-babenchmarkstyle) | Benchmark style. 
| aboveColor | [CIMRGBColor](CIMColor.md#cimrgbcolor) | Above color. 
| belowColor | [CIMRGBColor](CIMColor.md#cimrgbcolor) | Below color. 
| inBetweenColor | [CIMRGBColor](CIMColor.md#cimrgbcolor) | In-between color. 
| quartile1Color | [CIMRGBColor](CIMColor.md#cimrgbcolor) | Quartile 1 color. 
| quartile2Color | [CIMRGBColor](CIMColor.md#cimrgbcolor) | Quartile 2 color. 
| quartile3Color | [CIMRGBColor](CIMColor.md#cimrgbcolor) | Quartile 3 color. 
| quartile4Color | [CIMRGBColor](CIMColor.md#cimrgbcolor) | Quartile 4 color. 
| geographyLevels | [string] | Standard geography levels that can be added to the results table. 





### Enumeration: BABenchmarkMethod
#### Specifies options for setting a benchmark. Site attributes and variables for the input features are compared against the benchmark. 

|Property | Value | Description | 
|---------|--------|--------|
| Average| 1| The benchmark set to the average values for site attributes and variables for all features. 
| Median| 2| The benchmark set to the median values for site attributes and variables for all features. 
| Feature| 3| The benchmark set to values for all site attributes and variables for a selected feature. 
| None| 4| No benchmark will be set. 



### Enumeration: BABenchmarkStyle
#### Specifies the colors used in the results table fields to show differences from the benchmark. 

|Property | Value | Description | 
|---------|--------|--------|
| AboveOrBelow| 1| Above or below. 
| AboveInBetweenOrBelow| 2| Above, in-between or below. 
| Quartiles| 3| Quartiles. 



### Enumeration: BABoundaryMode
#### Represents Color Coded Layer bounday type. 

|Property | Value | Description | 
|---------|--------|--------|
| Geographies| 1| Standard Geographies mode. 
| H3Hexagons| 2| H3 Hexagon mode. 




## CIMBAColorCodedLayerParameters
#### Represents Business Analyst Color Coded Layer Properties. 


### CIMBAColorCodedLayerParameters 

|Property | Type | Description | 
|---------|--------|--------|
| dataSource | string | The data source used in calculation of distances. Structure of the value is TYPE;COUNTRY_INFO;LOCAL_DATA_INFO where TYPE can be ONLINE, LOCAL, or CUSTOM. COUNTRY_INFO is country_id{|hierarchy}. For example, US|census or US. LOCAL_DATA_INFO is ID of local dataset. For example, USA_ESRI_2019. For example, for local US 2019 dataset it will be: "LOCAL;;USA_ESRI_2019". If online US data source is used, it may be "ONLINE;US|census;". Can be value of baDataSource GP GPEnvironment variable. https://pro.arcgis.com/en/pro-app/tool-reference/environment-settings/ba-data-source.htm. 
| rendererProperties | [BARendererProperties](Types.md#barendererproperties) | The Color Coded Map renderer properties. 
| variable | string | The demographic variable name. 
| areaOfInterest | [CIMBAAreaOfInterest](CIMBusinessAnalyst.md#cimbaareaofinterest) | The area of interest parameters. 
| activeLevelOfDetail | string | The level of details. It's a layer ID of a standard geography. If ActiveLevelOfDetail is empty, automatic level selection based on the current map scale will be used. 
| levelsOfDetail | [[CIMBALevelOfDetail]](CIMBusinessAnalyst.md#cimbalevelofdetail) | The level of detail items. 
| boundaryMode | [enumeration BABoundaryMode](CIMBusinessAnalyst.md#enumeration-baboundarymode) | The Color Coded Layer boundary mode. 
| resultsPaneSettings | [BAResultsPaneSettings](Types.md#baresultspanesettings) | The results pane settings. 





### Enumeration: BACombinationMethod
#### Represents Suitability Analysis combination method. 

|Property | Value | Description | 
|---------|--------|--------|
| Sum| 1| Sum combination method, to sum the weighted scores. 
| Mean| 2| Sum combination method, to use the mean (or average) of the weighted scores. 
| Product| 3| Product combination method to use the product of the weighted scores. 
| GeometricMean| 4| Geometric mean combination method to use the geometric mean of the weighted scores. 



### Enumeration: BACriterionInfluence
#### Represents Suitability Analysis criterion influence. 

|Property | Value | Description | 
|---------|--------|--------|
| Positive| 1| Positive criterion influence. 
| Inverse| 2| Inverse criterion influence. 
| Ideal| 3| Ideal criterion influence. 
| TargetSite| 4| Target site criterion influence. 




## CIMBAFeatureClassAreaOfInterestItem
#### Represents Business Analyst Color Coded Layer feature class based area of interest item. 


### CIMBAAreaOfInterestItem 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The area of interest item name. 


### CIMBAFeatureClassAreaOfInterestItem 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [CIMStandardDataConnection](CIMVectorLayers.md#cimstandarddataconnection) | The feature class data connection. 






## CIMBAFeatureLayerAreaOfInterestItem
#### Represents Business Analyst Color Coded Layer feature layer based area of interest item. 


### CIMBAAreaOfInterestItem 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The area of interest item name. 


### CIMBAFeatureLayerAreaOfInterestItem 

|Property | Type | Description | 
|---------|--------|--------|
| URI | string | The area of interest feature layer URI. 






## CIMBAFieldBasedCriterion
#### Represents a Business Analyst Suitability Analysis field-based criterion. 


### CIMBASuitabilityAnalysisCriterion 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The ID of the criterion. 
| title | string | The title of the criterion. 
| valueField | string | The value of the criterion. 
| weight | double | The weight of the criterion. 
| isEnabled | boolean | A value indicating whether the criterion is enabled. 
| isLocked | boolean | A value indicating whether the criterion is locked. 
| influence | [enumeration BACriterionInfluence](CIMBusinessAnalyst.md#enumeration-bacriterioninfluence) | The influence of the criterion. 
| min | double | The min of the criterion. 
| max | double | The max of the criterion. 
| idealValue | double | The ideal value of the criterion. 
| targetValue | double | The calculated value of the Target Site of the criterion. 


### CIMBAFieldBasedCriterion 

|Property | Type | Description | 
|---------|--------|--------|
| fieldName | string | The Selected Field Name. 





### Enumeration: BAFinalScoreMethod
#### Represents Suitability Analysis final score scale method. 

|Property | Value | Description | 
|---------|--------|--------|
| None| 0| None method to leave the data as is, without scaling it. 
| Method0_1| 1| 0 to 1 method to calculate a final score with the lowest value of 0 and the highest value of 1. 
| Method0_100| 2| 0 to 100 method to calculate a final score with the lowest value of 0 and the highest value of 100. 




## CIMBAGraduatedColorsRendererProperties
#### Represents Business Analyst Color Coded Layer graduated colors renderer properties. 


### CIMBARendererProperties 

|Property | Type | Description | 
|---------|--------|--------|


### CIMBAGraduatedColorsRendererProperties 

|Property | Type | Description | 
|---------|--------|--------|
| numBreaks | long | The number of breaks for classification renderer. 
| classificationMethod | [enumeration ClassificationMethod](CIMRenderers.md#enumeration-classificationmethod) | The classification method. 
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| classificationField | string | The classification field name in the levels of detail feature classes. Each level of detail may contain several fields for classification, depending on the variable flavors (i.e. "base", "percent", "average", "index", etc). ClassificationField is used to switch between the flavours to quickly update the classification renderer. 





### Enumeration: BAHistogramSubsetSelectionMethod
#### Represents histogram chart subset selection methods. 

|Property | Value | Description | 
|---------|--------|--------|
| Outliers| 1| Histogram chart selection is defined by outliers. 
| Percentage| 2| Histogram chart selection is defined by percentage. 
| StandardDeviation| 3| Histogram chart selection is defined by standard deviation. 




## CIMBALevelOfDetail
#### Represents Business Analyst Color Coded Layer level of detail. 


### CIMBALevelOfDetail 

|Property | Type | Description | 
|---------|--------|--------|
| levelID | string | The level of detail LevelID. 
| dataConnection | [CIMStandardDataConnection](CIMVectorLayers.md#cimstandarddataconnection) | The level of detail data connection. 





### Enumeration: BAPointCriterionType
#### Represents Suitability Analysis point layer based criterion type. Defines the type of spatial relationship to be used as criteria. 

|Property | Value | Description | 
|---------|--------|--------|
| Count| 1| Count criteria type. 
| Weight| 2| Weight criteria type. 
| MinDistance| 3| Minimal distance criteria type. 




## CIMBAPointLayerBasedCriterion
#### Represents a Business Analyst Suitability Analysis point layer-based criterion. 


### CIMBASuitabilityAnalysisCriterion 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The ID of the criterion. 
| title | string | The title of the criterion. 
| valueField | string | The value of the criterion. 
| weight | double | The weight of the criterion. 
| isEnabled | boolean | A value indicating whether the criterion is enabled. 
| isLocked | boolean | A value indicating whether the criterion is locked. 
| influence | [enumeration BACriterionInfluence](CIMBusinessAnalyst.md#enumeration-bacriterioninfluence) | The influence of the criterion. 
| min | double | The min of the criterion. 
| max | double | The max of the criterion. 
| idealValue | double | The ideal value of the criterion. 
| targetValue | double | The calculated value of the Target Site of the criterion. 


### CIMBAPointLayerBasedCriterion 

|Property | Type | Description | 
|---------|--------|--------|
| dataSource | string | The data source used in calculation of distances. Structure of the value is TYPE;COUNTRY_INFO;LOCAL_DATA_INFO where TYPE can be ONLINE, LOCAL, or CUSTOM. COUNTRY_INFO is country_id{|hierarchy}. For example, US|census or US. LOCAL_DATA_INFO is ID of local dataset. For example, USA_ESRI_2019. For example, for local US 2019 dataset it will be: "LOCAL;;USA_ESRI_2019". If online US data source is used, it may be "ONLINE;US|census;". Can be value of baDataSource GP GPEnvironment variable. https://pro.arcgis.com/en/pro-app/tool-reference/environment-settings/ba-data-source.htm. 
| siteLayerIdField | string | The Site Layer Id Field name. 
| pointLayerDataConnection | [CIMStandardDataConnection](CIMVectorLayers.md#cimstandarddataconnection) | The data connection to the Point Layer. 
| pointCriterionType | [enumeration BAPointCriterionType](CIMBusinessAnalyst.md#enumeration-bapointcriteriontype) | The point criterion Type. 
| weightField | string | The Weight Field. 
| statisticsType | [enumeration BAPointStatisticsType](CIMBusinessAnalyst.md#enumeration-bapointstatisticstype) | The Statistics Type. 
| distanceUnits | [LinearUnit](ExternalReferences.md#linearunit) | Distance units used in calculation of distances. 
| useTimeUnits | boolean | A value indicating whether to use time units. 
| timeUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | Time units used in calculation of distances. 
| travelModeId | string | ID of travel mode used in calculation of distances. 
| useNetworkDistance | boolean | A value indicating whether to use network dataset to calculate distances. 
| siteCentersLayerDataConnection | [CIMStandardDataConnection](CIMVectorLayers.md#cimstandarddataconnection) | The data connection to the Site Centers Layer. 
| siteCentersLayerId | string | The Site Centers Layer Id. 
| cutoffDistance | double | The Cutoff Distance. 0 for no cutoff. 





### Enumeration: BAPointStatisticsType
#### Represents Suitability Analysis point layer based criterion statistics type. The type of statistical operation to be applied to the weighted field. 

|Property | Value | Description | 
|---------|--------|--------|
| Sum| 1| Sum statistics type. 
| Ave| 2| Average statistics type. 
| StdDev| 3| Standard Deviation statistics type. 
| Min| 4| Minimum statistics type. 
| Max| 5| Maximum statistics type. 



### Enumeration: BAPreprocessingMethod
#### Represents Suitability Analysis preprocessing method. 

|Property | Value | Description | 
|---------|--------|--------|
| MinMax| 1| Minimum-maximum preprocessing method. 
| Percentile| 2| Percentile preprocessing method. 
| ZScore| 3| Z-score preprocessing method. 
| Raw| 4| Raw values preprocessing method. 



### Enumeration: BAPresetMethod
#### Represents Suitability Analysis preset method. 

|Property | Value | Description | 
|---------|--------|--------|
| CombineValues| 1| Combine values preset method. For preprocessing, it uses the Minimum-maximum method. For combination, it uses the Sum method. 
| CompoundDifferences| 2| Compound differences preset method. For preprocessing, it uses the Minimum-maximum method. For combination, it uses the Geometric mean method. 
| Custom| 3| Custom preset method. 




## CIMBAResultsPaneSettings
#### Represents Business Analyst Results Pane settings. 


### CIMBAResultsPaneSettings 

|Property | Type | Description | 
|---------|--------|--------|
| matchTopBottomChartToLayerSymbology | boolean | A value indicating whether top/bottom charts should match layer symbology. 
| histogramSubsetSelectionMethod | [enumeration BAHistogramSubsetSelectionMethod](CIMBusinessAnalyst.md#enumeration-bahistogramsubsetselectionmethod) | The histogram chart subset selection method. 
| histogramSubsetSelectionValue | double | The histogram chart subset selection method value. 
| histogramBinCount | long | The number of bins in the histogram chart. 
| histogramFillSymbolProperties | [CIMChartFillSymbolProperties](CIMCharts.md#cimchartfillsymbolproperties) | The fill symbol properties of the histogram chart bar. 
| tableSortDirection | [enumeration SortOrderType](CIMLayer.md#enumeration-sortordertype) | The direction of the sort in the Results Pane table. 
| tableSortField | string | The sort field of the Results Pane table. 





### Enumeration: BAScatterplotChartType
#### Represents scatterplot chart types. 

|Property | Value | Description | 
|---------|--------|--------|
| Scatterplot| 1| Scatterplot chart type. 
| BubbleChart| 2| Bubble chart type. 




## CIMBAStdGeoAreaOfInterestItem
#### Represents Business Analyst Color Coded Layer standard geography based area of interest item. 


### CIMBAAreaOfInterestItem 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The area of interest item name. 


### CIMBAStdGeoAreaOfInterestItem 

|Property | Type | Description | 
|---------|--------|--------|
| levelID | string | The standard geography level ID. 
| geographyID | string | The standard geography geography ID. 






## CIMBASuitabilityAnalysisLayer
#### Represents a Business Analyst Suitability Analysis layer. 


### CIMBASuitabilityAnalysisLayer 

|Property | Type | Description | 
|---------|--------|--------|
| suitabilityAnalysisSubLayer | [BASuitabilityAnalysisSubLayer](Types.md#basuitabilityanalysissublayer) | The Suitability Analysis sub-layer. 
| targetSite | [CIMBASuitabilityAnalysisTargetSiteSubLayer](CIMBusinessAnalyst.md#cimbasuitabilityanalysistargetsitesublayer) | The Suitability Analysis Target Site. 
| criteria | [[CIMBASuitabilityAnalysisCriterion]](Types.md#basuitabilityanalysiscriterion) | The Suitability Analysis criterion info items. 
| presetMethod | [enumeration BAPresetMethod](CIMBusinessAnalyst.md#enumeration-bapresetmethod) | The Suitability Analysis preset method. 
| preprocessingMethod | [enumeration BAPreprocessingMethod](CIMBusinessAnalyst.md#enumeration-bapreprocessingmethod) | The Suitability Analysis preprocessing method. 
| combinationMethod | [enumeration BACombinationMethod](CIMBusinessAnalyst.md#enumeration-bacombinationmethod) | The Suitability Analysis combination method. 
| finalScoreScale | [enumeration BAFinalScoreMethod](CIMBusinessAnalyst.md#enumeration-bafinalscoremethod) | The Suitability Analysis final score scale method. 
| rendererProperties | [BARendererProperties](Types.md#barendererproperties) | The Suitability Analysis layer renderer properties. 
| classificationTransparency | double | The classification transparency. 
| outlineColor | [Color](Types.md#color) | The outline color. 
| outlineWidth | double | The outline width. 
| resultsPaneSettings | [CIMBASuitabilityAnalysisResultsPaneSettings](CIMBusinessAnalyst.md#cimbasuitabilityanalysisresultspanesettings) | The results pane settings. 






## CIMBASuitabilityAnalysisResultsPaneSettings
#### Represents Suitability Analysis Results Pane settings. 


### CIMBAResultsPaneSettings 

|Property | Type | Description | 
|---------|--------|--------|
| matchTopBottomChartToLayerSymbology | boolean | A value indicating whether top/bottom charts should match layer symbology. 
| histogramSubsetSelectionMethod | [enumeration BAHistogramSubsetSelectionMethod](CIMBusinessAnalyst.md#enumeration-bahistogramsubsetselectionmethod) | The histogram chart subset selection method. 
| histogramSubsetSelectionValue | double | The histogram chart subset selection method value. 
| histogramBinCount | long | The number of bins in the histogram chart. 
| histogramFillSymbolProperties | [CIMChartFillSymbolProperties](CIMCharts.md#cimchartfillsymbolproperties) | The fill symbol properties of the histogram chart bar. 
| tableSortDirection | [enumeration SortOrderType](CIMLayer.md#enumeration-sortordertype) | The direction of the sort in the Results Pane table. 
| tableSortField | string | The sort field of the Results Pane table. 


### CIMBASuitabilityAnalysisResultsPaneSettings 

|Property | Type | Description | 
|---------|--------|--------|
| histogramCriterionID | string | The criterion ID for the histogram chart. 
| showRegressionLineOnScatterplot | boolean | A value indicating whether the regression line should be shown on the scatterplot chart. 
| scatterplotChartType | [enumeration BAScatterplotChartType](CIMBusinessAnalyst.md#enumeration-bascatterplotcharttype) | The scatterplot chart type. 
| scatterplotXAxisCriterionID | string | The criterion ID for the X-Axis of the scatterplot chart. 
| scatterplotYAxisCriterionID | string | The criterion ID for the Y-Axis of the scatterplot chart. 
| scatterplotDotSizeCriterionID | string | The criterion ID for the dot size of the scatterplot chart. 






## CIMBASuitabilityAnalysisSubLayer
#### Represents a sub-layer of a Business Analyst Suitability Analysis layer. 


### CIMBASuitabilityAnalysisSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| featureClassDataConnection | [CIMStandardDataConnection](CIMVectorLayers.md#cimstandarddataconnection) | The Suitability Analysis sub-layer data connection. 






## CIMBASuitabilityAnalysisTargetSiteSubLayer
#### Represents a Business Analyst Suitability Analysis target site layer. 


### CIMBASuitabilityAnalysisSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| featureClassDataConnection | [CIMStandardDataConnection](CIMVectorLayers.md#cimstandarddataconnection) | The Suitability Analysis sub-layer data connection. 


### CIMBASuitabilityAnalysisTargetSiteSubLayer 

|Property | Type | Description | 
|---------|--------|--------|
| sourceTargetSiteDataConnection | [CIMStandardDataConnection](CIMVectorLayers.md#cimstandarddataconnection) | The Suitability Analysis target site data connection. 
| selectedSourceTargetSiteObjectID | string | The object ID of the Suitability Analysis target site. 






## CIMBAUniqueValueRendererProperties
#### Represents Business Analyst Color Coded Layer unique values renderer properties. 


### CIMBARendererProperties 

|Property | Type | Description | 
|---------|--------|--------|


### CIMBAUniqueValueRendererProperties 

|Property | Type | Description | 
|---------|--------|--------|
| colorRamp | [ColorRamp](Types.md#colorramp) | The color ramp. 
| classificationField | string | The classification field name in the levels of detail feature classes. 






## CIMBAVariableBasedCriterion
#### Represents a Business Analyst Suitability Analysis demographic variable-based criterion. 


### CIMBASuitabilityAnalysisCriterion 

|Property | Type | Description | 
|---------|--------|--------|
| ID | string | The ID of the criterion. 
| title | string | The title of the criterion. 
| valueField | string | The value of the criterion. 
| weight | double | The weight of the criterion. 
| isEnabled | boolean | A value indicating whether the criterion is enabled. 
| isLocked | boolean | A value indicating whether the criterion is locked. 
| influence | [enumeration BACriterionInfluence](CIMBusinessAnalyst.md#enumeration-bacriterioninfluence) | The influence of the criterion. 
| min | double | The min of the criterion. 
| max | double | The max of the criterion. 
| idealValue | double | The ideal value of the criterion. 
| targetValue | double | The calculated value of the Target Site of the criterion. 


### CIMBAVariableBasedCriterion 

|Property | Type | Description | 
|---------|--------|--------|
| dataSource | string | The data source used in calculation of distances. Structure of the value is TYPE;COUNTRY_INFO;LOCAL_DATA_INFO where TYPE can be ONLINE, LOCAL, or CUSTOM. COUNTRY_INFO is country_id{|hierarchy}. For example, US|census or US. LOCAL_DATA_INFO is ID of local dataset. For example, USA_ESRI_2019. For example, for local US 2019 dataset it will be: "LOCAL;;USA_ESRI_2019". If online US data source is used, it may be "ONLINE;US|census;". Can be value of baDataSource GP GPEnvironment variable. https://pro.arcgis.com/en/pro-app/tool-reference/environment-settings/ba-data-source.htm. 
| variable | string | The demographic variable name. 






## CIMBAVariableList
#### Represents Business Analyst variable list. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMBAVariableList 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | Name of variable list. 
| iconData | string | Base64 encoded icon. 
| author | string | The name of the author of the variable list. 
| tags | string | The tags for the variable list. Tags are keywords or short phrases that facilitate discovery of the variable list. Separate terms with commas. 
| dataSource | string | Data source of the variable list. Structure of the value is TYPE;COUNTRY_INFO;LOCAL_DATA_INFO where TYPE can be ONLINE, LOCAL, or CUSTOM. COUNTRY_INFO is country_id{|hierarchy}. For example, US|census or US. LOCAL_DATA_INFO is ID of local dataset. For example, USA_ESRI_2019. For example, for local US 2019 dataset it will be: "LOCAL;;USA_ESRI_2019". If online US data source is used, it may be "ONLINE;US|census;". Can be value of baDataSource GP GPEnvironment variable. https://pro.arcgis.com/en/pro-app/tool-reference/environment-settings/ba-data-source.htm. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant) | Creation date of the variable list. 
| lastRevisionDate | [TimeInstant](ExternalReferences.md#timeinstant) | Last revision date of the variable list. 
| variables | [[CIMBAVariableListVariable]](CIMBusinessAnalyst.md#cimbavariablelistvariable) | Variables. 





### Enumeration: BAVariableListValueType
#### Represents variable value type. 

|Property | Value | Description | 
|---------|--------|--------|
| Number| 0| Number value type. 
| Percent| 1| Percent value type. 
| Average| 2| Average value type. 
| Index| 3| Index value type. 




## CIMBAVariableListVariable
#### Represents variable of at variable list. 


### CIMBAVariableListVariable 

|Property | Type | Description | 
|---------|--------|--------|
| names | [string] | Names of the variable. 
| valueTypes | [[CIMBAVariableListValueType]](CIMBusinessAnalyst.md#cimbavariablelistvaluetype) | Value types of the variable. If null, Number value type is used. 






## CIMHuffModelAttractivenessVariable
#### Represents attractiveness variable used in Huff Model. 


### CIMHuffModelAttractivenessVariable 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the variable. 
| exponent | double | The exponent of the variable. 






## CIMHuffModelCalibrationDocument
#### Represents a Huff Model calibration. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMHuffModelCalibrationDocument 

|Property | Type | Description | 
|---------|--------|--------|
| RMSError | double | RMS error of Huff Model calibration. 
| RMSErrorLinear | double | Linearized RMS error of Huff Model calibration. 
| attractivenessVariables | [[CIMHuffModelAttractivenessVariable]](CIMBusinessAnalyst.md#cimhuffmodelattractivenessvariable) | Attractiveness variables of Huff Model calibration. 
| distanceParameters | [CIMHuffModelDistanceParameters](CIMBusinessAnalyst.md#cimhuffmodeldistanceparameters) | Distance parameters of Huff Model calibration. 
| facilities | [DataConnection](Types.md#dataconnection) | Facilities dataset used in Huff Model calibration. 
| facilitiesIDFieldName | string | Facility ID field name used in Huff Model calibration. 
| customers | [DataConnection](Types.md#dataconnection) | Customers dataset used in Huff Model calibration. 
| customersIDFieldName | string | Customer ID field name used in Huff Model calibration. 
| customerWeightFieldName | string | Customer weight field name used in Huff Model calibration. 
| salesPotential | [DataConnection](Types.md#dataconnection) | Sales potential dataset used in Huff Model calibration. 
| salesPotentialIDFieldName | string | Sales potential ID field name used in Huff Model calibration. 
| author | string | Author of Huff Model calibration. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant) | Creation date of Huff Model calibration. 
| lastRevisionDate | [TimeInstant](ExternalReferences.md#timeinstant) | Last revision date of Huff Model calibration. 






## CIMHuffModelDistanceParameters
#### Distance properties of the Huff Model calibration item. 


### CIMHuffModelDistanceParameters 

|Property | Type | Description | 
|---------|--------|--------|
| exponent | double | The exponent. 
| dataSource | string | Data source used in calculation of distances. Structure of the value is TYPE;COUNTRY_INFO;LOCAL_DATA_INFO where TYPE can be ONLINE, LOCAL, or CUSTOM. COUNTRY_INFO is country_id{|hierarchy}. For example, US|census or US. LOCAL_DATA_INFO is ID of local dataset. For example, USA_ESRI_2019. For example, for local US 2019 dataset it will be: "LOCAL;;USA_ESRI_2019". If online US data source is used, it may be "ONLINE;US|census;". Can be value of baDataSource GP GPEnvironment variable. https://pro.arcgis.com/en/pro-app/tool-reference/environment-settings/ba-data-source.htm. 
| distanceUnits | [LinearUnit](ExternalReferences.md#linearunit) | Distance units used in calculation of distances. 
| useTimeUnits | boolean | A value indicating whether to use time units. 
| timeUnits | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | Time units used in calculation of distances. 
| useNetworkDistance | boolean | A value indicating whether to use network dataset to calculate distances. 
| travelModeId | string | ID of travel mode used in calculation of distances. 
| towardsFacility | boolean | A value indicating whether to calculate distances toward facilities. 
| timeOfDay | [TimeInstant](ExternalReferences.md#timeinstant) | Time of day used in calculation of distances. 
| timeZone | string | Time zone used in calculation of distances. 






## CIMSegmentationProfile
#### Business Analyst segmentation profile. Segmentation profile represents distribution of the market (e.g. people or households) between the segments of the segmentation system. For example, it could represent the distribution of the customer base between the segments. Segmentation profile can include the volumetric information in addition to the counts, e.g. it could also provide the distribution of the sales between segments. 


### CIMSegmentationProfile 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the segmentation profile. 
| segmentationSystem | string | The segmentation system of the segmentation profile. 
| segmentationBase | string | Segmentation base of the segmentation profile. 
| hasVolumetricData | boolean | A value indicating whether the segmentation profile contains volumetric information. 
| author | string | The name of the author of the segmentation profile. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant) | Creation date of the segmentation profile. 
| lastRevisionDate | [TimeInstant](ExternalReferences.md#timeinstant) | Last revision date of the segmentation profile. 
| counts | [long] | The counts of the segmentation profile. 
| volumetricValues | [double] | The volumetric values of the segmentation profile. 






## CIMSegmentationProfileDocument
#### Represents a document used for saving segmentation profile. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMSegmentationProfileDocument 

|Property | Type | Description | 
|---------|--------|--------|
| profile | [CIMSegmentationProfile](CIMBusinessAnalyst.md#cimsegmentationprofile) | The segmentation profile. 






## CIMSegmentationTarget
#### Business Analyst segmentation target. Target is a collection of market segments that are treated as a whole. A user might apply the same marketing strategy to all segments in a target, for example. 


### CIMSegmentationTarget 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of target. 
| segmentIDs | [string] | The segment IDs of the target. 
| color | [Color](Types.md#color) | The color of the target. 






## CIMSegmentationTargetGroup
#### Business Analyst target group. Target group represents a collection of targets. 


### CIMSegmentationTargetGroup 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the target group. 
| segmentationSystem | string | The segmentation system of the target group. 
| description | string | Description of the target group. 
| author | string | The name of the author of the target group. 
| creationDate | [TimeInstant](ExternalReferences.md#timeinstant) | Creation date of the target group. 
| lastRevisionDate | [TimeInstant](ExternalReferences.md#timeinstant) | Last revision date of the target group. 
| targets | [[CIMSegmentationTarget]](CIMBusinessAnalyst.md#cimsegmentationtarget) | The targets of the target group. 
| visualizationProperties | [CIMSegmentationTargetGroupVisualizationProperties](CIMBusinessAnalyst.md#cimsegmentationtargetgroupvisualizationproperties) | Visualization properties of the target group. 






## CIMSegmentationTargetGroupDocument
#### Represents a document used for saving target group. 


### CIMVersion 

|Property | Type | Description | 
|---------|--------|--------|
| version | string | Document version. Set by the system. 
| build | long | The build an item was created with. Set by the system. 


### CIMSegmentationTargetGroupDocument 

|Property | Type | Description | 
|---------|--------|--------|
| targetGroup | [CIMSegmentationTargetGroup](CIMBusinessAnalyst.md#cimsegmentationtargetgroup) | The target group. 






## CIMSegmentationTargetGroupVisualizationProperties
#### Visualization properties of Business Analyst Segmentation target group. 


### CIMSegmentationTargetGroupVisualizationProperties 

|Property | Type | Description | 
|---------|--------|--------|
| targetProfile | [CIMSegmentationProfile](CIMBusinessAnalyst.md#cimsegmentationprofile) | The target profile of the target group. 
| baseProfile | [CIMSegmentationProfile](CIMBusinessAnalyst.md#cimsegmentationprofile) | The base profile of the target group. 
| thresholdIndex | double | The Threshold Index of the target group. 
| thresholdComposition | double | The Threshold Composition of the target group. 



