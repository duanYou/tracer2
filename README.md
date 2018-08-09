## tracer2

Fork from [tracer](https://github.com/baryon/tracer).

### Install

```sh
$ npm i tracer2
```

### Usage

lib/logger.js

```js
const path = require('path')

const logger = require('tracer2').colorConsole({
  rootDir: path.join(__dirname, '..')
})

module.exports = logger
```

\*\*/\*.js

```js
const logger = require('path/to/lib/logger')
 
logger.log('hello')
logger.trace('hello', 'world')
logger.debug('hello %s',  'world', 123)
logger.info('hello %s %d',  'world', 123, {foo:'bar'})
logger.warn('hello %s %d %j', 'world', 123, {foo:'bar'})
logger.error('hello %s %d %j', 'world', 123, {foo:'bar'}, [1, 2, 3, 4], Object)
```

### Others

see [tracer](https://github.com/baryon/tracer).
