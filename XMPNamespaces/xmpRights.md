# XMP Rights Management namespace

The XMP Rights Management namespace contains properties that provide information regarding the legal restrictions associated with a resource.

- The namespace URI is http://ns.adobe.com/xap/1.0/rights/

- The preferred namespace prefix is xmpRights

**NOTE** *These XMP properties are intended to provide a means of rights expression. They are not intended to provide
digital rights management (DRM) controls.*

|Name|Description|Type|
|----|-----------|----|
|xmpRights:Certificate|A web URL for a rights management certificate. **NOTE:** *This is a normal (non-URI) simple value because of historical usage.*  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpRights:Marked|When true, indicates that this is a rights-managed resource. When false, indicates that this is a public-domain resource. Omit if the state is unknown.  |[Boolean](./XMPDataTypes/CoreProperties.md#boolean)|
|xmpRights:Owner|A list of legal owners of the resource.  |Unordered array of [ProperName](./XMPDataTypes/CoreProperties.md#propername)|
|xmpRights:UsageTerms|A collection of text instructions on how a resource can be legally used, given in a variety of languages.  |[Language Alternative](./XMPDataTypes/CoreProperties.md#language-alternative)|
|xmpRights:WebStatement|A Web URL for a statement of the ownership and usage rights for this resource. **NOTE:** *This is a normal (non-URI) simple value because of historical usage.*  |[Text](./XMPDataTypes/CoreProperties.md#text)|
