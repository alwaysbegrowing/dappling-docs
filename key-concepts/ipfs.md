# IPFS

### Overview

The [InterPlanetary File System (IPFS) ](https://ipfs.tech)is a protocol and network designed to create a content-addressable, peer-to-peer method of storing and sharing data in a distributed file system. dAppling utilizes its decentralized design which presents numerous benefits, making it a valuable tool in Web3 frontend development.&#x20;

### Understanding IPFS

IPFS is a decentralized alternative to the standard [Hypertext Transfer Protocol (HTTP)](https://en.wikipedia.org/wiki/HTTP). Instead of relying on a central location to request and receive data, IPFS operates on a distributed network of nodes that find and deliver data based on its content, not its location. This content-addressability ensures that data isn't tied to a specific location and can be served by any node that holds it.

#### How IPFS Works&#x20;

1. **Content Identifiers (CIDs)**: Every file and all of the blocks within those files are given a unique content identifier (CID). This CID is a cryptographic hash of the content in the file. If any part of the file changes, the CID changes too. This system allows IPFS to track each piece of content and every version of it, providing an inherent version control mechanism. It also provides de-duplication since identical files (with the same CID) won't be stored multiple times.
   * On dAppling, each successful deployment is assigned a CID. You can access this through the project overview page, or on the individual deployment page. The CID you receive on dAppling is the IPFS CID, meaning you can use it to directly access your content through IPFS. However, dAppling also makes accessing IPFS deployments simple by pinning the files and assigning it a stable name using IPNS.
2. **Distributing Content:** When a node looks to access a file, it uses the CID to request the file from the IPFS network. Because files are broken into blocks, the requesting node can fetch different blocks from different nodes. This means that the speed of data retrieval isn't limited by a single server's capacity and can result in faster delivery times.
3. **Data Persistence**: IPFS operates with a model called "unpinning" and "pinning". By default, files retrieved by a node are cached or "pinned" to that node for a short period and then discarded to free up space, a process known as "unpinning". However, if a node wants to ensure the persistence of a file on the network, it can choose to "pin" the file permanently. This allows the node to serve that file to others even if the original provider goes offline.
   * dAppling automatically pins all deployments using filebase for quick, easy access to your content.
4. **Decentralized Naming System**: IPFS also includes a decentralized naming system called IPNS (InterPlanetary Naming System). While CIDs in IPFS are great for content-addressability, they change every time the content changes. If you want to keep a stable name while updating the content, you can use IPNS. With IPNS, you can create a mutable pointer to your content and update it as your content changes.
5. **Transport Protocols**: IPFS isn't tied to a specific method of moving data. Instead, it works on top of other network transport protocols like TCP, UDP, and others. This makes it versatile and adaptable to various network conditions.

### Importance of IPFS

With the ever-increasing volume of data being created, shared, and consumed, the limitations of traditional data storage and transfer methods are being tested. Centralized systems are vulnerable to outages, censorship, and attacks. Additionally, they can create data inefficiencies and redundancies. IPFS is designed to address these issues, allowing for a more robust, efficient, and resilient web.

### Benefits of IPFS

#### Decentralization and Redundancy

With IPFS, files and data are distributed across multiple nodes in the network. This decentralization means there's no single point of failure. If one node goes down, the data can still be accessed from another node. This redundancy enhances the reliability and robustness of data storage and retrieval.

#### Efficiency

IPFS allows nodes to fetch data from the closest or fastest nodes available, not just from a central server. This results in faster data transfer times and less strain on the network. In addition, identical files are stored only once in the network, saving storage space and further increasing efficiency.

#### Permanence and Version Control

Content in IPFS is identified by its hash, which changes with every modification to the file. This makes it possible to track versions of files and datasets over time. Even if the original provider of the file goes offline, the content can still be available from other nodes.

#### Resistance to Censorship

Since there's no central authority in IPFS, it's much harder to censor or control data. Information can't be manipulated or removed by a single entity, preserving the democratic nature of information.

### Conclusion

IPFS represents a significant step forward in the way we handle data on the web. With its decentralized design, it ensures more reliable, efficient, and resilient data storage and transfer. The system's resistance to censorship and support for version control also contributes to a more democratic and open internet. Though there are challenges in implementing and operating within the IPFS network, the potential benefits are substantial and well-suited to Web3 protocols.&#x20;
