#System Design Interview

System design is a very broad topic. Even a software engineer with many years of working experience at top IT company is not an expert
on system design. If you want to become an expert, you need to read many books, articles, and solve real large scale system design problems.

This repository only teaches you to handle the system design interview with a systematic approach in a short time. You can dive into each topic if you have time.

## <a name='toc'>Table of Contents</a>
* [System Design Interview Tips](#tips)
* [Basic Knowledge about System Design](#intro)
* [Company Engineering Blogs](#blog)
* [Products and Systems](#system)
* [Hot Questions and Reference](#qs)
* [Other Related Topics](#other)

###<a name='tips'>System Design Interview Tips:</a>

**Clarify the constraints and identify the user cases**

Spend a few minutes questioning the interviewer and agreeing on the scope of the system.
Remember to make sure you know all the requirements the interviewer didn't tell your about in the beginning.

User cases indicate the main functions of the system, and constraints list the scale of the system such as requests 
per second, requests types, data written per second, data read per second.

**High-level architecture design**

Sketch the important components and the connections between them, but don't go into some details. 
Usually, a scalable system includes webserver (load balancer), service (service partition), database (master/slave database cluster plug cache).
 
**Component Design**

For each component, you need to write the specific APIs for each component. You may need to finish
the detailed OOD design for a particular function. You may also need to design the database schema for the database.

###<a name='intro'>Basic Knowledge about System Design:</a>

Here are some articles about system design related topics.  

* [How to Rock a Systems Design Interview](http://www.palantir.com/2011/10/how-to-rock-a-systems-design-interview/)
* [Scalable Web Architecture and Distributed Systems](http://www.aosabook.org/en/distsys.html)
* [Numbers Everyone Should Know](http://everythingisdata.wordpress.com/2009/10/17/numbers-everyone-should-know/)
* [Scalable System Design Patterns](http://horicky.blogspot.com/2010/10/scalable-system-design-patterns.html)
* [Introduction to Architecting Systems for Scale](http://lethain.com/introduction-to-architecting-systems-for-scale/)
* [Transactions Across Datacenters](http://snarfed.org/transactions_across_datacenters_io.html)
* [A Plain English Introduction to CAP Theorem](http://ksat.me/a-plain-english-introduction-to-cap-theorem/)
* [The CAP FAQ](https://github.com/henryr/cap-faq)
* [Paxos Made Simple](http://research.microsoft.com/en-us/um/people/lamport/pubs/paxos-simple.pdf)
* [Consistent Hashing](http://www.tom-e-white.com/2007/11/consistent-hashing.html)
* [NOSQL Patterns](http://horicky.blogspot.com/2009/11/nosql-patterns.html)

Of course, if you want to dive into system related topics, here is a good collection of reading list about [services-engineering](https://github.com/mmcgrana/services-engineering), and
a good collection of material about [distributed systems](http://dancres.github.io/Pages/).


###<a name='blog'>Company Engineering Blogs:</a>

If you are going to have an onsite with a company, you should read their engineering blog. 

* [High Scalability](http://highscalability.com/)
* [The GitHub Blog](https://github.com/blog/category/engineering)
* [Engineering at Quora](http://engineering.quora.com/)
* [Yelp Engineering Blog](http://engineeringblog.yelp.com/)
* [Twitter Engineering](https://engineering.twitter.com/)
* [Facebook Engineering](https://www.facebook.com/Engineering)
* [Yammer Engineering](http://eng.yammer.com/blog/)
* [Etsy Code as Craft](http://codeascraft.com/)
* [Foursquare Engineering Blog](http://engineering.foursquare.com/)
* [Airbnb Engineering](http://nerds.airbnb.com/)
* [WebEngage Engineering Blog](http://engineering.webengage.com/)
* [LinkedIn Engineering](http://engineering.linkedin.com/blog)
* [The Netflix Tech Blog](http://techblog.netflix.com/)
* [BankSimple Simple Blog](https://www.simple.com/engineering/)
* [Square The Corner](http://corner.squareup.com/)
* [SoundCloud Backstage Blog](https://developers.soundcloud.com/blog/)
* [Flickr Code](http://code.flickr.net/)
* [Instagram Engineering](http://instagram-engineering.tumblr.com/)
* [Dropbox Tech Blog](https://tech.dropbox.com/)
* [Cloudera Developer Blog](http://blog.cloudera.com/blog/)
* [Bandcamp Tech](http://bandcamptech.wordpress.com/)
* [Oyster Tech Blog](http://tech.oyster.com/)
* [THE REDDIT BLOG](http://www.redditblog.com/)
* [Groupn Engineering Blog](https://engineering.groupon.com/)
* [Songkick Technology Blog](http://devblog.songkick.com/)
* [Google Research Blog](http://googleresearch.blogspot.com/)
* [Pinterest Engineering Blog](http://engineering.pinterest.com/)
* [Twilio Engineering Blog](http://www.twilio.com/engineering)
* [Bitly Engineering Blog](http://word.bitly.com/)


###<a name='system'>Products and Systems:</a>

The following papers/articles/slides can help you to understand the general design idea of different real products and systems. 

* [MapReduce: Simplied Data Processing on Large Clusters](http://static.googleusercontent.com/media/research.google.com/zh-CN/us/archive/mapreduce-osdi04.pdf)
* [Bigtable: A Distributed Storage System for Structured Data](http://www.read.seas.harvard.edu/~kohler/class/cs239-w08/chang06bigtable.pdf)
* [The Google File System](http://static.googleusercontent.com/media/research.google.com/zh-CN/us/archive/gfs-sosp2003.pdf)
* [The Chubby lock service for loosely-coupled distributed systems](http://static.googleusercontent.com/external_content/untrusted_dlcp/research.google.com/en/us/archive/chubby-osdi06.pdf)
* [Dynamo: Amazon's Highly Available Key-value Store](http://www.read.seas.harvard.edu/~kohler/class/cs239-w08/decandia07dynamo.pdf)
* [Introduction to Memcached](http://www.slideshare.net/oemebamo/introduction-to-memcached)
* [Cassandra Introduction Features](http://www.slideshare.net/planetcassandra/cassandra-introduction-features-30103666)
* [Introduction to HBase](http://www.slideshare.net/alexbaranau/intro-to-hbase)
* [Introduction to MongoDB](http://www.slideshare.net/mdirolf/introduction-to-mongodb)
* [Introduction to Redis](http://www.slideshare.net/dvirsky/introduction-to-redis)
* [Storm](http://www.slideshare.net/previa/storm-16094009)
* [Introduction to Zookeeper](http://www.slideshare.net/sauravhaloi/introduction-to-apache-zookeeper)
* [Kafka](http://www.slideshare.net/mumrah/kafka-talk-tri-hug)
* [YouTube Architecture](http://highscalability.com/youtube-architecture)
* [Scalinig Pinterest](http://highscalability.com/blog/2013/4/15/scaling-pinterest-from-0-to-10s-of-billions-of-page-views-a.html)
* [Google Architecture](http://highscalability.com/google-architecture)
* [Scaling Twitter](http://highscalability.com/scaling-twitter-making-twitter-10000-percent-faster)
* [The WhatsApp Architecture](http://highscalability.com/blog/2014/2/26/the-whatsapp-architecture-facebook-bought-for-19-billion.html)
* [Flickr Architecture](http://highscalability.com/flickr-architecture)
* [Amazon Architecture](http://highscalability.com/amazon-architecture)
* [Stack Overflow Architecture](http://highscalability.com/blog/2009/8/5/stack-overflow-architecture.html)
* [Pinterest Architecture](http://highscalability.com/blog/2012/5/21/pinterest-architecture-update-18-million-visitors-10x-growth.html)
* [Tumblr Architecture](http://highscalability.com/blog/2012/2/13/tumblr-architecture-15-billion-page-views-a-month-and-harder.html)
* [Instagram Architecture](http://highscalability.com/blog/2011/12/6/instagram-architecture-14-million-users-terabytes-of-photos.html)
* [TripAdvisor Architecture](http://highscalability.com/blog/2011/6/27/tripadvisor-architecture-40m-visitors-200m-dynamic-page-view.html)
* [Scaling Mailbox](http://highscalability.com/blog/2013/6/18/scaling-mailbox-from-0-to-one-million-users-in-6-weeks-and-1.html)
* [Salesforce Architecture ](http://highscalability.com/blog/2013/9/23/salesforce-architecture-how-they-handle-13-billion-transacti.html)
* [ESPN's Architecture](http://highscalability.com/blog/2013/11/4/espns-architecture-at-scale-operating-at-100000-duh-nuh-nuhs.html)

###<a name='qs'>Hot Questions and Reference:</a>

**Design a CDN network**

**Design a Google document system**

**Design a random ID generation system**

**Design a key-value database**

**Design the Facebook new seed function**

**Design a function to return the top k requests during past time interval**

**Design an online card game game** 

**Design a graph search function**

**Design a picture storage system** 

**Design a search engine**

**Design a recommender system**

**Design a tinyurl system** 

**Design a garbage collection system**
 
**Design a scalable web crawling system**

**Design the facebook chat function**

**Design a cache system** 

**Design a payment system**

###<a name='other'>Other Related Topics:</a>


