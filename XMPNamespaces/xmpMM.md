# XMP Media Management namespace

This namespace is primarily for use by digital asset management (DAM) systems.

The following properties are “owned” by the DAM system and should be set by applications under their direction; they should not be used by unmanaged files: *xmpMM:ManagedFrom, xmpMM:Manager, xmpMM:ManageTo, xmpMM:ManageUI, xmpMM: ManagerVariant*.

The following properties are owned by the DAM system for managed files, but can also be used by applications for unmanaged files: *xmpMM:DerivedFrom, xmpMM:DocumentID, xmpMM: RenditionClass, xmpMM:RenditionParams, xmpMM:VersionID, xmpMM:Versions*.

The *xmpMM:History* property is always owned by the application.

- The namespace URI is http://ns.adobe.com/xap/1.0/mm/

- The preferred namespace prefix is xmpMM

|Name|Description|Type|
|----|-----------|----|
|xmpMM:DerivedFrom|A reference to the original document from which this one is derived. It is a minimal reference; missing components can be assumed to be unchanged. For example, a new version might only need to specify the instance ID and version number of the previous version, or a rendition might only need to specify the instance ID and rendition class of the original.  |[ResourceRef](./XMPDataTypes/ResourceRef.md)|
|xmpMM:DocumentID|The common identifier for all versions and renditions of a resource. It should be based on a UUID; Created once for new resources. Different renditions are expected to have different values for xmpMM:DocumentID.  |[GUID](./XMPDataTypes/CoreProperties.md#guid)|
|xmpMM:InstanceID|An identifier for a specific incarnation of a resource, updated each time a file is saved. It should be based on a UUID;   |[GUID](./XMPDataTypes/CoreProperties.md#guid)|
|xmpMM:OriginalDocumentID|The common identifier for the original resource from which the current resource is derived. For example, if you save a resource to a different format, then save that one to another format, each save operation should generate a new xmpMM:DocumentID that uniquely identifies the resource in that format, but should retain the ID of the source file here. It links a resource to its original source.  |[GUID](./XMPDataTypes/CoreProperties.md#guid)|
|xmpMM:RenditionClass|The rendition class name for this resource. This property should be absent or set to default for a document version that is not a derived rendition.  |[RenditionClass](./XMPDataTypes/CoreProperties.md#renditionclass)|
|xmpMM:RenditionParams|Can be used to provide additional rendition parameters that are too complex or verbose to encode in xmpMM: RenditionClass.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpMM:History|An ordered array of high-level user actions that resulted in this resource. It is intended to give human readers a description of the steps taken to make the changes from the previous version to this one. The list should be at an abstract level; it is not intended to be an exhaustive keystroke or other detailed history. The description should be sufficient for metadata management, as well as for workflow enhancement.  |Ordered array of [ResourceEvent](./XMPDataTypes/ResourceEvent.md)|
|xmpMM:Ingredients|References to resources that were incorporated, by inclusion or reference, into this resource.  |Unordered array of [ResourceRef](./XMPDataTypes/ResourceRef.md)|
|xmpMM:Pantry|Each array item has a structure value with a potentially unique set of fields, containing extracted XMP from a component. Each field is a property from the XMP of a contained resource component, with all substructure preserved. Each pantry entry shall contain an **xmpMM:InstanceID**. Only one copy of the pantry entry for any given **xmpMM:InstanceID** shall be retained in the pantry. Nested pantry items shall be removed from the individual pantry item and promoted to the top level of the pantry. |Unordered array of struct|
|xmpMM:ManagedFrom|A reference to the document as it was prior to becoming managed. It is set when a managed document is introduced to an asset management system that does not currently own it. It may or may not include references to different management systems.  |[ResourceRef](./XMPDataTypes/ResourceRef.md)|
|xmpMM:Manager|The name of the asset management system that manages this resource. Along with xmpMM: ManagerVariant, it tells applications which asset management system to contact concerning this document.  |[AgentName](./XMPDataTypes/CoreProperties.md#agent-name)|
|xmpMM:ManageTo|A URI identifying the managed resource to the asset management system; the presence of this property is the formal indication that this resource is managed. The form and content of this URI is private to the asset management system.  |[URI](./XMPDataTypes/CoreProperties.md#uri)|
|xmpMM:ManageUI|A URI that can be used to access information about the managed resource through a web browser. It might require a custom browser plug-in.  |[URI](./XMPDataTypes/CoreProperties.md#uri)|
|xmpMM:ManagerVariant|Specifies a particular variant of the asset management system. The format of this property is private to the specific asset management system.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpMM:VersionID|The document version identifier for this resource. Each version of a document gets a new identifier, usually simply by incrementing integers 1, 2, 3 . . . and so on. Media management systems can have other conventions or support branching which requires a more complex scheme.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|xmpMM:Versions|The version history associated with this resource. Entry 1 is the oldest known version for this document, entry[last()] is the most recent version. Typically, a media management system would fill in the version information in the metadata on check-in. It is not guaranteed that a complete history of versions from the first to this one will be present in the xmpMM:Versions property. Interior version information can be compressed or eliminated and the version history can be truncated at some point.  |Ordered array of [Version](./XMPDataTypes/Version.md)|
