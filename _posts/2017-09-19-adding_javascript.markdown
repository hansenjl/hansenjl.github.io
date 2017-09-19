---
layout: post
title:  "Adding Javascript"
date:   2017-09-19 01:15:57 +0000
---


As I worked my way through the JavaScript unit, I remember thinking, "this isn't too bad... there are so many similarities to what we've already done." What I realized by the time I was starting my project, however, was that there are so many things you can do with JavaScript including seamlessly integrating jQuery, which makes it a lot more complicated. I feel like I learned so much, but still have so much more to learn as I finish up adding JavaScript to my rails project. I am very happy with the progress I made and seeing the new functionality that's possible with JS, but like previous projects, I still want to learn how to do more complex things.

It is funny how one simple addition in JavaScript, can have a cascading effect of other changes that then need to occur. For example, I created a travel app and added the JS functionality to see the next or previous city without a browser refresh.  That part was fairly simple to add. Then I thought, "I should add images to the cities."  That part alone was quite simple, but soon I found myself having to update the previous and next city functions I had just created.  Likewise, I wanted to add comments to the city show page. Creating a form and posting to the create route using AJAX was very straightforward but I realized I now had to add a way for the comments to transfer from one page to the next. It makes you realize that there is a lot more work that goes on behind the scenes to add in seemingly simple functionality. 

At present, my app meets the project specs, but I hope to keep adding to it over the next few weeks. JavaScript opens up so many possibilities for making the application more user friendly and I'm excited to continue to improve the functionality. As it currently stands, I am most proud of the delete comment button that I added to the city show page. It seems so trivial but to make sure that only the current user could delete his or her comments even as the current city changed required modifying the way comments were added. Not only did the city#show view have to ensure that only the current user could delete comments, but the JavaScript responsible for loading the next city, also had to be responsible for this logic. 

Above all, I am so thankful I have now opened the door to JavaScript and jQuery and hope to continue to learn how to master them. It completely expands the functionality possibilities and gives me ways to add features I have wanted to deploy.





