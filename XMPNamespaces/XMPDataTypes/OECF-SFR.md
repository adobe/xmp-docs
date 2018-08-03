# OECF-SFR

A structure describing the OECF/SFR.

- The namespace URI is http://ns.adobe.com/exif/1.0/

- The preferred namespace prefix is exif

|Name|Description|Type|
|----|-----------|----|
|exif:Columns|Number of columns,*n* |[Integer](./CoreProperties.md#integer)|
|exif:Names|Column item names, *n* entries  |Ordered array of [Text](./CoreProperties.md#text)|
|exif:Rows|Number of rows,*m*  |[Integer](./CoreProperties.md#integer)|
|exif:Values|OECF/SFR values, sequence should be, in order: *value[0, 0] ... value[n - 1, 0] value[0, m - 1] ... value[n - 1, m - 1]*  |Ordered array of [Rational](./CoreProperties.md#rational)|
