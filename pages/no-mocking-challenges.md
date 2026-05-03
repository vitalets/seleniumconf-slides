###### PROBLEM

# What breaks without mocks?

| Challenge | Impact |
| --- | --- |
| **Unreliable tests** | The API can reorder users, rename users, throttle, fail, or return new data while the app still works. |
| **Limited scenarios** | Empty lists and error flows cannot be tested unless the response can be controlled. |

We need deterministic data, but we do not want to change the application for every test case.

<!--
Cue: This is the transition into API mocking. The goal is control, not just isolation.
-->
