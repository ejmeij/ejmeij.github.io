---
title: "OpenGeist: Insight in the Stream of Page Views on Wikipedia"
date: "2012-07-03"
categories: 
  - "publication"
  - "workshop"
tags: 
  - "api"
  - "bettina-berendt"
  - "edgar-meij"
  - "google-plus-api"
  - "opengeist"
  - "rest"
  - "time-series"
  - "wikipedia"
  - "wikistats"
coverImage: "taia2.jpg"
---

We present a RESTful interface that captures insights into the zeitgeist of Wikipedia users. In recent years many so-called zeitgeist applications have been launched. Such applications are used to gain insights into the current gist of society and actual affairs. Several news sources run zeitgeist applications for popular and trending news. In addition, there are zeitgeist applications that report on trending publications such as LibraryThing, and trending topics, such as Google Zeitgeist. There is an interesting open data source from which a stream of people’s changing interests can be observed across a very broad spectrum of areas: the [Wikimedia access logs](http://dumps.wikimedia.org/other/pagecounts-raw/ "Wikimedia raw page counts"). These logs contain the number of requests made to any Wikimedia domain, sorted by subdomain, and aggregated on an hourly basis. Since they are a log of the actual requests, they are noisy and can also contain non-existing pages. They are also quite large, yielding 60 GB worth of compressed textual data per month. Currently, we update the data on a daily basis and filter the raw source data by matching the URLs of all English Wikipedia articles and their redirects.

In this paper we describe an API that facilitates easy access to the access logs. We have identified the following requirements our system should have:

- The user must have access to the raw time series data for a concept.
- The user must be able to find the N most temporally similar concepts.
- The user must be able to group concepts and their data, based either on the categorial system of Wikipedia or on similarity between concepts.
- The system must return either a textual or a visual representation.
- The user should be able to apply time series filters to extract trends and (recurring) events.

The API is an interface for clustering and comparing concepts based on the time series of the number of views of their Wikipedia page.

See http://www.opengeist.org for more info and examples.

\[bibtex key=SIGIR-WS:2012:Peetz\]
