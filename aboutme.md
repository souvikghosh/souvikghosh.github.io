---
layout: page
title: Projects
subtitle: Something practical!
---

##Data Mining & Analysis

-  **[Twitter Sentiment Analysis](http://github.com/souvikghosh/TwitterSentimentAnalysis)** - A python based sentiment analysis module based on <b>nltk</b>, <b>scikit learn</b> and <b>tweepy</b> libraries. This basic purpose behind this project is to classify an incoming tweet into a positive or negative sentiment and to graph it live using <b>matplotlib</b>. <br><br>
Various tools of nltk are used in the very beginning to format the unstructured data(tweets) example- <b>tokenizing</b>, removing stop words, <b>pos</b> tagging. For training and testing the classifier, movie review corpora is used which has 1000 postive and negative reviews. To test things out,<b>Naive Bayes classifier</b> from the nltk module itself is used. Investigating the bias I found the classifier biased towards negative.<br><br>
To make the system more reliable a number of classifiers from sklearn's linear and svm modules are used. A voting system is implemented wherein each classifier votes either positve or negative and a confidence rating. Only if certain number of classifiers have the same result and the confidence is above a certain threshold(80% in this case), is the classification accepted.

-  **[Popularity classifification using Tweepy](http://github.com/souvikghosh/TwitterAnalysis)** - This project uses Twiter data to compare the popularity of three teams(manchester united, real madrid and barcelona). Twitter data is accessed using the <b>tweepy</b> to connect to twitter streaming API.<br><br> Python libraries used for analysis are : <b>json</b> for parsing the data, <b>pandas</b> for data manipulation, <b>matplotlib</b> for creating charts, and <b>re</b> for regular expressions. 3 charts describe all the results, which team got how many tweets, top 5 languages in which the tweets were written, and top 5 countries from which the tweets were sent.

##Networks and Communications

-  **[Design of a TDMA based coordinated MAC protocol whyNET](https://drive.google.com/file/d/0B1h-tBgm4w9VWHhSeFlqMVYyWHc/view?usp=sharing)** - This project provides a high level description of Link layer and MAC layer for a new High Speed Wireless Network (whyNET). WhyNET is a packet based <b>TDMA</b> network which essentially makes better utilization of the network. Existing 802.11n protocols have a large chunk of data transmissions as overheads which reduces throughput to a large extent.<br><br> The reason behind developing this protocol is to make a better utilization of the bandwidth. This is achieved by using lower values of interframe space and reducing the overheads. 
In traditional 802.11 protocols real time data is not handled very efficiently. whyNET addresses that by first of all segregating data into asynchronous and isochronous and giving higher priority to isochronous.<br><br> The issue of throughput degradation because of unnecessary interframe spaces in 802.11 protocols cannot be solved just by increasing the bandwidth. There is a fundamental challenge posed by using CSMA/CA method which needs new approach. whyNET provides a completely new approach to solving the problems posed by traditional 802.11 protocols. Throughput is only about 50% while using a traditional 802.11 network whereas using whyNET it increases significantly.

##Embedded System

-  **[GSM Based Voting System](https://docs.google.com/presentation/d/1SwUJ1Veg-fo0YyJ87p4SAU5JfBwtyE7vf4HIxDfZ8HM/edit?usp=sharing)** - This project is an attempt to explore the field of sms based voting system through the use of gsm.The basic thought behind this is the use of our mobile devices for the purpose of voting.Using this sms based voting system we can vote from our mobile using a specified format.Each voter will  be provided with a unique password and identification number.<br><br>A GSM module will receive the sms and decode it along with verifying the password and the id number.If  both the numbers match then the system will accept the vote and display the vote count for all the parties on the LCD.In the case either one or both the codes do not match then the system will reject the vote and a fail message will appear on the LCD. AT89C51 (an 8051 microprocessor from Atmel) was used along with a standard GSM module and programmed using the xilinx software.
