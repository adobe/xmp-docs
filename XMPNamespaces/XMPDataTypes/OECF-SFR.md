# OECF-SFR

A structure describing the OECF/SFR.

- The namespace URI is http://ns.adobe.com/exif/1.0/

- The preferred namespace prefix is exif

|Name|Description|Type|
|----|-----------|----|
|exif:Columns|Number of columns,*n* |[Integer](./CoreProperties.md#Integer)|
|exif:Names|Column item names, *n* entries  |Ordered array of [Text](./CoreProperties.md#Text)|
|exif:Rows|Number of rows,*m*  |[Integer](./CoreProperties.md#Integer)|
|exif:Values|OECF/SFR values, sequence should be, in order: *value[0, 0] ... value[n - 1, 0] value[0, m - 1] ... value[n - 1, m - 1]*  |Ordered array of [Rational](./CoreProperties.md#Rational)|
