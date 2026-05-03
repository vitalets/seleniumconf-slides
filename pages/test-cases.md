###### TEST CASES

# Three states we want to automate

| Case | State | Expected UI |
| --- | --- | --- |
| 1 | **Normal load** | The users list is displayed. |
| 2 | **Empty list** | The app shows a clear "no users found" message. |
| 3 | **Error flow** | The app displays useful API error details. |

The normal path is easy to trigger. Empty and error states require control over the API response.

<!--
Cue: We can generate more cases, but these three are enough to expose the testing problem.
-->
