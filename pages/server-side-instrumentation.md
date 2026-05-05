###### Header-based mocks

# App Instrumentation

Intercept `fetch()` requests on server and apply mocks from headers.

```js
// instrumentation.js

if (process.env.NODE_ENV !== 'production') {
  setupFetchInterceptor(async () => {
    const { headers } = await import('next/headers.js');
    return headers();
  });
}
```

> 👉 Depends on your framework and programming language.

