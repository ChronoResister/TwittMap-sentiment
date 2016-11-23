# TwittMap-sentiment

### Group member: Bingxin Chen(bc1958) Zeyu Meng(zm649)

![alt text](https://raw.githubusercontent.com/ChronoResister/TwittMap-sentiment/master/sc1.jpeg "Screenshot1")
![alt text](https://raw.githubusercontent.com/ChronoResister/TwittMap-sentiment/master/sc2.jpeg "Screenshot2")
![alt text](https://raw.githubusercontent.com/ChronoResister/TwittMap-sentiment/master/sc3.jpeg "Screenshot3")

##Using Java Servlet and Tomcat 

- BacnEnd.java: Run on aws beanstalk worker environment. Backend of the Java Servlet. Load processed tweets from ElasticSearch.
- GetTweet.java: Use AWS SQS to stream tweets with key words.
- TweetProcess.java: Worker uses Alchemy API and AWS SNS, process tweets from SQS then send to backend.
- Tweet.java: define processed tweet as JSON format.
- frontend: use markers with different colors to represent different sentiment. Green - positive, blue - neural, red - negative. Staying mouse on markers will show the twitter text. Initial webpage shows all the keywords.




