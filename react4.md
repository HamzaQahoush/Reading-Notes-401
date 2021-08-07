## Dynamic Routes

Next.js allows you to statically generate pages with paths that depend on external data. This enables dynamic URLs in Next.js.


<img src="https://nextjs.org/static/images/learn/dynamic-routes/page-path-external-data.png" >

## Here’s a graphic summary of what we just talked about:

<img src="https://nextjs.org/static/images/learn/dynamic-routes/how-to-dynamic-routes.png" >

## Implement getStaticProps

<img src="https://nextjs.org/static/images/learn/dynamic-routes/how-to-dynamic-routes.png">

## Deploying 

1.Push to GitHub

2. Deploy to Vercel
The easiest way to deploy Next.js to production is to use the Vercel platform developed by the creators of Next.js.

Vercel is a serverless platform for static and hybrid applications built to integrate with your headless content, commerce, or database. We make it easy for frontend teams to develop, preview, and ship delightful user experiences, where performance is the default. You can start using it for free — no credit card required.


Develop, Preview, Ship
We’ve just gone through the workflow we call DPS: Develop, Preview, and Ship.

Develop: We’ve written code in Next.js and used the Next.js development server running to take advantage of its hot reloading feature.
Preview: We’ve pushed changes to a branch on GitHub, and Vercel created a preview deployment that’s available via a URL. We can share this preview URL with others for feedback. In addition to doing code reviews, you can do deployment previews.
Ship: We’ve merged the pull request to main to ship to production.
We strongly recommend using this workflow when developing Next.js apps — it will help you iterate on your app faster.


## Other Hosting Options
Next.js can be deployed to any hosting provider that supports Node.js.

If you’ve followed the instructions so far, your package.json should have the following build and start scripts

In your own hosting provider, run the build script once, which builds the production application in the .next folder.


`npm run build`

After building, the start script starts a Node.js server that supports hybrid pages, serving both statically generated and server-side rendered pages, and API Routes.


`npm run start`
