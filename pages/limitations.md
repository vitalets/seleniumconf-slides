###### LIMITS

# Header-based mocks limitations

| Limitation | Meaning |
| --- | --- |
| **Declarative mocks** | Mock definitions must be serializable. Arbitrary functions do not travel in headers. |
| **Header size** | Practical request header limits are often around 4-8 KB, depending on the environment. |

> 👉 In practice, this is usually acceptable. Mocks should focus on the small state the test actually needs.


