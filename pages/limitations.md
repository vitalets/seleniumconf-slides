**LIMITS**

# Request mocking still needs rules

| Limitation | Meaning |
| --- | --- |
| **Declarative mocks** | Mock definitions must be serializable. Arbitrary functions do not travel in headers. |
| **Header size** | Practical request header limits are often around 4-8 KB, depending on the environment. |

In practice, this is usually acceptable when mocks are focused on the state the test actually needs.

<!--
Cue: Be clear about the tradeoffs. RMP is useful, but it is not an unlimited data transport.
-->
