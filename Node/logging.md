# Logging

## pino

* <https://medium.com/@maxantonov/better-nodejs-logging-99836a77a660>

* install lib

```shell
npm install pino pino-pretty --save
```

* package.json scripts

```json
"scripts": {
    "start": "node index.js | ./node_modules/.bin/pino-pretty --translateTime",
    "prod": "LOG_LEVEL=info node index.js | ./node_modules/.bin/pino-pretty --translateTime"
}
```
