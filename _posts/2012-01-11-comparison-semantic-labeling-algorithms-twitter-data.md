---
title: "A comparison of five semantic linking algorithms on tweets"
date: "2012-01-11"
categories:
  - "blog"
tags:
  - "algorithm-to-compare-text-semantically"
  - "clef-2012-replab"
  - "compare-semantic-search-with-full-text-search"
  - "dbpedia"
  - "entity-linking"
  - "microblogs"
  - "semantic-linking"
  - "semantic-search"
  - "semantic-algorithms-compare"
  - "semantic-text-api-compared"
  - "semantic-versioni-compare"
  - "semanticizing"
  - "spotlight-opencalais-comparison"
  - "text-mining"
  - "text-semantics-algorithms"
  - "twitter"
  - "twitter-api-spam-algorithm"
  - "twitter-hashtag-dbpedia"
  - "what-all-content-analysis-algorithms-are-there"
  - "wikipediaionsearchwikipediaconcept"
coverImage: "Twitter-256.png"
---

Late last December, Yahoo! released a new version of their Content Analysis service and they announced that the initial version will be deprecated in 2012. Inspired by a recent post by Tony Hirst, entitled [A Quick Peek at Three Content Analysis Services](http://blog.ouseful.info/2011/12/22/a-quick-peek-at-three-content-analysis-services/ "A Quick Peek at Three Content Analysis Services"), this seemed like a perfect opportunity to test out various algorithms/APIs for semantically annotating text, in particular tweets. For my WSDM paper, [Adding Semantics to Microblog Posts](http://edgar.meij.pro/adding-semantics-microblogs/ "Adding Semantics to Microblog Posts") (with Wouter Weerkamp and Maarten de Rijke), we have developed a gold-standard test collection for exactly this, i.e., automatically identifying concepts (in the form of Wikipedia articles) that are contained in or meant by a tweet.

What I wanted to do here is take [our recently released test collection](http://edgar.meij.pro/dataset-adding-semantics-microblog-posts/ "Dataset for “Adding Semantics to Microblog Posts”") and compare several off-the-shelf annotation APIs. In the paper, we already compare various methods, including Tagme and DBpedia spotlight. There, we add to this a variant solely based on the anchor texts found in Wikipedia, called 'CMNS' in the paper. In this post, I also include the new Yahoo! service and a service called Wikimeta. I have excluded OpenCalais from this list, mainly because it doesn't link to Wikipedia.

Highlights of the experimental setup:

- Approximately 500 tweets, with a maximum of 50 retrieved concepts, i.e., Wikipedia articles, per tweet.
- The tweet is tokenized, i.e., punctuation and capitalization is removed. Twitter-specific "terms" such as mentions and URLs, are also removed. For hashtags, I remove the '#' character but leave the term itself. Stopwords are removed. (More on this later.)

First, some general observations with respect to each API.

- DBpedia Spotlight feels sluggish and actually takes the longest to annotate all tweets (approx. 30 minutes).
- Tagme is blazingly fast, processing all tweets in under 60 seconds.
- Yahoo! is also fast, but not very robust. It gives intermittent HTTP 500 responses to web service calls.
- Wikimeta, well... First of all, the returned XML is not valid, containing unescaped '&' characters. After having manually fixed the output, it started nicely, but the web service seems to have crashed after processing 50 tweets. Update: things are back up and it finished within a few minutes.
- Finally, our method is also quite fast; it finished processing all tweets in under 90 seconds. Obviously we have a local installation of this, so there is little networking overhead.

Now, onto the results. Below, I report on a number of [metrics](http://nlp.stanford.edu/IR-book/html/htmledition/evaluation-of-ranked-retrieval-results-1.html "Evaluation of ranked retrieval results "), including average R-precision, i.e., precision at _R_, where *R* denotes the number of relevant concepts per tweet, reciprocal rank, i.e., the reciprocal of the rank of the first relevant concept, recall, and MAP (mean average precision)

\[table id=1 /\]

From this table it is clear that Tagme obtains high precision, with our method a close second. Reciprocal rank is high for both methods---a value of 0.6289 indicates the average rank of the first relevant concept lies around 1.6. Our method obtains highest recall--retrieving over 80% of all relevant concepts--and MAP, this time with Tagme as close second.

When running these experiments, it turned out that some methods use capitalization, punctuation, and related information to determine candidate concept links and targets; in particular Wikimeta and Yahoo! seem to be affected by this. So, in the next table you'll find the same results, only this time without any tokenization performed (and also without any stopwords removed). Indeed, Wikimeta improves considerably and also Yahoo! improves somewhat. There seems to be a little gain for DBpedia Spotlight in this case.

\[table id=2 /\]

To round up, some concluding remarks. Tweets are inherently different from "ordinary" text, and this evaluation has shown that the methods that perform best on short texts (for instance, the Tagme system) also perform best on tweets, when there is little data available for disambiguation. Wikimeta parses the input text and is thus helped by providing it with full-text (for as far as that goes with Twitter).

Finally, I discovered something interesting with respect to our test collection, namely that some of the contents already seem to be outdated. One of the tweets refers to "[Pia Toscano](http://en.wikipedia.org/wiki/Pia_Toscano "Pia Toscano")," but she wasn't in the annotators' version of Wikipedia yet. As such, some systems retrieve her correctly, although the annotations deem her not relevant. "Dynamic semantics." Sounds like a nice title for my next paper.
