# React 4

---
## Next.js - Dynamic Routes

How to Statically Generate Pages with Dynamic Routes
In our case, we want to create dynamic routes for blog posts :


- We want each post to have the path /posts/<id>, where <id> is the name of the markdown file under the top-level posts directory.
- Since we have ssg-ssr.md and pre-rendering.md, we’d like the paths to be /posts/ssg-ssr and /posts/pre-rendering.

***Overview of the Steps***

We can do this by taking the following steps. You don’t have to make these changes yet — we’ll do it all on the next page.

First, we’ll create a page called [id].js under pages/posts. Pages that begin with [ and end with ] are dynamic routes in Next.js.

In pages/posts/[id].js, we’ll write code that will render a post page — just like other pages we’ve created.


```
import Layout from '../../components/layout'

export default function Post() {
  return <Layout>...</Layout>
}
```

---
## Next.js Deployment

***Push to GitHub***

Before we deploy, let’s push our Next.js app to GitHub if you haven’t done so already. This will make deployment easier.

On your personal GitHub account, create a new repository called nextjs-blog.
The repository can be public or private. You do not need to initialize it with a README or other files.
If you need help setting up your repo, take a look at this guide on GitHub.
Then:

If you haven’t initialized the git repository locally for your Next.js app, do so now.
Push the Next.js app to your GitHub repository.

To push to GitHub, you can run the following commands (replace <username> with your GitHub username):

> git remote add origin https://github.com/<username>/nextjs-blog.git


> git push -u origin main

Once your GitHub repository is ready, continue to the next page.


![Next.js](https://hassancorrigan.com/static/4f9e4d81dd3f2d4c1a39d6ee27bbf002/ace28/nextjs-back-button.jpg)


***Deploy to Vercel***

The easiest way to deploy Next.js to production is to use the Vercel platform developed by the creators of Next.js.

Vercel is a serverless platform for static and hybrid applications built to integrate with your headless content, commerce, or database. We make it easy for frontend teams to develop, preview, and ship delightful user experiences, where performance is the default. You can start using it for free — no credit card required.

***Next.js and Vercel***

Vercel is made by the creators of Next.js and has first-class support for Next.js. When you deploy your Next.js app to Vercel, the following happens by default :

Pages that use Static Generation and assets (JS, CSS, images, fonts, etc) will automatically be served from the Vercel Edge Network, which is blazingly fast.


Pages that use Server-Side Rendering and API routes will automatically become isolated Serverless Functions. This allows page rendering and API requests to scale infinitely.

---
## Sources and references

- ***[Next.js - Dynamic Routes .](https://nextjs.org/learn/basics/dynamic-routes)***

- ***[Next.js - Deployment .](https://nextjs.org/learn/basics/deploying-nextjs-app)***

- ***[ Next.js 10 is here .](https://www.youtube.com/watch?v=JWCS5IdECVI)***

- ***[Next.js - Static File Serving .](https://nextjs.org/docs/basic-features/static-file-serving)***

---
#### **[Back To Home Page](https://mhmadwrekat.github.io/reading-notes)**

---
<b>
<p align="center">
© Mohammad alwrekat
</p>
