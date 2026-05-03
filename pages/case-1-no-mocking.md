###### No mocks

# First attempt: no mocking

<style scoped>
h3 + ul {
  margin-top: 0.9rem;
}
</style>

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

<div v-click="5">

<br>

- **Unreliable**: API can reorder, rename, or fail while the app still works
- **Limited scenarios**: empty lists and error flows need response control

</div>


<!--
Cue: Introduce the straightforward approach. Then switch to VS Code and open the no-mocks test.
-->
