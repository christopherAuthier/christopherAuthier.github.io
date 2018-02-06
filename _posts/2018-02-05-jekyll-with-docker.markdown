---
layout: post
title:  Jekyll with Docker
date:   2018-02-05 21:02:00
categories: jekyll, docker
---

I am currently using [Github Pages](https://pages.github.com/) to host my jekyll site.

This makes it really easy for maintenance but I have recently learnt about Docker and I like to try new things. Here is the command to run jekyll anywhere you have Docker installed:
```
docker container run -d -p 80:4000 -v $(pwd):/site bretfisher/jekyll-serve
```

You now have your Jekyll site running in a container!

**Note:** Real hero here is Bret Fisher for the great docker image!
