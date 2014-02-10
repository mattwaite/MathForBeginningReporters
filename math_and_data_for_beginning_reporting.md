#Math and Data for beginning reporting#

#####Credits#####

This document was started by Matt Waite, professor of practice in the College of Journalism and Mass Communications at the University of Nebraska-Lincoln. 

**Contributors**

    names here

##Summary##

All communicators, regardless of interest, discipline or medium, need to understand numbers to do their jobs effectively. More and more of society is being transformed by data as our lives are increasingly stored in databases. If you can't understand data and the basic math that you'll use regularly on the job, you are at the mercy of people who can.

This module is designed to solve a particular problem: How do you get basic data journalism into a beginning reporting class that many feel is packed as it is? My answer is to combine the basic math for reporters with instructions on how to apply those concepts in a spreadsheet using real data, all aimed at generating real story ideas. This document will show: 

* Basic math concepts and how to calculate them by hand.
* How to apply those basic math concepts to a spreadsheet of data.
* How to turn basic math + a spreadsheet of data into a story idea.

Contained in this repository are the datasets used to illustrate the concepts. They are kept here in .csv format, so you can use Excel, OpenOffice or Google Spreadsheets to do the same analysis. The spreadsheet formulas and concepts will work on any of those three software platforms.

##Introduction##

#####Bad at math is a lie#####

Let me guess: There's a not-insignificant part of you that's pretty happy to be in journalism school because the math requirements are pretty minimal. Have you ever said, out loud, "I can't do math, I'm a journalism major!" Have you ever thought "It's okay, I'm bad at math." Have you been bad at math your whole life?

First, you're not alone.

Second, you're living a lie.

That's right. A lie. Bad at math is not a thing. And you are not bad at math. You just think you are. [And it's a destructive lie you tell yourself.](http://www.niemanlab.org/2013/11/matt-waite-how-i-faced-my-fears-and-learned-to-be-good-at-math/)

You, like me, struggled with math at some point when your friends didn't. They kept going, you kept struggling, and suddenly they were good at math and you were not. And here you are today.

Except with journalism today, you can't continue to live the lie. You are surrounded by data. You are surrrounded by numbers. If you continue to believe you're bad at math, you will be easy to fool by people who aren't. You'll be unable to see stories that are sitting there in the numbers. 

In short: you won't be a very good journalist.

The good news? This isn't very hard. The types of math that get you in the door are really quite easy. And you can do some very powerful things.

#####How high school algebra won a Pulitzer Prize#####

If you were at all paying attention in pre-college science classes, you have probably seen this equation:

    d = rt or distance = rate*time
    
In English, that says we can know how far something has travelled if we know how fast it's going and for how long. If we multiply the rate by the time, we'll get the distance.

If you remember just a bit about algebra, you know we can move these things around. If we know two of them, we can figure out the third. So, for instance, if we know the distance and we know the time, we can use algebra to divide the distance by the time to get the rate.

    d/t = r or distance/time = rate 

In 2012, the South Florida Sun Sentinel found a story in this formula.

People were dying on South Florida tollways in terrible car accidents. What made these different from other car fatal car accidents that happen every day in the US? Police officers driving way too fast were causing them. 

But do police regularly speed on tollways or were there just a few random and fatal exceptions? 

Thanks to Florida's public records laws, the Sun Sentinel got records from the toll transponders in police cars in south Florida. The transponders recorded when a car went through a given place. And then it would do it again. And again.

Given that those places are fixed -- they're toll plazas -- and they had the time it took to go from one toll plaza to another, they had the distance and the time.

[It took high school algebra to find how fast police officers were driving. And the results were shocking.](http://www.sun-sentinel.com/news/local/speeding-cops/fl-speeding-cops-20120211,0,3706919.story)

Twenty percent of police officers had exceeded 90 miles per hour on toll roads. In a 13-month period, officers drove between 90 and 110 mph more than 5,000 times. And these were just instances found on toll roads. Not all roads have tolls.

The story was a stunning find, and the newspaper documented case after case of police officers violating the law and escaping punishment. And, in 2013, they won the Pulitzer Prize for Public Service. 

All with simple high school algebra.


##The basics of the basics##

**If you don't know these, you are doomed from the start.**

#####Notation####

One of the most difficult hurdles for beginning students of mathematics to get over is notation. If you miss a day, tune out for a class, or just never get around to asking what something means, you'll be lost. So lets just cover some bases and make sure we all understand some ultra-basic notation. 

You might laugh at these, but someone reading them is looking up Gods on Wikipedia to thank. So do yourself a favor and refresh.


|Symbol|Meaning|Example| 
|------|-------|-------|
|+|addtion|5+2|
|-|subtraction|6-2|
|* |multiplication|7*2|
|/|division|8/2|
|^|exponent|2^3|
|sqrt|square root|sqrt(4)|

	Author notes: More? Delta? Sigma? Coming back to this.


#####Order of operations#####

One of the most important and often overlooked concepts in basic math is the order that you do the calculations. When you have something like `5+5*5^2`, which gets done first? Or, as you'll read in the next section, what comes first when you calculate the average of a thing? The adding up of all the numbers or the division by the number of numbers?

Thankfully, math teachers have provided us an easy to remember memonic that you probably learned in sixth grade and forgot until now. 

**PEMDAS** -- **P**arenthesis, **E**ponents, **M**ultiplication, **D**ivision, **A**ddition, **S**ubtraction

What that means is when you look at a mathematical formula, you do the calculations in the order PEMDAS tells you. Something in parenthesis? Do that first. Is there an expoennt? Do that next. Muliplication or division? It's next and so forth.  Knowing PEMDAS will save you from stupid mistakes down the road.

##Mean##

#####The basics#####

Here's the thing about mean -- you probably already get it. It's the average. It's a measure of the middle. You've used averages your whole life. They're everywhere. 

But you may not know that average is just one measure of the middle -- what mathematicians call measures of central tendency. The others are the median (more on that later) and mode (which no one except mathematicians ever talks about).

Knowing when to use average and when to use median takes a little bit of thinking. Why? Because averages, by how they are calculated, are sensitive to extremes. What does this mean? Let's use an example. 

Let's pretend for a second that I'm taking a poll of a college class of 5 students on how much everyone makes per year. It's full of students, so the annual salaries are $8,000, $9,500, $7,200, $10,000 and $6,400. That makes the average annual income of these five students $8,220 (we'll talk about how to calculate the average in the next section). In our group of five students, given their incomes, $8,220 is pretty much in the middle. A student might make a little more, or a little less, but $8,220 is in the ballpark.

But I teach at the University of Nebraska. And we love us some football. And surprise! Head Coach Bo Pelini visits class. He makes $2.875 million. Per year. 

The average salary now? $486,016. And 67 cents. Who feels average now?

(This problem gets solved in the next section)

The above example, while a little silly, illustrates the point: If you have a set of numbers that has no constraints -- there could be really big numbers or really small numbers in the mix -- then a mean probably isn't the number you're looking for. But when the numbers are constrained, or there aren't any extreme values in the set, averages work great. 

#####How to calculate a mean#####

How to calculate a mean is pretty simple: Take your numbers, add them up, and then divide them by the number of numbers you have. Let's take our previous example of the class of five and work through it step by step.

First, we need to add up the salaries in the class.

`8000 + 9500 + 7200 + 10000 + 6400 = 41100`

Then, we divide that 41100 by 5, the number of students in the class. 

`41100 / 5 = 8220`

Calculating the mean of a set of numbers is a very basic and simple way to measure the middle of the group. But be careful with sets of numbers

#####How to calculate a mean in a spreadsheet#####




#####How to turn a mean into a story#####

##Median##

#####The basics#####

#####How to calculate a median#####

#####How to calculate a median in a spreadsheet#####

#####How to turn a median into a story#####

##Percentages of a whole##

#####The basics#####

#####How to calculate a percentage#####

#####How to calculate a percentage in a spreadsheet#####

#####How to turn a percentage into a story#####

##Percent change##

#####The basics#####

#####How to calculate a percent change#####

#####How to calculate a percent change in a spreadsheet#####

#####How to turn a percent change into a story#####

##Minimums and maximums##

#####The basics#####

#####How to calculate a minimum or maximum#####

#####How to calculate a minumum or maximum in a spreadsheet#####

#####How to turn a minimum or maxiumum into a story#####

##Sorting##

#####The basics#####

#####How to sort in a spreadsheet#####

#####How to turn a simple sort into a story#####

##Probability##

#####The basics#####

#####How to calculate a probabiity#####

#####How to calculate probability in a spreadsheet#####

#####How to turn a probability into a story#####

##Odds##

#####The basics#####

#####How to calculate odds#####

#####How to calculate odds in a spreadsheet#####

#####How to turn the odds into a story#####

##Equations of a line##

#####The basics#####

#####How to calculate slope and find the equation of a line#####

#####How to calculate slope and the equation of a line in a spreadsheet#####

#####How to turn the equation of a line into a story#####
