<h3 id="kpisCreate">kpisCreate
  <code>prestigos.kpisCreate(options)</code>
</h3>

Create a KPI, then add it to the group as one of the available KPIs and add permissions to the user who is creating it.

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| name        | string        | Name of the KPI
| description | string        | Description
| positive    | boolean       | Is this a positive KPI?
| monetary    | boolean       | This KPI has the monetery factor?
| has_quantity| boolean       | It counts quantity?
| duration    | boolean       | It stores duration?
| geo         | boolean       | It stores the longitude and latitude of the events?
| is_private  | boolean       | Is private? (that is, is available to other groups?)
| limits      | object        | The limits of the values.

#### limits:

The limits object have properties, where each property is an object with the properties `min` and `max`.

The available properties are the following:


| Property    | Type          | Description |
| ----------- | --------------|------------ |
| duration    | object        | `min` and `max` possible duration of the event, in seconds. The minimal number must be equal or larger than 0
| monetary    | object        | `min` and `max` possible amount of money, The minimal number must be equal or larger than 0
| quantities  | object        | `min` and `max` possible quantity per event. The minimal number must be equal or larger than 1

