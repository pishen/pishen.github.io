---
layout: github
---

# Pishen Tsai
[github.com/pishen](https://github.com/pishen) | [facebook.com/pishen](https://www.facebook.com/pishen)

## Experience

### Engineer @ KKBOX Research Center

(2014-11 - 2016-09)

Introduced the knowledge and solutions of Scala/Spark into KKBOX. Helped training other programmers to use Scala/Spark in big data processing jobs, such as analytics report of users' behavior log or recommendation system. Created tool like [spark-deployer](https://github.com/KKBOX/spark-deployer) to help lowering the learning and maintaining burden of big data workflow.


On the other hand, I participated in the development of KKBOX's new recommendation system, including personalized feed, playlist generation, and radio system. Using machine learning tools like Google's word2vec, Spark's MLlib, and some speed-up indexing algorithms like locality sensitive hashing or [spotify/annoy](https://github.com/spotify/annoy).
I also developed an internal web application called "KKRadio", which can let a KKBOX's user login, choose preference, and listen to an auto-generated radio playlist. The algorithm used to generate the radio can be added, removed, and switched easily for the QA and developers to compare the performance between different algorithms.

### Summer Intern @ Yahoo! Taiwan

(2013-07 - 2013-08)

Surveyed how to use Spark and gave some tech-sharing to colleagues in Data Team. Rewrote the collaborative filtering algorithm in Yahoo! Shopping Mall using Spark and achieved a 7x speed up. I also demonstrated the result on Yahoo! Intern Day and won the Most Popular Award.

## Projects

### VocaRadio
[vocaradio.com](https://www.vocaradio.com) is a 24/7 web radio station which contains 1600+ VOCALOID songs. The songs are played by YouTube's embedded player. And the system will synchronize all playing status between each listener to make everyone listen to the same location of the same song at same time. Hence the listeners can discuss currently playing song in a websocket chat room. All the song information are searched and updated from YouTube's API. There's also a request system that can let user change the order of incoming songs, and a backend panel for DJ to add/remove songs and manage current playlist. The whole station is written in Scala using Play Framework.

### spark-deployer
[KKBOX/spark-deployer](https://github.com/KKBOX/spark-deployer) is a SBT plugin which is able to deploy Spark cluster on Amazon EC2 in a very simple command. Developers can use it to go through the whole big data workflow from writing and compiling their job's source code to running it on a real cluster. All the dirty works are done by SBT, which is the only required tool if you want to write a Spark job. This tool is open sourced under KKBOX and has got adoption and [pull request](https://github.com/KKBOX/spark-deployer/pull/11) from Vpon. I also gave a [talk](https://www.youtube.com/watch?v=XWhQlhuBq2Q) about spark-deployer at JCConf 2015.

### lsh4s/annoy4s
LSH (Locality Sensitive Hashing) is an approximated algorithm which can speed-up the retrieval of nearest neighbors in a large and high-dimension vector space. This algorithm is especially useful when your vector space is large, such as KKBOX's song model in recommendation system, which contains millions of songs. In KKBOX, I implemented a simple LSH algorithm called [lsh4s](https://github.com/pishen/lsh4s), which can be combined with Spark in a very easy way. On the other hand, I also wrote a JNA wrapper called [annoy4s](https://github.com/pishen/annoy4s), which can control the C++ library of [spotify/annoy](https://github.com/spotify/annoy) directly from Scala/JVM. Both projects are open sourced on github. And annoy4s is proud to be mentioned on spotify/annoy's readme page.

## Talks
In my spare time, I join a group called [Scala Taiwan](http://www.meetup.com/Scala-Taiwan-Meetup/), where we hold small meetups in Taipei every month since 2016. I also gave two talks about [spark-deployer](https://speakerdeck.com/pishen/deploy-your-own-spark-cluster-in-4-minutes-using-sbt) and [SBT](https://speakerdeck.com/pishen/sbt-basic-concepts). In the meetup, we share knowledge and news about Scala, and help each other to work out some problems in programming. The community is growing and attracting more people to try Scala in Taiwan.

## Skills

* Spark, Play, Akka, Breeze, SBT, and 170+ starred Scala libraries and tools on github.
* Concepts of Scala's design, why static-typed, why functional, why actor model, why using `Future` in asynchronous programming.
* How to release open source project. How to write test and connect with TravisCI.
* Basic usage/understanding of collaborative filtering, word2vec, matrix factorization, SVM, decision tree, and the content of Hsuan-Tien Lin's [machine learning courses](https://www.coursera.org/instructor/htlin) on coursera.
* My main languages are Java and Scala, but I can write simple JavaScript, HTML and CSS, and can copy and paste Python code to make things work.

## Education
I got my bachelor and master degree from Computer Science and Information Engineering department in National Taiwan University (2007 - 2014).
