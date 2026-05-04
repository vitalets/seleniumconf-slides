###### Alternative

# Mock via HTTP Header

Put the whole mock data into a custom HTTP header.

<div v-click>

![RMP](/rmp-schema.png)

```http
x-mock-request: {"url":"/users","status":200,"body":[...]}
```

</div>

<div v-click>

> ✅ No external mock server. Each test carries its own mock data. Highly scalable.

</div>



