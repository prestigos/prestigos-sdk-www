<h3 id="commentsCreate">commentsCreate
  <code>prestigos.commentsCreate(options)</code>
</h3>

Create a comment

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| entity      | string        | The entity id.
| is_medal    | boolean       | _[optional]_<br>Is this a medal?<br>Default value: `false`.
| content     | string        | The main content.

```javascript
prestigos.commentsCreate({
  entity        : 'a2a2aa33bbbbccccddd',
  is_medal      : true,
  content       : 'He did a good job'
}).then(...);
```

