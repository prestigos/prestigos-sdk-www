<h3 id="tagCategoriesEdit">tagCategoriesEdit
  <code>prestigos.tagCategoriesEdit(options)</code>
</h3>

Edit an existant category

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| id          | string        | The id of the category
| name        | string        | The name of the category. Must be lowercase and no contain no spaces.
| description | string        | Description of the category
| kind        | string        | The kind of category. Can be `kpi` or `entity`
| required    | object        | An object where each property is the id of a registry, and contains an array with the kpis where this category is required.

```javascript
prestigos.tagCategoriesEdit({
  id            : 'a24ebcaaaabbbb8',
  required      : {
    "1" : [
      "aaaaabbbbbcccc",
      "ccccbbbbbddddd",
      "dddd1111222222"
    ]
  }
}).then(...);
```
