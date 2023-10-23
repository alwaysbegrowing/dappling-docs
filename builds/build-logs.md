# Build Logs

When you deploy your website to dAppling, the platform generates build logs that display the deployment progress. These build logs contain information about:

* The version of the build tools used.
* Warnings or errors encountered during the build process.
* Details about the files and dependencies that were installed, compiled, or built during the deployment.

Build logs are an invaluable resource for debugging issues that may arise during deployment. If a deployment encounters problems, these logs can assist you in pinpointing the root cause.

To access the build logs, simply navigate to a deployment and scrroll down to the build logs section.

## How build logs work?

Build logs are generated during the build process for all deployments. These logs closely resemble the output of your framework's Build Command, with some minor additions from the dAppling build system. It's important to note that once a build is complete, no new logs will be recorded.

In addition to the list of build actions, you can identify errors or warnings in the logs. These are highlighted with different colors, such as yellow for warnings and red for errors. This color coding provides flexibility in investigating why your build may have failed and which part of your website is affected. It's worth mentioning that build logs are stored indefinitely for each deployment, ensuring you have access to historical information as needed for debugging and analysis.



:cactus:_Fun Fact: Rhubarb leaves are poisonous due to high levels of oxalic acid, even though the stalks are edible._
