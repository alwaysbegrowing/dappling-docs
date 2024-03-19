---
description: This GET route returns nameserver data for a single domain.
---

# /domains/{domain}

## Request

The request object must be formatted as a GET request. The only required header is for [Authentication](./#authentication).&#x20;

### Parameters

The queried domain must be appended to the end of the url as a full root domain (e.g. https://dappling.network/api/v1/domains/dappling.fi).

### Examples

```powershell
curl --location 'https://dappling.network/api/v1/domains/dappling.fi' \
--header 'Authorization: {DAPPLING_AUTH_TOKEN}'
```

```javascript
const myHeaders = new Headers();
myHeaders.append("Authorization", {DAPPLING_AUTH_TOKEN});

const requestOptions = {
  method: "GET",
  headers: myHeaders,
};

fetch("https://dappling.network/api/v1/domains/dappling.fi", requestOptions)
  .then((response) => response.json())
  .then((result) => console.log(result))
  .catch((error) => console.error(error));
```

## Response

The /domains/{domain} endpoint returns a 200 status code with the domain object.

### Structure

* **domain**: domain name of the record
* **Nameservers:** an array that contains objects with details about the nameservers associated with the domain
  * Within each "Nameservers" object:
    * **updatedAt:** the last update time of the nameserver records for the domain
    * **records:** an array of strings, each representing a nameserver record associated with the domain. These are the addresses of the DNS servers that manage the DNS records for the domain.

### Example

```
{
  "domain": "dappling.fi",
  "Nameservers": [
    {
      "updatedAt": "2024-03-07T04:21:12.193Z",
      "records": [
        "ns-1325.awsdns-37.org.",
        "ns-1809.awsdns-34.co.uk.",
        "ns-456.awsdns-57.com.",
        "ns-581.awsdns-08.net."
      ]
    }
  ]
}
```

### Errors

If the dAppling database is not tracking a particular domain, it will return a 404 Not Found error.



:cactus:_Fun Fact: Some species of bamboo can grow up to 91 cm (36 in) within a 24-hour period, making it one of the fastest-growing plants in the world._
