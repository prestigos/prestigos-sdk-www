<h3 id="layersCreate">layersCreate
  <code>prestigos.layersCreate(options)</code>
</h3>

Create a layer

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| name        | string        | Name to identify the layer
| description | string        | Description of the layer
| elements    | array         | The elements of the layer


The `elements` property is an array of objects. Each object has the following properties:

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| title       | string        | Title of the element
| description | string        | Description of the element
| type        | string        | The type of the element
| icon        | string        | _[optional]_<br>URL with the icon
| strokeColor | string        | _[optional]_<br>The color of the stroke
| fillColor   | string        | _[optional]_<br>The color of the fill
| fillOpacity | string        | _[optional]_<br>The opacity of the fill
| geo         | object        | _[optional]_<br>Object containing the longitude and latitude on the `lon` and `lat` properties respectively
| paths       | array         | _[optional]_<br>Array containing objects, and each object contains the longitude and latitude on the `lon` and `lat` properties respectively

```javascript
prestigos.layersCreate({
  name          : 'layer-pack-1',
  description   : 'Some layers',
  elements      : [
    {
      title       : 'First',
      description : 'The first layer',
      icon        : 'http://imgur.com/truoneru'
      geo         : {
        lon : 10.89908893467,
        lat : 1.897489349233
      }
    }
  ]
}).then(...);
```

