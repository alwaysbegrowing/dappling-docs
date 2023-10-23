# Package managers

dAppling will automatically detect the package manager used in your project and install the dependencies during deployment. This detection is based on the lock file present in your project, which allows dAppling to infer the correct package manager to use.

## Supported package managers

Here are the supported package managers along with their install commands and versions

| Package Manger | Lock File           | Install Command | Versions |
| -------------- | ------------------- | --------------- | -------- |
| yarn           | `yarn.lock`         | `yarn install`  | 1        |
| npm            | `package-lock.json` | `npm install`   | 6,7,8    |
| pnpm           | `pnpm-lock.yaml`    | `pnpm install`  | 6,7,8    |
| bun            | `bun.lockb`         | `bun install`   | 1        |

\
While dAppling automatically selects the package manager based on your project's lock file, the specific version of that package manager is determined by the version information in the lock file or associated configuration files.

## Manually specifying a package manager

If you wish to manually specify a package manager for all deployments in your project, you can use the build setting in your project's [Build & Development Settings](configure-a-build.md). Follow these steps:

1. Navigate to your dashboard and select your project.
2. Select the Settings tab.
3. Add your desired install command. Once saved, it will be applied in your next deployment.



:cactus:_Fun Fact: The world's most poisonous plant is the castor bean plant; just one bean can kill a human._
