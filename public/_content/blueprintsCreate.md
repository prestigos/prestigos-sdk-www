<h3 id="blueprintsCreate">blueprintsCreate
  <code>prestigos.blueprintsCreate(options)</code>
</h3>

Create a blueprint

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| name        | string        | The name of the blueprint
| description | string        | Description of the blueprint
| facility    | string        | id of the facility
| image_url   | string        | url of the image

```javascript
prestigos.blueprintsCreate({
  name          : 'floor1',
  description   : 'This is the description'
  facility      : 'aabbccddd',
  image_url     : 'https://s3.prestigos.com/tnrdunreooeu'
}).then(...);
```
