# Create Deployments

So your app was deployed upon initial creation. We automatically assigned a “production” URL for you which looks something like [https://honeysuckle-aloe-tgsrtj6.dappling.network/](https://honeysuckle-aloe-tgsrtj6.dappling.network/). Each deployment will also create a similar looking “preview” domain.

There are two ways we deploy your app

1. manual deployment
2. automatic deployment through GitHub

### Manual Deployment

If you navigate to the deployments tab of your project, you’ll see two buttons to deploy your app manually. There is a preview and production build option.

<figure><img src="../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

#### Production

On every “production” deployment, we will take your configured production branch (see the settings tab) and create a build. After the build is complete, we will assign both

* your production URL, which never changes through the life of the project
* your configured domains (see the domains tab)

For example, if you configured a domain at [https://ipfs.example.com](https://ipfs.example.com), after a successful production deployment, your users will see the new code at the [https://ipfs.example.com](https://ipfs.example.com) domain.

#### Preview

For each preview build, we go through the same build process as well as using the production branch, but the production domain as well as the configured domains in the domains tab are not updated. instead, we create a newly generated preview url that looks like [https://chive-lily-zfiuy3b.dappling.network](https://chive-lily-zfiuy3b.dappling.network) This preview URL will never be updated again.

<figure><img src="../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

#### Project page while deploying

<figure><img src="../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

#### Deployment page while deploying

<figure><img src="../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

### GitHub Deployment

Like the manual deployment we have production and preview deployments through GitHub automatically upon PR creation.

#### Production

On any push to “main” including when a PR is merged into main, a production deployment is kicked off. You can see this in the project’s deployments.

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

#### Preview

When a PR is created and any subsequent pushes to the PR, a preview build is created. This preview build is visible in your project’s deployments as well. It will notify you that it is building first.

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

After it’s built, you can view the preview URL right in the PR.

<figure><img src="../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>



:cactus:_Fun Fact: The world's largest flower, Rafflesia arnoldii, can grow to nearly 3 feet in diameter. Ironically, it has a scent akin to rotting flesh._
