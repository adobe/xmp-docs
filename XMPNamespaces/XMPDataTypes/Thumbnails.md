# Thumbnail

A thumbnail image for a file.

- The namespace URI is http://ns.adobe.com/xap/1.0/g/img/

- The preferred namespace prefix is xmpGImg

|Name|Description|Type|
|----|-----------|----|
|xmpGImg:format|The image encoding. Defined value: JPEG.  |Closed choice of [Text](./CoreProperties.md#Text)|
|xmpGImg:height|Height in pixels  |[Integer](./CoreProperties.md#Integer)|
|xmpGImg:width|Width in pixels  |[Integer](./CoreProperties.md#Integer)|
|xmpGImg:image|The full thumbnail image data, converted to base 64 notation(according to section 6.8 of RFC 2045). This is the thumbnail data typically found in a digital image, such as the value of tag 513 in a JPEG stream.  |[Text](./CoreProperties.md#Text)|
