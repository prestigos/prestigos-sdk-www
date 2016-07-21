<h3 id="tagCategoriesCreate">tagCategoriesCreate
  <code>prestigos.tagCategoriesCreate(options)</code>
</h3>

Create a tag category

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| name        | string        | The name of the category. Must be lowercase and no contain no spaces.
| description | string        | Description of the category
| kind        | string        | The kind of category. Can be `kpi` or `entity`
| required    | object        | An object where each property is the id of a registry, and contains an array with the kpis where this category is required.

```javascript
prestigos.tagCategoriesCreate({
  name          : 'places',
  description   : 'This is the description of the places category',
  kind          : 'kpi',
  required      : {
    "1" : [
      "aaaaabbbbbcccc",
      "ccccbbbbbddddd",
      "dddd1111222222"
    ]
  }
}).then(...);
```
