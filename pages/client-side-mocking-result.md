###### RESULT

# All client-side scenarios are now testable

| Scenario | Mock |
| --- | --- |
| **Normal list** | ✅ Return two known users and assert count + first name |
| **Empty list** | ✅ Return `[]` and assert the empty state message |
| **API error** | ✅ Return status `500` and assert error details |

For client-side fetches, BiDi gives the test direct control over browser network requests.

<!--
Cue: Summarize the client-side win before switching to the server-side rendering problem.
-->
