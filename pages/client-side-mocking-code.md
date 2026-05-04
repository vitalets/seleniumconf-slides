###### Test code

# Writing the Test

<div v-click>

```js {all|2-5|7-8|10-11|all}{at:2}
it('non-empty list (client mocks)', async () => {
  await mockClientSideRequest(network, 'https://jsonplaceholder.typicode.com/users?_limit=6', [
    { id: 1, name: 'User 1' },
    { id: 2, name: 'User 2' },
  ]);

  await driver.get('http://localhost:3000');
  const users = await driver.wait(until.elementsLocated(By.css('.users-list li')), 3000);

  assert.equal(users.length, 2);
  assert.match(await users[0].getText(), /User 1/);
});
```

</div>

<div v-click="5" style="margin-top: 20px">

### ▶️ Run the test

</div>

<!--
Cue: Walk through setup, page load, and assertions. Run the test before opening the helper.
-->
