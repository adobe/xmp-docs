# ResourceEvent

A structure denoting a high-level event that occurred in the processing of a resource.

- The namespace URI is http://ns.adobe.com/xap/1.0/sType/ResourceEvent#

- The preferred namespace prefix is stEvt

**Note** *The structure shall include the stEvt:action and stEvt:when fields; other fields need not be present.*

|Name|Description|Type|
|----|-----------|----|
|stEvt:action|The action that occurred.Defined values are: `converted`, `copied`, `created`, `cropped`, `edited`, `filtered`, `formatted`, `version_updated`, `printed`, `published`, `managed`, `produced`, `resized`, `saved`. New values should be verbs in the past tense. |Open Choice of [Text](./CoreProperties.md#Text)|
|stEvt:changed|A semicolon-delimited list of the parts of the resource that were changed since the previous event history. If not present, presumed to be undefined. When tracking changes and the scope of the changed components is unknown, it should be assumed that anything might have changed. |[Text](./CoreProperties.md#Text)|
|stEvt:instanceID|The value of the xmpMM:InstanceID property for the modified (output) resource  |[GUID](./CoreProperties.md#GUID)|
|stEvt:parameters|Additional description of the action  |[Text](./CoreProperties.md#Text)|
|stEvt:softwareAgent|The software agent that performed the action  |[AgentName](./CoreProperties.md#AgentName)|
|stEvt:when|Timestamp of when the action occurred. For events that create or write to a file, this should be the approximate modification time of the file.  |[Date](./CoreProperties.md#Date)|
