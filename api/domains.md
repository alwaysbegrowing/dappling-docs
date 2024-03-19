---
description: >-
  This GET route fetches domain items for which dAppling is monitoring
  nameserver changes.
---

# /domains

## Request

The request object must be formatted as a GET request. The only required header is for [Authentication](./#authentication).&#x20;

### Examples

```markup
curl --location 'https://dappling.network/api/v1/domains' \
--header 'Authorization: {DAPPLING_AUTH_TOKEN}'
```

```javascript
const myHeaders = new Headers();
myHeaders.append("Authorization", {DAPPLING_AUTH_TOKEN});

const requestOptions = {
  method: "GET",
  headers: myHeaders
};

fetch("https://dappling.network/api/v1/domains", requestOptions)
  .then((response) => response.json())
  .then((result) => console.log(result))
  .catch((error) => console.error(error));
```

## Response

The /domains endpoint returns a 200 status code with an array of the 25 most recent nameserver changes for each domain dAppling is tracking.

### Structure

* **domain**: domain name of the record
* **Nameservers:** an array that contains objects with details about the nameservers associated with the domain
  * Within each "Nameservers" object:
    * **updatedAt:** the last update time of the nameserver records for the domain
    * **records:** an array of strings, each representing a nameserver record associated with the domain. These are the addresses of the DNS servers that manage the DNS records for the domain.

### Example

```json
[
  {
    "domain": "altbox.one",
    "Nameservers": [
      {
        "updatedAt": "2024-03-10T08:35:52.770Z",
        "records": [
          "ns1.3dns.box.",
          "ns2.3dns.box."
        ]
      }
    ]
  },
  {
    "domain": "ottoinbio.it",
    "Nameservers": [
      {
        "updatedAt": "2024-03-10T02:36:25.403Z",
        "records": [
          "bart.ns.cloudflare.com.",
          "becky.ns.cloudflare.com."
        ]
      }
    ]
  },
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
  },
  {
    "domain": "basedlabs.wtf",
    "Nameservers": [
      {
        "updatedAt": "2024-03-06T00:48:18.493Z",
        "records": [
          "ns1.3dns.box.",
          "ns2.3dns.box."
        ]
      }
    ]
  },
  {
    "domain": "lookbeforeyou.link",
    "Nameservers": [
      {
        "updatedAt": "2024-03-08T07:35:31.981Z",
        "records": [
          "ns1.vercel-dns.com.",
          "ns2.vercel-dns.com."
        ]
      },
      {
        "updatedAt": "2024-03-05T04:00:00.792Z",
        "records": [
          "ns3.vercel-dns.com.",
          "ns4.vercel-dns.com."
        ]
      }
    ]
  },
  {
    "domain": "holistichospitality.one",
    "Nameservers": [
      {
        "updatedAt": "2024-03-04T20:55:15.570Z",
        "records": [
          "ns1.3dns.box.",
          "ns2.3dns.box."
        ]
      }
    ]
  },
  {
    "domain": "adventourz.com",
    "Nameservers": [
      {
        "updatedAt": "2024-03-06T09:26:09.596Z",
        "records": [
          "ns63.domaincontrol.com.",
          "ns64.domaincontrol.com."
        ]
      },
      {
        "updatedAt": "2024-03-03T10:07:25.207Z",
        "records": [
          "ns23.domaincontrol.com.",
          "ns24.domaincontrol.com."
        ]
      }
    ]
  },
  {
    "domain": "ggpvault.com",
    "Nameservers": [
      {
        "updatedAt": "2024-03-01T03:45:19.955Z",
        "records": [
          "dns1.registrar-servers.com.",
          "dns2.registrar-servers.com."
        ]
      }
    ]
  },
  {
    "domain": "seafi.app",
    "Nameservers": [
      {
        "updatedAt": "2024-03-01T03:45:19.980Z",
        "records": [
          "dns1.registrar-servers.com.",
          "dns2.registrar-servers.com."
        ]
      }
    ]
  }
]
```



:cactus:_Fun Fact: The orange carrot was developed in the 17th century in the Netherlands. Before that, carrots were primarily purple, white, or yellow._
