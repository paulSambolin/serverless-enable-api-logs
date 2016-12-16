# serverless-enable-api-logs
Enables Coudwatch logging for API Gateway events


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
