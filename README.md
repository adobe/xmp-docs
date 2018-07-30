<img src="./xmp_tagline.png" width="200" align="middle">
<br/>

Metadata is any data that helps describe the content or characteristics of a file. You may already be accustomed to viewing and adding some basic metadata through the File Info or Document Properties box found in many software applications and some operating systems. You may also use an asset or content management system (CMS) that captures some file properties and displays them for you.

**Adobe’s Extensible Metadata Platform (XMP)** is a file labeling technology that lets you embed metadata into files themselves during the content creation process. With an XMP enabled application, your workgroup can capture meaningful information about a project (such as titles and descriptions, searchable keywords, and up-to-date author and copyright information) in a format that is easily understood by your team as well as by software applications, hardware devices, and even file formats. Best of all, as team members modify files and assets, they can edit and update the metadata in real time during the workflow.

With XMP, desktop applications and back-end publishing systems gain a common method for capturing, sharing, and leveraging this valuable metadata. Adobe has taken the “heavy lifting” out of metadata integration, offering content creators an easy way to embed meaningful information about their projects and providing industry partners with standards-based building blocks to develop optimized workflow solutions.

<br/>

**Open standards**

By providing a standard way of tagging files with metadata across products from Adobe and other vendors, XMP is a powerful solution enabler. As an open source technology, it is freely available to developers, which means that the user community benefits from the innovations contributed by developers worldwide. The XMP SDKs are available in the downloads section. Furthermore, XMP is extensible — it can accommodate existing metadata schemas, so systems don’t need to be rebuilt from scratch. A growing number of third-party applications now support XMP.

Since early 2012, XMP is also an [ISO standard (16684-1)](https://www.iso.org/news/2012/03/Ref1525.html).

<br/>

**Key benefits**

* Create smart assets that retain their context when traveling across software, devices, and databases.
* Provide full extensibility by adding arbitrary metadata to media while visualizing it in Adobe products.
* Enable powerful search and retrieval of rich media across diverse file formats and database systems.
* Manage relationships of assets throughout their lifecycle of content creation and consumption.
* Build on open standards and open source licenses to foster a common exchange across the industry.

<br/>

**Highlights**

[Metadata Working Group](http://www.metadataworkinggroup.org/)
<br/>
Learn more about how companies are getting together to build metadata interoperability across operating systems, mobile devices, cameras, and online services.

<br/>

**XMP SDKs**

Adobe offers two SDKs for XMP, the XMP Toolkit SDK and the XMP Metadata UI SDK.

The XMP Toolkit SDK allows you to integrate XMP functionality into your product or solution. The XMP Metadata UI SDK lets you modify Adobe Creative Cloud applications to display custom metadata UI to either adapt the existing UI to its own workflow or to be able to interact with custom metadata. [Learn more or download the SDKs now ›](https://www.adobe.com/devnet/xmp.html)

<br/>

**XMP Specification**

[Part 1, Data model, Serialization, and Core Properties](https://wwwimages2.adobe.com/content/dam/acom/en/devnet/xmp/pdfs/XMP%20SDK%20Release%20cc-2016-08/XMPSpecificationPart1.pdf) [April, 2012] covers the basic metadata representation model that is the foundation of the XMP standard format. The Data Model prescribes how XMP metadata can be organized; it is independent of file format or specific usage. The Serialization Model prescribes how the Data Model is represented in XML, specifically RDF.
Part 1 is also a covered as part of **_ ISO 16684-1:2012, Graphic technology – Extensible metadata platform (XMP) specification – Part 1: Data model, serialization and core properties. _** You can read more about it here and access the standard from the [ISO Store](https://www.iso.org/standard/57421.html).

[Part 2, Additional Properties](https://wwwimages2.adobe.com/content/dam/acom/en/devnet/xmp/pdfs/XMP%20SDK%20Release%20cc-2016-08/XMPSpecificationPart2.pdf) [Aug, 2016] provides detailed property lists and descriptions for standard XMP metadata schemas; these include general-purpose schemas such as Dublin Core, and special-purpose schemas for Adobe applications such as Photoshop. It also provides information on extending existing schemas and creating new schemas.

[Part 3, Storage in Files](https://wwwimages2.adobe.com/content/dam/acom/en/devnet/xmp/pdfs/XMP%20SDK%20Release%20cc-2016-08/XMPSpecificationPart3.pdf) [Aug, 2016] provides information about how serialized XMP metadata is packaged into XMP Packets and embedded in different file formats. It includes information about how XMP relates to and incorporates other metadata formats, and how to reconcile values that are represented in multiple metadata formats.

[Description of XMP schemas using RELAX NG](https://www.iso.org/standard/57422.html)[Dec, 2014] is a ISO 16684-2:2014 standard which specifies the use of RELAX NG to describe serialized XMP metadata. This applies to how conforming schemas can use the features of RELAX NG. This standard is published as ISO 16684-2:2014 Graphic technology – Extensible metadata platform (XMP) – Part 2: Description of XMP schemas using RELAX NG.
 
<br/>
 
**XMP Documentation**

The Partners Guide to XMP for Dynamic Media provides guidance to developers writing applications that read, write, and modify dynamic media documents, so that those applications can maintain the integrity of the composition and editing history and temporal metadata in composed documents.

[Partners Guide to XMP for Dynamic Media](https://wwwimages2.adobe.com/content/dam/acom/en/devnet/xmp/pdfs/DynamicMediaXMPPartnerGuide.pdf)

<br/>

## Overview of XMP technology

XMP standardizes a data model, a serialization format and core properties for the definition and processing of extensible metadata. It also provides guidelines for embedding XMP information into popular image, video and document file formats, such as *JPEG* and *PDF*, without breaking their readability by applications that do not support XMP. Therefore, the non-XMP metadata have to be reconciled with the XMP properties. Although metadata can alternatively be stored in a sidecar file, embedding metadata avoids problems that occur when metadata is stored separately.

<br/>

**XMP namespace definitions** 

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
