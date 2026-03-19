---
title: Why and How I am here
date: 2026-03-18 12:19:11
tags:clarification
---

So excited to finally have my own dedicated website today:**mfzq.tech**

Since this is the very first post, I naturally want to document how I built it. Actually, I’ve wanted to own a personal website for a long time—a place to record my daily life and thoughts. My goal was always to have a site quietly hosted on an undisturbed IP address, paired with a domain name that’s easy to remember. Ideally, it would run on a server that lasts forever, is easy to maintain and update, and allows me to publish content from my local computer with just one click. <!-- More -->

However, as I started putting this into practice, I realized it wasn’t a small goal at all; it turned out to be a pretty tough journey. Finding a stable server was difficult. Many quick-deployment services are based overseas, which makes them incredibly unstable given the connectivity issues we face (you know what I mean by "that invisible wall"). Plus, domain names cost money, and they aren’t exactly cheap.

Here’s a breakdown of how I actually got this site up and running. In short, these were the steps:

- Bought the domain mfzq.tech on Alibaba Cloud for 8 RMB.
- Created a GitHub account.
- Set up a new repository on GitHub.
- Installed Node.js and git and hexo on my local machine.
- Used Hexo to generate the website content locally.
  
  > run the git bash with administrator role
  > 
  > ``` git bash
  > cd \g
  > hexo init myblog
  > cd myblog
  > npm install
  > git submodule add https:/github.com/Siricee/hexo-theme-Chic.git themes/Chic
  > npm install hexo-renderer-pug hexo-render-stylus --save
  > ```
  > 
  > change the theme to Chic in the file _config.yml
  > 
  > go back to git bash:
  > 
  > ```git
  > git init 
  > git add .
  > git commit -m"my first upload"
  > git branch -M main
  > git remote add origin https:/github.com/mygithub/myblog.git
  > git push -u origin main
  > ```
- Deployed the site using Netlify after pushed the code to my GitHub repository.
- Configured free DNS resolution via Cloudflare.

And just like that, my website is live! I plan to keep updating it gradually from here on out.