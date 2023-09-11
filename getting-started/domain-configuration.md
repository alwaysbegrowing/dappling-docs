# Domain Configuration

To add new domains to your project, and to have your new code pushed to them, head over to the project’s domains tab. By default, there is a domain configured for you under the [dappling.network](http://dappling.network) domain.

<figure><img src="../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

#### Adding a custom domain

To add a new domain, put the desired domain. Maybe try with a subdomain of `ipfs`. For example, I would like to add a domain for my site [splitcapta.in](http://splitcapta.in). I would:

1. Enter in [ipfs.splitcapta.in](http://ipfs.splitcapta.in) \*\*\*\*in the domains input
2. Press “Add”
3. Wait for the configuration to load

<figure><img src="../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

4. Head over to the domain registrar. For my case, I use Namecheap, but this process would be similar for different registrars. You will have to see how to add these DNS settings on a case-by-case basis. Look at your DNS documentation to figure out how to do it if you’re not using Namecheap.

<figure><img src="../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

Here is the resulting DNS settings for Namecheap. Notice the “name” is called “Host” and “Value” is called “Value”.

<figure><img src="../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

After the records propagate (this might take a while), the domain will report as validated, but again, the code will not exist at the URL until the next production deployment.

<figure><img src="../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

To do this, head over to the deployments tab or push to your “production” branch on GitHub. The new domain should be shown in the project page. See [Create Deployments](create-deployments.md) for more information about subsequent deployments.

<figure><img src="../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

After that build succeeds, you can see the code at the configured domain: [https://ipfs.splitcapta.in](https://ipfs.splitcapta.in)

#### Google Domains

The same process as above, but add records:

1. navigate the the DNS section
2. make sure you are on default name servers
   1. if not, you will have to change the DNS records wherever the custom name servers are
3. click “manage custom records”

<figure><img src="../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

Then, add the two new CNAME records and click “save”

<figure><img src="../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>



:cactus:_Fun Fact: Plants can communicate with each other through their roots and chemical signals. When a plant is under attack, for example, it releases volatile organic compounds that can warn other plants of the danger._
