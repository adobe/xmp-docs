# Camera Raw namespace

This namespace specifies settings associated with image files produced in camera raw mode.

- The namespace URI is http://ns.adobe.com/camera-raw-settings/1.0/

- The preferred namespace prefix is crs

|Name|Description|Type|
|----|-----------|----|
|crs:AutoBrightness|When true, Brightness is automatically adjusted.  |[Boolean](./XMPDataTypes/CoreProperties.md#Boolean)|
|crs:AutoContrast|When true, Contrast is automatically adjusted.  |[Boolean](./XMPDataTypes/CoreProperties.md#Boolean)|
|crs:AutoExposure|When true, Exposure is automatically adjusted.  |[Boolean](./XMPDataTypes/CoreProperties.md#Boolean)|
|crs:AutoShadows|When true,Shadows is automatically adjusted.  |[Boolean](./XMPDataTypes/CoreProperties.md#Boolean)|
|crs:BlueHue|Blue Hue setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:BlueSaturation|Blue Saturation setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:Brightness|Brightness setting. Range 0 to 150  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:CameraProfile|Camera Profile setting.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|crs:ChromaticAberrationB|Chomatic Aberration, Fix Blue/Yellow Fringe setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:ChromaticAberrationR|Chomatic Aberration, Fix Red/Cyan Fringe setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:ColorNoiseReduction|Color Noise Reducton setting. Range 0 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:Contrast|Contrast setting. Range -50 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:CropTop|When Has Crop is true, top of crop rectangle.  |[Real](./XMPDataTypes/CoreProperties.md#Real)|
|crs:CropLeft|When Has Crop is true, left of crop rectangle.  |[Real](./XMPDataTypes/CoreProperties.md#Real)|
|crs:CropBottom|When Has Crop is true, bottom of crop rectangle.  |[Real](./XMPDataTypes/CoreProperties.md#Real)|
|crs:CropRight|When Has Crop is true, right of crop rectangle.  |[Real](./XMPDataTypes/CoreProperties.md#Real)|
|crs:CropAngle|When Has Crop is true, angle of crop rectangle.  |[Real](./XMPDataTypes/CoreProperties.md#Real)|
|crs:CropWidth|Width of resulting cropped image in CropUnits units.  |[Real](./XMPDataTypes/CoreProperties.md#Real)|
|crs:CropHeight|Height of resulting cropped image in CropUnits units.  |[Real](./XMPDataTypes/CoreProperties.md#Real)|
|crs:CropUnits|Units for Crop Width and Crop Height. One of: 0=pixels 1=inches 2=cm.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:Exposure|Exposure setting. Range -4.0 to 4.0.  |[Real](./XMPDataTypes/CoreProperties.md#Real)|
|crs:GreenHue|Green Hue setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:GreenSaturation|Green Saturation setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:HasCrop|When true, image has a cropping rectangle.  |[Boolean](./XMPDataTypes/CoreProperties.md#Boolean)|
|crs:HasSettings|When true, non-default camera raw settings.  |[Boolean](./XMPDataTypes/CoreProperties.md#Boolean)|
|crs:LuminanceSmoothing|Luminance Smoothing setting. Range 0 to 100  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:RawFileName|File name for raw file (not a complete path).  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|crs:RedHue|Red Hue setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:RedSaturation|Red Saturation setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:Saturation|Saturation setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:Shadows|Shadows setting. Range 0 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:ShadowTint|Shadow Tint setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:Sharpness|Sharpness setting. Range 0 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:Temperature|Temperature setting. Range 2000 to 50000.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:Tint|Tint setting. Range -150 to 150.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:ToneCurve|Array of points (Integer, Integer) defining a Tone Curve.  |Ordered array of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:ToneCurveName|The name of the Tone Curve described by ToneCurve. One of: `Linear` , `Medium Contrast` , `Strong Contrast` , `Custom` or `a user-defined preset name` |Open Choice of [Text](./XMPDataTypes/CoreProperties.md#Text)|
|crs:Version|Version of Camera Raw plugin.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|crs:VignetteAmount|Vignetting Amount setting. Range -100 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:VignetteMidpoint|Vignetting Midpoint setting. Range 0 to 100.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|crs:WhiteBalance|White Balance setting. One of: `As Shot` , `Auto` , `Daylight` , `Cloudy` , `Shade` , `Tungsten` ,`Fluorescent` , `Flash` , `Custom` |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#Text)|
