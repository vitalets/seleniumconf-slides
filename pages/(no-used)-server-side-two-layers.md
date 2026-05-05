###### Server-side mocks

# Two interception layers

| Layer | Responsibility |
| --- | --- |
| <span style="white-space: nowrap;">**Browser layer**</span> | BiDi intercepts the navigation request and attaches the serialized mock schema. |
| **Server layer** | The server intercepts outgoing request, reads the header and returns mocked responses.
