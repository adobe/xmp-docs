# Camera Raw namespace

This namespace specifies settings associated with image files produced in camera raw mode.

- The namespace URI is http://ns.adobe.com/camera-raw-settings/1.0/

- The preferred namespace prefix is crs

|Name|Description|Type|
|----|-----------|----|
|crs:AutoBrightness|When true, Brightness is automatically adjusted.  |[Boolean](./XMPDataTypes/CoreProperties.md#boolean)|
|crs:AutoContrast|When true, Contrast is automatically adjusted.  |[Boolean](./XMPDataTypes/CoreProperties.md#boolean)|
|crs:AutoExposure|When true, Exposure is automatically adjusted.  |[Boolean](./XMPDataTypes/CoreProperties.md#boolean)|
|crs:AutoShadows|When true,Shadows is automatically adjusted.  |[Boolean](./XMPDataTypes/CoreProperties.md#boolean)|
|crs:BlueHue|Blue Hue setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:BlueSaturation|Blue Saturation setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:Brightness|Brightness setting. Range 0 to 150  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:CameraProfile|Camera Profile setting.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|crs:ChromaticAberrationB|Chomatic Aberration, Fix Blue/Yellow Fringe setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:ChromaticAberrationR|Chomatic Aberration, Fix Red/Cyan Fringe setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:ColorNoiseReduction|Color Noise Reducton setting. Range 0 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:Contrast|Contrast setting. Range -50 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:CropTop|When Has Crop is true, top of crop rectangle.  |[Real](./XMPDataTypes/CoreProperties.md#real)|
|crs:CropLeft|When Has Crop is true, left of crop rectangle.  |[Real](./XMPDataTypes/CoreProperties.md#real)|
|crs:CropBottom|When Has Crop is true, bottom of crop rectangle.  |[Real](./XMPDataTypes/CoreProperties.md#real)|
|crs:CropRight|When Has Crop is true, right of crop rectangle.  |[Real](./XMPDataTypes/CoreProperties.md#real)|
|crs:CropAngle|When Has Crop is true, angle of crop rectangle.  |[Real](./XMPDataTypes/CoreProperties.md#real)|
|crs:CropWidth|Width of resulting cropped image in CropUnits units.  |[Real](./XMPDataTypes/CoreProperties.md#real)|
|crs:CropHeight|Height of resulting cropped image in CropUnits units.  |[Real](./XMPDataTypes/CoreProperties.md#real)|
|crs:CropUnits|Units for Crop Width and Crop Height. One of: 0=pixels 1=inches 2=cm.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:Exposure|Exposure setting. Range -4.0 to 4.0.  |[Real](./XMPDataTypes/CoreProperties.md#real)|
|crs:GreenHue|Green Hue setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:GreenSaturation|Green Saturation setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:HasCrop|When true, image has a cropping rectangle.  |[Boolean](./XMPDataTypes/CoreProperties.md#boolean)|
|crs:HasSettings|When true, non-default camera raw settings.  |[Boolean](./XMPDataTypes/CoreProperties.md#boolean)|
|crs:LuminanceSmoothing|Luminance Smoothing setting. Range 0 to 100  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:RawFileName|File name for raw file (not a complete path).  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|crs:RedHue|Red Hue setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:RedSaturation|Red Saturation setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:Saturation|Saturation setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:Shadows|Shadows setting. Range 0 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:ShadowTint|Shadow Tint setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:Sharpness|Sharpness setting. Range 0 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:Temperature|Temperature setting. Range 2000 to 50000.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:Tint|Tint setting. Range -150 to 150.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:ToneCurve|Array of points (Integer, Integer) defining a Tone Curve.  |Ordered array of [Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:ToneCurveName|The name of the Tone Curve described by ToneCurve. One of: `Linear` , `Medium Contrast` , `Strong Contrast` , `Custom` or `a user-defined preset name` |Open Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|crs:Version|Version of Camera Raw plugin.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|crs:VignetteAmount|Vignetting Amount setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:VignetteMidpoint|Vignetting Midpoint setting. Range 0 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|crs:WhiteBalance|White Balance setting. One of: `As Shot` , `Auto` , `Daylight` , `Cloudy` , `Shade` , `Tungsten` ,`Fluorescent` , `Flash` , `Custom` |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
