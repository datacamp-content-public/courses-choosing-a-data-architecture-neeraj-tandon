---
title: Insert title here
key: 35a9424dc6a263187b08bcf4cc18ccab

---
## Lesson 2.1: Intro to normalization

```yaml
type: "TitleSlide"
key: "a2526eb530"
```

`@lower_third`

name: Neeraj Tandon 
title: Instructor


`@script`



---
## Scenario: Managing Sales Data

```yaml
type: "FullSlide"
key: "b0e33f4877"
center_content: true
```

`@part1`
![](https://assets.datacamp.com/production/repositories/4703/datasets/f88d03cfe407bb928ae3f6bf6d8f23a7eb7e044a/data_camp_asset1.png)


`@script`
I’d like you to imagine you are a store manager of a new hip pet store called Pete's Pets. In this position you manage sales representatives, work with customers, and are charged with reporting sales performance back to Pete's Pets headquarters.


---
## Scenario: Managing Sales Data

```yaml
type: "FullSlide"
key: "6f207cf015"
```

`@part1`
Sales Log


![Sales Log](https://assets.datacamp.com/production/repositories/4703/datasets/5348c3327359a2b9d75d0e0f8be941d06e8abaed/datacamp_asset2.png)


`@script`
Currently, you use a spreadsheet where you task sales reps with logging their sales on a daily basis. This log gets reviewed on a weekly basis...
As you see we have a lot of fields. The log was created with the intention of tracking sales, but it looks like it’s also tracking other information like customer details, and store location. These are all important and valid data points to track, but what if we want to track more data points in the future? As our business grows we notice that the data grows as well. With more fields being added, we will be left with one gigantic table multiple sales reps will have to go in and update daily and include a lot of redundant information each item.


---
## Problem Scenario: Updating Customer Information

```yaml
type: "TwoColumns"
key: "909e3ece6b"
```

`@part1`
![Sales Log](https://assets.datacamp.com/production/repositories/4703/datasets/5348c3327359a2b9d75d0e0f8be941d06e8abaed/datacamp_asset2.png)


`@part2`
![](https://assets.datacamp.com/production/repositories/4703/datasets/1ac80a278e9ee568b083cbe80b093b97f6788305/datacamp_asset3.png)


`@script`
For instance, in the case of customer information, what if a customer updated their email?  To update the email, you would have to go to each transaction made in the sales log and manually change the customer’s email address. This is not only tedious but an error-prone process. Since email address tends to be used as a unique identifier for a customer, you run into the possibility of losing customer information if the email doesn’t get updated in all the right places. You no longer have a reliable method of capturing overall sales data and would struggle to do any sort of customer segmentation with your data. 


Structuring data this way is clearly problematic and with so many entities being represented, we certainly have our work cut out for us. Luckily there are some foundational rules for normalization that we use to our advantage to organize our data.


---
## Let's normalize this!

```yaml
type: "FinalSlide"
key: "6ec09ed301"
```

`@script`


