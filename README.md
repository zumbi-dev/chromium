# chromium

Deploy [@sparticuz/chromium](https://github.com/Sparticuz/chromium) as a AWS Lambda Layer.

## Usage

```yaml
plugins:
  - serverless-latest-layer-version

functions:
  handler:
    handler: handlers/handler.handler
  layers:
    - arn:aws:lambda:${aws:region}:${aws:accountId}:layer:chromium:latest
```

## Latest layer version

For convenience, use the plugin [serverless-latest-layer-version](https://github.com/mooyoul/serverless-latest-layer-version) to always get the latest layer version.
