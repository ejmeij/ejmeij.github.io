---
title: "Dataset for 'Adding Semantics to Microblog Posts'"
date: "2012-01-05"
categories:
  - "blog"
tags:
  - "adding-semantics-to-micro-blog-posts"
  - "dataset-adding-semantics-microblog"
  - "dbpedia"
  - "don-meij-wiki"
  - "edgar-meij-pro"
  - "edgar-meij-twitter"
  - "entity-linking"
  - "microblogs"
  - "prodataset"
  - "semantic-linking"
  - "semantic-search"
  - "semantic-microblog-linking"
  - "semanticizing"
  - "text-mining"
  - "trec-2012"
  - "trec-micro-blogging"
  - "trec-microblogging-2012"
  - "twitter"
  - "twitter-dataset"
  - "twitter-tweets-dataset-json"
  - "wikipedia"
coverImage: "twitter_research.png"
---

As promised, I'm releasing the dataset used for my WSDM paper, [Adding Semantics to Microblog Posts](http://edgar.meij.pro/adding-semantics-microblogs/ "Adding Semantics to Microblog Posts") (with Wouter Weerkamp and Maarten de Rijke). In the paper, we evaluate various methods for automatically identifying concepts (in the form of Wikipedia articles) that are contained in or meant by a tweet. This release will consist of a number of parts and be downloadable from [http://ilps.science.uva.nl/resources/wsdm2012-adding-semantics-to-microblog-posts/](http://bit.ly/tDnf1n 'Twitter to concept annotations for the WSDM paper "Adding Semantics to Microblog Posts"'). The first part, described below, contains the tweets that we used, as well as the manual annotations, i.e., links to Wikipedia articles. If there is sufficient interest, I will also release the extracted features that were used in the paper. Let me know in the comments or drop me a line.

If you make use of this dataset, do remember to cite our paper. The bibliographic details can be found at [here](http://edgar.meij.pro/adding-semantics-microblogs/ "Adding Semantics to Microblog Posts"). If you have any questions, don't hesitate to ask me in the comments or by sending me an e-mail.

# Tweets

Twitter's Terms of Service do not allow me to redistribute the tweets directly, so I'm providing a file containing the tweet IDs, the username, and the MD5 checksum of each tweet. With the file 'wsdm2012_tweets.dat' you can use the [official tools](https://github.com/lintool/twitter-tools/ "twitter-corpus-tools @ GitHub") used in the [TREC Microblog track](https://sites.google.com/site/microblogtrack/ "TREC Microblog track homepage") to fetch them. Because of Twitter rate limits, I recommend using the JSON option in blocks of 150 tweets. If you are unsuccessful in downloading the tweets, drop me a line and I'll try to help you out.

Note that for the experiments done in the paper, we have annotated 562 tweets. In the mean time, however, tweets were deleted and accounts were banned. As such, you'll find that we are left with a slightly smaller number of tweets: 502 in particular.

# Annotations

We have asked two volunteers to manually annotate the tweets. They were presented with an annotation interface with which they could search through Wikipedia articles using separate article fields such as title, content, incoming anchor texts, first sentence, and first paragraph. The annotation guidelines specified that the annotator should identify concepts contained in, meant by, or relevant to the tweet. They could also indicate that an entire tweet was either ambiguous (where multiple target concepts exist) or erroneous (when no relevant concept could be assigned). For the 502 tweets listed above, the statistics are slightly different than reported in the paper. The average length of a tweet in this set equals 37. Out of the 502 tweets, 375 were labeled as not being in either of the two erroneous categories. For these, the annotators identified 2.17 concepts per tweet on average.

In the file 'wsdm2012_annotations.txt' you will find a tab-separated list with annotations. Here, the first column contains the tweet ID, the second column the annotated Wikipedia article ID, and the third column the title of the Wikipedia article. For ambiguous tweets the Wikipedia article ID equals '-1' and for unknown tweets the ID equals '-2' (for both of these cases the Wikipedia article title equals '-').

The 'wsdm2012_qrels.txt' file is a so-called _qrels_ file (in TREC parlance), that can be used with a tool such as [trec_eval](http://trec.nist.gov/trec_eval/ "NIST's trec_eval download ") as a gold standard. This file is derived from the manual annotations by considering all annotated links between a tweet and Wikipedia articles as 'relevant' and the remainder as being non-relevant. Recall that in our paper, we approach the task of linking tweets to concepts as a ranking task; more relevant concepts should be ranked above less relevant concepts. As such, we can rank Wikipedia articles for a given tweet and use [common Information Retrieval metrics](http://nlp.stanford.edu/IR-book/html/htmledition/evaluation-of-ranked-retrieval-results-1.html "Information Retrieval metrics for ranked result lists"), such as precision, MAP, R-precision, etc. to evaluate and compare different methods.
