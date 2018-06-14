<h3 id="blueprintsEdit">blueprintsEdit
  <code>prestigos.blueprintsEdit(options)</code>
</h3>

Edit a blueprint

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| id          | string        | The blueprint id.
| name        | string        | _[optional]_<br>The name of the blueprint
| description | string        | _[optional]_<br>Description of the blueprint
| facility    | string        | _[optional]_<br>id of the facility
| image_url   | string        | _[optional]_<br>url of the image
```javascript
prestigos.blueprintsEdit({
  id            : '8ababacccc88',
  name          : 'floor14',
  image_url     : 'https://s3.prestigos.com/tnrdunreooeu'
}).then(...);
```



