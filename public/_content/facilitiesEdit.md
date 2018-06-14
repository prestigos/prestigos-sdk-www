<h3 id="facilitiesEdit">facilitiesEdit
  <code>prestigos.facilitiesEdit(options)</code>
</h3>

Edit a facility

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| id          | string        | The facility id.
| name        | string        | _[optional]_<br>The name of the facility. Must be lowercase and no contain no spaces.
| description | string        | _[optional]_<br>Description of the category

```javascript
prestigos.facilitiesEdit({
  id            : 'cccc888ababa'
  name          : 'downtown-facility'
}).then(...);
```



