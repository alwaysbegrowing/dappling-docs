---
description: dAppling has support for both ENS and DNS domains.
---

# Domains

## Introduction to Domains

A domain is like an easy-to-remember address for a website on the internet, such as `dAppling.network`.

### DNS: The Domain Name System

DNS translates human-friendly domain names to computer-readable IP addresses, a process known as DNS resolution.

### The DNS Query Process

Here's how a DNS query unfolds:

1. **User's Request:** Enter a domain like `example.dAppling.network` in your browser.
2. **Recursive Resolver:** If the IP is not cached, the browser queries a recursive resolver.
3. **DNS Server Hierarchy:** The resolver consults a series of DNS servers.
4. **IP Address Retrieval:** The authoritative nameserver provides the IP address.

### DNS Network Hierarchy

DNS is structured hierarchically with root, TLD, and authoritative nameservers.

### Efficiency in DNS Queries

DNS queries are optimized for speed, with caching mechanisms in browsers and resolvers.

### Developer Perspective: Setting Up a Site on dAppling.network

Deploying a project on dAppling.network requires configuring DNS settings to point your domain to the correct IP address.

### Configuring DNS Settings on dAppling.network

Your Dashboard provides guidance on setting various DNS records.

### Key DNS Records and Their Functions

* **CNAME (Canonical Name)**
* **A (Address)**
* **NS (Nameserver)**
* **MX (Mail Exchange)**

### SSL Certificates

SSL Certificates ensure a secure connection from your domain to your website.

***

:cactus:_Fun Fact: Cactus can perform photosynthesis at night, unlike most plants, which only do so during the day._
