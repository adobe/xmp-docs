# Media

A reference to a media asset. This is typically a local file, but can be anything that can be specified with a URL. Contains information about usage in the parent media (typically a sequence), and the associated media rights.

- The namespace URI is http://ns.adobe.com/xmp/1.0/DynamicMedia/

- The preferred namespace prefix is xmpDM

|Name|Description|Type|
|----|-----------|----|
|xmpDM:duration|The duration of the asset in the timeline  |[Time](./Time.md)|
|xmpDM:managed|When true, this is a rights-managed resource  |[Boolean](./CoreProperties.md#Boolean)|
|xmpDM:path|The location of the asset  |[URI](./CoreProperties.md#URI)|
|xmpDM:startTime|The timeline position of the start of the asset, an offset from the beginning of the file that contains the track  |[Time](./Time.md)|
|xmpDM:track|An identifier for the track that contained this asset. Could be a track name or a number.  |[Text](./CoreProperties.md#Text)|
|xmpDM:webStatement|The location of a web page describing the owner and/or rights statement for this resource  |[URI](./CoreProperties.md#URI)|
