<h3 id="tagsCreate">tagsCreate
  <code>prestigos.tagsCreate(options)</code>
</h3>

Create a tag

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| name        | string        | The actual tag. Must be lowercase and no contain no spaces.
| description | string        | Description of the tag
| category    | string        | Id of the category

```javascript
prestigos.tagsCreate({
  name          : 'some-tag',
  description   : 'This is the description of some-tag',
  category      : 'a2a2aa33bbbbccccddd'
}).then(...);
```
