<h3 id="queriesExecute">queriesExecute
  <code>prestigos.queriesExecute(options)</code>
</h3>

Execute a query using the passed options.

The argument is an object with the following properties:

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| registry      | integer       | The id of the registry to use the query with. |
| query         | string        | _[optional]_<br> The id of the query.<br>If `cluster` is `true`, it will be ignored and set to the default value.<br>Default value is `_default`, which is the id of the default query.|
| cluster       | boolean       | _[optional]_<br> Boolean to show the `_default` query of the cluster. If is set to `true`, it will ignore the `query` and `entity` properties.<br>Default value is `false`. |
| entity        | string        | _[optional]_<br> Pass the id of an entity to show the query applied only to that entity. If is undefined, it will show the result to all the entities. This property is ignored if `cluster` is `true`.<br>Default value is `undefined`|
| kpi           | string        | _[optional]_<br> Pass the id of a KPI to show the query applied only to that KPI. If is undefined, it will show the data of the complete registry.<br>Default value is `undefined`|
| months        | array         | _[optional]_<br> A list to show only the desired months, each month should be an string in the format `YYYY-MM`. Example: `["2015-01","2015-02","2015-05"]`.<br>Default value is `undefined`
| includeDocs   | boolean       | _[optional]_<br> If true, it will return each document in the list.<br>Default value is `false`
| editable      | boolean       | _[optional]_<br> If true, it will show only the editable events.

```javascript
// Process "myquery", and return the total of the entire time
// of every user entity from registry 1
prestigos.queriesExecute({
  query         : 'myquery',
  registry      : 1,
  total         : true
}).then(...);

// Process "myquery", and return the total per month of every user entity
// from the kpi "aaaabbbccc" for 3 january months of 3 different years
prestigos.queriesExecute({
  kpi           : 'aaaabbbccc',
  months        : [ '2014-01', '2015-01', '2016-01' ],
  query         : 'myquery',
  registry      : 1,
  total         : true
}).then(...);

// Process "myquery", and return every event from the user entity "eafadaea" from registry 1
prestigos.queriesExecute({
  entity        : 'eafadaea',
  include_docs  : true,
  kpi           : 'aaaabbbccc',
  query         : 'myquery',
  registry      : 1
}).then(...);
```
