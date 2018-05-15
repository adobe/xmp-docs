<img src="./xmp_tagline.png" width="150" align="right">

# XMP (Extensible Metadata Platform) 

The **Extensible Metadata Platform (XMP)** is an ISO standard, originally created by Adobe Systems Inc., for the creation, processing and interchange of standardized and custom metadata for digital documents and data sets.

XMP standardizes a data model, a serialization format and core properties for the definition and processing of extensible metadata. It also provides guidelines for embedding XMP information into popular image, video and document file formats, such as *JPEG* and *PDF*, without breaking their readability by applications that do not support XMP. Therefore, the non-XMP metadata have to be reconciled with the XMP properties. Although metadata can alternatively be stored in a sidecar file, embedding metadata avoids problems that occur when metadata is stored separately.

**XMP Specification is divided into *three* parts**

[Part 1, Data Model, Serialization, and Core Properties](./XMPSpecifications/XMPSpecificationPart1.pdf)

[Part 2, Additional Properties](./XMPSpecifications/XMPSpecificationPart2.pdf)

[Part 3, Storage in Files](./XMPSpecifications/XMPSpecificationPart3.pdf)

## XMP namespace definitions 

The namespaces define a set of properties. In any given XMP Packet, a property may be absent or present.For any given XMP, there is no requirement that all properties from a given namespace must be present. For structured properties, there is no requirement that all fields be present (unless otherwise specified by a namespace).

XMP metadata may include properties from one or more of the namespaces. For example, a typical subset used by many Adobe applications might include the following: 	

* Dublin Core namespace: **dc:title, dc:creator, dc:description, dc:subject, dc:format, dc:rights**
* XMP basic namespace: **xmp:CreateDate, xmp:CreatorTool, xmp:ModifyDate, xmp:MetadataDate**
* XMP rights management namespace: **xmpRights:WebStatement, xmpRights:Marked**
* XMP media management namespace: **xmpMM:DocumentID**

XMP defines namespaces into *two* catagories:

1. *XMP standard namespaces*, provides namespace definitions for standard general-purpose namespaces.
2. *Specialized Namespaces*, provides namespace definitions for namespaces that are specialized for Adobe applications or usages

**XMP Standard Namespaces**

* [XMP Namespace](XMPNamespaces/xmp.md)
* [XMP Media Management Namespace](XMPNamespaces/xmpMM.md)
* [XMP Basic Job Ticket Namespace](XMPNamespaces/xmpBJ.md)
* [XMP Paged-text Namespace](XMPNamespaces/xmpTPg.md)
* [XMP Dynamic Media Namespace](XMPNamespaces/xmpDM.md)
* [XMP Rights Management Namespace](XMPNamespaces/xmpRights.md)

**XMP Specialized Namespaces**
* [Adobe PDF Namespace](XMPNamespaces/pdf.md)
* [Photoshop Namespace](XMPNamespaces/photoshop.md)
* [Camera Raw Namespace](XMPNamespaces/crs.md)
* [Exif Namespace](XMPNamespaces/exif.md)
* [Tiff Namespace](XMPNamespaces/tiff.md)
* [Dublin Core Namespace](XMPNamespaces/dc.md)
* [IPTC Core Namespace](XMPNamespaces/Iptc4xmpCore.md)
