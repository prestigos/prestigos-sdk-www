<h3 id="journalEntryCreate">journalEntryCreate
  <code>prestigos.journalEntryCreate()</code>
</h3>

Create an entry in the journal


| Property    | Type          | Description |
| ----------- | --------------|------------ |
| content     | string        | Content of the entry
| tags        | array         | The assigned tags
| kpis        | array         | The assigned kpis

```javascript
prestigos.journalEntryCreate({
  content : 'This is the entry',
  tags    : [ 'aaaabbcccddddd', '6666eeee66e6e6' ],
  kpis    : [ 'ccccc433333333', 'aaaaabbbbbbccc' ]
}).then(...);
```


