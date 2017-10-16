# Marker

A marker type used to describe an important location in an audio or video sequence. It is a value of the xmpDM:markers array in a [Track](Track.md).

- The namespace URI is http://ns.adobe.com/xmp/1.0/DynamicMedia/

- The preferred namespace prefix is xmpDM

|Name|Description|Type|
|----|-----------|----|
|xmpDM:comment|Optional. A descriptive comment  |[Text](./CoreProperties.md#Text)|
|xmpDM:cuePointParams|Optional. An ordered sequence of processing parameters for an FLVCuePoint-type marker  |Ordered array of [CuePointParam](./CuePointParam.md)|
|xmpDM:cuePointType|Optional. The cue-point type for an FLVCuePoint-type marker, one of Navigation or Event  |[Text](./CoreProperties.md#Text)|
|xmpDM:duration|Optional. The duration of the marker.Default is 0. This is a number of ticks/frames in the timescale specified by an optionally included frame rate. If the parent [Track](Track.md) specifies *xmpDM:frameRate*, that becomes the default frame rate for all member markers.If no frame rate is specified in either the marker or the track, this value is a number of seconds (frames at the default frame rate of 1fps).  |[FrameCount](./CoreProperties.md#FrameCount)|
|xmpDM:location|Optional. The URL of the location to jump to, for a WebLink-type marker.For example, http://www.mysite.com.  |[URI](./CoreProperties.md#URI)|
|xmpDM:name|The name of the marker. For timed text, the phrase, word, or syllable.  |[Text](./CoreProperties.md#Text)|
|xmpDM:probability|Optional. For auto-detected speech, the probability that the word is accurate.  |[Real](./CoreProperties.md#Real)|
|xmpDM:speaker|Optional. The name or other identifier of the speaker or performer, for a Speech-type marker. The speaker need only be identified if it changes from the previous phrase.  |[Text](./CoreProperties.md#Text)|
|xmpDM:startTime|The timeline position of the marker.Default is 0, the beginning of the file that contains the track.  |[FrameCount](./CoreProperties.md#FrameCount)|
|xmpDM:target|Optional. A frame target, for a WebLink-type marker  |[Text](./CoreProperties.md#Text)|
|xmpDM:type|A comma-delimited list of marker types. The type indicates how a marker or set of markers is intended to be used, and what other information is associated with it. Predefined value types include:Chapter,Cue,Index,Speech,Track. This type overrides any type specified in the containing [Track](Track.md) |Open Choice of [Text](./CoreProperties.md#Text)|
