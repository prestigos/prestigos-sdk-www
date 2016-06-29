<h3 id="userEntitiesCreate">userEntitiesEdit
  <code>prestigos.userEntitiesEdit(options)</code>
</h3>

Edit a user entity.

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| id          | string        | The id of the user entity
| registry    | integer       | The id of the registry
| phone       | string        | _[optional]_<br>The phone number
| email       | string        | _[optional]_<br>Email address
| tags        | array         | _[optional]_<br>Default tags for this entity. Each element of the array must be the id of the tag.
| address     | object        | _[optional]_<br>The current address of the entity. Each property must contain an string.
| extra       | object        | _[optional]_<br>Additional fields that the group can add. Each property must contain an string.

```javascript
prestigos.userEntitiesEdit({
  id        : 'a5a678bcde',
  registry  : 1,
  phone     : '56961720',
  email     : 'user@someweb.com',
  tags      : [ 'aaaaabbbbbbccccc', 'cccccdddddeeee' ]
}).then(...);
```
