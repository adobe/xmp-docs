# Basic Job Ticket namespace

This namespace describes very simple workflow or job information.

- The namespace URI is http://ns.adobe.com/xap/1.0/bj/

- The preferred namespace prefix is xmpBJ

|Name|Description|Type|
|----|-----------|----|
|xmpBJ:JobRef|References an external job management file for a job process in which the document is being used. Use of job names is under user control. Typical use would be to identify all documents that are part of a particular job or contract.       There are multiple values because there can be more than one job using a particular document at any time, and it can also be useful to keep historical information about what jobs a document was part of previously.  |Unordered array of [Job](./XMPDataTypes/Job.md)|
