


## CIMCMYKColor
Represents a color in the CMYK color model. A color in the CMYK (cyan, magenta, yellow, black) color model. CMYK is a subtractive color model commonly used in color printing.


### CIMColor

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.
| values | [number], //[double],|The values for the color and alpha channels as defined by the color model. Alpha is the last value in the array for all colors.


### CIMCMYKColor

|Property | Type | Description |
|---------|--------|--------|





### Enumeration: ColorSpaceType
Specifies color spaces used for colors.

|Property | Value | Description |
|---------|--------|--------|
| RGB| 1| The RGB (red, green, blue) color space.
| CMYK| 2| The CMYK (cyan, magenta, yellow, black) color space.
| Gray| 3| The Grayscale color space.
| HSV| 4| The HSV (hue, saturation, value (brightness)) color space.
| HLS| 5| The HSL (hue, saturation, lightness) color space.
| XYZ| 7| The XYZ color space.
| LAB| 8| The LAB color space.
| Spot| 9| Spot color space.




## CIMFixedColorRamp
Represents a color scheme composed of discrete colors A color scheme composed of an ordered list of discrete colors.


### CIMColorRamp

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.


### CIMFixedColorRamp

|Property | Type | Description |
|---------|--------|--------|
| colors | [CIMColor](Types.md#cimcolor) |The ordered list of colors in the color scheme.






## CIMGrayColor
Represents a grayscale color defined by lightness A color in a grayscale model, where the value of lightness is defined.


### CIMColor

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.
| values | [number], //[double],|The values for the color and alpha channels as defined by the color model. Alpha is the last value in the array for all colors.


### CIMGrayColor

|Property | Type | Description |
|---------|--------|--------|






## CIMHSLColor
Represents a color defined by hue, saturation, and lightness. Transforms RGB values by defining the hue, saturation, and lightness of the color. The three values do not represent individual color channels but the HSL coordinates used to define the color in the RGB color model.


### CIMColor

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.
| values | [number], //[double],|The values for the color and alpha channels as defined by the color model. Alpha is the last value in the array for all colors.


### CIMHSLColor

|Property | Type | Description |
|---------|--------|--------|






## CIMHSVColor
Represents a color defined by hue, saturation, and brightness (value). Transforms RGB values by defining the hue, saturation, and brightness (value) of the color. The three values do not represent individual color channels but the HSV coordinates used to define the color in the RGB color model.


### CIMColor

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.
| values | [number], //[double],|The values for the color and alpha channels as defined by the color model. Alpha is the last value in the array for all colors.


### CIMHSVColor

|Property | Type | Description |
|---------|--------|--------|






## CIMICCColorSpace
Represents a color space defined by an International Color Consortium (ICC) color profile. A color space defined by an International Color Consortium (ICC) color profile.


### CIMColorSpace

|Property | Type | Description |
|---------|--------|--------|


### CIMICCColorSpace

|Property | Type | Description |
|---------|--------|--------|
| URL | string|The URL of short name of the color space definition. As a shortcut, the following strings can be set instead of full URLs: "Default RGB", "Default CMYK", "CIELAB", "CIEXYZ", and "Default Gray".






## CIMLABColor
Represents a color defined in the LAB color space. Defines colors in the CIELAB color space, which is a color-opponent space with dimension L for lightness and a and b for the color-opponent dimensions.


### CIMColor

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.
| values | [number], //[double],|The values for the color and alpha channels as defined by the color model. Alpha is the last value in the array for all colors.


### CIMLABColor

|Property | Type | Description |
|---------|--------|--------|






## CIMLinearContinuousColorRamp
Represents a linear continuous color ramp scheme. A color ramp color scheme that has a linear transition between two colors. This ramp is created using the CIELAB algorithm which blends two colors without traversing the intervening hue space.


### CIMColorRamp

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.


### CIMContinuousColorRamp

|Property | Type | Description |
|---------|--------|--------|
| fromColor | [Color](Types.md#color)|The beginning color for the color ramp (also known as a color scheme).
| toColor | [Color](Types.md#color)|The ending color for the color ramp (also known as a color scheme). This is the color that the scheme transitions to.
| primitiveName | string|The primitive name.


### CIMLinearContinuousColorRamp

|Property | Type | Description |
|---------|--------|--------|






## CIMMultipartColorRamp
Represents a multipart color ramp scheme A color ramp scheme defined by combining two or more continuous, discrete, or random ramps.


### CIMColorRamp

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.


### CIMMultipartColorRamp

|Property | Type | Description |
|---------|--------|--------|
| colorRamps | [CIMColorRamp](Types.md#cimcolorramp) |The ordered list of color ramps (also known as schemes) that are combined to build the multipart ramp. Typically these are continuous color ramps.
| weights | [number], //[double],|The proportional weight for each color ramp (also known as a color scheme) that make up the multipart ramp. This allows for ramp to ramp transition at specific weight points.






## CIMPolarContinuousColorRamp
Represents a polar continuous color ramp scheme. A color ramp scheme that has a polar transition between two colors. This scheme uses the HSV algorithm which uses a path around the color wheel to transition the hue, saturation, and value of the beginning color to the hue, saturation, and value of the ending color.


### CIMColorRamp

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.


### CIMContinuousColorRamp

|Property | Type | Description |
|---------|--------|--------|
| fromColor | [Color](Types.md#color)|The beginning color for the color ramp (also known as a color scheme).
| toColor | [Color](Types.md#color)|The ending color for the color ramp (also known as a color scheme). This is the color that the scheme transitions to.
| primitiveName | string|The primitive name.


### CIMPolarContinuousColorRamp

|Property | Type | Description |
|---------|--------|--------|
| interpolationSpace | [enumeration ColorSpaceType](CIMColor.md#enumeration-colorspacetype)|The colorspace in which the polar interpolation occurs. HSV, HLS, and LAB are the only supported color space types.
| polarDirection | [enumeration PolarDirection](CIMColor.md#enumeration-polardirection)|The direction of the polar progression for the path from the beginning hue to the ending hue.





### Enumeration: PolarDirection
Specifies the direction of the polar progression for the path from the beginning hue to the ending hue.

|Property | Value | Description |
|---------|--------|--------|
| Auto| 0| The shortest path, clockwise or counter clockwise.
| Clockwise| 1| The spectral order from red through orange, yellow, green, and blue to violet.
| Counterclockwise| 2| The reverse spectral order from violet, through blue, green, yellow, and orange to red.




## CIMRGBColor
Represents a color in the RGB color model. A color in the RGB (red, green, blue) color model. RGB is an additive, or light-emissive model based on red, green, and blue values.


### CIMColor

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.
| values | [number], //[double],|The values for the color and alpha channels as defined by the color model. Alpha is the last value in the array for all colors.


### CIMRGBColor

|Property | Type | Description |
|---------|--------|--------|






## CIMRandomHSVColorRamp
Represents a random HSV color ramp scheme A color ramp scheme where the colors are randomly selected within the set range of hue, saturation, and value values.


### CIMColorRamp

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.


### CIMRandomHSVColorRamp

|Property | Type | Description |
|---------|--------|--------|
| minH | number //float|The hue from which the color ramp (also known as a color scheme) will start. Values can range from 0-360.
| maxH | number //float|The hue at which the color ramp (also known as a color scheme) will end. Values can range from 0-360.
| minS | number //float|The minimum saturation possible for the colors within the color ramp (also known as a color scheme). Values can range between 0-100.
| maxS | number //float|The maximum saturation possible for the colors within the color ramp (also known as a color scheme). Values can range between 0-100.
| minV | number //float|The minimum value possible for the colors within the ramp (also known as a scheme). Values can range between 0-100.
| maxV | number //float|The maximum value possible for the colors within the color ramp (also known as a color scheme). Values can range between 0-100.
| minAlpha | number //float|The minimum alpha or transparency for all of the colors. Can be a value between 0-100, where 0 is fully transparent.
| maxAlpha | number //float|The maximum alpha or transparency for all of the colors. Can be a value between 0-100, where 0 is fully transparent.
| seed | number //int32|The starting point for the random generation of the colors.






## CIMSpotColor
Represents a spot color. A color defined by a specific ink standard and typically used in offset printing where the color corresponds to a pure or premixed ink. When a spot color is displayed on the screen the alternative color is used


### CIMColor

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.
| values | [number], //[double],|The values for the color and alpha channels as defined by the color model. Alpha is the last value in the array for all colors.


### CIMSpotColor

|Property | Type | Description |
|---------|--------|--------|
| name | string|The spot color name.






## CIMSpotColorSpace
Represents a color space for spot colors. A color space defined for spot colors including alternate and book colors.


### CIMColorSpace

|Property | Type | Description |
|---------|--------|--------|


### CIMSpotColorSpace

|Property | Type | Description |
|---------|--------|--------|
| description | string|A description of the ink. This can provide more information than the name.
| name | string|The defined ink name for the spot color. Usually this is a well-known color standard name.
| alternativeColor | [Color](Types.md#color)|The standard (non-spot) color that is used to display the color on-screen.
| bookColor | [Color](Types.md#color)|The if present, the color used during output.






## CIMXYZColor
Represents a color in the XYZ color model. A color in the XYZ color space which is based on direct measurements of the human eye.


### CIMColor

|Property | Type | Description |
|---------|--------|--------|
| colorSpace | [ColorSpace](Types.md#colorspace)|The color spaced used defined by an ICC color profile.
| values | [number], //[double],|The values for the color and alpha channels as defined by the color model. Alpha is the last value in the array for all colors.


### CIMXYZColor

|Property | Type | Description |
|---------|--------|--------|
