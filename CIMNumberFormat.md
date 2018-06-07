


## CIMAngleFormat
#### Represents an angle format. 


### CIMNumberFormat 

|Property | Type | Description | 
|---------|--------|--------|


### CIMNumericFormat 

|Property | Type | Description | 
|---------|--------|--------|
| alignmentOption | [enumeration esriNumericAlignmentEnum](ExternalReferences.md#enumeration-esrinumericalignmentenum)|Gets and sets the alignment option. 
| alignmentWidth | long|Gets and sets the alignment width. 
| roundingOption | [enumeration esriRoundingOptionEnum](ExternalReferences.md#enumeration-esriroundingoptionenum)|Gets and sets the rounding option. 
| roundingValue | long|Gets and sets the rounding value, whose meaning depends on the rounding option. 
| showPlusSign | bool|Gets and sets a boolean option indicating if formatted numbers contain a plus sign for positive numbers. 
| useSeparator | bool|Gets and sets a boolean option indicating if formatted numbers contain digit grouping symbols. 
| zeroPad | bool|Gets and sets a boolean option indicating if formatted numbers contain padded zeros to the right of the decimal. 


### CIMAngleFormat 

|Property | Type | Description | 
|---------|--------|--------|
| angleInDegrees | boolean|Gets and sets a boolean option indicating whether to display the angle in degrees. 
| displayDegrees | boolean|Gets and sets a boolean option indicating whether to display degrees. 






## CIMCurrencyFormat
#### Represents a currency format. 


### CIMNumberFormat 

|Property | Type | Description | 
|---------|--------|--------|


### CIMCurrencyFormat 

|Property | Type | Description | 
|---------|--------|--------|






## CIMCustomNumberFormat
#### Represents a custom number format. 


### CIMNumberFormat 

|Property | Type | Description | 
|---------|--------|--------|


### CIMCustomNumberFormat 

|Property | Type | Description | 
|---------|--------|--------|
| formatString | string|Gets and sets the format string (e.g. ###-## -#### ) 






## CIMDirectionFormat
#### Represents a direction format. 


### CIMNumberFormat 

|Property | Type | Description | 
|---------|--------|--------|


### CIMDirectionFormat 

|Property | Type | Description | 
|---------|--------|--------|
| decimalPlaces | long|Gets and sets the number of decimal places to show. 
| format | [enumeration DirectionFormatOption](CIMNumberFormat.md#enumeration-directionformatoption)|Gets and sets the format. 
| directionType | [enumeration DirectionType](CIMNumberFormat.md#enumeration-directiontype)|Gets and sets the direction type. 
| units | [enumeration DirectionUnits](CIMNumberFormat.md#enumeration-directionunits)|Gets and sets the direction units. 
| useNegativeAngles | bool|Gets and sets a boolean option indicating whether of not to use negative angles. 





### Enumeration: DirectionFormatOption
#### Direction format options. 

|Property | Value | Description | 
|---------|--------|--------|
| DegreesMinutesSeconds| 0| Degrees minutes seconds. 
| QuadrantBearing| 1| Quadrant bearing. 



### Enumeration: DirectionType
#### Direction type. 

|Property | Value | Description | 
|---------|--------|--------|
| NorthAzimuth| 0| North azimuth. 
| SouthAzimuth| 1| South azimuth. 
| Polar| 2| Polar. 
| QuadrantBearing| 3| Quadrant bearing. 



### Enumeration: DirectionUnits
#### Direction units. 

|Property | Value | Description | 
|---------|--------|--------|
| Radians| 0| Radians 
| DecimalDegrees| 1| Decimal degrees. 
| DegreesMinutesSeconds| 2| Degrees minutes seconds. 
| Gradians| 3| Gradians. 
| Gons| 4| Gons. 




## CIMFractionFormat
#### Represents a fraction format. 


### CIMNumberFormat 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFractionFormat 

|Property | Type | Description | 
|---------|--------|--------|
| option | [enumeration FractionOption](CIMNumberFormat.md#enumeration-fractionoption)|Gets and sets the fraction option determines how the numerator and denominator of the fraction are treated. 
| factor | long|Gets and sets the maximum number of digits for the numerator or denominator, or the denominator of the formatted fraction. 





### Enumeration: FractionOption
#### Fraction options. 

|Property | Value | Description | 
|---------|--------|--------|
| Digits| 0| Digits. 
| Denominator| 1| Denominator. 




## CIMLatLonFormat
#### Represents a lat lon format. 


### CIMNumberFormat 

|Property | Type | Description | 
|---------|--------|--------|


### CIMNumericFormat 

|Property | Type | Description | 
|---------|--------|--------|
| alignmentOption | [enumeration esriNumericAlignmentEnum](ExternalReferences.md#enumeration-esrinumericalignmentenum)|Gets and sets the alignment option. 
| alignmentWidth | long|Gets and sets the alignment width. 
| roundingOption | [enumeration esriRoundingOptionEnum](ExternalReferences.md#enumeration-esriroundingoptionenum)|Gets and sets the rounding option. 
| roundingValue | long|Gets and sets the rounding value, whose meaning depends on the rounding option. 
| showPlusSign | bool|Gets and sets a boolean option indicating if formatted numbers contain a plus sign for positive numbers. 
| useSeparator | bool|Gets and sets a boolean option indicating if formatted numbers contain digit grouping symbols. 
| zeroPad | bool|Gets and sets a boolean option indicating if formatted numbers contain padded zeros to the right of the decimal. 


### CIMLatLonFormat 

|Property | Type | Description | 
|---------|--------|--------|
| showDirections | boolean|Gets and sets a boolean option indicating if a directional letter (N-S-E-W) is appended to the formatted number. 
| isLatitude | boolean|Gets and sets a boolean option indicating if a formatted number is a latitude or not. 
| showZeroMinutes | boolean|Gets and sets a boolean option indicating if zero minutes are included in formatted output. 
| showZeroSeconds | boolean|Gets and sets a boolean option indicating if zero seconds are included in formatted output. 





### Enumeration: NumericAlignment
#### Numeric alignment types. 

|Property | Value | Description | 
|---------|--------|--------|
| AlignRight| 0| Align right. 
| AlignLeft| 1| Align left. 




## CIMNumericFormat
#### Represents a numeric format. 


### CIMNumberFormat 

|Property | Type | Description | 
|---------|--------|--------|


### CIMNumericFormat 

|Property | Type | Description | 
|---------|--------|--------|
| alignmentOption | [enumeration esriNumericAlignmentEnum](ExternalReferences.md#enumeration-esrinumericalignmentenum)|Gets and sets the alignment option. 
| alignmentWidth | long|Gets and sets the alignment width. 
| roundingOption | [enumeration esriRoundingOptionEnum](ExternalReferences.md#enumeration-esriroundingoptionenum)|Gets and sets the rounding option. 
| roundingValue | long|Gets and sets the rounding value, whose meaning depends on the rounding option. 
| showPlusSign | bool|Gets and sets a boolean option indicating if formatted numbers contain a plus sign for positive numbers. 
| useSeparator | bool|Gets and sets a boolean option indicating if formatted numbers contain digit grouping symbols. 
| zeroPad | bool|Gets and sets a boolean option indicating if formatted numbers contain padded zeros to the right of the decimal. 


### CIMNumericFormatSuffix 

|Property | Type | Description | 
|---------|--------|--------|
| suffix | string|Gets and sets the numeric suffix. 






## CIMPercentageFormat
#### Represents a percentage format. 


### CIMNumberFormat 

|Property | Type | Description | 
|---------|--------|--------|


### CIMNumericFormat 

|Property | Type | Description | 
|---------|--------|--------|
| alignmentOption | [enumeration esriNumericAlignmentEnum](ExternalReferences.md#enumeration-esrinumericalignmentenum)|Gets and sets the alignment option. 
| alignmentWidth | long|Gets and sets the alignment width. 
| roundingOption | [enumeration esriRoundingOptionEnum](ExternalReferences.md#enumeration-esriroundingoptionenum)|Gets and sets the rounding option. 
| roundingValue | long|Gets and sets the rounding value, whose meaning depends on the rounding option. 
| showPlusSign | bool|Gets and sets a boolean option indicating if formatted numbers contain a plus sign for positive numbers. 
| useSeparator | bool|Gets and sets a boolean option indicating if formatted numbers contain digit grouping symbols. 
| zeroPad | bool|Gets and sets a boolean option indicating if formatted numbers contain padded zeros to the right of the decimal. 


### CIMPercentageFormat 

|Property | Type | Description | 
|---------|--------|--------|
| adjustPercentage | boolean|Gets and sets a boolean indicating whether or not to adjust the percentage. 






## CIMRateFormat
#### Represents a rate format. 


### CIMNumberFormat 

|Property | Type | Description | 
|---------|--------|--------|


### CIMNumericFormat 

|Property | Type | Description | 
|---------|--------|--------|
| alignmentOption | [enumeration esriNumericAlignmentEnum](ExternalReferences.md#enumeration-esrinumericalignmentenum)|Gets and sets the alignment option. 
| alignmentWidth | long|Gets and sets the alignment width. 
| roundingOption | [enumeration esriRoundingOptionEnum](ExternalReferences.md#enumeration-esriroundingoptionenum)|Gets and sets the rounding option. 
| roundingValue | long|Gets and sets the rounding value, whose meaning depends on the rounding option. 
| showPlusSign | bool|Gets and sets a boolean option indicating if formatted numbers contain a plus sign for positive numbers. 
| useSeparator | bool|Gets and sets a boolean option indicating if formatted numbers contain digit grouping symbols. 
| zeroPad | bool|Gets and sets a boolean option indicating if formatted numbers contain padded zeros to the right of the decimal. 


### CIMRateFormat 

|Property | Type | Description | 
|---------|--------|--------|
| factor | double|Gets and sets the rate factor. 
| label | string|Gets and sets the label appended to the formatted rate number. 





### Enumeration: RoundingOption
#### Rounding options 

|Property | Value | Description | 
|---------|--------|--------|
| NumberOfDecimals| 0| Rounding by number of decimals. 
| NumberOfSignificantDigits| 1| Rounding by number of significant digits. 




## CIMScientificNumberFormat
#### Represents scientific number format. 


### CIMNumberFormat 

|Property | Type | Description | 
|---------|--------|--------|


### CIMScientificNumberFormat 

|Property | Type | Description | 
|---------|--------|--------|
| decimalPlaces | long|Gets and sets the number of decimal places to show. 



