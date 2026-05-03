###### HOW IT WORKS

# Two interception layers

| Layer | Responsibility |
| --- | --- |
| **Browser layer** | BiDi intercepts the navigation request and attaches the serialized mock schema. |
| **Server layer** | The server reads the header and returns mocked responses when matching API calls happen. |

> **RMP helper**
>
> Code sample to be added later.

<!--
Cue: This is Request Mocking Protocol: serialized mocks plus server cooperation.
-->
