---
layout: post
title:  "CLI Recipe Finder"
date:   2017-07-21 23:22:58 +0000
---


I have finally finished my first project and am excited to actually use the project to generate ideas for daily dinner recipes. I went about creating this project a tad bit backwards in that I wanted to make it on my own without first watching the videos. This caused me quite a bit of frustration in the final stages but I do feel like I learned more this way.  I had designed mine similar to other labs whereas there was an enviornment file inside of a config folder, so I had a lot of restructuring to do today in order to make my project mirror the ruby gem structure. It would have been easier to start using the gem structure but I needed to do it tmy own way first so that I could prove to myself I had the skills to create a CLI application.

While creating the Recipe Finder, I tried to keep the focus on object oriented programming and ensuring that the objects had collaboration with each other. Therefore, each food category had many foods and each food belonged to a category. At times, this caused me a bit of confusion becuase when I would call on one food instance, it would list that food's category including the very long list of food instances belonging to that category. It created a very big interrelated web that made it difficult to see which food instance was being called upon unless I also called the name method for that food. The web only got bigger when each food had a recipe instance that belonged to the food item. Beacuse of this big interconnected web of objects, the categories with many food items would take longer to load than I would have liked. 

Future functionality that I would like to add to this project would be to create a method that lists the recipes in order of the time it takes to make them. Becuase the times that are scraped from the website are very inconsistently listed (i.e.: 5 minutes, 95 minutes, 1.5 hours, 1 hour and 45 minutes), I decided to hold off on that method for now. I would also like to go back and clean up the code as I learn more and become a more proficeint coder. 

If you would like to check out my project, you can do so below:

[Recipe Finder App](https://github.com/hansenjl/JenniferHansen-cli-app)
