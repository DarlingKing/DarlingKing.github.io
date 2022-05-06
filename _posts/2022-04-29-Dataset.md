---
layout:     post
title:      Dataset
subtitle:   Twitter Friends
date:       2022-04-29
author:     Espen Sivertsen
header-img: img/the-first.png
catalog:   true
---
The dataset used was provided by Hubert Wassner and downloaded from “[Kaggle](https://www.kaggle.com/datasets/hwassner/TwitterFriends)”. The dataset is 448.5 MB, consists of 40 000 tweets (rows) and has the following 10 properties (columns) for each tweet

•	id the id of the author of the tweet
br
•	screenName The screen name of the author
br
•	tags The hashtags in the tweet (can be with or without #).
br
•	avatar URL to the profile picture of the tweeter.
br
•	followersCount Amount of people the tweeter is following
br
•	friendsCount Amount of people following the tweeter
br
•	lang Language, declared by the user.
br
•	lastSeen Time stamp of when this tweeter last tweeted
br
•	tweetId Id of the tweet
br
•	friends The IDs of the users the tweeter follows.

The tweets are chosen because they are tweets about Twitter trending topics. To filter out spam and non-informative accounts the creator of the set filtered out users that has less than 100 followings and followers. 

The dataset was chosen as it was based on trending topics. If it was just 40 000 completely random tweets, there is a chance that there will be no coherence between the tweets, say there is 40 000 unique tags. This analysis requires some degree of coherence to find the connection between users.

For the data pre-processing part, the data was changed to the required dictionaries, as all the data in the dataset is not necessary for the analysis. The dictionaries required were

•	user_friends a user and his friends. Started by building an unweighted edge, then built a graph based on that edgelist.
br
•	user_tags a user and his used tags
br
•	tag_users a tag and its corresponding users

The network analyzed has 12 891 798 nodes, 32 842 959 edges and the average degree is 5.095. The reason there are 12 891 798 users and not 40 000 is because every user’s friend is also counted as a node as well. This means that if a user has 500 friends, all 500 friends are treated as nodes.