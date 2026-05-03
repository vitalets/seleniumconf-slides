###### Client side mocks

# Client-side mocking with Selenium BiDi

```mermaid
flowchart LR
  request[Browser request<br/>GET /users] --> bidi[BiDi interception<br/>before request is sent]
  bidi --> response[Mock response<br/>known status, headers, body]
```

The browser asks the test how to handle a matching request.
The browser asks the test how to handle a matching request.

<!--
Cue: Introduce the core idea: intercept the request and return known data before the real API is touched.
-->
