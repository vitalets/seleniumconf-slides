###### Alternative

# Request Mocking Protocol

```mermaid
flowchart LR
  data[Test data<br/>serialized mock schema] --> header[Navigation header<br/>attached by BiDi]
  header --> server[Server<br/>applies mocks while rendering]
```

No external mock server. Each test carries its own mock data.

