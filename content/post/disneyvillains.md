---
title: "1. Disney Villains"
date: 2021-12-07T10:31:53+01:00
featured_image: '/images/disney.jpeg'
body_classes: "avenir bg-white"
---


## Motivation

When thinking of Disney films, most people feel a rush of nostalgia, as if they were watching one of those films with a bowl of cereal on a Sunday morning. Everybody has their favourite character and that one villain that they were a little bit afraid off. In this project, the villains of Disney, will be explored further and hopefully seen in a new light.


## Dataset

The dataset was extracted from the Disney Fandom Wiki webpage, and it contains all the character villains from Disney. That includes characters from different universes, e.g Marvel, Pixar, Star Wars, Walt Disney and other. After building and visualising the network, it was decided to narrow the scope and maintaining at least some possibility of analysing information about the dataset, do to lack of internal connections in the whole Disney Villains dataset. From that a decision was made to select a subset of the data, that represents one universe, Marvel. (https://disney.fandom.com/wiki/Category:Villains)


## Goal

The goal of the project is to create an interesting network and extract valuable information about villains connections. It is interesting to discover a new perspective of the villains in the Disney universe and then include some type of discovery in the results and see what characterises an evil villain. 


## Basic statistics

Some basic statistics about our dataset:

![stats1]({{< baseurl >}}/images/stats.png)

Which universe kills the most of its main antagonists?

![stats2]({{< baseurl >}}/images/stats2.png)

Bar plot that shows the percentage of alive vs. deceased characters per universe:

![stats3]({{< baseurl >}}/images/stats3.png)

From the figure above it is concluded that the Star Wars Universe, is the universe with the highest percentage of deceased main villains. Indeed, the only ones that are currently alive in the Star Wars Universe, are the villains from the series currently on tv. Grand Admiral Thrawn, is the only one that (not a spoiler) got out of the whole tv show alive, even though it was implied that he was dead. Moreover, at first sight, Walt Disney seems to have quite a high percentage of deceased characters. This makes sense when we think about what used to happen with villains in older Disney movies, such as, Scar, Ursula, and more. Finally, what is needed to point out, is that if someone wants to be a bad guy, Pixar is the safest environment to do so, with only a 13% death rate of villains.


## Disney Villains Network

![stats]({{< baseurl >}}/images/villain_network.png)

This is the whole Villains network, with different colors for all four universes and when looking at it, is sure does look a little crazy. On the figure, there are some groups that are better connected than others. Those groups represent the different universes. The Marvel universe is displayed with green color, Star Wars with red color, Pixar with gray color, Walt Diseny with blue color and the villains who are not a part of a specific universe, are represented with pink color (Unknown).


## WordClouds per universe

![stats]({{< baseurl >}}/images/marvel.png)


![stats]({{< baseurl >}}/images/disneyw.png)


![stats]({{< baseurl >}}/images/starwars.png)


![stats]({{< baseurl >}}/images/pixar.png)

These are the WordClouds for all four universes. They tell a good story about different universes. When taking a further look into the Marvel WordCloud, words like Spiderman, Loki, Marvel, comics, kill, return, Hulk and Thor are displayed. These words are a great example of what the Marvel universe is all about. The same can be said about the other universe WordCloud, for example, in the Disney WordCloud there are words such as tell, time, show, and appearance, these are all words that fit well when telling a story as Walt Disney does. In the Star Wars WordCloud, there are words like Vader which is a famous character in the Star Wars movie. Finally, in the Pixar WordCloud, there are words such as Buzz, toy, Mater, incredible, and Woody.


## Connection between universes 

Looking both at the Disney villains network and the WordClouds for different universes, we want to examine if there is any strong connection between different universes. We decided to compute the 10 highest connections among different universes an the results are displayed in the DataFrame below.

![stats]({{< baseurl >}}/images/dataframe.png)

When looking at the DataFrame, we see that Darth Vader is the villain that has the highest number of connections to other universes. When exploring this further, we saw that these connections were not because Darth Vader appears or recognizes characters from other Disney moveies. Rather because that there are some characters in other movies that are inspired by him and his features.

These results motivated us to narrow down the subject, and take a further look into one cluster or universe in the whole giant component Disney villain network. When looking at the figure of the network above, we can see that the green nodes or the nodes that represent Marvel universe, form a large separated group. From this we decided to take a subset of the whole network, and look even further into the Marvel universe. 


To read more about the Marvel universe check-out the next page 


