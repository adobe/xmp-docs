# IPTC Core namespace

IPTC Photo Metadata provides data about photographs and the values can be processed by software. Each individual metadata entity is called a property and they are grouped into Administrative, Descriptive and Rights Related properties.

- The namespace URI is http://iptc.org/std/Iptc4xmpCore/1.0/xmlns/

- The preferred namespace prefix is Iptc4xmpCore

|Name|Description|Type|
|----|-----------|----|
|Iptc4xmpCore:CreatorContactInfo|The creator contact information provides all necessary information to get in contact with the creator of this news object and comprises a set of sub-properties for proper addressing  |[ContactInfo](./XMPDataTypes/ContactInfo.md)|
|Iptc4xmpCore:IntellectualGenre|Describes the nature, intellectual or journalistic characteristic of a news object, not specifically its content.  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|Iptc4xmpCore:Scene|Describes the scene of a photo content. Specifies one or more terms from the IPTC Scene-NewsCodes. Each Scene is represented as a string of 6 digits in an unordered list.  |Unordered array of [Text](./XMPDataTypes/CoreProperties.md#text)|
|Iptc4xmpCore:Location|Name of a location the content is focussing on -- either the location shown in visual media or referenced by text or audio media. This location name could either be the name of a sublocation to a city or the name of a well known location or (natural) monument outside a city. In the sense of a sublocation to a city this element is at the fourth level of a top-down geographical hierarchy  |[Text](./XMPDataTypes/CoreProperties.md#text)|
|Iptc4xmpCore:CountryCode|Code of the country the content is focussing on -- either the country shown in visual media or referenced in text or audio media. This element is at the top/first level of a top-down geographical hierarchy. The code should be taken from ISO 3166 two or three letter code. The full name of a country should go to the "Country" element  |[Locale](./XMPDataTypes/CoreProperties.md#locale)|
|Iptc4xmpCore:SubjectCode|Specifies one or more Subjects from the IPTC Subject-NewsCodes taxonomy to categorize the content. Each Subject is represented as a string of 8 digits in an unordered list.  |Unordered array of [Text](./XMPDataTypes/CoreProperties.md#text)|
