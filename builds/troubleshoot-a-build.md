# Troubleshoot a Build

## Troubleshoot Build Failures

If your build encounters an issue, dAppling will report the error message on the Deployments page, allowing you to investigate and address the underlying problem.&#x20;

### Investigating Build logs

Build logs offer insights into what occurred during the deployment build and can be accessed by following these steps:

* From your dAppling dashboard, select the project, and then navigate to the Deployments tab.
* Choose the specific deployment. When there are build issues, you will notice an error status next to the deployment name.

On the deployment's page with an error status, you'll find a summary of the error in the preview section. In the Deployment Details section, expand the Building accordion to access the logs.

Scroll through the build logs until you find a red section with the keyword "Error." This keyword may appear once or multiple times. In many cases, the last mention of "Error" may not provide the most indicative information. Look a few lines above to find additional error messages, which can help pinpoint the problem. Sometimes, errors may not be explicitly mentioned, but the output often contains clues about the issue's location.

### Preventing Build Issues

It is advisable to build your project on your local machine first, using the build command specific to your project. This helps catch issues that are specific to your code or your project's dependencies. For instance, if you encounter an error from `npm run build` locally, you can address it before deploying on dAppling.

### Build Duration

The total build duration is shown on the deployments page.

Please note that a build can last a maximum of 25 minutes. If the build exceeds this time limit, the deployment will be canceled, and the error will be shown in the Deployment's Build logs. If you encounter this limit, reach out to our support.
