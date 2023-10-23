# Configure a Build

When you initiate a deployment on dAppling, the platform builds your project. During this process, dAppling performs a clone on your repository.&#x20;

dAppling automatically configures build settings for various front-end frameworks, but you can also customize these settings to suit your project's requirements. To configure your dAppling build with customized settings, follow these steps:

1. Choose a project from the dashboard.
2. Go to its Settings tab.

## Build and Development Settings

If you want to override settings or specify a different framework, you can do so from the Build & Development Settings section.

### Framework Preset

You have a wide range of frameworks to choose from, including Next.js, Svelte, and Vite. In many cases, dAppling automatically detects your project's framework and sets the best settings for you. You can use the drop-down menu inside the Framework Preset settings to select the framework of your choice. This selection will be applied to all deployments within your project.

* [Next.js](https://nextjs.org/docs)
* [Create React App](https://create-react-app.dev/docs/getting-started/)
* [Vite](https://vitejs.dev/)
* Svelte
* Vue
* 11ty
* No Framework

However, if no framework is detected, "Other" will be selected. In this case, the Override toggle for the Build Command will be enabled by default so that you can enter the build command manually. The remaining deployment process is that for default frameworks.

### Build Command

dAppling automatically configures the Build Command based on the framework. If you want to override the Build Command for all deployments in your project, you can specify a custom command.

### Output Directory

After building a project, most frameworks output the resulting build in a directory. Only the contents of this Output Directory will be served statically by dAppling.&#x20;

If dAppling detects a framework, the output directory will automatically be configured.&#x20;

If you update the Override setting, it will be applied on your next deployment.&#x20;

&#x20;If your project doesn't have a public directory, it will serve the files from the root directory.&#x20;

### Install Command

dAppling automatically detects the install command during the build step. It installs dependencies from package.json

For more details, refer to the documentation on manually specifying a package manager. To find out which package managers are supported on dAppling, consult the [package manager support documentation](package-managers.md).

## Root Directory

In some projects, the top-level directory of the repository may not be the root directory of the app you'd like to build. For instance, your repository might contain a front-end directory with a standalone Next.js app. For such scenarios, you can specify the project's Root Directory.&#x20;



:cactus:_Fun Fact: The concept of a "Zen garden" originated in Japan and is meant to imitate the essence of nature, not its actual appearance._
