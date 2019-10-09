#### Logging
- pino (https://github.com/pinojs/pino)
- pino-pretty (https://github.com/pinojs/pino-pretty)
```
$ yarn add pino pino-pretty
```
To use pino and pino-pretty on code
```
const pino = require('pino')
const logger = pino({
  prettyPrint: { colorize: true }
})
```
For Example you can use like this
```
  logger.info(`[server] ${socket.id}`, message)
```
