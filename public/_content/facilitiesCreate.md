<h3 id="facilitiesCreate">facilitiesCreate
  <code>prestigos.facilitiesCreate(options)</code>
</h3>

Create a facility

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| name        | string        | The name of the facility. Must be lowercase and no contain no spaces.
| description | string        | Description of the category

```javascript
prestigos.facilitiesCreate({
  name          : 'downtown-facility',
  description   : 'This is the description of the facility'
}).then(...);
```
