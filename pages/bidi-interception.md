**HOW IT WORKS**

# BiDi network interception

```mermaid
flowchart LR
  setup[Enable intercept<br/>match the API URL] --> pause[Before request<br/>browser pauses]
  pause --> event[Test receives event<br/>request details over WebSocket]
  event --> decision[Test decides<br/>continue, fail, or fulfill]
```

> **BiDi helper**
>
> Code sample to be added later.

<!--
Cue: Emphasize that BiDi allows browser-initiated events. If the test does not answer, the browser waits.
-->
