---
title: From WordPress to JAMstack
date: 2020-01-04T05:09:16.674Z
thumb_img_path: /images/jamstack.webp
content_img_path: /images/jamstack.webp
template: post
---
I've used WordPress for...well...forever. As the defacto website publishing platform, there's almost no discussion when starting a new project: grab WordPress and some trusty plugins and get building. At the same time, I've been a [long-time](https://twitter.com/mhamann/status/73232759753150464) [critic](https://twitter.com/mhamann/status/19049200655) of [WordPress's](https://twitter.com/mhamann/status/71049672407519232) [architecture](https://twitter.com/mhamann/status/5702544956).

Granted, things have improved in some areas over the years, but it's still a huge mess overall. Additionally, it's technically important to keep up with WordPress version updates, given that security vulnerabilities are frequently discovered and fixed. Numerous sites have been breached due to outdated WordPress installations--and that's just the core. Most WordPress sites require several plugins to be installed, which broadens the attack surface and the amount of code that has to be maintained.

Given all of that (and the fact that I rarely applied WordPress updates), the so-called "[JAMstack](https://jamstack.org/)" is pretty enticing: produce a website that requires zero (or at least very few) security updates, no databases, and no application runtimes. JAMstack sites are "static" in that they are just HTML, CSS, and some Javascript. As a result, they can also be lightning fast and aren't as susceptible to traffic spikes.

JAMstack is still in the early adopter phase to some degree. There are some great frameworks (Gatsby, Hugo, and Jekyll to name a few popular ones) out there for building static sites, but the tools surrounding them are still pretty rough. The authoring and site management experience pales greatly in comparison to WordPress, and there are a lot fewer "batteries included" options (e.g. form handling).

Even so, several offerings are evolving rapidly. Netlify (which hosts this site) and Stackbit are definitely making it easier than ever to get up and running with a JAMstack site. Netlify has even championed a CMS project/service for authoring and managing site content. Again--the experience is a bit rough, but it works passably.
