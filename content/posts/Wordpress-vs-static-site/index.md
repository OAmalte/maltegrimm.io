+++
title = "Wordpress vs. static site generator"
date = "2020-12-16"
+++

Wordpress vs. static site generator: I know, it's comparing apples with oranges, but this was the decision I faced and the story of how it came about. 
<!--more-->
And the headline isn't even correct, more precise would be "Wordpress vs. static HTML generator'. For the last 10 years, every time i set up a website or blog i've wordpress and it was always a good choice.
I have tried several times to start a regular blog, but it always ended in a very unregular blog. Instead i always tinkered around to make the webstite as fast es possible. Tuning nginx, writing scripts for super efficient Photo compression, monitoring and optimizing MySQL Cache Hits and in the end i cached the whole wordpress blog with a reverse proxy.

And at this point a CMS like Wordpress on a root server for an almost abondened blog, with only user and probably only one reader seems like overkill. I've learned a lot from optimizing my LAMP/LEMP stacks and that was what drove me most of the time. 

++This is not an objectiv decision++
I want to move on and use, at least for me, new technologies and concepts. And make it "simple", so no full CMS with a database and user management and tons of functions that i won't need.
Back to plain HTML Files on some "free" webspace? Like we did around 1995, copying some snippits from selfhtml and build something ugly?
No, i dont want to write every HTML line by myself, so looked at some static site generators and chosen HUGO and a nice theme.

++Storage++
Almost every webspace should do the trick, I've got only static files, so i don't need any scripting support. But the "free" webspaces are often coming with downsides like Ads or unwanted cookies. I looked into github pages and AWS S3 and you're looking at a S3 hosted website right now.
AWS is interesting for me, because i want to look into other AWS services as well. And documenting it here will keep this blog alive. Eventually. 

