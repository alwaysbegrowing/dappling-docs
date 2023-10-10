# IPNS

### Overview of IPNS (InterPlanetary Naming System)

[IPNS](https://docs.ipfs.tech/concepts/ipns/#mutability-in-ipfs), which stands for InterPlanetary Naming System, is an important part of the IPFS ecosystem. While IPFS provides a way to access files based on their content, IPNS provides a way to access files based on a stable identifier. This makes it easier to manage and reference files that may change over time.

### How IPNS Works

**Mutable Identifiers**

The key feature of IPNS is its ability to provide mutable identifiers, as opposed to the immutable content identifiers (CIDs) that IPFS uses. When content changes, its CID in IPFS changes too, making it a bit inconvenient for frequently updated resources like websites. IPNS solves this by providing a constant name (identifier) for changing content.

**Name Publishing**

An IPNS name is essentially a public-private key pair. The public key is the name, and the owner uses the corresponding private key to sign records, providing proof of ownership. When you want to update the content that your IPNS name points to, you create a new IPFS record, sign it with your private key, and then broadcast that information to the network.

**Time-to-Live (TTL)**

IPNS records come with a Time-to-Live (TTL) feature, meaning they expire after a set amount of time. This ensures that you don't access outdated pointers, and it allows content owners to update their records accordingly.

### Benefits of IPNS

**Dynamic Content**

IPNS is invaluable for serving dynamic content that changes over time. With IPNS, you can keep the same identifier while changing the content it points to.

**Versioning and Redirection**

Since IPNS names can point to different content at different times, they can be used for versioning. You can easily redirect an IPNS name to point to the latest version of your content.

**Decentralization and Security**

Like IPFS, IPNS benefits from being a part of a decentralized system. The use of cryptographic key pairs ensures that only the owner can update the content that an IPNS name points to, adding an extra layer of security.

### Use Cases

**Decentralized Websites**

Decentralized applications (dApps) and websites can use IPNS to maintain stable URLs while their content changes.

dAppling uses IPNS to make assigning the content hash of your ENS name cheap and easy. By setting your ENS name's content hash to be the IPNS key as opposed to the CID, and updating the IPNS name to point to your most recent production CID on each deployment, your ENS name will always point to the correct version of your site, without you having to spend gas and time updating the content hash.

#### Conclusion

IPNS provides a critical layer of functionality atop IPFS, enabling mutable pointers to immutable content. It offers the best of both worlds, combining the permanence and integrity of CIDs with the flexibility of mutable identifiers.

