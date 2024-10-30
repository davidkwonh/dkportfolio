---
layout: ../../layouts/LayoutBlogPost.astro
title: "My First Blog Post"
date: "2024-10-29"
description: "A short intro to my journey building this blog."
---

## Building and Deploying My First Blog with Astro and Netlify 🚀

Creating and deploying my first profile and blog entry with [Astro](https://astro.build/) and [Netlify](https://www.netlify.com/) was both a learning experience and a fun dive into the world of static site generation. I wanted a simple yet powerful platform that would let me create a performant profile/blog, and I am excited to share the journey from the first line of code to the final deployment. Let's dive into the steps I followed and the lessons I learned along the way.

## Why I Chose Astro and Netlify

I needed a framework that:
- Prioritizes speed and performance.
- Supports Markdown natively.
- Is straightforward to deploy.

Astro fit the bill perfectly. It’s a modern, static site generator optimized for fast-loading pages. As for deployment, Netlify’s seamless integration with GitHub made it a no-brainer, as I wanted an easy setup without dealing with servers.


## Why Netlify

Netlify’s automatic deployment from GitHub means that each time I push an update, the site redeploys automatically—perfect for rapid iterations and easy content updates.

## Build/Deployment

Once the blog was set up, I needed to deploy it. Here's how I did it:

Pushed the Project to GitHub: I created a new repository on GitHub and pushed my Astro project there.

Linked GitHub Repo to Netlify: In Netlify, I connected the repo and selected the branch I wanted to deploy (usually main).

Set the Build Command:

Build command: npm run build
Publish directory: /
Triggering the First Deployment: Netlify automatically detected the Astro project and triggered a build. Within a few minutes, the portfolio was live!

## Challenges & Lessons Learned

Managing Content with Markdown: Astro's Markdown support is fantastic, but organizing content effectively with frontmatter metadata is key. Planning out the structure from the beginning helped streamline the process.

Handling Image Optimization: I had to be mindful of image sizes since Astro doesn't come with built-in image optimization (though it does support the <picture> tag and responsive images).

SEO and Meta Tags: Initially, I missed adding proper meta tags for SEO and social sharing. I ended up creating an SEO.astro component to handle this and added it to each page layout.

Astro-Specific Syntax: Astro’s syntax for props and slots takes some getting used to. It’s different from frameworks like React, but after a few days, it felt intuitive.