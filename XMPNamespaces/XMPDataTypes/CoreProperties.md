# XMP data types

This page defines a collection of XMP data types that are used to represent values of XMP properties

## Basic types

1.  ### Boolean

    Boolean values shall be "**True**" or "**False**".

2.  ### Date

    A date-time value is represented using a subset of the formats as defined in Date and Time Formats:  

    _YYYY_  
    _YYYY-MM_  
    _YYYY-MM-DD_  
    _YYYY-MM-DDThh:mmTZD_  
    _YYYY-MM-DDThh:mm:ssTZD_  
    _YYYY-MM-DDThh:mm:ss.sTZD_  

    In which:  
    • **YYYY** = four-digit year  
    • **MM** = two-digit month (01=January)  
    • **DD** = two-digit day of month (01 to 31)  
    • **hh** = two digits of hour (00 to 23)  
    • **mm** = two digits of minute (00 to 59)  
    • **ss** = two digits of second (00 to 59)  
    • **s** = one or more digits representing a decimal fraction of a second  
    • **TZD** = time zone designator (Z or +hh:mm or -hh:mm  

    The time zone designator need not be present in XMP. When not present, the time zone is unknown, and an XMP processor should not assume anything about the missing time zone.  

    Local time-zone designators +hh:mm or -hh:mm should be used when possible instead of converting to UTC.  

    __NOTE__ : If a file was saved at noon on October 23, a timestamp of 2004-10-23T12:00:00-06:00 conveys more information than 2004-10-23T18:00:00Z.

3.  ### Integer

    A signed or unsigned numeric string used as an integer number representation. The string consists of an arbitrary-length decimal numeric string with an optional leading “+” or “–” sign.

4.  ### Real

    A simple text value denoting a floating-point numeric value, written using decimal notation of an optional sign followed by an integer part and a fraction part. Either the integer part or the fraction part, but not both, may be omitted. The sign, if present, is "+" (U+002B) or "-" (U+002D). The integer part, if present, is a sequence of one or more decimal digits (U+0030 to U+0039). The fraction, if present, is a decimal point (".", U+002E) followed by a sequence of one or more decimal digits.  

    The precise range and precision for the general type are not specified by this document. If converted to a binary value, an XMP processor shall support at least the 32-bit IEEE 754 range and precision, and it should support at least the 64-bit IEEE 754 range and precision. A particular use of the Real type may specify a required range or precision, such as nonnegative or microsecond resolution (for a duration in seconds).

5.  ### Text

    A possibly empty Unicode string.

## Derived types

1.  ### Agent Name

    The name of an XMP processor, a _Text_ value. It is recommended that the value use this format convention:It is recommended that the value use this format convention:  

    _Organization Software_name Version (token;token;...)_

    *   Organization: The name of the company or organization providing the software, no SPACEs.
    *   Software_name: The full name of the software, SPACEs allowed.
    *   version: The version of the software, no SPACEs.
    *   tokens: Can be used to identify an operating system, plug-in, or more detailed version information.  

        **EXAMPLE**: _"Adobe Acrobat 9.0 (Mac OS X 10.5)"_

2.  ### Choice

    A value chosen from a vocabulary of values. Vocabularies provide a means of specifying a limited and possibly extensible set of values for a property.  

    A choice can be open or closed:

    *   An open choice has one or more lists of preferred values, but other values can be used freely.
    *   A closed choice has one or more lists of allowed values, other values shall not be used.  
    __NOTE__ An XMP reader would be more robust if it tolerated unexpected values for closed choice types when the set of allowed values can be expected to grow over time.
    
3.  ### GUID

    A string representing a “globally unique identifier”. A GUID shall be a normal (non-URI) simple value, even though it might appear similar to a URI string. This document does not require any particular methodology for creating a GUID, nor does it require any specific means of formatting the GUID as a simple XMP value. The only valid operations on GUIDs are to create them, to assign one to another, and to compare two of them for equality. This comparison shall use the Unicode string value as-is, using a direct byte-for-byte check for equality.

4.  ### Language Alternative

    An alternative array of simple text items. Language alternatives facilitate the selection of a simple text item based on a desired language. Each array item shall have an xml:lang qualifier. Each xml:lang value shall be unique among the items. As defined in IETF RFC 3066, the xml:lang value is composed of one or more parts: a primary language subtag and a (possibly empty) series of subsequent subtags. The same primary subtag may be used alone and in conjunction with one or more lower-level subtags. A default value, if known, should be the first array item. The order of other array items is not specified by this document.  

    An xml:lang value of "x-default" may be used to explicitly denote a default item. If used, the "x-default" item shall be first in the array and its simple text value should be repeated in another item in which xml:lang specifies its actual language. However, an "x-default" item may be the only item, in which case there is only a default value in no defined language.

5.  ### Locale

    A simple text value denoting a language code as defined in IETF RFC 3066.

6.  ### MIMEType

    A simple text value denoting a digital file format as defined in IETF RFC 2046.

7.  ### ProperName

    A simple text value denoting the name of a person or organization.

8.  ### RenditionClass

    A simple text Open Choice value denoting the form or intended usage of a resource. A series of colonseparated (":", U+003A) tokens and parameters, the first of which names the basic usage of the rendition. Additional tokens need not be present; they provide specific characteristics of the rendition.  

    Defined values for rendition tokens

    |Token    |Defined value                                                                                                                                                                                             |
    |---------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    |default  |The master resource; no additional tokens allowed.                                                                                                                                                        |
    |draft    |A review rendition.                                                                                                                                                                                       |
    |low-res  |A low-resolution, full-size stand-in.                                                                                                                                                                     |
    |proof    |A review proof.                                                                                                                                                                                           |
    |screen   |Screen resolution or Web rendition.                                                                                                                                                                       |
    |thumbnail|A simplified or reduced preview. Additional tokens can provide characteristics. The recommended order is: thumbnail:format:size:colorspace. EXAMPLE thumbnail:jpeg, thumbnail:16x16, thumbnail:gif:8x8:bw.|


9.  ### URI

    Text denoting an Internet Uniform Resource Identifier as defined in IETF RFC 3986.

1.  #### ResourceRef

    A structure denoting a multiple-component reference to a resource. The field values are taken from various properties in the referenced resource.  

    *   The field namespace URI shall be "http://ns.adobe.com/xap/1.0/sType/ResourceRef#".
    *   The preferred field namespace prefix is stRef.  
    Following table lists the fields available in ResourceRef. Fields need not be present. The fields, if used, shall be of the specified types. The field content should be as described. 8.2.2.10 URI  

    ResourceRef fields

    |Name|Type|Field content|
    |----|----|-------------|
    |stRef:documentID|GUID|The value of the xmpMM:DocumentID property from the referenced resource.|
    |stRef:filePath|URI|The referenced resource’s file path or URL.|
    |stRef:instanceID|GUID|The value of the xmpMM:InstanceID property from the referenced resource. 
    __NOTE__ The difference in capitalization between stRef:documentID and xmpMM:DocumentID is real, the result of historical accident. This is also true of the other ResourceRef fields.|
    |stRef:renditionClass|RenditionClass|The value of the xmpMM:RenditionClass property from the referenced resource.|
    |stRef:renditionParam|Text|The value of the xmpMM:RenditionParams property from the referenced resource.|    

2.  #### URL

    Text denoting an Internet Uniform Resource Locator as defined in URIs, URLs, and URNs: Clarifications and Recommendations.

3.  #### Rational

    To represent Exif rational values in XMP, they must be converted to text. The recommended approach is to use a value of type Text of the form numerator /denominator. For example, the value 2/3 becomes the text value "2/3" when converted to XMP.

4.  #### FrameRate

    A frame-rate value can be part of the FrameCount specification of a Marker. For Markers within a Track, however, the frame count can     be a simple integer, and the associated frame rate is specified separately, in the xmpDM:frameRate of the Track.

    A frame rate is expressed as a number of frames divided by a number of seconds (f/s). The number of seconds is called the rate           basis; it defaults to 1, for the common frames-per-second (fps) expression. If no frame rate is specified in either the frame count     itself or in the associated track, the frame count is also the number of seconds, at the default rate of 1 fps.  
    The string value is in one of these formats:
    
    |Name|Field content|
    |----|-------------|
    |"f###"|The frame rate in frames-per-second (fps). The rate basis is assumed to be 1. For example, a frame rate of 24fps is specified as “f24”.|
    |"f###s###"|Specifies a frame rate with a rate basis. The second number is the rate basis, a number of seconds. For example, the         NTSC 29.97 frame rate is specified as “f30000s1001”|
    
5.  #### FrameCount
    
    A number of frames at a given frame rate, which specifies an audio or video time value for a Marker (as the value of *xmpDM:duration or xmpDM:startTime*). Can also be used in the time portion of a document Part.
    
    The frame-count value can include the frame rate as shown. For a Marker within a Track, the frame rate can be specified separately in the *xmpDM:frameRate* of the Track.
    
    The string value is in one of these formats:
    
    |Name|Field content|
    |----|-------------|
    |"##"|For a Marker that is not in a Track, a simple integer value is interpreted as a number of seconds, at the default frame rate of 1 fps. For Markers within a Track, an integer value is interpreted as ticks/frames in the timescale specified by the track’s xmpDM:frameRate. When the count is zero, no frame rate should be specified.|
    |"##f###" or "##f###s###"|A number of frames specified together with a FrameRate, which can contain an optional rate basis. The rate basis defaults to 1. These examples show how a FrameCount value of 15 is expressed for common video and audio frame rates: Film at 24 fps (frame rate = 24, rate basis = 1): "15f24", Speech-to-text in milliseconds (frame rate = 1000, rate basis = 1): "15f1000", NTSC at 29.97 fps (frame rate = 30000, rate basis = 1001): "15f30000s1001", DVATicks (frame rate = 254016000000, rate basis = 1): "15f254016000000"|
    |"maximum"|Allowed for a duration value; indicates that the time span is unlimited, or is determined automatically up to the full duration of the source.|

6.  #### Part

    A Unicode string that identifies a portion of a resource. This is typically a general or logical portion, rather than a specific physical portion. For example, the metadata or the content, or the audio portion of a movie or the video portion.
    
    Part names are a hierarchy of arbitrary depth, specified using path syntax where levels in the hierarchy shall be indicated by a slash ("/", U+002F). The slash shall not be used for any other purpose in these strings. The leftmost character shall be a slash. A path may be just a slash, indicating any or all parts.
    
    All paths implicitly encompass further descendants. For example, "/content" includes all content, whereas "/content/audio" includes all audio but excludes other content such as "/content/video". The collection of part components is open. Additional levels of subparts or alternatives for existing levels may be used; for example, "/content/audio/channels/left" or "/content/audio/FFTaudio/high". When such subparts are used, each subpart name shall be unique and signify a component that is disjoint from any of its siblings.
    
    A part component name shall follow a restricted syntax of an XML Name as defined in Extensible Markup Language. At most one colon (":" U+003A) shall be used, and a colon shall not be the first character. Of the XML Name characters below U+0080, only "A" through "Z", "a" through "z", "0" through "9", and colon may be used. Other XML Name characters below U+0080 are reserved for future use. XMP readers should tolerate reserved characters, and should ignore the remainder of a path from the leftmost component containing a reserved character.

    |Part specification|Part that changed or is referenced|
    |------------------|----------------------------------|
    |/|Any (specific part unknown) or all (all parts of the content and metadata).|
    |/metadata |Portions of the metadata.|
    |/content|Any or all of the content (non-metadata).|
    |/content/audio|Any or all sound.|
    |/content/visual|Some image data (video or still).|
    |/content/visual/video|Video or animation.|
    |/content/visual/raster|Static raster image.|
    |/content/visual/vector|Static vector image.|
    |/content/visual/form/data|Form field data.|
    |/content/visual/form/template|Form template.|
    |/content/visual/annots|Applied annotations (comments).|
    |[/]time:##, [/]time:##d##, [/]time:##r##|A time, duration, or time range specifier. May be standalone (meaning all parts starting at the time or within the range specified) or may be added to any of the listed specifications. **##**: The start time, a frame count, **##d##**: Duration (start time and duration time) , **##r##**: Range (start time and end time). Each ## value is a FrameCount specifier, which can include an optional frame rate. The default frame rate is 1fps. The default duration is "maximum", the entire length of the asset.In a fromPart or toPart value, the leading / is optional. For an stEvt:changed part descriptor in a history record, the leading / is required. For a fromPart value, the start time is an offset from the start of the current ingredient’s file. For a toPart value, the start time is measured from the start of the destination file. If time values are not specifically given, the default start time is 0, meaning the beginning of the relevant file.|
