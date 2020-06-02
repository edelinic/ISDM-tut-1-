# Project Objectives
A major travel company has tasked us with developing an information system that improves the operation of their in-house call management centre. 
This system will automatically assign end customers to well informed relationship managers with appropriate knowledge of the destination and its traditions. 
This process is done based on the match between a customer's profile and a relationship managers profile and skill. 
A customers profile will be automatically made using a profiler tool and a relationship managers profile is made through a 10 minute questionnaire upon them being hired. 
A relationship managers profile may include age, sex, culture, language proficiency, experience and product knowledge. 
The system retrieves the customer details from the database and provides the relationship manager guidelines and a script to help provide improved service to the end customer. 
For Inbound calls a customer contacts the CMC which has its own private branch exchange to route calls. 
A customer will get a score from 1-10 based on the likelihood to purchase the product (e.g. repeat customers may have a higher score, customers from particular postcodes may have lower scores, etc..). 
Similarly a skill score is allocated to a relationship manager based on their previous call duration and profile. 
Customer is redirected to a relationship manager according to skills and best match. 
During busy times a customer is directed to an interactive voice response unit promoting them for options, and gathering information.

# Approaches/Justification
In our approach to this information systems development project we have decided to use design thinking. Design thinking is an approach that involves considering what technological assets available and what business strategies are reasonable can be converted into customer value. We have applied all 5 stages of design thinking in the project:

Empathise: In this stage we considered stakeholders involved with the information system development project and try to regard their wants/needs. Since we couldn't utilize interviews, we instead made reasonable assumptions based the requirement document given to us, and also created empathy maps to give us deeper insight to stakeholders.

Define: We define the problems that have been identified through empathising stage. We brainstormed point of view statements based off the requirements, assumptions and user story maps. These POV statements will allow us to ideate with a set goal in mind.

Ideate: Ideas are generated to solve the problems at hand and the best idea is used as the solution. We used the POV statemts to create HMW statemtents to help us come with ideas for the issues we have gathered. From there, we brainstormed user stories and developed a best solution.

Prototype: In this stage an early version of the product is made to test the voted solution, get feedback on the prototyped solution, reduce assumptions and answer questions. Models that we used in this project include:

1. * Case Diagrams: Give a simplist overview of the entities, relationships and cases. Furthermore, it can be used as a communication tool to between the development team and less software-literate stakeholders.

2. * Activity Diagrams: Give an overview of the flow of data within a specific case diagram. This will allow the development team to visualise what is the system needs.

3. * Class Diagrams: Give indepth view of the structure of the system. Classes, attributes, operations and relationships between objects are shown allowing for the developers to easily understand what needs to be done.

4. * Collaboration Diagrams: Show the relaionship between objects to create a particular use case. This will allow developers to easily understand and implement the objects and their relationships accordingly.

Test: This is an iterative process where tests are done on the completed product. Results used in this phase are used to redefine problems and show the understanding of a user when they are using the product. In this case we got weekly feedback from out tutor and made adjustments accordingly.

# Development Methodology (Agile)
The development methodology we have chosen to use is Scrum Methodology, which assumes the software development process is unpredictable. It is a continual iterative process where development is planned out into small increments and adjusted accordingly to any of the possible outcomes. The activities that we have used from scrum include:

1. * Backlog: We made a backlog using the github issues function to allocate tasks that needed to be done each week. This will allow us to keep track and prioritise tasks during development.

2. * User Stories: We made user stories to descripe features of the product. Furthermore we made a user story map to prioritise them. This will allow us to create object oriented artifacts that will assist in development.

3. * Sprint Planning/Retrospective: We planned out the work that had to be done according to the backlog and after the sprint we would get feedback on our progress from our tutor/customer and them we would reflect on the feedback. 

# Scope/Assumptions
1. RM Questionaire will be conducted at hiring to populate system, existing RMs will be required to complete questionaire
    * Assumes most employees will disclose their age, sex and culture - however some fields should be optional and provide a netural value
    * For fields like "product knowlege," preliminary score will be provided based on matrix of employee's self-reported confidence/prior experience, and confidence of hiring managers
2. Outbound calls are made based on stored information such as sex, age, packages interested, interested location, collected by:
    * Previous calls 
    * Their website that uses sign-ups, server-logs and cookies 
3. Customers agree to be recorded for training purposes 
4. Interactive voice response unit has good voice recognition and can have users list words that respond with their call
5. Age Region From, Region Interested are stored as large categories, eg. 
    * Age <18, 28>, <28-38> <38-48>, <58 , 100>
    * Region from <Asia, Africa, Europe, Latin America/Caribbean, Northern America, Oceania>
6. Passport holdings data will be stored as individual categories 
8. System has a capacity of withstanding a maximum of 500 calls at a peak time
9. Customers will be given a standard wait time of 15 minutes, and provided their place in queue. 
11. Employees have knowledge of all travel packages available, along with a database they can quickly search during a call. 
Employees will be trained prior to new packages being available.
12. RM are able to see caller demographics/data on their screen automatically as they recieve call
13. RMs will be able to manually redirect calls to other hotlines, or other RMs if they dont feel they can adequatley service a customer
14. Customers profiles are made with the use of a profiler tool.
15. Customer profile includes information such as:
    * Age
    * Sex
    * Culture
    * Language Proficiency
    * Address
    * Sale Success Rating
    * Phone Number
16. RM profile include information such as:
    * Age
    * Sex
    * Culture
    * Language Proficiency
    * Product Knowledge
    * Experience, Skill Score Rating
    * Phone Number
    * Employee ID
17. Customer sale success rating is based on:
    * If the customer is a repeat customer
    * If the customer is from a particular post code
    * The amount of travel packages purchased by the customer
    * The amount of time a customer spends on average talkining to a relationship manager
    * The voice quality of the customer
18. RM skill score rating is based on:
    * Previous call duration
    * Similarities between relationship managers profile and customers profile. 
19. Call Centres will be located in various countries across the world, and system can see which regionsare online Staff will work between business hours 9:00 - 17:00. 
20. Customer's inbound calls go through quick questionnaire with robot before being redirected to appropriate RM
21. CMC system will be used in conjunction with existing systems, such as forms that RM already use to sell Travel Packages
22. CMC system has another system in place to allow recording of all incoming calls
23. RM's profile is automatically updated with every customer they deal with
24. There will be a payment function for customer over the phone that will be processed by the RM through the system.

# Stakeholders
![table-idsm](https://user-images.githubusercontent.com/59853181/83491086-86dfa280-a4f4-11ea-8d84-ad26ae69b043.PNG)

# Empathy Maps
## Customer 
![empathy map](https://user-images.githubusercontent.com/62222787/80952888-c788c500-8e3d-11ea-81c6-745241f2036f.png)

## Developer 
![Developer Empathy Map](https://github.com/edelinic/ISDM-tut-1-/blob/master/DeveloperEmpathyMap.png)

## Relationship Manager 
![Relationship-Manager-Empathy-Map](https://user-images.githubusercontent.com/59853181/81492332-102afd00-92da-11ea-8330-59202f72a95b.jpg)
## Product Owner
![Empathy Map](https://user-images.githubusercontent.com/62222787/83399403-7d96fd00-a444-11ea-9017-77ebfa71e7fc.JPG)

# Pov Statements
1. * A customer needs to have a meaningful conversation with the relationship manager because they are investing a large amount of money and time with their purchase.

2. * A customer needs to be able to communicate effectively to the relationship manager because it will reduce the loss of information between them, furthermore it reduces tension and stress.

3. * A customer needs to be able to securely pay for the service because they are investing a large amount of money and trust into the product.

4. * A customer needs to understand how to use the interactive response unit because they might hang up if they are confused.

5. * A relationship manager needs to have the right knowledge that a customer needs because they want to ensure the customer gets quality service and to reduce their call times allowing for more calls.

6. * A relationship manager needs to be able to communicate effectively to the customer because it will reduce the loss of information between them, furthermore it reduces tension and stress.

7. * A relationship manager needs to be able to securely process payment for the service because they want to ensure the customer gets the service and they do not want to be liable for any possible malfunctions.

8. * A relationship manager needs to be able to understand how the system works with ease because it will allow them to work efficiently and reduces the amount of stress from learning.

# HMW Statements
1. * How might we speed up call times between customers and relationship managers?

2. * How might we facilitate meaningful conversations between customer and relationship managers?

3. * How might we inform a customer about the product whilst in a call?

4. * How might we prepare the relationship manager before their call?

5. * How might we ensure both customer and relationship managers can communicate with each other effectively?

6. * How might we ensure that payments are secure for both customer and relationship managers?

7. * How might we ensure that customers are not confused during calls or when they are connected to the interactive response unit?

# User Story Map
![user-story-map-png](https://user-images.githubusercontent.com/59853181/82756723-3777e300-9e1f-11ea-88b5-1db816d76e1c.PNG)

# Case Diagram
![image](https://user-images.githubusercontent.com/62222787/82164760-82609a80-98f5-11ea-8a3b-b9ab987afbca.png)

# Class Diagram 
![Travel Company](https://user-images.githubusercontent.com/59853181/82755441-cd5b4000-9e16-11ea-93e2-26bed286b881.jpg)

# Activity Diagram

## Payment Over Phone
![image](https://user-images.githubusercontent.com/59853181/83352293-c50e8200-a38d-11ea-894e-c3f869e16ea0.png)

## Create RM Profile
![Create RM Profile AD](https://user-images.githubusercontent.com/62222776/82164363-9c00e280-98f3-11ea-91c6-b8b9bb1f2ca8.png)

## Inbound Call
![Inbound Call AD](https://user-images.githubusercontent.com/62222787/83398141-209a4780-a442-11ea-8869-894f5439b2c3.JPG)

## Voice Response Unit
![Voice Response Unit AD](https://user-images.githubusercontent.com/62222787/83398340-84247500-a442-11ea-862a-230bc93e65ea.JPG)

## Outbound Call
![Outbound call AD](https://user-images.githubusercontent.com/62222787/83398444-b635d700-a442-11ea-9a37-ad9fae54d7fa.JPG)

## Customer Calling Agency
![Customer Calling Agency](https://github.com/edelinic/ISDM-tut-1-/blob/master/Customer%20Calling%20Agency%20Activity%20diagram.png)


# Collaborative Diagrams
## Create RM Profile
![Untitled Diagram](https://user-images.githubusercontent.com/62222776/83156745-1fb59d00-a146-11ea-9241-3b86db1ced23.png)
## Customer Calling CMC
![Untitled Diagram](https://github.com/edelinic/ISDM-tut-1-/blob/master//Customer_calling_Collaborative.png)
## Payment Over Phone
![make-payment-collaborative](https://user-images.githubusercontent.com/59853181/83406224-8a6e1d80-a451-11ea-9097-2522cb97dada.PNG)
## Voice Response Unit
![Voice Response Unit CD](https://user-images.githubusercontent.com/62222787/83410558-ed63b280-a459-11ea-8616-7a3a35d93efe.JPG)
## Inbound Call
![Inbound Call CD](https://user-images.githubusercontent.com/62222787/83410648-15ebac80-a45a-11ea-9350-ad4512232586.JPG)
## Outbound Call
![Outbound Call CD](https://user-images.githubusercontent.com/62222787/83410683-2bf96d00-a45a-11ea-9e2d-35c7e7480194.JPG)

# Outcomes
## Competitive Advantages
This new system will create a competitive advantage over other travel companies. Through automation, inbound customer calls will automatically be redirected to an appropriate RM, considering their previous customer history with the travel agency, as well as the customer’s desired travel location. 

Each call is logged, and ratings calculated to rate the success of a call. This is beneficial as it will allow customers to get in contact with the appropriate RM as quick as possible to reduce the amount of people the customer will have to go through to get to their RM. This system also comes with an Interactive Voice Response unit to handle calls when the CMC gets overloaded with calls during peak times, as to not lose custoemr calls.

For outbound calls, the system automatically dials customers while simultaneously generating a script for the RM to guide them for a more successful call. This provides a competitive edge over other companies as it not only provides information on each customer, but also specifically tailors a script for each individual customer, allowing for a more personalised approach. 

With the rating of each call and sale afterwards and the above new feature, it will allow RMs to improve their techniques in making effective calls. Each RM is given a 10-minute survey to complete to analyse their area of expertise to help target specific customers.

## If the Project Fails
If the project is considered as a failure, there is a number of consequences. This includes losing trust from respective stakeholders, losing funding which leads to bankruptcy, and sustaining a bad reputation out in the workforce. Such consequences can negatively affect it's respective employees with a bad employee record or simply being pointed out working in a terrible company with a negative perspective from future employers. 

In addition, losing trust in stakeholders provides an excuse for employers to question the former employees whether or not their performance may affect the employer's company in a negative way. If the project loses its funding from various stakeholders, the project becomes unsustainable and is unable to continue with it's basic functions of the project. 

Another leading consequence from declaring bankruptcy is allowing the project's major and minor competitors to surpass the failed project in terms of net worth, high reputation, and reliability. Here on, more customers and stakeholders will follow the more successful and reliant projects of respective competitors. Overall, the employes/investors from the failed project would have lost a lot of money and time from the failed project.

[Presentation Youtube Link](https://youtu.be/mBAdbKHoRPE)
