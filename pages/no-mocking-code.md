###### No mocks

# First attempt: no mocking

<div v-click>

```js {all|2|4|6-7|all}{at:2}
it('non-empty list (no mocks)', async () => {
  await driver.get('http://localhost:3000');

  const users = await driver.wait(until.elementsLocated(By.css('.users-list li')), 3000);

  assert.equal(users.length, 6);
  assert.match(await users[0].getText(), /Leanne Graham/);
});
```

</div>

<div v-click="5" style="margin-top: 20px">

### ▶️ Run the test

</div>
