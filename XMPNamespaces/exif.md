# EXIF namespace


EXIF Schema For EXIF-Specific Properties. These properties defined solely by EXIF.

- The namespace URI is http://ns.adobe.com/exif/1.0/

- The preferred namespace prefix is exif

|Name|Description|Type|
|----|-----------|----|
|exif:ApertureValue|EXIF tag 37378, 0x9202. Lens aperture, unit is APEX.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:BrightnessValue|EXIF tag 37379, 0x9203. Brightness, unit is APEX.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:CFAPattern|EXIF tag 41730, 0xA302. Color filter array geometric pattern of the image sense.  |[CFAPattern](./XMPDataTypes/CFAPattern.md)|
|exif:ColorSpace|EXIF tag 40961, 0xA001. Color space information:`1 = sRGB`, `65535 = uncalibrated`  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:CompressedBitsPerPixel|EXIF tag 37122, 0x9102. Compression mode used for a compressed image is indicated in unit bits per pixel.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:Contrast|EXIF tag 41992, 0xA408. Indicates the direction of contrast processing applied by the camera:`0 = Normal`, `1 = Soft`, `2 = Hard` |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:CustomRendered|EXIF tag 41985, 0xA401. Indicates the use of special processing on image data: `0 = Normal process`, `1 = Custom process` |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:DateTimeDigitized|EXIF tag 36868, 0x9004 (primary) and 37522, 0x9292 (subseconds). Date and time when image was stored as digital data, can be the same as DateTimeOriginal if originally stored in digital form. Stored in ISO 8601 format. Includes the EXIF SubSecTimeDigitized data. This value is used in XMP as xmp:CreateDate  |[Date](./XMPDataTypes/CoreProperties.md#Date)|
|exif:DateTimeOriginal|EXIF tags 36867, 0x9003 (primary) and 37521, 0x9291 (subseconds). Date and time when original image was generated, in ISO 8601 format. Includes the EXIF SubSecTimeOriginal data. Note that Exif date-time values have no time zone information.  |[Date](./XMPDataTypes/CoreProperties.md#Date)|
|exif:DeviceSettingDescription|EXIF tag 41995, 0xA40B. Indicates information on the picture-taking conditions of a particular camera model.  |[DeviceSettings](./XMPDataTypes/DeviceSettings.md)|
|exif:DigitalZoomRatio|EXIF tag 41988, 0xA404. Indicates the digital zoom ratio when the image was shot.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:ExifVersion|EXIF tag 36864, 0x9000. EXIF version number.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:ExposureBiasValue|EXIF tag 37380, 0x9204. Exposure bias, unit is APEX.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:ExposureIndex|EXIF tag 41493, 0xA215. Exposure index of input device.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:ExposureMode|EXIF tag 41986, 0xA402. Indicates the exposure mode set when the image was shot : `0 = Auto exposure`, `1 = Manual exposure`, `2 = Auto bracket` |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:ExposureProgram|EXIF tag 34850, 0x8822. Class of program used for exposure: 0 = not defined, `1 = Manual`, `2 = Normal program`, `3 = Aperture priority`, `4 = Shutter priority`, `5 = Creative program`, `6 = Action program`, `7 = Portrait mode`, `8 = Landscape mode` |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:ExposureTime|EXIF tag 33434, 0x829A. Exposure time in seconds.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:FileSource|EXIF tag 41728, 0xA300. Indicates image source: 3(DSC) is the only choice.  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:Flash|EXIF tag 37385, 0x9209. Strobe light (flash) source data.  |[Flash](./XMPDataTypes/Flash.md)|
|exif:FlashEnergy|EXIF tag 41483, 0xA20B. Strobe energy during image capture.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:FlashpixVersion|EXIF tag 40960, 0xA000. Version of FlashPix.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:FNumber|EXIF tag 33437, 0x829D. F number.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:FocalLength|EXIF tag 37386, 0x920A. Focal length of the lens, in millimeters.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:FocalLengthIn35mmFilm|EXIF tag 41989, 0xA405. Indicates the equivalent focal length assuming a 35mm film camera, in mm. A value of 0 means the focal length is unknown. Note that this tag differs from the FocalLength tag.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:FocalPlaneResolutionUnit|EXIF tag 41488, 0xA210. Unit used for FocalPlaneXResolution and FocalPlaneYResolution. `2 = inches`, `3 = centimeters`  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:FocalPlaneXResolution|EXIF tag 41486, 0xA20E. Horizontal focal resolution, measured pixels per unit.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:FocalPlaneYResolution|EXIF tag 41487, 0xA20F. Vertical focal resolution, measured in pixels per unit.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:GainControl|EXIF tag 41991, 0xA407. Indicates the degree of overall image gain adjustment: `0 = None`, `1 = Low gain up`, `2 = High gain up`, `3 = Low gain down`, `4 = High gain down` |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:ImageUniqueID|EXIF tag 42016, 0xA420. An identifier assigned uniquely to each image. It is recorded as a 32 character ASCII string, equivalent to hexadecimal notation and 128-bit fixed length.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:ISOSpeedRatings|EXIF tag 34855, 0x8827. ISO Speed and ISO Latitude of the input device as specified in ISO 12232. A native Exif ISO value of exactly 65535 indicates an ISO value of above 64K, which cannot be stored in the native Exif Tag 34855. The real value should be stored in the XMP  |Ordered array of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:LightSource|EXIF tag 37384, 0x9208. Light source: `0 = unknown`, `1 = Daylight`, `2 = Fluorescent`, `3 = Tungsten`, `4 = Flash`, `9 = Fine weather`, `10 = Cloudy weather`, `11 = Shade`, `12 = Daylight fluorescent (D 5700 – 7100K)`, `13 = Day white fluorescent (N 4600 – 5400K)`, `14 = Cool white fluorescent (W 3900 – 4500K)`, `15 = White fluorescent (WW 3200 – 3700K)`, `17 = Standard light A`, `18 = Standard light B`, `19 = Standard light C`, `20 = D55`, `21 = D65` ,`22 = D75`, `23 = D50`, `24 = ISO studio tungsten`, `255 = other`|Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:MaxApertureValue|EXIF tag 37381, 0x9205. Smallest F number of lens, in APEX.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:MeteringMode|EXIF tag 37383, 0x9207. Metering mode: `0 = unknown`,        `1 = Average`,        `2 = CenterWeightedAverage`,        `3 = Spot`,        `4 = MultiSpot`,        `5 = Pattern`,         `6 = Partial`,        `255 = other`|Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:OECF|EXIF tag 34856, 0x8828. Opto-Electoric Conversion Function as specified in ISO 14524.  |[OECF-SFR](./XMPDataTypes/OECF-SFR.md)|
|exif:PixelXDimension|EXIF tag 40962, 0xA002. Valid image width, in pixels.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:PixelYDimension|EXIF tag 40963, 0xA003. Valid image height, in pixels.  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:RelatedSoundFile|EXIF tag 40964, 0xA004. An 8.3 file name for the related sound file.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:Saturation|EXIF tag 41993, 0xA409. Indicates the direction of saturation processing applied by the camera:        `0 = Normal`,        `1 = Low saturation`,        `2 = High saturation`  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:SceneCaptureType|EXIF tag 41990, 0xA406. Indicates the type of scene that was shot:        `0 = Standard`,        `1 = Landscape`,        `2 = Portrait`,        `3 = Night scene`|Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:SceneType|EXIF tag 41729, 0xA301. Indicates the type of scene: 1(directly photographed image) is the only choice.  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:SensingMethod|EXIF tag 41495, 0xA217. Image sensor type on input device:        `1 = Not defined`,        `2 = One-chip colour area sensor`,        `3 = Two-chip colour area sensor`,        `4 = Three-chip colour area sensor`,      `5 = Colour sequential area sensor`,        `7 = Trilinear sensor`,        `8 = Colour sequential linear sensor`|Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:Sharpness|EXIF tag 41994, 0xA40A. Indicates the direction of sharpness processing applied by the camera:        `0 = Normal`,         `1 = Soft`,        `2 = Hard`|Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:ShutterSpeedValue|EXIF tag 37377, 0x9201. Shutter speed, unit is APEX. See Annex C of the EXIF specification.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:SpatialFrequencyResponse|EXIF tag 41484, 0xA20C. Input device spatial frequency table and SFR values as specified in ISO 12233.  |[OECF-SFR](./XMPDataTypes/OECF-SFR.md)|
|exif:SpectralSensitivity|EXIF tag 34852, 0x8824. Spectral sensitivity of each channel.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:SubjectArea|EXIF tag 37396, 0x9214. The location and area of the main subject in the overall scene.  |Ordered array of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:SubjectDistance|EXIF tag 37382, 0x9206. Distance to subject, in meters.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:SubjectDistanceRange|EXIF tag 41996, 0xA40C. Indicates the distance to the subject:        `0 = Unknown`,        `1 = Macro`,        `2 = Close view`,        `3 = Distant view`  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:SubjectLocation|EXIF tag 41492, 0xA214. Location of the main subject of the scene. The first value is the horizontal pixel and the second value is the vertical pixel at which the main subject appears.  |Ordered array of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:UserComment|EXIF tag 37510, 0x9286. Comments from user.  |[Language Alternative](./XMPDataTypes/CoreProperties.md#LanguageAlternative)|
|exif:WhiteBalance|EXIF tag 41987, 0xA403. Indicates the white balance mode set when the image was shot:        `0 = Auto white balance`,        `1 = Manual white balance`  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:GPSAltitude|GPS tag 6, 0x06. Indicates altitude in meters.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:GPSAltitudeRef|GPS tag 5, 0x5. Indicates whether the altitude is above or below sea level:        `0 = Above sea level`,        `1 = Below sea level`   |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:GPSAreaInformation|GPS tag 28, 0x1C. A character string recording the name of the GPS area.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSDestBearing|GPS tag 24, 0x18. Destination bearing, values from 0 to 359.99.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:GPSDestBearingRef|GPS tag 23, 0x17. Reference for movement direction:        `T = true direction`,        `M = magnetic direction`  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSDestDistance|GPS tag 26, 0x1A. Distance to destination.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:GPSDestDistanceRef|GPS tag 25, 0x19. Units used for speed measurement:        `"K" = kilometers`,        `"M" = miles`,        `"N" = knots`|Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSDestLatitude|GPS tag 20, 0x14 (position) and 19, 0x13 (North/South). Indicates destination latitude.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSDestLongitude|GPS tag 22, 0x16 (position) and 21, 0x15 (East/West). Indicates destination longitude.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSDifferential|GPS tag 30, 0x1E. Indicates whether differential correction is applied to the GPS receiver:  `0 = Without correction`,        `1 = Correction applied`  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:GPSDOP|GPS tag 11, 0x0B. Degree of precision for GPS data.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:GPSImgDirection|GPS tag 17, 0x11. Direction of image when captured, values range from 0 to 359.99.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:GPSImgDirectionRef|GPS tag 16, 0x10. Reference for movement direction:        `"T" = true direction`,        `"M" = magnetic direction`  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSLatitude|GPS tag 2, 0x02 (position) and 1, 0x01 (North/South). Indicates latitude.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSLongitude|GPS tag 4, 0x04 (position) and 3, 0x03 (East/West). Indicates longitude.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSMapDatum|GPS tag 18, 0x12. Geodetic survey data.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSMeasureMode|GPS tag 10, 0x0A. GPS measurement mode, Text type: `"2" = two-dimensional measurement`, `"3" = three-dimensional measurement`.  |Closed Choice of [Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|exif:GPSProcessingMethod|GPS tag 27, 0x1B. A character string recording the name of the method used for location finding.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSSatellites|GPS tag 8, 0x08. Satellite information, format is unspecified.  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSSpeed|GPS tag 13, 0x0D. Speed of GPS receiver movement.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:GPSSpeedRef|GPS tag 12, 0x0C. Units used for speed measurement:        `"K" = kilometers per hour`,        `"M" = miles per hour`,        `"N" = knots`  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSStatus|GPS tag 9, 0x09. Status of GPS receiver at image creation time:        `"A" = measurement in progress`,        `"V" = measurement is interoperability`  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSTimeStamp|GPS tag 29 (date), 0x1D, and, and GPS tag 7 (time), 0x07. Time stamp of GPS data, in Coordinated Universal Time. NOTE: The GPSDateStamp tag is new in EXIF 2.2. The GPS timestamp in EXIF 2.1 does not include a date. If not present, the date component for the XMP should be taken from exif:DateTimeOriginal, or if that is also lacking from exif:DateTimeDigitized. If no date is available, do not write exif:GPSTimeStamp to XMP.  |[Date](./XMPDataTypes/CoreProperties.md#Date)|
|exif:GPSTrack|GPS tag 15, 0x0F. Direction of GPS movement, values range from 0 to 359.99.  |[Rational](./XMPDataTypes/CoreProperties.md#Rational)|
|exif:GPSTrackRef|GPS tag 14, 0x0E. Reference for movement direction:        `"T" = true direction`,        `"M" = magnetic direction`  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#Text)|
|exif:GPSVersionID|GPS tag 0, 0x00. A decimal encoding of each of the four EXIF bytes with period separators. The current value is "2.3.0.0".  |[Text](./XMPDataTypes/CoreProperties.md#Text)|
