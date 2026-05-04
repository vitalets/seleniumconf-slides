###### Test code

# Writing the Test

<div v-click>

```js {all|2-10|12-13|15-16|all}{at:2}
it('non-empty list (server mocks)', async () => {
  await mockServerSideRequest(
    network,
    'http://localhost:3000/ssr',
    'https://jsonplaceholder.typicode.com/users?_limit=6',
    [
      { id: 1, name: 'User 1' },
      { id: 2, name: 'User 2' },
    ],
  );

  await driver.get('http://localhost:3000/ssr');
  const users = await driver.wait(until.elementsLocated(By.css('.users-list li')), 3000);

  assert.equal(users.length, 2);
  assert.match(await users[0].getText(), /User 1/);
});
```

</div>

<div v-click="5" style="margin-top: 5px">

### ▶️ Run the test

</div>
