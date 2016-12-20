# serverless-enable-api-logs
Enables Coudwatch logging for API Gateway events

# Resources
- [Github](https://github.com/paulSambolin/serverless-enable-api-logs)
- [NPM](https://www.npmjs.com/package/serverless-enable-api-logs)

# Usage
```yaml
...

plugins:
  - serverless-enable-api-logs

...

functions:
  get:
    handler: index.handler
    events:
      - http:
          path: user/{id}
          method: get
```
