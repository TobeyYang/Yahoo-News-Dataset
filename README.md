# Yahoo! News Dataset
This repository contains the Yahoo! news dataset in paper [Read, Attend and Comment: A Deep Architecture for Automatic News Comment Generation (EMNLP2019)](https://www.microsoft.com/en-us/research/publication/read-attend-and-comment-a-deep-architecture-for-automatic-news-comment-generation/). The dataset is available [here]().

We build this dataset by crawling news articles and the associated comments from [Yahoo! News](https://news.yahoo.com/). The side information associated with news including:
* __Paragraph__. After pre-processing, we retain the paragraph structure of news article.
* __Category__. There are 31 news categories and the distribution is shown in figure 1.
* __Wiki-Entities__. The Wikipedia entities mentioned in the news articles are extracted.
* __Vote__.  Each comment has upvote, downvote and abusevote information from news readers.
* __Sentiment__. Each comment is annotated with POSITIVE, NEGATIVE or NEUTRAL by Yahoo!.

[//]:![1](distribution_realease.png)
<img src="distribution_realease.png" width="200" height="200">

After pre-processing, We randomly sample a training set, a validation set and a test set. The details are:

| | Train | Validation | Test|
|:----|:----:|:----:|:----:|
|\# News | 152,355  | 5,000 | 3,160 |
|Avg. \# Comments per News | 20.6     | 20.5  | 20.5|
|Avg. \#Upvotes per Comment | 31.4     | 30.2  | 32.0|
|Avg. \#DownVotes per Comment | 4.8      | 4.8   | 4.9|
|Avg. \#AbuseVotes per Comment | 0.05     | 0.05  | 0.05|


 
