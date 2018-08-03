# XMP Dynamic Media namespace

This namespace specifies properties used by the Adobe dynamic media group.

- The namespace URI is http://ns.adobe.com/xmp/1.0/DynamicMedia/

- The preferred namespace prefix is xmpDM

|Name|Description|Type|
|----|-----------|----|
|xmpDM:absPeakAudioFilePath|The absolute path to the file’s peak audio file. If empty, no peak file exists.  |[URI](./XMPDataTypes/CoreProperties.md#uri)|
|xmpDM:album|The name of the album.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:altTapeName|An alternative tape name, set via the project window or timecode dialog in Premiere. If an alternative name has been set and has not been reverted, that name is displayed.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:altTimecode|A timecode set by the user. When specified, it is used instead of the startTimecode.  |[Timecode](./XMPDataTypes/Timecode.md)|
|xmpDM:artist|The name of the artist or artists.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:audioChannelType|The audio channel type. One of:`Mono`,`Stereo`,`5.1`,`7.1`,`16 Channel`,`Other`|Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:audioCompressor|The audio compression used. For example, MP3.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:audioSampleRate|The audio sample rate. Can be any value, but commonly 32000, 44100, or 48000.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|xmpDM:audioSampleType|The audio sample type. One of:`8Int`,`16Int`,`24Int`,`32Int`,`32Float`,`Compressed`,`Packed`,`Other`|Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:beatSpliceParams|Additional parameters for Beat Splice stretch mode.  |[beatSpliceStretch](./XMPDataTypes/beatSpliceStretch.md)|
|xmpDM:cameraAngle|The orientation of the camera to the subject in a static shot, from a fixed set of industry standard terminology. Predefined values include: `Low Angle` , `Eye Level` , `High Angle` , `Overhead Shot` , `Birds Eye Shot` , `Dutch Angle` , `POV` , `Over the Shoulder` , `Reaction Shot`  |Open Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:cameraLabel|A description of the camera used for a shoot. Can be any string, but is usually simply a number, for example "1", "2", or more explicitly "Camera 1"  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:cameraModel|The make and model of the camera used for a shoot.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:cameraMove|The movement of the camera during the shot, from a fixed set of industry standard terminology. Predefined values include:`Aerial` , `Boom Up` , `Boom Down` , `Crane Up` , `Crane Down` , `Dolly In` , `Dolly Out` , `Pan Left` , `Pan Right` , `Pedestal Up` , `Pedestal Down` , `Tilt Up` , `Tilt Down` , `Tracking` , `Truck Left` , `Truck Right` , `Zoom In` , `Zoom Out`|Open Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:client|The client for the job of which this shot or take is a part.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:comment|A user’s comments.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:composer|The composer’s name.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:contributedMedia|An unordered list of all media used to create this media.  |Unordered array of [Media](./XMPDataTypes/Media.md)|
|xmpDM:director|The director of the scene.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:directorPhotography|The director of photography for the scene.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:duration|The duration of the media file.  |[Time](./XMPDataTypes/Time.md)|
|xmpDM:engineer|The engineer’s name.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:fileDataRate|The file data rate in megabytes per second. For example:"36/10" = 3.6 MB/sec  |[Rational](./XMPDataTypes/CoreProperties.md#rational)|
|xmpDM:genre|The name of the genre.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:good|A checkbox for tracking whether a shot is a keeper.  |[Boolean](./XMPDataTypes/CoreProperties.md#boolean)|
|xmpDM:instrument|The musical instrument.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:introTime|The duration of lead time for queuing music.  |[Time](./XMPDataTypes/Time.md)|
|xmpDM:key|The audio’s musical key. One of:`C`, `C#`, `D`, `D#`, `E`, `F`, `F#`, `G`, `G#`, `A`, `A#`, `B`  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:logComment|User’s log comments.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:loop|When true, the clip can be looped seamlessly.  |[Boolean](./XMPDataTypes/CoreProperties.md#boolean)|
|xmpDM:numberOfBeats|The total number of musical beats in a clip; for example, the beats-per-second times the duration in seconds.  |[Real](./XMPDataTypes/CoreProperties.md#real)|
|xmpDM:markers|An ordered list of markers. See also [xmpDM:Tracks](./XMPDataTypes/Track.md).  |Ordered array of [Marker](./XMPDataTypes/Marker.md)|
|xmpDM:outCue|The time at which to fade out.  |[Time](./XMPDataTypes/Time.md)|
|xmpDM:projectName|The name of the project of which this file is a part.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:projectRef|A reference to the project of which this file is a part.  |[ProjectLink](./XMPDataTypes/ProjectLink.md)|
|xmpDM:pullDown|The sampling phase of film to be converted to video (pull-down). One of:`WSSWW` , `SSWWW` , `SWWWS` , `WWWSS` , `WWSSW` , `WWWSW` , `WWSWW` , `WSWWW` , `SWWWW` , `WWWWS`  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:relativePeakAudioFilePath|The relative path to the file’s peak audio file. If empty, no peak file exists.  |[URI](./XMPDataTypes/CoreProperties.md#uri)|
|xmpDM:relativeTimestamp|The start time of the media inside the audio project.  |[Time](./XMPDataTypes/Time.md)|
|xmpDM:releaseDate|The date the title was released.  |[Date](./XMPDataTypes/CoreProperties.md#date)|
|xmpDM:resampleParams|Additional parameters for Resample stretch mode.  |[resampleStretch](./XMPDataTypes/resampleStretch.md)|
|xmpDM:scaleType|The musical scale used in the music. One of: `Major`, `Minor`, `Both`, `Neither`. Neither is most often used for instruments with no associated scale, such as drums.  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:scene|The name of the scene.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:shotDate|The date and time when the video was shot.  |[Date](./XMPDataTypes/CoreProperties.md#date)|
|xmpDM:shotDay|The day in a multiday shoot. For example: Day 2, Friday.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:shotLocation|The name of the location where the video was shot. For example: "Oktoberfest, Munich Germany". For more accurate positioning, use the Exif GPS values.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:shotName|The name of the shot or take.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:shotNumber|The position of the shot in a script or production, relative to other shots. For example: 1, 2, 1a, 1b, 1.1, 1.2.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:shotSize|The size or scale of the shot framing, from a fixed set of industry standard terminology. Predefined values include:`ECU --extreme close-up ` , `MCU -- medium close-up ` , `CU -- close-up ` , `MS -- medium shot ` , `WS -- wide shot ` , `MWS -- medium wide shot ` , `EWS -- extreme wide shot`  |Open Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:speakerPlacement|A description of the speaker angles from centre front in degrees. For example: “Left = -30, Right = 30, Centre = 0, LFE = 45, Left Surround = -110, Right Surround = 110”  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:startTimecode|The timecode of the first frame of video in the file, as obtained from the device control.  |[Timecode](./XMPDataTypes/Timecode.md)|
|xmpDM:stretchMode|The audio stretch mode. One of:`Fixed length, ` , `Time-Scale ` , `Resample ` , `Beat Splice  ` , `Hybrid`  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:takeNumber|A numeric value indicating the absolute number of a take.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|xmpDM:tapeName|The name of the tape from which the clip was captured, as set during the capture process.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:tempo|The audio’s tempo.  |[Real](./XMPDataTypes/CoreProperties.md#real)|
|xmpDM:timeScaleParams|Additional parameters for Time-Scale stretch mode.  |[timeScaleStretch](./XMPDataTypes/timeScaleStretch.md)|
|xmpDM:timeSignature|The time signature of the music. One of:`2/4`, `3/4`, `4/4`, `5/4`, `7/4`, `6/8`, `9/8`, `12/8`, `other`  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:trackNumber|A numeric value indicating the order of the audio file within its original recording.  |[Integer](./XMPDataTypes/CoreProperties.md#integer)|
|xmpDM:Tracks|An unordered list of tracks. A track is a named set of markers, which can specify a frame rate for all markers in the set.See also [xmpDM:markers](./XMPDataTypes/Marker.md).  |Unordered array of [Track](./XMPDataTypes/Track.md)|
|xmpDM:videoAlphaMode|The alpha mode. One of: straight, pre-multiplied , or none  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:videoAlphaPremultipleColor|A colour in CMYK or RGB to be used as the premultiple colour when alpha mode is premultiplied.  |[Colorants](./XMPDataTypes/Colorants.md)|
|xmpDM:videoAlphaUnityIsTransparent|When true, unity is clear, when false, it is opaque.  |[Boolean](./XMPDataTypes/CoreProperties.md#boolean)|
|xmpDM:videoColorSpace|The colour space. One of:`sRGB (used by Photoshop)`, `CCIR-601 (used for NTSC)`, `CCIR-709 (used for HD)`  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:videoCompressor|Video compression used. For example, jpeg.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:videoFieldOrder|The field order for video. One of:`Upper`, `Lower`, `Progressive`  |Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:videoFrameRate|The video frame rate. Predefined values include:`24`, `NTSC`, `PAL`  |Open Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:videoFrameSize|The frame size. For example: w:720, h: 480, unit:pixels  |[Dimensions](./XMPDataTypes/Dimensions.md)|
|xmpDM:videoPixelAspectRatio|The aspect ratio, expressed as wd/ht. For example: “648/720” = 0.9  |[Rational](./XMPDataTypes/CoreProperties.md#rational)|
|xmpDM:videoPixelDepth|The size in bits of each colour component of a pixel. Standard Windows 32-bit pixels have 8 bits per component. One of:`8Int`, `16Int`, `24Int`, `32Int`, `32Float`, `Other`|Closed Choice of [Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:partOfCompilation|Part of compilation.|[Boolean](./XMPDataTypes/CoreProperties.md#boolean)|
|xmpDM:lyrics|Lyrics text. No association with timecode.|[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpDM:discNumber|If in a multi-disc set, might contain total number of discs. For example: 2/3.|[Text](./XMPDataTypes/CoreProperties.md#text)|
