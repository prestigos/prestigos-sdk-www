<h3 id="HRAnalytics">HRAnalytics
  <code>prestigos.HRAnalytics(options)</code>
</h3>

Get the HR analytics report.


The argument is an object with the following properties:

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| registry      | integer       | The id of the registry to use the query with. |
| query         | string        | _[optional]_<br> The id of the query.<br>Default value is `_default`, which is the id of the default query.|
| kpis          | array         | Array containing the id of the desired KPIs. It must contain at least be one KPI.
