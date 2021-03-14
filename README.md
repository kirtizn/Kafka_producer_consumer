# Kafka_producer_consumer
Kafka Producer and consumer code to read csv file

### Problem 1:

- Kafka producer that will read “SalesRecords.csv” file and convert each line to json and send the data to a Kafka topic(“test.topic.raw”)
- Kafka Consumer to check wheather the data was written to the topic or not.


### Problem 2:

Kafka consumer that will read data from the topic named “test.topic.raw”. It should read the data from the beginning and do the below filtering of data: 
 - Select only those data whose “Total Cost” value is greater than 304017.56 
 - After selection, it should send the filtered data to another topic named “test.topic.threshold_costs”


### Problem 3:
Write a Kafka consumer that will read data from multiple topics:
- The name of the topics is "test.topic.raw" and "test.topic.threshold_costs"
- Filter the data based on the country and send data to different topic depending on country value “test.topic.{country}"


### Problem 4:
Write down 2 Kafka consumers, both reading data from the same topic “test.topic.raw”. Both the consumers should receive the same messages and do as described ahead.

 Consumer1 should do the following:
- Get the “Sale Channel” from json data.
- Send data to a  Kafka topic depending on the channel of the sale. 
- List the topics, you should see all the topics created for each Sale Channel.

Consumer2 should do the following:
- Filter the data based on Unit Cost
 - Send data to Kafka topic named “topic.costly_order” if ‘Unit Cost’ is more than “10000” 
- Start consumer console to verify data reaching to the given topic.
        
  



 
