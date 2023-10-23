---
description: Understand how the build step works when creating a dAppling Deployment.
---

# Builds

When you create a new project or push a new commit to a project on dAppling, you trigger a deployment. A deployment consists of several steps, with the primary focus on the build step, where dAppling validates and builds your source code, and then stores all assets.

For any of the supported frameworks, dAppling will automatically configure the build settings with the most common configurations for the framework. However, if you have specific settings, you can configure the build, output, and environment variables when you create a new dAppling project or within your project's settings.

## Build Limits

It's important to be aware of certain build limitations on dAppling:

* The maximum duration of a build is 25 minutes. If this limit is reached, the build will be interrupted, and the deployment will fail.
* The build container is allocated a specific amount of resources that can be increased by reaching out to our support.

These limitations are essential to consider when working with dAppling to ensure your deployments run smoothly within the specified constraints.



:cactus:_Fun Fact: Bamboo is the fastest-growing plant; some species can grow up to 35 inches in a single day._
