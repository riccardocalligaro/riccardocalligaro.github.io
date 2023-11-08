---
title: "PassioneVespa"
layout: post
date: 2023-11-08 18:00
tag: nextjs, typescript, website
headerImage: false
projects: true
description: "The reference website for vintage Vespa enthusiasts."
category: project
author: riccardo
externalLink: false
---

<span class="project-used-item">NextJS</span>
<span class="project-used-item">Typescript</span>
<span class="project-used-item">Serverless</span>
<span class="project-used-item">Fast loading</span>
<span class="project-used-item">SSR & SSG</span>
<span class="project-used-item">ChakraUI</span>
<span class="project-used-item">Server components</span>
<span class="project-used-item red-project">Closed source <span class="ec-lock"></span></span>

<div align="center">
<img src="../../img/featured/passione-vespa/app_logo_rounded.png" alt="PassioneVespa banner" height="125px" >
</div>

Key features:

- 📁 Comprehensive **archive** of vintage Vespas: Explore a meticulously curated archive with detailed information on the production of vintage Vespas, including precise details on colors by year and frame numbers. Whether you're a collector, a restorer, or just an enthusiast, the app gives you access to an organized collection of all available historical data.

- 📅 **Calendar** of gatherings and events: Stay updated on the latest events in the Vespa community. The app's simple and intuitive interface allows you to discover gatherings, events, and Vespa Club meetings in your vicinity. Plan your outings and connect with fellow enthusiasts more easily than ever.

- 📜 **Historical documentation**: Delve into the rich heritage of Vespa with access to historical manuals, advertisements, and vintage brochures. Explore the fascinating history of the brand and witness its evolution through the decades. Immerse yourself in the nostalgia of the timeless appeal of Vespas.

**PasioneVespa** was built with a modern and efficient web development stack that prioritizes speed, performance, and scalability. The frontend framework, **Next.js**, utilizes TypeScript for type safety and improved development experience. The backend is serverless, using edge functions on **Vercel** to handle API requests and other dynamic operations.

For data persistence, I used a **NeonDB** serverless postgres database, providing a scalable and cost-effective solution for storing and managing website data.

**Cloudflare R2** is used for storing images and other static assets. To optimize image loading performance, WebP images are served whenever possible.

I gathered all the data from a lot of different sources with the help of scraping and other data gathering tools.

I started the project in August of 2023 and deployed it in November.

<div style="text-align: center; margin-top: 30px;">
<img src="../../img/featured/passione-vespa/passione-vespa-mockup.webp" alt="passione vespa" />
</div>
