---
layout: post
title: Subdomains with Github Pages
categories:
- blog
---

It's been a pleasure setting up cfn.io. First, since I'm hosting it in the same account as [chrisfnicholson.com](http://chrisfnicholson.com), when I first pushed the cfn.io repo live, it took down my personal blog.

It turns out you have to regenerate each site when you push a new domain live. I asked on #github on Freenode, and a Github engineer reloaded it for me. I ran into the same problem when setting up [events.cfn.io](http://events.cfn.io), so I just repushed cfn.io and events started working.

If you're in the same position as me (or some related position, more likely), here are the tips I wish I'd found in someone else's blog post.

* A domain hosted on Github Pages should be pointed with an A record at the Github Pages IP address: 202.234.175.78. 
If you want to use subdomains, point two records, one A record named "@", and one named "\*".


