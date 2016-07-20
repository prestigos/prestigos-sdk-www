<h3 id="tagsEdit">tagsEdit
  <code>prestigos.tagsEdit(options)</code>
</h3>

Edit an existant tag

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| id          | string        | The id of the tag
| tag         | string        | The actual tag. Must be lowercase and no contain no spaces.
| description | string        | Description of the tag
| category    | string        | Id of the category

```javascript
prestigos.tagsEdit({
  id            : 'a24ebcaaaabbbb8',
  tag           : 'this-tag'
}).then(...);
```
