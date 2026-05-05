###### No mocks

# Flakiness and limited coverage

| Scenario | Result |
| --- | --- |
| **Normal load** | ⚠️ Flaky due to API response variability |
| **Empty list** | ❌ Not available: can't control the API response |
| **API error** | ❌ Not available: can't force the server to fail |

> ❗️ Without mocking, tests are **flaky** and scenario coverage is **limited**.

