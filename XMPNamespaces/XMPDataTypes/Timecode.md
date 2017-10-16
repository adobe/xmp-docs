# Timecode

A timecode value in video.

- The namespace URI is http://ns.adobe.com/xmp/1.0/DynamicMedia/

- The preferred namespace prefix is xmpDM

|Name|Description|Type|
|----|-----------|----|
|xmpDM:timeFormat|The format used in the timeValue. One of:`24Timecode`,`25Timecode`,`2997DropTimecode (semicolon delimiter)`,`2997NonDropTimecode`,`30Timecode,50Timecode`,`5994DropTimecode`,`5994NonDropTimecode`,`60Timecode,23976Timecode`  |Closed Choice of [Text](./CoreProperties.md#Text)|
|xmpDM:timeValue|A time value in the specified format. Time values use a colon delimiter in all formats except 2997drop, which uses a semicolon. The four fields indicate hours, minutes,seconds, and frames: **hh:mm:ss:ff**.The actual duration in seconds depends on the format  |[Text](./CoreProperties.md#Text)|
