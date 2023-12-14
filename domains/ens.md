---
description: dAppling has support for both ENS and DNS domains.
---

# ENS

## Introduction to Ethereum Name Service (ENS)

ENS is a decentralized domain name system built on the Ethereum blockchain. It allows users to assign human-readable names to cryptocurrency addresses, content hashes, and metadata, much like how traditional DNS works.

### ENS vs Traditional DNS

Unlike DNS, which operates on centralized servers, ENS runs on a decentralized network, offering enhanced security and resistance to censorship.

### The ENS Naming Process

ENS uses `.eth` domains, making web addresses more accessible and memorable. For example, `yourproject.eth` can be an address for your website.

### Setting Up a Website with ENS

To host a website using ENS, you first need to acquire an `.eth` domain. You can purchase one at ENS Domains ([https://ens.domains/](https://ens.domains/))&#x20;

### Integrating ENS with Your Website

Once you have an ENS domain, you can add it with the dAppling app. We set the contenthash of your ENS name to your website's IPFS hash.

### ENS Resolution Process

When a user enters your `.eth` domain, ENS resolves this into a machine-readable content hash, which then retrieves your website content.

### The Role of Ethereum Smart Contracts in ENS

ENS relies on smart contracts for managing domain registrations and record updates, providing a trustless and automated system.

### Why ENS?

Front-end hacks, as seen in recent incidents with platforms like Balancer, Velodrome, and Frax, reveal the vulnerabilities inherent in the traditional domain name systems (DNS).

#### Benefits of Using ENS for Web Hosting

1. **Enhanced Security Against Social Engineering Attacks**: ENS domains offer a higher level of security against social engineering attacks, which have been used to manipulate service providers into redirecting DNS records to malicious sites. ENS operates on the Ethereum blockchain, making it inherently resistant to such attacks due to its decentralized nature.
2. **Decentralization**: ENS is built on the Ethereum blockchain, which means it's decentralized. This decentralization reduces the risk of a single point of failure, which is a common issue with traditional DNS providers.
3. **Reduced Risk of DNS Hijacking**: Since ENS domains are blockchain-based, they are not susceptible to traditional DNS hijacking methods. The control of an ENS domain is determined by the possession of a corresponding private key, making unauthorized changes to DNS records significantly more challenging.
4. **Ownership and Control**: ENS domains provide users with full ownership and control over their domain. Unlike traditional domain names, where the registrar has ultimate control, ENS domain owners have complete authority over their domain without any intermediary.
5. **Transparent and Immutable Record Keeping**: All changes and transactions made in ENS are recorded on the Ethereum blockchain, ensuring transparency and immutability. This feature aids in tracking and verifying any alterations made to a domain, providing an additional layer of security.
