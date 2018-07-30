
## Overview of XMP technology

XMP standardizes a data model, a serialization format and core properties for the definition and processing of extensible metadata. It also provides guidelines for embedding XMP information into popular image, video and document file formats, such as *JPEG* and *PDF*, without breaking their readability by applications that do not support XMP. Therefore, the non-XMP metadata have to be reconciled with the XMP properties. Although metadata can alternatively be stored in a sidecar file, embedding metadata avoids problems that occur when metadata is stored separately.


## XMP Specification

[Part 1, Data model, Serialization, and Core Properties](https://wwwimages2.adobe.com/content/dam/acom/en/devnet/xmp/pdfs/XMP%20SDK%20Release%20cc-2016-08/XMPSpecificationPart1.pdf) [April, 2012] covers the basic metadata representation model that is the foundation of the XMP standard format. The Data Model prescribes how XMP metadata can be organized; it is independent of file format or specific usage. The Serialization Model prescribes how the Data Model is represented in XML, specifically RDF.
Part 1 is also a covered as part of **_ ISO 16684-1:2012, Graphic technology – Extensible metadata platform (XMP) specification – Part 1: Data model, serialization and core properties. _** You can read more about it here and access the standard from the [ISO Store](https://www.iso.org/standard/57421.html).

[Part 2, Additional Properties](https://wwwimages2.adobe.com/content/dam/acom/en/devnet/xmp/pdfs/XMP%20SDK%20Release%20cc-2016-08/XMPSpecificationPart2.pdf) [Aug, 2016] provides detailed property lists and descriptions for standard XMP metadata schemas; these include general-purpose schemas such as Dublin Core, and special-purpose schemas for Adobe applications such as Photoshop. It also provides information on extending existing schemas and creating new schemas.

[Part 3, Storage in Files](https://wwwimages2.adobe.com/content/dam/acom/en/devnet/xmp/pdfs/XMP%20SDK%20Release%20cc-2016-08/XMPSpecificationPart3.pdf) [Aug, 2016] provides information about how serialized XMP metadata is packaged into XMP Packets and embedded in different file formats. It includes information about how XMP relates to and incorporates other metadata formats, and how to reconcile values that are represented in multiple metadata formats.

[Description of XMP schemas using RELAX NG](https://www.iso.org/standard/57422.html)[Dec, 2014] is a ISO 16684-2:2014 standard which specifies the use of RELAX NG to describe serialized XMP metadata. This applies to how conforming schemas can use the features of RELAX NG. This standard is published as ISO 16684-2:2014 Graphic technology – Extensible metadata platform (XMP) – Part 2: Description of XMP schemas using RELAX NG.

 
### XMP Documentation

The Partners Guide to XMP for Dynamic Media provides guidance to developers writing applications that read, write, and modify dynamic media documents, so that those applications can maintain the integrity of the composition and editing history and temporal metadata in composed documents.

[Partners Guide to XMP for Dynamic Media](https://wwwimages2.adobe.com/content/dam/acom/en/devnet/xmp/pdfs/DynamicMediaXMPPartnerGuide.pdf)