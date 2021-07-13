





##  Review  

**What’s the difference between a FIFO and a standard queue?**  
`Standard queues` provide at-least-once delivery, which means that each message is delivered at least once. `FIFO queues` provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it.


**How can the server be assured a message was properly received?**   
we can create a connection msg to ensure the connection and other for disconnection


**What classic design pattern is best represented by event driven programming?**   
Event Notification pattern   

**How do you test an event driven system?**  
1. Unit tests are the most basic tests you will write.   
2. Service tests, as the name suggests, treat the entire service as the SUT, and increasingly, in microservice architectures this is where the bulk of automated testing occurs.    
3. end-to-end tests.

##  Vocabulary   

| voc                               | related to |
|-------------------------------------|--------------|
|FIFO Queue |queue that operates on a first-in, first-out (FIFO) principle.|
|Pub/Sub|pub/sub model, any message published to a topic is immediately received by all of the subscribers to the topic. |
|




## Preview  


*Which 3 things had you heard about previously and now have better clarity on?*  
- Pub/Sub
- testing
  

*Which 3 things are you hoping to learn more about in the upcoming lecture/demo?*  
-   Pub/Sub
-   testinp
  

*What are you most excited about trying to implement or see how it works?*  
- diving more deep on event driven system

&nbsp;

## Preparation Materials

> AWS SNS and SQS     
- Amazon SNS allows applications to send time-critical messages to multiple subscribers through a “push” mechanism, eliminating the need to periodically check or “poll” for updates. Amazon SQS is a message queue service used by distributed applications to exchange messages through a polling model, and can be used to decouple sending and receiving components—without requiring each component to be concurrently available.    

- Amazon SNS) is a fully managed messaging service for both application-to-application (A2A) and application-to-person (A2P) communication.   


* difference between SQS and SNS?
SNS is 
- `SQS` is mainly used to decouple applications or integrate applications.   
- `SNS` distributes several copies of message to several subscribers.

