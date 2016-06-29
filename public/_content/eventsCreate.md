<h3 id="eventsCreate">eventsCreate
  <code>prestigos.eventsCreate(events)</code>
</h3>

Create an event or a series of events.

The passed argument is an array contaning objects, each object containing the properties of an event.
It's also possible to just pass one object, containing one event.

The properties accepted for an event are the following:

| Property    | Type          | Description |
| ----------- | --------------|------------ |
| entity      | string        | The id of the entity that commited the event. |
| kpi         | string        | The id of the KPI of the event. |
| registry    | integer       | The id of the registry of the event. |
| event_date  | string / date | The DateTime of the event.<br>It can be a JavaScript Date object, or an string, in **ISO 8601** format.<br>If the time part is omited, it assumes the time as `12:00:00` |
| quantity    | integer       | _[optional]_<br>The quantity property of the event. It must be an integer of value 1 or higher.<br>Default value: 1 |
| amount      | number        | _[optional]_<br>The monetary amount the event had. It must be an number of value 0 or higher.<br>Default value: 0 |
| comment     | string        | _[optional]_<br> An string containing a comment about the event. |
| duration    | integer       | _[optional]_<br> The duration of the event, in seconds. |
| geo         | object        | _[optional]_<br> The longitude and latitude where the event occured. It must be an object containing the 2 properties `lon` and `lat` passed as numbers.<br>Like this: `"geo" : { "lon" : 37.769573, "lat" : -122.483123 }`  |
| tags        | array         | _[optional]_<br> Array containing the ids of the tags of the event. |

```javascript
var events = [
  {
    entity        : 'aaabbbccc',
    event_date    : new Date('2015-01-01'),
    registry      : 1,
    tags          : [ 'b281555ef6ecc6' ],
    kpi           : 'ggggccccc'
  },
  {
    entity        : 'eeefffggg',
    event_date    : new Date('2015-02-10'),
    registry      : 2,
    comment       : 'This is a comment',
    kpi           : '99g9g9g99'
  }
];
prestigos.eventsCreate(events).then(....);
```

