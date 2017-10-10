---
layout: post
title:      "React Apps"
date:       2017-10-10 22:50:11 +0000
permalink:  react_apps
---


As I have been building my final project, I continue to be amazed at the new functionality possibilities because of React. Even as I submit my project, I keep adding to a list of more features to add. I decided to create a circuit builder application meant specifically for physics teachers (essentially something I could have used when I was teaching). There are a lot of advanced circuit builder applications for electrical engineers but I wanted an easy way to create many different simple circuits that I could use for creating class problems, examples, and worksheets. The end goal being that I would have an image I could easily screenshot and add to a word document that listed the values of different resistors. 

Throughout building this project, I learned a lot more about the various data types that can be used. I initially used the data type of 'integer' for all of the resistance, current, and voltage values but it didn't take long to realize that this was inherently flawed since most of the values were actually decimal values. Once I reconfigured the database to accept decimal values, I had a new issue on hand - too many repeating decimals. After a quick search on the web, I discovered the handy .toFixed() method. This lead to another learning opportunity about data types as the .toFixed() method converts the decimal into a string. I had used this method to limit to calculated current for each resistor.  However, this cause the total current to be wrong because I accidently was added the string values of each resistor's current to find the total current. 

Ultimately, I still used .toFixed() but only on data that did not need to be manipulated further. I also continued to use parseInt on the resistance input values since those are limited to only be integers.  Out of all the apps I have built so far, this one has been the most enjoyable to build because I can see the practical applications. I only wish I had built this before I stopped teaching.


As for the future, I plan to add the following to the application:
*More complex combination circuits
*Sorting all circuits by difficulty
*Adding the ability for users to solve the circuit and check their answers
*Downloadable images for each circuit
*Better placement of resistors
*Higher quality rendering of the circuit images


