###### Header-based mocks

# Limitations

<v-click>

| Limitation | Meaning |
| --- | --- |
| **Declarative mocks** | Mock definitions must be serializable to be transfered in headers. |
| **Header size** | Request header size is typically limited to ~4–8 KB. |

</v-click>

<v-click>

<SpeechBubble>

👉 In practice, this is usually acceptable. Mocks should focus on the **minimal state** the test actually needs.

</SpeechBubble>

</v-click>
