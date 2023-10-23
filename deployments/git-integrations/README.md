# Git Integrations

dAppling allows for automatic deployments on every branch push and merges onto the Production Branch of your GitHub projects.

Utilizing Git with dAppling offers several advantages:

* Preview Deployments for every push.
* Production Deployments for the most recent changes from the Production Branch.
* Instant rollbacks when reverting changes assigned to a custom domain (coming soon).

When working with Git, designate a branch as your production branch, typically named "main." After creating a pull request (PR) to that branch, dAppling generates a unique deployment for previewing any changes. Once you're satisfied with the changes, you can merge your PR into the main branch, and dAppling will create a production deployment.

You also have the flexibility to select a different branch as the Production Branch if needed.

## Supported Git Providers

* [GitHub Free](https://github.com/pricing)
* [GitHub Team](https://github.com/pricing)
* [GitHub Enterprise Cloud](https://docs.github.com/en/get-started/learning-about-github/githubs-products#github-enterprise)
* [GitHub Enterprise Server](https://vercel.com/guides/how-can-i-use-github-actions-with-vercel)

## Deploying a Git Repository

Setting up your GitHub repository on dAppling is a straightforward process. Simply click the [New Project](https://dappling.network/new) button located at the top right of your dashboard and follow these steps:

1. After clicking the button, you'll see a list of Git repositories associated with the Git account you've signed up with, and that you have write access to.
2. To choose a different Git namespace, you can utilize the dropdown list on the top left of the section.
3. Once you've selected the Git repository you wish to use for your new project, you'll be directed to a page where you can configure your project before deployment.
4. Here, you can:
   * Select a [Framework Preset.](../../legacy-docs/getting-started/frameworks.md)
   * Choose the root directory of your project.
   * Configure Build Output Settings.
   * Set [Environment Variables.](../../projects/environment-variables.md)
5. Once you've ensured that your settings are correct, click the Deploy button to initiate the deployment process.

## Production Branch

Each time you merge to the Production Branch, a Production Deployment will be automatically generated.

### Default Configuration

When you create a new Project from a Git repository on dAppling, the Production Branch will be selected as the git repositories default branch.

### Customizing the Production Branch

In the Project Settings on the Git page, you have the flexibility to change your Production Branch. Whenever a new commit is pushed to the branch you configure here, a Production Deployment will be created.

## Preview Branches

Preview Branches encompass all Git branches except the Production Branch mentioned earlier. For instance, if your Production Branch is named `main` then all Git branches that are not `main` are considered Preview Branches. While there can be multiple Preview Branches, there is only a single Production Branch.

Preview Branches, as the name implies, serve the purpose of previewing changes before making them available to your visitors (by merging them into Production). By default, each Preview Branch automatically receives its unique Domain whenever a commit is pushed to it.

Once you're satisfied with your changes, you can proceed to merge the respective Preview Branch into your Production Branch.



:cactus:_Fun Fact: The smell of freshly-cut grass is actually a plant distress call, signaling damage to other plants._
