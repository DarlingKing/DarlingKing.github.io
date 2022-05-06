---
layout:     post
title:      Discussion
subtitle:   Twitter Friends
date:       2022-04-29
author:     Espen Sivertsen
header-img: img/the-first.png
catalog:   true
---
As seen from the results one can definitely conclude that the "Six Degrees of Separation" exists in twitter. In every context tested the average distance is between 2-3 contacts, and the majority of the pairs are within 2-4 contacts. The results comply well with the idea introduced by Frigyes Karinthy, but are the results too good to be true?

Some of the elements in our dataset that may end up improving our results may be the size of the dataset, exclusively users with 100 followers/following, tweets based on trending topics and the uncertainty the term "social contact" in the twitter world.

The dataset only consists of tweets from users with more than 100 followers/following. Since there is a lot of users with less than this amount the results are not necessarily representative for the "average" twitter user, and therefore the "average" human. Maybe even there is a coherence between amount of followers and social interests? That will improve our stats if that is the case. This was a risk decided to be taken though, to be able to make sure that bots and spam got cleaned out, as mentioned earlier.

The dataset is based on tweets on trending topics. There is a greater chance that people that tweet about the same topics have a social contact only a few steps away, which again may be a reason for our good results. For example, if you are interested in football (soccer) and your followers/following is only people in the football industry, it will be easier to find a connection to other football fans than to people tweeting about domestic political problems in the Philippines. Thus, by only using trending tags it is a possibility that the paths may be shorter than if it was just completely randomized over a larger dataset.

Another question is whether twitter followers and people one follow are to be considered “social contacts”. Celebrities have millions of followers and should then every single one of these be considered as a part of the given celebrities social network? As seen from the code/results, a user in the dataset has just shy of 240k followers. These users may be a reason for such short distances. Maybe the results would have been more accurate if there was max limit of followers as well? Also, a lot of organizations (companies, sports teams, etc.) also use twitter to usually promote their own product, but also just to tweet about trending topics. Should they be considered social contacts?

There is also a chance that a too low sample size prevents a path of fewer steps. It is not unreasonable to assume that there are pairs in the dataset that would have been connected in a fewer steps if every single user would have been analysed. One pair that needs seven steps in this analysis may have a mutual friend that is not considered in the sample used, and therefore the path is longer than it could have been. This may be a reasoning for people not being within six steps.