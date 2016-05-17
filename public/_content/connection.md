To create an instance, it's necesary to require the module. That module is a function, and should be called like this:

```javascript
var prestigos = require('prestigos-sdk')({
  hash      : 'your-token',
  username  : 'your-username',
  group     : 'your-group'
});
```

The returned object is a **Prestigos connection** instance, where all the methods to access Prestigos are available.
