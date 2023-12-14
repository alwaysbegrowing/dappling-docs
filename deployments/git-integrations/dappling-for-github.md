# dAppling for Github

dAppling for GitHub automates the deployment of your GitHub projects with dAppling. It offers Preview Deployment URLs and automatic updates for Custom Domains.

## Supported Github Products

* [GitHub Free](https://github.com/pricing)
* [GitHub Team](https://github.com/pricing)
* [GitHub Enterprise Cloud](https://docs.github.com/en/get-started/learning-about-github/githubs-products#github-enterprise)
* [GitHub Enterprise Server](https://vercel.com/docs/deployments/git/vercel-for-github#using-github-actions)

## A Deployment for Each Push

dAppling for GitHub will deploy every push by default. This includes pushes and pull requests made to branches. This allows those working within the repository to preview changes made before they are pushed to production.

With each new push, if dAppling is already building a previous commit, the current build will be canceled to build the most recent commit so that you always have the latest changes deployed as quickly as possible.

## Updating the Production Domain

When[ Custom Domains](../../domains/) are configured through a project's domains dashboard, any pushes or merges to the Production Branch (often named "main") will make the latest deployment from a push live on those domains.

## Preview URLs for the Latest Changes for Each Pull Request

The most recent push to any pull request will be automatically accessible at a unique preview URL. This URL is derived from the project name, branch, and team or username. You can find these URLs conveniently provided through a comment on each pull request.



:cactus:_Fun Fact: The stinging nettle has tiny, hair-like needles that inject histamine and other chemicals when touched, causing that well-known stinging sensation._
