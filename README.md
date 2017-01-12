# serverless-enable-api-logs
Enables Coudwatch logging for API Gateway events


# Usage
```yaml
...

plugins:
  - serverless-enable-api-logs

...
custom:
  stageVariables:
    thirdPartyEndpoint: http://supercool.endpoint.com/openapi/something

functions:
  get:
    handler: index.handler
    events:
      - http:
          path: user/{id}
          method: get
```
