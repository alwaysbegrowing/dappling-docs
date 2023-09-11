# Deploy a New Project

#### Creating your first project

On your dashboard, your projects will be empty. After you create a project, this dashboard will show all of the projects that exist. After the first one is added, the main button will disappear, but there is always the “+ New Project” button near your username.

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

On the new project magician, you will first need to connect an account. On subsequent project deployments, all of the repos that you authorize here will be available and will not need to be re-added. After clicking connect account, a pop-up will ask to give permissions. These permissions affect the repositories that you explicitly allow.

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

After you’ve connected your repositories, you will see your accounts in the account dropdown. Select the one with the repo you want to deploy.

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

#### Configure your app’s settings

Nice! Now we should be seeing a screen with one of two things.

1. we have not detected your project type. You will see only a framework selector.

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

2. we have detected your project! You will see some of the build commands partially filled out

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

In either case, you should select and double check the settings for your project. If you need help selecting the settings, there are some informational bubbles next to each for more information.

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

#### Build commands.

The ideal way to figure these out would be letting our app auto-detect the settings. However, we realize that all of the edge-cases cannot be covered so there may be some manual steps you will have to do. We recommend you build your code locally first, see where the resulting files are saved to, and then use that knowledge to fill out the settings. If you can find a built “index.html” file, that’s a good sign.

**Framework:** These are the app types that we support currently. React projects created using [Create React App](https://create-react-app.dev/), [NextJs](https://nextjs.org/), and ones without any framework, for example a static site. There is also an “other” choice that may work for your app-type, but we have not done extensive testing with all types. We would be happy to help work through your project. Just hit the green chat icon in the bottom right!

**How do you install dependencies?** This is the package manager that your project uses. We auto-detect this based on the lock file within the code directory. It’s the command used for your initial installation like `npm i`. Do note, we might not have found your code because it is located in a sub-directory. That would be changed in the **Root Directory**. More on that below.

**How do you export your project?** This is a tricky one. Since your app needs to be deployed as a “static” website, this may be abnormal for your regular dev flow. For NextJs as an example, the export commands you need to run are

* `next build`
* `next export`

You’ll see the recommendation is `npx next build && npx next export` which uses [npx](https://www.npmjs.com/package/npx) to call the necessary next commands within your project’s scope.

**Where are the exported files located?** Similar to the exporting of the project, the export directory might be something new to you as well. When you build your project, the static files will go into a folder within your root directory most likely. These are the files that we will upload to serve the app. For NextJs, the directory is “out” by default, and for CRA, it’s “build”.

**Which branch is your production branch?** finally a straight-forward setting! This should be the branch that has the “live” or “production” code for your app. This will be used for what we call “production deployments” and are pushed out to your configured domains.

**Node Version** is the NodeJS version used in your project. By default, we build projects using version 18 (version 16 for Create React App projects). If your project requires a different version, make sure to select that version or it will not build correctly. If you are unsure what version is required for your project, run `node -v` in your terminal or check the `engines` section of your `package.json` file.&#x20;

**Root Directory** is the place in your GitHub repository where the entrypoint of your code is. That usually means it’s either the place where your “package.json” file is located or the “index.html” file of your static site.

Again, if you need any help, please reach out. We want to improve this process as much as we can!

#### Deploy the project

After that is all configured, go to the next page. If there are red errors, your project will likely not deploy. Yellow warnings will likely deploy, but highlight problems potentially worth looking into.

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

You will be presented with the deployment screen which means that your app is being built. After it is complete the page will refresh showing that the build process is complete.

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

Clicking on “View Logs” will take you to the deployment page where you can view the progress of the actual deployment.

<figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

#### Celebrate?

Shortly after, your first project should be deployed! woo hoo!

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

If this screen doesn’t appear so happy, something must have gone wrong. Again, please reach out as we’re trying to improve our app.



:cactus:_Fun Fact: A single teaspoon of garden soil can hold up to one billion bacteria along with various species of fungi, protozoa, and nematodes. These microorganisms help in nutrient cycling and maintaining soil fertility._
