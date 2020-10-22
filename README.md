# Sanity + Next.js + Vercel example

> A bare bones example of a Vercel-deployable project with a Next.js frontend and a Sanity Studio on /studio

## Getting started

1. Clone repo
    ```
    git clone https://github.com/sanity-io/sanity-nextjs-examle
    ```
1. Install dependencies
    ```
    npm install
    ```
1. Setup Sanity
    ```
    cd studio && sanity init
    ```
    This will prompt you if you want to reconfigure the project. Answer yes and follow instructions to create a new project.
1. Setup Vercel deployment
    ```
    vercel
    ```
   When asked about build settings, make sure to use `npm run dev` as the development command 

## Notes
In development (using `npm run dev`)
- The Next.js application will run on https://localhost:3000
- The Sanity Studio dev server will run on http://localhost:3333/studio
 
In production (`using vercel`)
- The Next.js application will be available on `https://<your-domain>` 
- The Sanity Studio will be accessible on `https://<your-domain>/studio` 
