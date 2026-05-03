###### CASE 1

# First attempt: no mocking

```mermaid
flowchart LR
  test[Test opens the page] --> app[App calls the real API]
  app --> assertions[Assertions check real data]
```

Simple, but coupled to whatever the external service returns today.
Simple, but coupled to whatever the external service returns today.

<!--
Cue: Introduce the straightforward approach. Then switch to VS Code and open the no-mocks test.
-->
