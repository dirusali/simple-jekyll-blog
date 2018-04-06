## Simple Jekyll Blog

This repo contains a really simple blog site that utilisies githubs simple Jekyll blog

### Setup instructions

Install Jekyll on your dev machine, follow the instructions on the Jekyll home page, (Install Jenkyll)[https://jekyllrb.com/docs/installation/]

Verify you have Jekyll installed,  `jekyll -v`

Install all the gem dependencies for the blog site locally so you can develop and test the site.

``` bash
bundle installed
```

You can no run the site and see it rendered in a browser.

``` bash
jekyll serve
```

The blog will be available locally open the following url in a web-browser to view (http://localhost:4000)[http://localhost:4000]

# Creating a new Post

create a new file in the `_posts` directory, i.e `2018-01-01-blog-awesome.md`

At the top of the file you need to include metadata that will describe what the post is about and provide information to the Jekyll engine, here is an example of the metadata,

```
---
layout: post
title: "Cats Blog"
date: 2018-01-01
desc: "An awesome Blog"
tags: [Awesomeness]
---
```
copy the above into your post file and customise as necessary. You can add as much content as you would like, the post need t be written in `kramdown` which is a superset of `Markdown` for syntax guides go here (kramdown QuickRef)[https://kramdown.gettalong.org/quickref.html]
