<h3 id="journalCommentCreate">journalCommentCreate
  <code>prestigos.journalCommentCreate()</code>
</h3>

Create a comment for an entry in the journal


| Property    | Type          | Description |
| ----------- | --------------|------------ |
| entry       | string        | Id of the entry
| content     | string        | The comment itself.
| parent      | string        | _[optional]_<br>If this comment is a reply to another comment, the id of the comment that is replying to.

```javascript
prestigos.journalCommentCreate({
  content : 'This is a comment',
  entry   : 'aaaaaaaaaabbbbbbb',
  parent  : 'bbbbbccccccdddddd'
}).then(...);
```



