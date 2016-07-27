<h3 id="journalEntryEdit">journalEntryCreate
  <code>prestigos.journalEntryEdit()</code>
</h3>

Edit an entry in the journal


| Property    | Type          | Description |
| ----------- | --------------|------------ |
| id          | string        | Id of the entry
| content     | string        | Content of the entry
| tags        | array         | The assigned tags
| kpis        | array         | The assigned kpis

```javascript
prestigos.journalEntryEdit({
  content : 'This is the entry',
  tags    : [ 'aaaabbcccddddd', '6666eeee66e6e6' ],
  kpis    : [ 'ccccc433333333', 'aaaaabbbbbbccc' ]
}).then(...);
```


