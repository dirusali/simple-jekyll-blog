## Simple Jekyll Blog

This repo contains a simple blog site that utilises Github Pages, it's built using the Jekyll template engine and the Maxima theme.  The posts are written in Markdown and compiled on the Github Pages service.

### Setup Instructions

Install Jekyll on your dev machine, todo this follow the instructions on the Jekyll home page, [Install Jenkyll](https://jekyllrb.com/docs/installation)

Verify you have Jekyll installed,  `jekyll -v`

Install all the gem dependencies for the blog site locally so you can develop and test the site.

``` bash
bundle install
```

You can no run the site and see it rendered in a browser.

``` bash
jekyll serve
```

The blog will be available locally open the following url in a web-browser to view [http://localhost:4000](http://localhost:4000)

### Creating a new Post

Create a new file in the `_posts` directory, i.e `2018-01-01-blog-awesome.md`

At the top of the file you need to include *metadata* that will describe what the post is about and provide information to the Jekyll engine, here is an example of the metadata,

```
---
layout: post
title: "Cats Blog"
date: 2018-01-01
desc: "An awesome Blog"
tags: [Awesomeness]
---
```

copy the above into your post file and customise as necessary. You can add as much content as you would like after the metadata, the posts are written in `kramdown` which is a superset of `Markdown` for syntax guides go here [kramdown QuickRef](https://kramdown.gettalong.org/quickref.html)

### Pushing to Github Pages

Go to settings and enable github pages for your repo. This means when you push new commits to the repo, the Github Jekyll engine will process the markdown files and render the html via the github pages url.  The `_site` folder is never committed, this is a generated directory that is used by the Github pages web server.  

### Topology of the site

There are three main page templates, *index.html*, *about.md* & *404.html* this shows the two variants of the page styles, raw html or Markdown.  Any additional pages that are created at the top level will be added to the Navigation bar.
