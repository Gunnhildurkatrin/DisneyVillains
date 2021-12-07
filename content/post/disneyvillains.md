---
title: "Disney Villains"
date: 2021-12-07T10:31:53+01:00
featured_image: '/images/disney.jpeg'
body_classes: "avenir bg-white"
---


## Motivation
When we think of Disney films, we feel a rush of nostalgia, as if we were watching one of those films with a bowl of cereal on a Sunday morning. We all have our favourite characters and we all have that one villain that we are a little bit afraid off. Therefore, it was an easy decision to take a further look into the villains of Disney, and explore the characters which we are still to this day gradually a little bit afraid of in a new light.


## Dataset

The dataset was extracted from the Disney Fandom Wiki webpage, and it contains all the character villains from Disney. That includes characters from different universes, e.g Marvel, Pixar, Star Wars, Walt Disney and other. After having built and visualised the network, we decided to narrow the scope and maintaining at least some possibility of analysing information about the dataset, do to lack of internal connections in the whole Disney Villains dataset. We then chose to select a subset of the data, that represents one universe, Marvel.

## Goal

The goal of the project is to create an interesting network and extract valuable information about villains connections. We are interested in discovering a new perspective of the villains in the Disney universe and we also want to include some type of discovery in our results and se what characterises an evil villain. We want to be able to use the tools and methods that we have learned in this course, such as, sentimental analyses, WordClouds, extracting communities, and TF-IDF.


## Basic statistics

Some basic statistics about our dataset:

![stats]({{< baseurl >}}/images/stats.png)


Which universe kills the most of it's main antagonists?

![stats]({{< baseurl >}}/images/stats2.png)



![stats]({{< baseurl >}}/images/stats3.png)


In the bar plot above we see that the Star Wars Universe, is the universe with the highest percentage of deceased main villains. Indeed, the only ones that are currently alive in the Star Wars Universe, are the villains from the series currently on tv. Grand Admiral Thrawn, is the only one that (not a spoiler) got out of the whole tv show alive, even though it was implied that he was dead. Moreover, at first sight, Walt Disney seems to have quite a high percentage of deceased characters. This makes sense when we think about what used to happen with villains in older Disney movies, such as, Scar, Ursula, and more.  Finally, what we need to point out, is that if someone wants to be a bad guy, Pixar is the safest environment to do so, with only a 13% death rate of villains.

## Disney Villains Network

![stats]({{< baseurl >}}/images/villain_network.png)

This is the whole Villains network, with different colors for all four universes and we must say it looks a little crazy. On the figure, we see that there are some groups that are better connected than others. Those groups represent the different universes. The Marvel universe is displayed with green color, Star Wars with red color, Pixar with gray color, Walt Diseny with blue color and the villains who are not a part of a specific universe, are represented with pink color (Unknown).

# WordClouds per universe

![stats]({{< baseurl >}}/images/marvel.png)


![stats]({{< baseurl >}}/images/disneyw.png)


![stats]({{< baseurl >}}/images/starwars.png)


![stats]({{< baseurl >}}/images/pixar.png)

These are the WordClouds for all four universes, we were extremely happy with the outcome. We thought the WordClouds told a good story about different universes. If we take a further look into the Marvel WordCloud we see words like Spiderman, Loki, Marvel, comics, kill, return, Hulk and Thor, these words are a great example of what the Marvel universe is all about. The same can be said about the other universe WordCloud, for example, in Disney WordCloud we see words such as tell, time, show, and appearance, these are all words that fit well when telling a story as Walt Disney does. In the Star Wars WordCloud, we see words like Vader which is a famous character in the Star Wars movie. Finally, in the Pixar WordCloud, we see words such as Buzz, toy, Mater, incredible, and Woody.







