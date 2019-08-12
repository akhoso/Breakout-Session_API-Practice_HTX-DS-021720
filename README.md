---
title: APIs-and-python
layout: post
weight: 10
hidden: true
---
​
APIs and Python Lesson Plan
===
​
​
**Course**: Data Science   <br/>
**Mod**: Module 2   V2                 <br/>
**Topic**: APIs and Python  <br/>
**Amount of time**: 1 hour <br/>
**Author**: Rachel Hirsch
​
​(Adapted from the ds-lesson-starters repository here)[]
***

#### Lesson Summary:

This lesson introduces the what and why of APIs followed by introductory examples of how to write some simple API requests using the requests package. The lesson gives some good backgrounds on HTTP requests and response status codes. Another package, `sodapy` is also introduced to make http requests to the NYC 311 API. Students are asked to investigate the structure of the data they receive and perform some initial exploratory analysis throughout.

#### Topic:

API Requests

#### Learn.co material:

* [HTTP Request/Response Cycle - Codealong](https://github.com/learn-co-curriculum/dsc-http-request-response-codealong)
* [Yelp API - Codealong](https://github.com/learn-co-curriculum/dsc-using-yelp-api-codealong)

#### Prerequisite knowledge/ Prework:

Lists and dictionaries.

#### Learning goals for this lesson:

  - Identify and discuss APIs
  - Explain the difference between POST and GET requests
  - Check the status of a request and interpret status codes
  - Discuss and explain different request (GET, POST, PUT, DELETE) and CRUD operations
  - Access data from an API using custom libraries and the requests library
  - Create a pandas dataframe from the data returned from an API and visualize the data

* Understand the concept of APIs
* Make API get requests
* Write Get request headers
* Parse an http response

#### Key Takeaways

* HTTP get requests will respond with an object that contains a status code AND content
* The content you are interested in will be stored under the `.json()`	method of the object.
* You can also send data to a HTTP endpoint with a post request
* JSON files are nested data structures similar to nested dictionaries and lists
* Be careful about API rate limits when making requests

#### Misconceptions / Notes


#### Materials
- Ipython notebook

#### Vocab / Concepts 

* HTTP Requests
* HTTP Status Codes: 200, 400, 404
* HTTP Get / Post Requests
* API
* Headers

#### Lesson Outline:

## Lesson Outline:

**Step**: Introduction and outline of lesson <br/>
**Time**: 2 min

_Goal/Scenario:_<br/>

_Learning Goals in sequence:_<br/>
  - Identify and discuss APIs
  - Explain the difference between POST and GET requests
  - Check the status of a request and interpret status codes
  - Discuss and explain different request (GET, POST, PUT, DELETE) and CRUD operations
  - Access data from an API using custom libraries and the requests library
  - Create a pandas dataframe from the data returned from an API and visualize the data

**Step**: Activation <br/>
**Time**: 3 min

Discussion prompts:
Using the following discussion prompts, ellicit responses from the students.
- What is an API?
- Why might data scientists be interested in utilizing APIs?

**Scope** Any time you want to get information from a given API, write a small test script and make sure it actually allows you to access the things you need in the way you require.<br>

*cost* Whatever the commercial model, all APIs have some kind of rate limiting. Because it costs money to keep computers running and because you could write a script to ask lots and lots of questions of an API, generally an API will have some kind of limitations on the number of "API calls" you can make against the service per unit of time. 


**Step**: Learning Goal 1: _Identify and discuss APIs_ <br/>
**Time**: 8 min

_Demonstrate_: 4 min <br/>
- Discuss what an API is and how it operates
- Discuss request-response cycles


_Application_: 3 min <br/>
- Students will name APIs they are familiar with, and discuss how they might work in practice.
- In pairs, students will discuss how a web page uses request-response cycles and share
- Class discussion on what APIs are important to a data scientist in the wild.

_Informal assessment_: 1 min <br/>
Quiz class: Which of these is an accurate description of a request?

**Step**: Learning Goal 2: _Explain the difference between POST and GET requests_ <br/>
**Time**: 7 min

_Demonstrate_: 3 min <br/>
- Using the requests library, demonstrate a GET request and discuss the results.
- Using the requests library, demonstrate a POST request and discuss the results.

_Application_: 3 min <br/>
- In pairs, students will come up with analogies for GET and POST requests, and share them with the class.
- In pairs, students will discuss how a GET request and a POST request function, and share with the class.

_Informal assessment_: 1 min <br/>
"Thumbs up: I understand the differences between GET and POST, thumbs down: I don't understand the differences, thumbs in the middle: I kind of understand the differences."
- follow up with any students who are not a thumbs up

**Step**: Learning Goal 3: _Check the status of a request and interpret status codes_ <br/>
**Time**: 7 min

_Demonstrate_: 3 min <br/>
- Show different classes of status codes and call out common codes
- Use requests to get status codes for a request that worked and a broken request

_Application_: 3 min <br/>
- Students will peruse http.cat to familiarize themselves with some different status codes and ask questions about them.

_Informal assessment_: 1 min <br/>
"Thumbs up, down, or middle on obtaining status codes from requests and interpreting them."
- follow up with any non-thumbs up reponses

**Step**: Learning Goal 4: _Discuss and explain different request (GET, POST, PUT, DELETE) and CRUD operations_ <br/>
**Time**: 9 min

_Demonstrate_: 3 min <br/>
- Discuss and describe the way GET, POST, PUT, and DELETE requests work with the database
- Discuss and explain CRUD operations (Create, Read, Update, and Delete) and how they fall in line with the requests

_Application_: 5 min <br/>
-
-

_Informal assessment_: 1 min <br/>
Quiz: "True or False: A POST request corresponds to the Update part of CRUD operations."


**Step**: Learning Goal 5: _Access data from an API using custom libraries and the requests library_ <br/>
**Time**: 12 min

_Demonstrate_: 4 min <br/>
- Grab a token from Socrata and discuss API keys verus secret keys
- pip install sodapy
- Use sodapy (custom, proprietary library to interact with API) to create a requests
- Use requests to create a request of the same API
- Compare results

_Application_: 7 min <br/>
- Students will pair together and code along with the instructor
- Students will grab their own tokens from Socrata to interact with APIs

_Informal assessment_: 1 min <br/>
"Thumbs up, down, or middle on accessing data from an API using Python."
- follow up with any non-thumbs up reponses

**Step**: Learning Goal 5: _Create a pandas dataframe from the data returned from an API and visualize the data_ <br/>
**Time**: 12 min

_Demonstrate_: 4 min <br/>
- Make a dataframe from the sodapy results

_Application_: 7 min <br/>
- Students will make a dataframe from the requests results
- Students will visualize the highest levels of complaints by total number

_Informal assessment_: 1 min <br/>
"Thumbs up, down, or middle on creating a pandas dataframe from the data returned from an API"
- follow up with any non-thumbs up reponses


**Step**: Assessment: API practicuum? <br/>
**Time**: 17 min<br/>


**Step**: Reflection:  <br/>
**Time**: 5 min <br/>
- "What was one thing that you found challenging, one thing that suprised you, and one thing you found interesting?"

#### To Do / Steps For Improvement

* Checks for Understanding
* Student Practice Questions
