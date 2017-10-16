# TIFF namespace

EXIF properties for TIFF-derived data.

- The namespace URI is http://ns.adobe.com/tiff/1.0/

- The preferred namespace prefix is tiff

|Name|Description|Type|
|----|-----------|----|
|tiff:Artist|Camera owner, photographer or image creator. **NOTE**: *This property is stored in XMP as the first item in the dc:creator array.*  |[ProperName](./XMPDataTypes/CoreProperties.md#ProperName)|
|tiff:BitsPerSample|Number of bits per component in each channel.  |Ordered array of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|tiff:Compression|Compression scheme. `1 = Uncompressed` , `6 = JPEG`  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|tiff:Copyright|Copyright information as an ASCII string. **NOTE**: *This property is stored in XMP as dc:rights.*  |[Language Alternative](./XMPDataTypes/CoreProperties.md#LanguageAlternative)|
|tiff:DateTime|Date and time when the file was last modified (no time zone in EXIF), stored in ISO 8601 format, not the original EXIF format. This property includes the value for the EXIF SubSecTime(37520, 0x9290) attribute. **NOTE**: *This property is stored in XMP as xmp:ModifyDate.*  |[Date](./XMPDataTypes/CoreProperties.md#Date)|
|tiff:ImageDescription|The title of the image as an ASCII string. **NOTE**: *This property is stored in XMP as dc:description.*  |[Language Alternative](./XMPDataTypes/CoreProperties.md#LanguageAlternative)|
|tiff:ImageLength|Image height in pixels.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|tiff:ImageWidth|Image width in pixels.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|tiff:Make|Manufacturer of recording equipment as an ASCII string.  |[ProperName](./XMPDataTypes/CoreProperties.md#ProperName)|
|tiff:Model|Model name or number of equipment as an ASCII string.  |[ProperName](./XMPDataTypes/CoreProperties.md#ProperName)|
|tiff:Orientation|Orientation. `1 = 0th row at the top,0th column at left`,        `2 = 0th row at the top,0th column at right`,         `3 = 0th row at the bottom,0th column at right`,         `4 = 0th row at the bottom,0th column at left`,         `5 = 0th row at the left,0th column at top`,         `6 = 0th row at the right,0th column at top`,         `7 = 0th row at the right,0th column at bottom`,        `8 = 0th row at the left,0th column at bottom`   |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|tiff:PhotometricInterpretation|Pixel Composition. `2 = RGB`, `6 = YCbCr`  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|tiff:PlanarConfiguration|Data layout. `1 = chunky`, `2 = planar`  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|tiff:PrimaryChromaticities|Chromaticity of the three primary colors.  |Ordered array of [Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|tiff:ReferenceBlackWhite|Reference black and white point values.  |Ordered array of [Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|tiff:ResolutionUnit|Unit used for XResolution and YResolution. Value is one of `2 = Inches`, `3 = Centimeters`  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|tiff:SamplesPerPixel|Number of components per pixel.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|tiff:Software|Software or firmware used to generate image. **NOTE**: *This property is stored in XMP as xmp:CreatorTool.*  |[AgentName](./XMPDataTypes/CoreProperties.md#AgentName)|
|tiff:TransferFunction|Transfer function for image described in tabular style with 3 * 256 entries.  |Ordered array of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|tiff:WhitePoint|Chromaticity of white point.  |Ordered array of [Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|tiff:XResolution|Horizontal resolution in pixels per unit.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|tiff:YResolution|Vertical resolution in pixels per unit.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|tiff:YCbCrCoefficients|Matrix coefficients for RGB to YCbCr transformation.  |Ordered array of [Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|tiff:YCbCrPositioning|Position of chrominance vs. luminance components. `1 = centered`, `2 = co-sited`  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|tiff:YCbCrSubSampling|Sampling ratio of chrominance components.         `[2,1] = YCbCr4:2:2`,        `[2,2] = YCbCr4:2:0`  |Ordered array of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
