---
layout: "post"
title: "On 'Big Boy' Hosting"
description: "How I Migrated to a Real Hosting Provider"
categories: ["blog"]
tags: ["website", "meta", "status update", "digital ocean"]
---

## Entering the Digital Ocean

As my primary task for today I registered with Digital Ocean and migrated jacobmoore.cool from free Github Pages hosting to a small Ubuntu droplet.

A couple of advantages to this approach:

* **Security.** GitHub Pages doesn't currently support SSL certificates. Moving to my own hosting makes this trivial.

* **Knowledge.** Setting up an Ubuntu droplet from scratch was a nice exercise. Using a statically generated site means that the process isn't too intense, but writing nginx config files and configuring DNS isn't nothing.

* **Scale.** I have a few other web projects planned, specifically one around the Cube League I run. Running an nginx host on my own droplet means that I will be able to host multiple small domains. GitHub Pages is free, but only allows for one site per username or project.

* **Work.** Making some daily effort toward a larger goal is the single greatest way to achieve the things that we set out to do. Starting this project today gave me momentum and some fodder for this post.

Check back tomorrow for some extended thoughts about GitHub and why I'll be moving to GitLab sooner rather than later.
