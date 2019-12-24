# Yahoo! News Dataset
This repository contains the Yahoo! news dataset in paper [Read, Attend and Comment: A Deep Architecture for Automatic News Comment Generation (EMNLP2019)](https://www.microsoft.com/en-us/research/publication/read-attend-and-comment-a-deep-architecture-for-automatic-news-comment-generation/). The dataset is available in [tar](https://rinnaphilly24722.blob.core.windows.net/yangze/datasets/release_v1.tar.gz?st=2019-12-24T13%3A28%3A26Z&se=2022-12-25T13%3A28%3A00Z&sp=rl&sv=2018-03-28&sr=b&sig=rZ6jDQIjXc4KST7wVlRPf%2BTd60LxOXy6QQxhHgEeFJI%3D) and [zip](https://rinnaphilly24722.blob.core.windows.net/yangze/datasets/release_v1.zip?st=2019-12-24T13%3A29%3A03Z&se=2022-12-25T13%3A29%3A00Z&sp=rl&sv=2018-03-28&sr=b&sig=nPbrvcAChNbj2UXbft0ut37g9fAUPdtPNUwN%2FsKBwjk%3D).

We build this dataset by crawling news articles and the associated comments from [Yahoo! News](https://news.yahoo.com/). The side information associated with news including:
* __Paragraph__. After pre-processing, we retain the paragraph structure of news article.
* __Category__. There are 31 news categories and the distribution is shown in figure 1.
* __Wiki-Entities__. The Wikipedia entities mentioned in the news articles are extracted.
* __Vote__.  Each comment has upvote, downvote and abusevote information from news readers.
* __Sentiment__. Each comment is annotated with POSITIVE, NEGATIVE or NEUTRAL by Yahoo!.

![1](distribution_realease.png)

[//]: # (<img src="distribution_realease.png" width="200" height="200">)

After pre-processing, We randomly sample a training set, a validation set and a test set. Please refer to the paper for more details.

| | Train | Validation | Test|
|:----|:----:|:----:|:----:|
|\# News | 152,355  | 5,000 | 3,160 |
|Avg. \# Comments per News | 20.6     | 20.5  | 20.5|
|Avg. \#Upvotes per Comment | 31.4     | 30.2  | 32.0|
|Avg. \#DownVotes per Comment | 4.8      | 4.8   | 4.9|
|Avg. \#AbuseVotes per Comment | 0.05     | 0.05  | 0.05|

## Citation
If you use this dataset in your research work, please cite our [EMNLP2019 paper](https://www.aclweb.org/anthology/D19-1512/).
```bash
@inproceedings{yang-etal-2019-read,
    title = "Read, Attend and Comment: A Deep Architecture for Automatic News Comment Generation",
    author = "Yang, Ze  and
      Xu, Can  and
      Wu, Wei  and
      Li, Zhoujun",
    booktitle = "Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing and the 9th International Joint Conference on Natural Language Processing (EMNLP-IJCNLP)",
    month = nov,
    year = "2019",
    address = "Hong Kong, China",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/D19-1512",
    doi = "10.18653/v1/D19-1512",
    pages = "5076--5088",
}
```
 
