sails-stringfile
===================

Localized stringfile containing messages used in Sails command-line interface and runtime.
This is one part of the effort towards making Sails more accessible to non-native English readers/speakers.



## Usage


```javascript
// From Sails core, an adapter, a generator, a hook, or some other dependency:
var STRINGFILE = require('sails-stringfile');

// Internally, this module runs node's native `util.format()` method,
// so you can also template strings:
var localizedMessage = STRINGFILE('cli.new.success', ['myApp', {some:'stuff'}, 'more stuff'])

// Then, appropriate msg is brought in auf deutsch, espanol, traditional chinese, english, etc.
console.log(localizedMessage);
```


## Status

These files are here for future use-- this project is an early-stage work in progress.

+ First, the existing strings need to be pulled out of sails core, generators, hooks, and adapters.

+ Then, those strings can be translated into different languages here.

+ Environment variables are used to determine a user's locale.  (defaults to English)

## License

MIT c. Mike McNeil 2014