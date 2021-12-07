---
title: "2. Marvel Villains"
date: 2021-12-06T14:29:55+01:00
featured_image: '/images/marvel.jpeg'
body_classes: "avenir bg-white"
---

## Basic statistics

Some basic statistics about the Marvel villain network. Below is the top 5 highest in- and out-degree for the Marvel villain network: 

![network]({{< baseurl >}}/images/in.png)

![network]({{< baseurl >}}/images/out.png)
 

Then we want to explore the betweenness centrality, here we can see the top 10 characters with the highest betweenness centrality in the Marvel universe:

![network]({{< baseurl >}}/images/BC.png)


Betweenness centrality is a measure, based on the shortest path. All the nodes in our network are connected, so for couple of the node, there is a shortest path. The value of betweenness centrality for a node n is measured as the number of shortest paths that pass through node n (not counting the shortest paths initiated or ended in n) and then modded by dividing with the total number of shortest paths in the network. Generally, the higher the number means the node has more influence in the network since more information passes through it.

In our network, we see that Thanos has by far the greatest influence in the Marvel universe, not only because he is a main antagonist in the most recent Marvel movies, but mostly because of his regular appearances in comics since 1973. This is represented by the fact that he is a part of 25% of the total shortest paths. In the next place is Loki, who has multiple on-screen appearances and third is Ultron who, as an enemy of Avengers, cooperates has joined forces with many other villains.

In the graph below we can see Thanos connections highlighted

#### Thanos connections
![network]({{< baseurl >}}/images/BC_vis.png)

## The network

This is the Marvel villains network. The nodes are ranked based on their degree, so bigger nodes have a higher degree, and vice versa. Ranking the nodes based on degree explains the network well, and it can be seen clearly what characters are the most connected. With this, we can get acquainted with the Marvel villain's network.

#### Marvel villains network

![network]({{< baseurl >}}/images/network.png)

## Communities

Below we can see the communities computed using a community detection algorithm, for the Marvel universe.  

![network]({{< baseurl >}}/images/communities.png)

Since the algorithm used is a stochastic process, the communities will differ every time the algorithm is run, however, we will be able to see specific patterns in relationships between characters. For example, Scorpio and Dr. Octapus will always be in the same community with The Venom as they are the main antagonists of Spiderman. In the same manner, Red Skull will be with Bucky Barnes, while Loki will be with the Asgardians (as well as with Variations of Loki that are considered different characters).

#### Communities visualised 

Furthermore, we used the information from the community detection algorithm to build the Marvel villains network in Gephi. We colored the nodes based on their communities.

![network]({{< baseurl >}}/images/network_comp.png)


## Sentiment analysis

We start by using the SentimentIntensityAnalyzer, which takes in a string and returns a dictionary with 4 scores for every character. The four scores are, negative, neutral, positive, and compound. The compound is computed by normalizing the three former mentioned scores. Then we compute the average compound score (happiness score), for the top 3 most connected characters in every community in our network.

The figure below shows the average compound scores for every community in our network. We notice that the community that contains Loki Laufeyson, Variants, and Asgardians always tend to have one of the lowest average compound scores, this is not a surprise since Loki Laufeyson is the biggest villain in the Marvel villain network.

![sentiment]({{< baseurl >}}/images/sentiment.png)


Next, we computed the happiness score for every villain in our Marvel network. Below are displayed both the top 10 villains with the highest happiness score and the top 10 villains with the lowest happiness score.

![sentiment]({{< baseurl >}}/images/happiness_score.png)

Then we found the average happiness score depending on the importance of a villain, in other words, if a character is a min antagonist or a lesser villain. We noticed that there is some difference in the scores, and the main antagonist tends to have a lower happiness score than the lesser villain. This seems accurate since the main antagonists are of course the worst villains.


![sentiment]({{< baseurl >}}/images/sentimental_graph.png)

From the figure above we see that the happiness score tends to be low. The mean value for the happiness score is -0.194 which is rather low and is in line with our network since we are examining the Marvel Villains and they are most often not described in a kind way.

Next, we looked at the average happiness score for the all the main antagonists of our network. The results can be seen on the figure below.

![sentiment]({{< baseurl >}}/images/sentimental_graph_2.png)

From this, we can conclude that the main antagonists are in fact much sadder than the others. By only looking at the main antagonists, the average happiness score dropped from -0.298 to -0.583.


![happy]({{< baseurl >}}/images/happy_wc.png)


![sad]({{< baseurl >}}/images/sad_wc.png) 

WordClouds were made for the happiest and the saddest villains, to get a better understanding of the data. We can see that the WordClouds tell a story. The happy WordCloud contains words and names. The names that appear large in the happy WordCloud are e.g Spider-Man, Nathaniel, and John. These are all defined as good characters in the Marvel universe. In the happy WordCloud, there also appear words like, find, power, shield, and life, which are all quite positive words.

However, in the sad WordCloud, there are names like Loki, Sylvie, and Mobius who are defined as bad characters in the Marvel universe. We also see words like kill, destroy, help, fight and take which are words that we can agree on describe sad situations.

## TF-IDF 

After examining the words from every community, we see that every community seems to tell a little story about part of the Marvel universe.

The stories are following:

-| Community 1: Marvel's Inhumans appear in this community, that are fictional characters who are Inhumans, a race of superhumans appearing in Marvel Comics
-| Community 2: This community is enhanced related. This category is for all individuals who were artificially enhanced.
-| Community 3: This comminity looks like it is Loki-related, who again, is the most connected villains in the Marvel universe.
-| Community 4: It looks like this community is Roxxon related. The Roxxon Energy Corporation is the name of a fictional massive petroleum industrial -| -|conglomerate in the Marvel Universe
-| Community 5: Finally, this community seems to be Combat-related, but Combat Was from Waco, Texas, and was highlight skilled in various forms of unarmed -|fighting.
Overall, within the Marvel universe, the communities appear to be rather reasonable.

## Description of Perfect villain

#### Description of EVILNESS: 

Description:

Be in the Marvel villain network.
Have high connections to other characters.
Be Main antagonist.
Have words like kill, fight and destroy in your description text.

And, if all else fails, just be more like LOKI LAUFEYJARSON!


