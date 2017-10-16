# XMP Paged-Text namespace

The Paged-Text namespace is used for text appearing on a page in a document.

- The namespace URI is http://ns.adobe.com/xap/1.0/t/pg/

- The preferred namespace prefix is xmpTPg

|Name|Description|Type|
|----|-----------|----|
|xmpTPg:Colorants|An ordered array of colorants (swatches) that are used in the document (including any in contained documents).  |Ordered array of [Colorants](./XMPDataTypes/Colorants.md)|
|xmpTPg:Fonts|An unordered array of fonts that are used in the document (including any in contained documents).  |Unordered array of [Font](./XMPDataTypes/Font.md)|
|xmpTPg:MaxPageSize|The size of the largest page in the document (including any in contained documents).  |[Dimensions](./XMPDataTypes/Dimensions.md)|
|xmpTPg:NPages|The number of pages in the document (including any in contained documents).  |[Integer](./XMPDataTypes/CoreProperties.md#Integer)|
|xmpTPg:PlateNames|An ordered array of plate names that are needed to print the document (including any in contained documents).  |Ordered array of [Text](./XMPDataTypes/CoreProperties.md#Text)|
