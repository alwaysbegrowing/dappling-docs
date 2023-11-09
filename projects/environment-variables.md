# Environment Variables

Environment Variables are key-value pairs configured outside your source code.

Your source code can read these values to change behavior during the Build Step.

dAppling does not support server side code or functions. This means that we only support environment variables that are consumed by the frontend during the build process. These variables will therefore be **public and unencrypted**. All environment variable values will be visible within the build files and to any user that has access to the [Project](./).&#x20;

{% hint style="danger" %}
**To ensure the security of your application, do not add sensitive information, such as API keys or secrets, as environment variables.**&#x20;
{% endhint %}

Changes to Environment Variables are not applied to previous deployments, they only apply to new deployments.

## Declare an Environment Variable

To declare an Environment Variable for your deployment, go to the Environment Variables section of your Project Settings.

Most frameworks have specific requirements for the naming of environment variables. For example Create React App requires frontend env variables to be prefixed with `REACT_APP_.`  If the variables are not named with the correct framework prefix, they will not be embedded during the build process.

### Framework Environment Variable Documentation

* [Create React App](https://create-react-app.dev/docs/adding-custom-environment-variables/)
* [NextJs](https://nextjs.org/docs/app/building-your-application/configuring/environment-variables)
* [Vite](https://vitejs.dev/guide/env-and-mode.html)
* [Vue](https://cli.vuejs.org/guide/mode-and-env.html)



:cactus:_Fun Fact: Apples belong to the rose family, Rosaceae, along with pears and plums._
