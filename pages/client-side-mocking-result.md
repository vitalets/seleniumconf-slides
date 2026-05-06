###### Client-side mocks

# All scenarios are covered

| Scenario | Mock |
| --- | --- |
| **Normal list** | ✅ Return two known users and assert count + first name |
| **Empty list** | ✅ Return `[]` and assert the empty state message |
| **API error** | ✅ Return status `500` and assert error details |

> 👍 Selenium BiDi gives the test direct control over browser network requests.

