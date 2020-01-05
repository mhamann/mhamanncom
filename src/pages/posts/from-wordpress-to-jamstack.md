---
title: From WordPress to JAMstack
date: 2020-01-04T05:09:16.674Z
thumb_img_path: /images/jamstack.webp
content_img_path: /images/jamstack.webp
excerpt: >-
  It's time to reconsider how we build websites. Where WordPress was once the
  de-facto solution for building a CMS-backed website, the JAMstack is
  positioned to succeed it in the new decade.
template: post
---
I've used WordPress for...well...it seems like forever. As the defacto website publishing platform, there's almost no discussion when starting a new project: grab WordPress, some trusted plugins, and begin building. At the same time, I've been a [long-time](https://twitter.com/mhamann/status/73232759753150464) [critic](https://twitter.com/mhamann/status/19049200655) of [WordPress's](https://twitter.com/mhamann/status/71049672407519232) [architecture](https://twitter.com/mhamann/status/5702544956), and have longed for a good alternative.

Granted, things have improved in some areas over the years, but it's still a huge mess overall. Additionally, it's technically important to keep up with WordPress version updates, given that security vulnerabilities are frequently discovered and fixed. Numerous sites have been breached due to outdated WordPress installations--and that's just the core. Most WordPress setups require multiple plugins to be installed--thus broadening both the attack surface and the amount of code that has to be maintained.

Given all of that (and the fact that I rarely found time to apply WordPress updates), the so-called "[JAMstack](https://jamstack.org/)" is pretty enticing: produce a website that requires zero (or at least very few) security updates, no databases, and no application runtimes. JAMstack sites are "static" in that they are just HTML, CSS, and some Javascript. As a result, they can also be lightning fast and aren't very susceptible to spikes in traffic.

JAMstack is still in the early adoption phase. There are some great frameworks out there for building static sites (Gatsby, Hugo, and Jekyll to name a few popular ones), but the tools surrounding them are still pretty rough. The authoring and site management experience pales greatly in comparison to what WordPress offers, and there are a lot fewer "batteries included" options (e.g. form handling, authentication, SEO analysis, etc).

Even so, several offerings are evolving rapidly. Netlify (which hosts this site) and Stackbit are definitely making it easier than ever to get up and running with a JAMstack site. Netlify has even championed an open CMS project/service for authoring and managing site content. Again--the experience is a bit rough, but it works well enough.

Given my own personal website was sorely in need of updating, and given I was tired of keeping PHP, MySQL, and WordPress up-to-date and running smoothly, I decided to hop on the JAMstack!

In brief, I replaced:

* A 2 CPU / 1GB RAM DigitalOcean droplet hosting ($10/mo)
* Apache HTTPD server
* PHP
* MariaDB (MySQL)
* WordPress + themes and plugins

with:

* [Netlify](https://netlify.com) hosting (free)
* [Gatsby](https://gatsbyjs.org) + a theme
* [Netlify CMS](https://netlifycms.org)
* [Stackbit](https://stackbit.com)

The result is a completely static site (just HTML, CSS, and a sprinkling of JS) running on Netlify's freemium hosting platform. On the surface, it seems like a lot of disparate technologies that have to work together, but this is where Stackbit really shines. It pulls all of the technology pieces together into a cohesive package and then deploys them to a supported platform.

Once deployed, I don't have to do any maintenance on the infrastructure whatsoever. And if ever Netlify doesn't meet my needs, it would be simple to move the site over to [Zeit's excellent Now platform](https://now.sh) or just drop it on a $5 DigitalOcean droplet running a simple nginx server. That's so much better than trying (and failing) to keep 7+ layers of infrastructure updated (and backed up!) just to run a simple blog.

These days, I can simply hop into Netlify CMS (or even a simple text editor), author a new blog post, PR the changes via GitHub for a quick preview, and finally merge the PR to get things into production.

For a developer, it's quick and easy. For those who are less technical, the Netlify CMS handles much of the complexity so touching GitHub is unnecessary. Again, it's not as smooth as WordPress yet, but that will change given enough time.

If you haven't tried JAMstack yet, give it a go! I think you'll see the potential.
