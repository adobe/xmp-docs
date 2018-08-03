# Font

A structure containing the characteristics of a font used in a document.

- The namespace URI is http://ns.adobe.com/xap/1.0/sType/Font#

- The preferred namespace prefix is stFnt

|Name|Description|Type|
|----|-----------|----|
|stFnt:childFontFiles|The list of file names for the fonts that make up a composite font  |Ordered array of [Text](./CoreProperties.md#text)|
|stFnt:composite|When true, this is a composite font  |[Boolean](./CoreProperties.md#boolean)|
|stFnt:fontFace|The font face name  |[Text](./CoreProperties.md#text)|
|stFnt:fontFamily|The font family name  |[Text](./CoreProperties.md#text)|
|stFnt:fontFileName|The font file name (not a complete path)  |[Text](./CoreProperties.md#text)|
|stFnt:fontName|PostScript® name of the font  |[Text](./CoreProperties.md#text)|
|stFnt:fontType|The font type, such as TrueType, Type 1, Open Type, and so on  |Open Choice of [Text](./CoreProperties.md#text)|
|stFnt:versionString|The version string `/version for Type1 fonts`,`nameId 5 for Apple True Type and OpenType`,`/CIDFontVersion for CID fonts`,`The empty string for bitmap fonts`. The Adobe CoolType font engine allows two fonts with the same PostScript name and different technologies to be used at the same time, but not if they are from different versions. So even without this data for a given document you will have unique font data. However, the version can tell you if the font has changed metrics, glyph forms or other important information. This is useful for comparing fonts in two documents or fonts in a document to those in your system.  |[Text](./CoreProperties.md#text)|
