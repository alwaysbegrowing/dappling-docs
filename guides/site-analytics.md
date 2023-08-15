# Site Analytics

So you want to know what your users have been up to...

Fortunately, dAppling has an analytics package to make configuring your site analytics quick and easy!

#### Install dappling-analytics in your project

Add the [dappling-analytics package](https://github.com/alwaysbegrowing/dapplingAnalytics) as a module within your project's repository. This is a very simple package that tracks page views and unique users across your site.

Once the package is installed, import that `Analytics` component and add the component to your app. For example, if you are using a Next.js project, import and add the `Analytics` component to the `_app.tsx` file.

```
import { Analytics } from 'dappling-analytics/react'

export default function App({ Component, pageProps }: CustomAppProps) {
  return (
  
      <SessionProvider session={pageProps.session}>
        {Component.public ? (
          <Component {...pageProps} />
        ) : (
          <Auth>
            <Component {...pageProps} />
          </Auth>
        )}
        <Analytics />
      </SessionProvider>
  
  )
}
```

When you push the changes to your main branch, the dAppling app should trigger a production deployment with your new changes. If a new deployment is not triggered, [**create a production deployment**](create-deployments.md) **to deploy the analytics changes**.

Your site is now configured with site analytics and you can watch the views roll in!

#### Analytics Panel

To view your analytics, navigate to the project page on [dAppling.network](https://dappling.network) and select the 'analytics' tab. Here you can view the total number of page views for your entire site, the total number of users, the number of views per page, and your page views over time. Change the time frame for the analytics by using the dropdown menu in the top righthand corner of the page.

<figure><img src="../.gitbook/assets/CleanShot 2023-08-15 at 10.21.54.png" alt=""><figcaption></figcaption></figure>

:cactus:_Fun Fact: The Silene stenophylla, a type of campion flower, was grown from a 32,000-year-old seed discovered in Siberian permafrost._
