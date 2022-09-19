This is a forked project from https://github.com/bug-hunters/oas3-tools with support for cors parameter

## usage example:

```
const options = {
    routing: {
        controllers: path.join(__dirname, './controllers'),
    },
    cors: cors(),
};

const expressAppConfig = oas3Tools.expressAppConfig(path.join(__dirname, './api/openapi.yaml'), options);

const app = expressAppConfig.getApp();
```