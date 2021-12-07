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

