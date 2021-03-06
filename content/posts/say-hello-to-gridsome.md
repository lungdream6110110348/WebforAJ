---
title: Say hello to Gridsome 🎉
date: 20
published: false
tags: ['Markdown','Releases']
canonical_url: false
description: "สถานทีฝึกงาน"
---


```html
<template>
  <Layout>
    <h2>Latest blog posts</h2>
    <ul>
      <li v-for="edge in $page.allWordPressPost.edges" :key="edge.node.id">
        {{ edge.node.title }}
      </li>
    </ul>
  </Layout>
</template>

<page-query>
query Blog {
  allWordPressPost (limit: 5) {
    edges {
      node {
        _id
        title
      }
    }
  }
}
</page-query>
```

You don't need to know GraphQL or Vue to get started with Gridsome - It's a great way to get introduced to both.


The GraphQL layer and all the data can be explored in a local GraphQL playground. The playground is usually located at `https://localhost:8080/___explore` when a Gridsome development project is running.




#### Perfect scores on Google Lighthouse - automagically 💚

One of the main goals of Gridsome is to make a framework that let you build websites that are optimized "out-of-the-box." It follows the [PRPL-pattern by Google.](https://developers.google.com/web/fundamentals/performance/prpl-pattern/) You don't need to be a performance expert to make fast websites with Gridsome. Your site gets almost perfect scores on Google lighthouse out-of-the-box. These are some of the performance steps that Gridsome takes care of:

- Image compressing & lazy-loading ⚡️ 
- CSS & JS minification ⚡️ 
- Code-splitting ⚡️ 
- HTML compressing ⚡️ 
- Critical CSS (Plugin) ⚡️ 
- Full PWA & Offline-support (plugin) ⚡️  


#### A better way to build websites

Gridsome is built for the JAMstack workflow - a new way to build websites that gives you better performance, higher security, cheaper hosting, and a better developer experience. Generate prerendered (static) pages at build time for SEO-purpose and add powerful dynamic functionality with APIs and Vue.js.

We believe the SSGs / JAMstack trend is just getting started. When you have first started to make websites this way there is no way back. You feel almost "dirty" when going back to a traditional WordPress / CMS setup. 

Try running the new Chrome Lighthouse (Audit tab in Developer tools) on a WordPress site - It is impossible to get good scores even with the best caching plugins and hosting. With Gridsome you don't even need caching plugins. Website optimization is taken care of at build time.

This is what we think is very exciting and is why we are building Gridsome. It is the **perfect SPA & PWA front-end solution** for any headless CMS or content APIs.


#### Whats next

In the next couple of months we're going to continue to improve the docs, create tutorials, add more source & transformer plugins and fix bugs. 

#### Contribute to Gridsome

We're currently just two brothers working on this, so any contribution is very welcome. We're passionate about building a faster web and make website building fun again.

You can also support us by giving [a GitHub star ★](https://github.com/gridsome/gridsome/stargazers) and spread the word :)
