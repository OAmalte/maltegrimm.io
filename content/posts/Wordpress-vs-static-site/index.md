+++
title = "Wordpress vs. static site generator"
date = "2020-12-16"
+++

Wordpress vs. static site generator: I know, it's comparing apples with oranges, but this was the decision I faced and the story of how it came about. 
<!--more-->
And the headline isn't even correct, more precise would be "Wordpress vs. static HTML generator'. For the last 10 years, every time i set up a website or blog i've wordpress and it was always a good choice.
I have tried several times to start a regular blog, but it always ended in a very unregular blog. Instead i always tinkered around to make the webstite as fast es possible. Tuning nginx, writing scripts for super efficient Photo compression, monitoring and optimizing MySQL Cache Hits and in the end i cached the whole wordpress blog with a reverse proxy.

And at this point a CMS like Wordpress on a root server for an almost abondened blog, with only user and probably only one reader (both me) seems like overkill. I've learned a lot from optimizing my LAMP/LEMP stacks and that was what drove me most of the time. 

## Feature Comparison ##

Usecase | WordPress | Hugo (Static Site Generator)
--- | --- | ---
Many Authors | Sure | no, not so easy
Themes | endless | a lot
Plugins | check | no
An admin UI | yes | for what



## In my case it´s not an objectiv decision ##
I want to move on and use, at least for me, new technologies and concepts. And make it "simple", so no full CMS with a database and user management and tons of functions that i won't need.
Back to plain HTML Files on some "free" webspace? Like we did around 1995, copying some snippits from selfhtml and build something ugly?
No, i dont want to write every HTML line by myself, so looked at some static site generators and chosen [HUGO](https://gohugo.io/) and a [nice theme](https://github.com/mrmierzejewski/hugo-theme-console/).

## static doesn´t mean static 1 ##
So this website is pretty static, as my wordpress blog was before. But i could use more javascipt, do some jquery magic and so on. And CSS. So this website could utilize a lot of fancy animations, but the files on the servers remain static. No extra serverside computing and html generating is done.

## Storage for a static webside ##
Almost every webspace should do the trick, I've got only static files, so i don't need any scripting support. But the "free" webspaces are often coming with downsides like Ads or unwanted cookies. I looked into [Github Pages](https://pages.github.com/) and [AWS S3](https://docs.aws.amazon.com/en_us/AmazonS3/latest/dev/Welcome.html) and you're looking at a S3 hosted website right now.
AWS is interesting for me, because i want to look into other AWS services as well. And documenting it here will keep this blog alive. Eventually. 

## static doesn´t mean static 2 ##
I didnt plan to at the moment, but with other **serverless** services from AWS it´s possible to still only provide static files from S3, but trigger backend scripts and receive data from DBs. But that will be another post.