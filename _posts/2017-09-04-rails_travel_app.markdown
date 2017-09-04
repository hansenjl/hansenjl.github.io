---
layout: post
title:  "Rails Travel App"
date:   2017-09-04 23:34:14 +0000
---


For my Rails app, I decided to make an application that would record places you've visited. The initial set-up of the application has become so much easier with the magic that is Rails. I appreciate that this then lets me focus on the more complex aspects of the app such as nested forms and relationships between objects. 

I definitely struggled the most with the nested forms aspect because there were multiple nested relationships at play. For example, when a user logged a visit into the system, the visits route was nested under the user route so that the user id would automatically be tracked. In the actually form for the visit creation, the user also had many choices. The user could choose from a city that had already been created or create a new city. This alone was not hard to incorporate, but I wanted to make it so that a city had to be attached to a country.  In a future world (once I've finished the program), I'm sure I could have made it so that first a country was selected, and then city options appeared. Unfortunately, I had to instead allow for users to input both the city and the country or choose from ones that were already created. As it is currently, it works fairly well but definitely leaves room for improvement once I have learned more.

The part of my app that I am most proud of is my use of helper views for the unranked and ranked city iterations. I  found it very useful to be able to describe html code for how each situation is handled and then be able to render it in multiple views.  I know I still could improve in making my views even more DRY, but I think I am at least moving in the right direction.

I also have a lot of future add-ons that I want to make a part of my app once I learn more and have some additional time. I think it would be much more user-friendly to show all of the already created cities with checkboxes that users can select to signify that they had visited that city. As soon as a user checks the box, a number-field would appear next to the city to allow the user to rate that visit. In this way, users could easily change their previous ratings for visits and easily add new visits. 


If you are interested in checking out my app, you can do so [here](https://github.com/hansenjl/Rails-Project---Travel-App/tree/master/app). Any comments or suggestions would be appreciated. 
