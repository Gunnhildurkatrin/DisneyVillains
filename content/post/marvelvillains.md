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

Betweenness centrality was explored. Here are displayed the top 10 characters with the highest betweenness centrality in the Marvel universe:

![network]({{< baseurl >}}/images/BC.png)


Betweenness centrality is a measure based on the shortest path. All nodes in a network are connected, so for some nodes, there is a shortest path. The value of betweenness centrality for a node n is measured as the number of shortest paths that pass through node n (not counting the shortest paths initiated or ended in n) and then modded by dividing with the total number of shortest paths in the network. Generally, the higher the number, the more influence a node has in a network, since more information passes through it.

In the Marvel villain's network, it can be seen that Thanos has the greatest influences in the Marvel universe, not only because he is one of the main antagonists in the most recent Marvel movies, but also because of his regular appearances in comics since 1973. This is represented by the fact that he is a part of 25% of the total shortest paths. The villain with the second-highest betweenness centrality is Loki, who has multiple on-screen appearances and the third is Ultron who, as an enemy of Avengers, has joined forces with many other villains.

In the graph below Thanos connections are highlighted:


#### Thanos connections
![network]({{< baseurl >}}/images/BC_vis.png)


## The network

This is the Marvel villain's network. The nodes are ranked based on their degree or the number of connections they have, so bigger nodes have more connections, and vice versa. Ranking the nodes based on degree explains the network well, and it is clear what characters are the most connected. Here it is obvious that Loki Laufeyson and Thanos are the most connected villains.



#### Marvel villains network

![network]({{< baseurl >}}/images/network.png)

## Communities

Below are all communities for the Marvel universe displayed, along with their size and the characters with the top three highest connections within per community. The communities are computed by using a community detection algorithm.   

![network]({{< baseurl >}}/images/communities.png)

Since the algorithm that is used to compute the communities uses a stochastic process, the communities will differ every time the algorithm is run. However, specific patterns in relationships between characters can be identified. For example, Scorpio and Dr. Octapus will always be in the same community with The Venom as they are the main antagonists of Spiderman. In the same manner, Red Skull will be with Bucky Barnes, while Loki will be with the Asgardians (as well as with Variations of Loki that are considered different characters).



#### Communities visualised 

Information from the community detection algorithm is used to build a Marvel villain's network in Gephi. The nodes are colored based on their communities. 

![network]({{< baseurl >}}/images/network_comp.png)



## Sentiment analysis

The figure below shows the average compound score for every community in the Marvel villains network. Communities that include Loki Laufeyson, Variants, and Asgardians always tend to have one of the lowest average compound scores, this is not a surprise since Loki Laufeyson is the biggest villain in the Marvel villain network.

![sentiment]({{< baseurl >}}/images/sentiment.png)

Next, the happiness score for every villain in the Marvel network is found. Below are displayed both the 10 villains with the highest happiness score and the 10 villains with the lowest happiness score.

![sentiment]({{< baseurl >}}/images/happiness_score.png)

#### The average happiness score for the Marvel Villains

![sentiment]({{< baseurl >}}/images/sentimental_graph.png)


The figure above shows that the happiness scores tend to be low. The mean value for the happiness score is -0.298 which is rather low but is in line with the network as this is a Marvel villains network and the villains are most often described in a bad way. 

Next, a bar plot of the average happiness score for all the main antagonists of the Marvel villain's network is displayed.

#### The average happiness score for the Marvel main antanogists

![sentiment]({{< baseurl >}}/images/sentimental_graph_2.png)

From this figure it can be concluded that the main antagonists are in fact much sadder than the other villains. By only looking at the main antagonists, the average happiness score dropped from -0.298 to -0.583.



#### Happy WordCloud

![happy]({{< baseurl >}}/images/happy_wc.png)

The names that appear large in the happy WordCloud are e.g Spider-Man, Nathaniel, and John. These are all defined as good characters in the Marvel universe. In the happy WordCloud, there also appear words like, find, power, shield, and life, which are all rather positive words.



#### Sad WordCloud

![sad]({{< baseurl >}}/images/sad_wc.png) 

However, in the sad WordCloud, there are names like Loki, Sylvie, and Mobius who are defined as bad characters in the Marvel universe. In the sad WordCloud, there also appear words like kill, destroy, help, fight and take which are words that describe sad situations.



## Description of EVILNESS: 

- Be in the Marvel villain network.
- Have high connections to other characters.
- Be alive
- Be a main antagonist.
- Have words like kill, fight and destroy in your description text.

And, if all else fails, just be more like THANOS and LOKI LAUFEYJARSON!
