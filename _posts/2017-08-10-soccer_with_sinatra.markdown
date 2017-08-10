---
layout: post
title:  "Soccer with Sinatra"
date:   2017-08-10 02:53:22 +0000
---


When starting my Sinatra project, I really wanted to make something that I would find useful. As a former soccer coach, I decided that having a place to manage all of my players and configure the starting line-up for each game would meet that goal. My vision for the Sinatra app was much grander than the actual final outcome, but that is mainly because I realized I still need to learn the later units like javascript to have my application function at the level that it does in my head. 

The models, views, and controller format with routes leading to different views was something I felt like I understood well, so I wanted to use this project as an opportunity to add additional functionality. Unfortunately, I struggled more than I thought I would to remember all the ins and outs of CSS and I learned that many of the things I wanted to add requred javascript. 

My first difficulty or area that fell short of my dream vision was the selecting a player for a position form. In my head, I imagined a drag and drop functionality that, as a result, easily showed the user which players had already been assigned a position and which ones were still available. I hope to go back and add this functionality once I learn how to add in that kind of dynamic site manipulation. 

I also had more difficulty than I thought I would linking a css stylesheet to my application. After a lot of web surfing and frustration, I realized that my browser was keeping the first blank style sheet that I made in it's cache instead of accessing it every time I refreshed the page. I learned that the whole time, I had been researching the wrong problem. My stylesheet was linked all along.  I think this is a really good lesson to remember when I get frustrated or stuck on an issue. Instead of trying the same or similar things over and over again, I should be sure to step back and reevaluate the problem to make sure there isn't a seperate issue altogether that I overlooked. 

Another thing I learned while testing my project, was how easily minor bugs can slip in as the size of the project begins to grow in scale. Multiple times, I felt like I had investigated all of the links, views, and forms to make sure they worked properly and then I would unexpectedly stumble upon a way to make it fail and then could correct my mistake. This helps me to appreicate the need for extensive testing. 

If you would like to view my Sinatra project, you can find it [here](https://github.com/hansenjl/sinatra-CRUD-soccer-project).
