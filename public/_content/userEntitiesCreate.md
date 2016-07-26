<h3 id="userEntitiesCreate">userEntitiesCreate
  <code>prestigos.userEntitiesCreate(options)</code>
</h3>

Create a user entity.

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| username    | string        | _[optional]_<br>The desired username
| internal_id | string        | _[optional]_<br>The id used by the group internally
| title       | string        | _[optional]_<br>The job's title used by the group internally
| registry    | integer       | The id of the registry
| legal       | string        | The legal id
| name        | string        | The name or names
| lastname    | string        | The last name
| lastname2   | string        | _[optional]_<br>Additional field for last name
| birthday    | string / date | The date of birth, as a Date object, or a string in the format YYYY-MM-DD
| phone       | string        | _[optional]_<br>The phone number
| email       | string        | _[optional]_<br>Email address
| sex         | string        | The sex, passed as M for male or F for female
| tags        | array         | _[optional]_<br>Default tags for this entity. Each element of the array must be the id of the tag.
| address     | object        | _[optional]_<br>The current address of the entity. Each property must contain an string.
| extra       | object        | _[optional]_<br>Additional fields that the group can add. Each property must contain an string.

```javascript
prestigos.userEntitiesCreate({
  legal     : 'EAGM0000000990',
  name      : 'maah',
  lastname  : 'tyl',
  lastname2 : 'eel',
  sex       : 'm',
  registry  : 1,
  group     : 'some-gruop-id',
  birthday  : new Date('1995-01-01')
}).then(...);
```
