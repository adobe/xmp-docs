# Time

A representation of a time value in seconds. This is similar to After Effect’s TDB, or QuickTime’s representation of time. They each have a value, and the scale of the value. For example, if the scale is the rational 1/25 (PAL 25fps), and the value is 50, the time is 2 seconds.

- The namespace URI is http://ns.adobe.com/xmp/1.0/DynamicMedia/

- The preferred namespace prefix is xmpDM

|Name|Description|Type|
|----|-----------|----|
|xmpDM:scale|The scale for the time value. For NTSC, use 1001/30000, or the less accurate 100/2997. For PAL, use 1/25.|[Rational](./CoreProperties.md#Rational)|
|xmpDM:value|The time value in the specified scale  |[Integer](./CoreProperties.md#Integer)|
