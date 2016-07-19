<h3 id="layersEdit">layersEdit
  <code>prestigos.layersEdit(options)</code>
</h3>

Edit a layer

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| id          | string        | The layer id.

The properties are the same as `layersCreate`

```javascript
prestigos.layersEdit({
  id            : 'aaaabbbccccc11111',
  elements      : [
    {
      title       : 'a-layer',
      description : 'Some layer',
      icon        : 'http://imgur.com/truoneru'
      geo         : {
        lon : 10.89908893467,
        lat : 1.897489349233
      }
    }
  ]
}).then(...);
```


