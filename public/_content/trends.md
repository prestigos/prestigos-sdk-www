<h3 id="trends">trends
  <code>prestigos.trends(options)</code>
</h3>

Get the trends report

The argument is an object with the following properties:

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| registry      | integer       | The id of the registry to use the query with. |
| query         | string        | _[optional]_<br> The id of the query.<br>Default value is `_default`, which is the id of the default query.|
| entity        | string        | _[optional]_<br> Pass the id of an entity to show the query applied only to that entity. If is undefined, it will show the result to all the entities.<br>Default value is `undefined`|
| kpi           | string        | _[optional]_<br> Pass the id of a KPI to show the query applied only to that KPI. If is undefined, it will show the data of the complete registry.<br>Default value is `undefined`|
| months        | array         | _[optional]_<br> A list to show only the desired months, each month should be an string in the format `YYYY-MM`. Example: `["2015-01","2015-02","2015-05"]`.<br>Default value is `undefined`

```javascript
// Process "myquery" on every user entity from registry 1
prestigos.trends({
  query         : 'myquery',
  registry      : 1
}).then(...);

// Process "myquery" on every user entity
// from the kpi "aaaabbbccc" for 3 january months of 3 different years
prestigos.queriesExecute({
  kpi           : 'aaaabbbccc',
  months        : [ '2014-01', '2015-01', '2016-01' ],
  query         : 'myquery',
  registry      : 1
}).then(...);
```

