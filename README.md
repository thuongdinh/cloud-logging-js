# cloud-logging-js

Cloud Logging client for javascript

# Feature
- Use for both browser & nodejs env
- Log a message
- Login
- Query messages

# Installing 

## Browser 
1. Download cloud-logging.js file
2. Include into your html
3. Create new instance:

```js
var logger = CloudLogging.getLogger({
	app: 'log',
	userId: 'userId'
});
```

## Nodejs
1. Install module: npm install cloud-logging-js
2. Create new instance:

```js
var logger = require('cloud-logging-js').CloudLogging.getLogger({
	app: 'log',
	userId: 'userId'
});
```

# Guide 

## Log

```js
// simple log
logger.log('Message'); // defaut is info
logger.log('Message', 'Debug'); // log with debug level

// specific method
logger.debug('Message');
logger.info('Message');
logger.error('Message');
logger.fatal('Message');
```

## Login & query logs
TODO