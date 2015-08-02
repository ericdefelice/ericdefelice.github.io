---
layout: post
title: New and Improved Website
categories: blog website
---
I've finally got around to updating the design of my website!  

I'm pretty happy with the current design, and maybe even more importantly, how easy it is to make new posts.  This was a big downside to my prevous design.  I had designed my old site from scratch using Node.js for the backend and Ember.js for the frontend.  These tools are very useful and allow for a big, complex web app to be created fairly quickly, but there is a bit of a learning curve.  In the end, it was starting to look like it would take a little too much maintance work for my taste, so I made the decision to update the site to something more simple.  So here we are, about 6 short months later, and I finally got around to it.


## A quick recap
I wanted to briefly explain the old site design (mainly so I can read this later as a refresher).  As I said, I had used Ember.js and Node.js for the site framework, and connected a database to the backend using PostgreSQL to store my blog posts and project pages.  I never used either of these tools before, so it was a learning experience.  After a weekend I had my Ember frontend up and runnin with the backend routing correctly, and things were looking pretty good if I do say so myself.  I struggled through some parts of it, but it was working, for the most part.   

It is actually still up and running here: [http://afternoon-eyrie-9941.herokuapp.com/](http://afternoon-eyrie-9941.herokuapp.com/)


## All good things must come to an end
Well, I'm not sure if I would classify my old site as <i>good</i>, but you know what I mean.  Anyways, the site was up and now I was ready to make a new blog post.  I didn't put in the work to make a interface for creating, modifying or deleting posts, nor did I really want to, so I had to manually enter them into the database.  This was a pain, as I couldn't check the formating quickly, so there was a lot of back-and-forth between updating the post in the database, then checking on the site, then fixing the post, then ...  It got old real fast.

That was when I decided that I would update my site's framework.  It took me a while, but I made the switch to using Jeykll.  I chose Jeykll mainly because it was static, meaning I wouldn't have to deal with databases for anything anymore.  And for a small blog like mine, this is just fine.


## The future
Now that it is up, I will hopefully post some updates on my projects more frequently to this site.  At least that is the plan. :)

I'd also like to make a couple of updates to the site somewhere down the line:

1. Enable comments for blog posts (probably using Disqus).

2. Enable searching and sorting using tags.  Right now the tags on the projects and blog posts are pretty much just for show.  I'd like to change this someday.