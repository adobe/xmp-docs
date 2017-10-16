# Flash

A structure describing the flash state.

- The namespace URI is http://ns.adobe.com/exif/1.0/

- The preferred namespace prefix is exif

|Name|Description|Type|
|----|-----------|----|
|exif:Fired|True if flash fired  |[Boolean](./CoreProperties.md#Boolean)|
|exif:Function|True if flash function is not present  |[Boolean](./CoreProperties.md#Boolean)|
|exif:Mode|The flash mode. One of: `0 = unknown`, `1 = compulsory flash firing`, `2 = compulsory flash suppression`, `3 = auto mode`  |Closed Choice of [Integer](./CoreProperties.md#Integer)|
|exif:RedEyeMode|True if red-eye reduction is supported  |[Boolean](./CoreProperties.md#Boolean)|
|exif:Return|Whether strobe return is supported and if supported, detected. One of: `0 = no strobe return detection`, `2 = strobe return light not detected`, `3 = strobe return light detected`  |Closed Choice of [Integer](./CoreProperties.md#Integer)|
