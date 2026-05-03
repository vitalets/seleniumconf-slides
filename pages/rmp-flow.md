###### RMP ON THE USERS APP

# Mock the server-side API call through navigation

```mermaid
flowchart LR
  nav[Browser navigation<br/>GET /users-page] --> header[BiDi adds header<br/>x-request-mocks]
  header --> html[Server renders HTML<br/>with mocked /users data]
```

```http
x-request-mocks: [{"url":"/users","status":200,"body":[...]}]
```

<!--
Cue: The browser request is intercepted, but the API substitution happens on the server.
-->
