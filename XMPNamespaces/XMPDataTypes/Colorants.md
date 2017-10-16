# Colorant

A structure containing the characteristics of a colorant (swatch) used in a document.

- The namespace URI is http://ns.adobe.com/xap/1.0/g/

- The preferred namespace prefix is xmpG

|Name|Description|Type|
|----|-----------|----|
|xmpG:A|A value when the mode is LAB. Range -128 to 127.  |[Integer](./CoreProperties.md#Integer)|
|xmpG:B|B value when the mode is LAB. Range -128 to 127.  |[Integer](./CoreProperties.md#Integer)|
|xmpG:L|L value when the mode is LAB. Range 0-100  |[Real](./CoreProperties.md#Real)|
|xmpG:black|Colour value when the mode is CMYK. Range 0-100.  |[Real](./CoreProperties.md#Real)|
|xmpG:cyan|Colour value when the mode is CMYK. Range 0-100.  |[Real](./CoreProperties.md#Real)|
|xmpG:magenta|Colour value when the mode is CMYK. Range 0-100.  |[Real](./CoreProperties.md#Real)|
|xmpG:yellow|Colour value when the mode is CMYK. Range 0-100.  |[Real](./CoreProperties.md#Real)|
|xmpG:blue|Colour value when the mode is RGB. Range 0-255.  |[Integer](./CoreProperties.md#Integer)|
|xmpG:green|Colour value when the mode is RGB. Range 0-255.  |[Integer](./CoreProperties.md#Integer)|
|xmpG:red|Colour value when the mode is RGB. Range 0-255.  |[Integer](./CoreProperties.md#Integer)|
|xmpG:mode|The colour space in which the colour is defined. One of: `CMYK`, `RGB`, `LAB`. Library colours are represented in the colour space for which they are defined.  |Open Choice of [Text](./CoreProperties.md#Text)|
|xmpG:swatchName|Name of the swatch.  |[Text](./CoreProperties.md#Text)|
|xmpG:type|The type of colour, one of `PROCESS` or `SPOT`  |Closed Choice of [Text](./CoreProperties.md#Text)|
