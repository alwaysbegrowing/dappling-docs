# ENS Configuration

We offer two different ways of integrating ENS with your project.

### dappling.eth Subdomain

ENS names can be a useful way of disseminating your site to your users. However, they can be expensive. Because we own the dappling.eth ENS name, we are able to assign every project deployed through dAppling a dappling.eth ENS subdomain.&#x20;

We use [NameStone](https://namestone.xyz/) to set and maintain these subdomains.&#x20;

Whenever a project is deployed, a dappling.eth subdomain is automatically assigned to it. This can be edited or deleted as needed.&#x20;

_Note: dappling.eth ENS subdomains cannot be added to projects. If you want to update the subdomain, choose to edit it, as opposed to deleting and re-adding. If you delete the subdomain you will not be able to add a new one to your project._

<figure><img src="../../.gitbook/assets/CleanShot 2023-09-06 at 13.44.26@2x.png" alt=""><figcaption></figcaption></figure>

### ENS Name

To add your own ENS name to your project, navigate to the domains tab and add your ENS name.

1. Type your ENS name in the `Associate ENS Name` card.
2. Press "Add"

<figure><img src="../../.gitbook/assets/CleanShot 2023-09-06 at 12.14.30@2x.png" alt=""><figcaption></figcaption></figure>

3. Connect your wallet.

<figure><img src="../../.gitbook/assets/CleanShot 2023-09-06 at 12.13.34@2x.png" alt=""><figcaption></figcaption></figure>

4. By selecting "Set Content Hash" you will initiate a transaction to set the hash of the project's IPNS key to the content hash of the ENS.&#x20;

Every time you create a new deployment, a new CID is created. Behind the scenes, we update the IPNS associated with your site to point to the new CID. Therefore, while your production CID will change every time you make a change to your project, your IPNS never does. Because we use the IPNS key (which is mutable) instead of the production CID (which is immutable), you will never have to reset the content hash on your ENS unless you want to move it to a different site. dAppling uses IPNS to make assigning the content hash of your ENS name cheap and easy. Your ENS name will always point to the correct version of your site, without you having to spend gas and time updating the content hash.

<figure><img src="../../.gitbook/assets/CleanShot 2023-09-06 at 12.24.10@2x.png" alt=""><figcaption></figcaption></figure>

5. Complete the transaction within your wallet.
6. The ENS domain card will signal the valid ENS configuration once the transaction has successfully been completed.

<figure><img src="../../.gitbook/assets/CleanShot 2023-09-06 at 13.50.37@2x.png" alt=""><figcaption></figcaption></figure>

7. :tada::tada: Celebrate!! Your ENS name is now pointing to your production CID. You can now navigate to {ENS name}.eth.limo to view the linked content.



:cactus:_Fun Fact: Studies have shown that plants can actually "hear" running water, and their roots will grow towards the sound._
