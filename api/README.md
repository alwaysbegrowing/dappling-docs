# API

## Overview

dAppling has an external API allowing external applications to access dAppling data.

### API URL

{% embed url="https://dappling.network/api/v1" %}

### Endpoints

#### /domains

This endpoint provides access to the nameserver information dAppling has been [tracking](https://dappling.network/monitor).

* [/domains](domains.md)

The /domain endpoint returns an array of all domain items being tracked by dAppling.

* [/domains/{domain}](domains-domain.md)

The /domains/{domain} endpoint allows users to query a specific domain to view any nameserver information or changes.

### Authentication

To access dAppling data, you must authenticate each request using an Authorization token in the header. Contact dAppling Network via [Twitter](https://twitter.com/dApplingNetwork) if you are interested in accessing the API.

Each API request must include the Authorization header containing a unique token.

#### Example

```javascript
const myHeaders = new Headers();
myHeaders.append("Authorization", {DAPPLING_AUTH_TOKEN});
```

### Errors

Failure to correctly include the token will result in either a 401 or 403 status code.



:cactus:_Fun Fact: Scientifically speaking, bananas are berries, while strawberries are not. Berries are defined as fruits coming from one flower with one ovary and typically have several seeds._
