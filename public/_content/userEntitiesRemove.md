<h3 id="userEntitiesCreate">userEntitiesRemove
  <code>prestigos.userEntitiesRemove(options)</code>
</h3>

Delete a user entity.

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| id          | string        | The id of the user entity
| registry    | integer       | The id of the registry

```javascript
prestigos.userEntitiesRemove({
  id        : 'a5a678bcde',
  registry  : 1
}).then(...);
```
