


## CIMBlackAndWhiteEffect
#### Represents a visual effect for reshading the scene to black and white. 


### CIMVisualEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMBlackAndWhiteEffect 

|Property | Type | Description | 
|---------|--------|--------|






## CIMBloomPostprocessingEffect
#### Represents a post-processing technique that reshades the scene with a glow effect. 


### CIMPostprocessingEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMBloomPostprocessingEffect 

|Property | Type | Description | 
|---------|--------|--------|
| strength | double | The strength of the effect. 
| threshold | double | The color value threshold that determines what is effected by the bloom effect. 






## CIMBlueprintEffect
#### Represents a visual effect for reshading the scene with a blueprint style. 


### CIMVisualEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMBlueprintEffect 

|Property | Type | Description | 
|---------|--------|--------|
| outlineStrength | double | The outline strength which influences the outline weight and the threshold used for edge detection. 
| gridSize | double | The size of the background grid in points. 
| gridSubdivisions | long | The number of width and height subdivisions for each cell in the grid. 






## CIMColorGradingPostprocessingEffect
#### Represents a post-processing technique that reshades the scene with adjusted color and luminance. 


### CIMPostprocessingEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMColorGradingPostprocessingEffect 

|Property | Type | Description | 
|---------|--------|--------|
| saturation | long | The saturation. 
| brightness | long | The brightness. 
| contrast | long | The contrast. 






## CIMCrossMosaicEffect
#### Represents a visual effect for reshading the scene with a cross mosaic texture. 


### CIMVisualEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMCrossMosaicEffect 

|Property | Type | Description | 
|---------|--------|--------|
| size | double | The size of the diamonds measured in points. 






## CIMDepthOfFieldEffect
#### Represents the data for simulating camera depth of field effect in 3D scenes. 


### CIMCameraEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMDepthOfFieldEffect 

|Property | Type | Description | 
|---------|--------|--------|
| focusDistance | double | The camera's focus distance measured in meters. 
| focusDepth | double | The camera's focus depth measured in meters. 
| maxBlur | [enumeration DepthOfFieldMaxBlur](CIMEffects.md#enumeration-depthoffieldmaxblur) | The kernel size indicating the maximum blur radius. 





### Enumeration: DepthOfFieldMaxBlur
#### Represents the kernel sizes for depth of field camera effect. 

|Property | Value | Description | 
|---------|--------|--------|
| Small| 0| Small kernel size 
| Medium| 1| Medium kernel size 
| Large| 2| Large kernel size 
| VeryLarge| 3| Very large kernel size 




## CIMGrainPostprocessingEffect
#### Represents a post-processing technique that reshades the scene with a grain effect. 


### CIMPostprocessingEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMGrainPostprocessingEffect 

|Property | Type | Description | 
|---------|--------|--------|
| strength | double | The strength of the grain. 
| size | double | The size of the grain in points. 






## CIMHalftoneEffect
#### Represents a visual effect for reshading the scene with halftone. 


### CIMVisualEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMHalftoneEffect 

|Property | Type | Description | 
|---------|--------|--------|
| dotSize | double | The maximum size of the halftone dots in points. 
| dotStrength | double | The strength of the halftone dots. 
| invertTone | boolean | A value indicating whether to use white halftone dots. 






## CIMHexMosaicEffect
#### Represents a visual effect for reshading the scene with a hexagonal mosaic texture. 


### CIMVisualEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMHexMosaicEffect 

|Property | Type | Description | 
|---------|--------|--------|
| size | double | The size of the hexagons measured in points. 






## CIMMonochromaticEffect
#### Represents a visual effect for reshading the scene to monochromatic tones. 


### CIMVisualEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMMonochromaticEffect 

|Property | Type | Description | 
|---------|--------|--------|
| color | [Color](Types.md#color) | The color of the effect. 






## CIMOutlineEffect
#### Represents a visual effect for reshading the scene with outlines. 


### CIMVisualEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMOutlineEffect 

|Property | Type | Description | 
|---------|--------|--------|
| outlineStrength | double | The outline strength which influences the outline weight and the threshold used for edge detection. 
| outlineColor | [Color](Types.md#color) | The effect's outline color. 
| backgroundColor | [Color](Types.md#color) | The effect's background color. 






## CIMPencilSketchEffect
#### Represents a visual effect for reshading the scene with a pencil sketch style. 


### CIMVisualEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMPencilSketchEffect 

|Property | Type | Description | 
|---------|--------|--------|
| grayscale | boolean | A value indicating whether to convert scene colors to grayscale. 
| crosshatchStrength | double | The strength of the crosshatching. 
| crosshatchAngleCount | long | The number of crosshatch angles. 






## CIMPixelatedEffect
#### Represents a visual effect for reshading the scene with a pixelated style. 


### CIMVisualEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMPixelatedEffect 

|Property | Type | Description | 
|---------|--------|--------|
| pixelSize | double | The size of the effect's simulated pixels in points. 
| colorFactor | long | The factor that exponentially influences the number of colors used in the color palette. 






## CIMTiltShiftEffect
#### Represents the data for simulating camera tilt-shift effect for creating a miniaturization effect in 3D scenes. 


### CIMCameraEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMTiltShiftEffect 

|Property | Type | Description | 
|---------|--------|--------|
| blurStrength | double | The strength (0-1) of the tilt-shift blur. 
| leftOffset | double | The width of the blurred area starting from the left of the screen measured in points. 
| rightOffset | double | The width of the blurred area starting from the right of the screen measured in points. 
| topOffset | double | The width of the blurred area starting from the top of the screen measured in points. 
| bottomOffset | double | The width of the blurred area starting from the bottom of the screen measured in points. 






## CIMToonEffect
#### Represents a visual effect for reshading the scene with a cartoon style. 


### CIMVisualEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMToonEffect 

|Property | Type | Description | 
|---------|--------|--------|
| lineStrength | double | The line strength which influences the line weight and the threshold used for edge detection. 






## CIMVignettePostprocessingEffect
#### Represents a post-processing technique that reshades the scene with a vignette effect. 


### CIMPostprocessingEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMVignettePostprocessingEffect 

|Property | Type | Description | 
|---------|--------|--------|
| size | double | The percentage of the view effected by the vignette effect. 
| strength | double | The strength of the vignette effect. 






## CIMWatercolorEffect
#### Represents a visual effect for reshading the scene with a watercolor style. 


### CIMVisualEffect 

|Property | Type | Description | 
|---------|--------|--------|
| isActive | boolean | A value indicating whether the effect should be applied to the scene. 


### CIMWatercolorEffect 

|Property | Type | Description | 
|---------|--------|--------|
| marginWidth | double | The width of the margin in percentage (0-1). 
| marginGradient | double | The percentage (0-1) across the margin where the midpoint of the gradient is applied. 
| drawMarginOutlines | boolean | A value indicating whether to draw the outlines in the margin. 
| backgroundColor | [Color](Types.md#color) | The background color. 



