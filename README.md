sails-stringfile
===================

Localized stringfile containing messages used in Sails command-line interface and runtime.
This is one part of the effort towards making Sails more accessible to non-native English readers/speakers.



## How This Module Works

These files are here for future use-- this project is an early-stage work in progress.

+ Environment variables are used to determine a user's locale.  (defaults to English)


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


## Languages

Current language support _targets_ are:

+ English
+ French
+ Spanish
+ Traditional Chinese
+ German


## How Can I Help?

+ First, the existing strings need to be pulled out of sails core, generators, hooks, and adapters.

+ Then, those strings can be translated into different languages here.








> (please send a PR if you have a request and we'll add it to this list!)

## License

MIT c. Mike McNeil 2014
