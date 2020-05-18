# Project Objectives
A major travel company has tasked us with developing an information system that improves the operation of their in-house call management centre. 
This system will automatically assign end customers to well informed relationship managers with appropriate knowledge of the destination and its traditions. 
This process is done based on the match between a customer's profile and a relationship managers profile and skill. 
A customers profile will be automatically made using a profiler tool and a relationship managers profile is made through a 10 minute questionnaire upon them being hired. 
A relationship managers profile may include age, sex, culture, language proficiency, experience and product knowledge. 
During outbound calls the system automatically calls a customer according to a customer target list. 
This list consists of tuples of information in the form of <potential customer, Product proposed> and it is provided to a specific relationship manager. 
The system retrieves the customer details from the database and provides the relationship manager guidelines and a script to help provide improved service to the end customer. 
For Inbound calls a customer contacts the CMC which has its own private branch exchange to route calls. 
A customer will get a score from 1-10 based on the likelihood to purchase the product (e.g. repeat customers may have a higher score, customers from particular postcodes may have lower scores, etc..). 
A customer with higher scores is served first. 
Similarly a skill score is allocated to a relationship manager based on their previous call duration and profile. 
Customer is redirected to a relationship manager according to skills and best match. 
During busy times a customer is directed to an interactive voice response unit promoting them for options. 
It may ask a few questions before redirecting the customer to the automatic call distributor routing the call to the first available appropriate relationship manager.

# Scope/Assumptions
1. RM Questionaire will be conducted at hiring to populate system, existing RMs will be required to complete questionaire
    * Most employees are comfortable with disclosing information about their age, sex and culture - however some fields should be optional and provide a netural value
    * For fields like "product knowlege," preliminary score will be provided based on matrix of employee's self-reported confidence/prior experience, and confidence of hiring managers
2. Outbound calls are made on preliminary information stored in database, which will include information of sex, age, packages interested, interested location, collected by:
    * Previous calls 
    * Their website that uses sign-ups, server-logs and cookies 
3. Customers agree to be recorded for training purposes 
4. Interactive voice response unit has good voice recognition and can have users list words that respond with their call
5. Age Region From, Region Interested are stored as large categories, eg. 
    * Age <18, 28>, <28-38> <38-48>, <58 , 100>
    * Region from <Asia, Africa, Europe, Latin America and the Caribbean, Northern America, Oceania>
6. Passport holdings data will be stored as individual categories 
8. System has a capacity of withstanding a maximum of 500 calls at a peak time, and less subsiquently based on Relationship Managers available at given time. 
9. Customers will be given a standard wait time of 15 minutes, and provided their place in queue. 
    * Existing statistics for average call time will be used in this function at first, but will become more accurate as RM use system
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
16. Relationship managers profile include information such as:
    * Age
    * Sex
    * Culture
    * Language Proficiency
    * Address, Product Knowledge
    * Experience, Skill Score Rating
    * Phone Number
    * Employee ID
    * Profile Image
17. Customer sale success rating is based on:
    * If the customer is a repeat customer
    * If the customer is from a particular post code
    * The amount of travel packages purchased by the customer
    * The amount of time a customer spends on average talkining to a relationship manager
    * The voice quality of the customer

18. Relationship managers skill score rating is based on:
    * Previous call duration
    * Similarities between relationship managers profile and customers profile. 
    
19. Call Centres will be located in various countries across the world, therefore re-routing systems can see which regions/centres are online to most adequately redirect calls.
Staff assumed to be hired between business hours 9:00 - 17:00. 

20. Customer's inbound calls go through quick questionnaire with robot before being redirected to appropriate RM based on answers selected on keypad

21. CMC system will be used in conjunction with existing systems, such as forms that RM already use to sell Travel Packages

22. CMC system has another system in place to allow recording of all incoming calls

23. RM's profile is automatically updated with every customer they deal with
    
# Empathy Maps
## Customer 
![empathy map](https://user-images.githubusercontent.com/62222787/80952888-c788c500-8e3d-11ea-81c6-745241f2036f.png)

## Developer 
![empathy map](https://github.com/edelinic/ISDM-tut-1-/blob/Developer-Empathy-map/DeveloperEmpathyMap.png)

## Relationship Manager 
![Relationship-Manager-Empathy-Map](https://user-images.githubusercontent.com/59853181/81492332-102afd00-92da-11ea-8330-59202f72a95b.jpg)
## Product Owner
<img width="557" alt="Annotation 2020-05-11 104959" src="https://user-images.githubusercontent.com/62222776/81515212-474eec00-9376-11ea-8175-e529d7bc1237.png">


# User Story Map


# User Story 

<table>
  <tr>
  <td colspan="9">Customer</td>
 </tr>
 <tr>
  <td>As a ____ I would like ____ so that I can ________</td>
  <td>As a ____ I would like ____ so that I can ________</td>
  <td>As a ____ I would like ____ so that I can ________</td>
  <td>As a ____ I would like ____ so that I can ________</td>
  <td>As a ____ I would like ____ so that I can ________</td>
   </tr>
  <tr>
  <td colspan="9">Relationship Manager</td>
 </tr>
 <tr>
  <td>As a RM I would like an interactive voice response unit so that I can have more streamlined calls</td>
  <td>As a RM I would like to see caller demograpics on my screen so that I can taylor my approach for each customer </td>
  <td>As a RM I would like to see all available travel packages so that I can discuss with customer </td>
  <td>As a RM I would like a script so that I can provide improved service to customers</td>
  <td>As a RM I would like to be able to redirect calls so that I can direct customers to other RMs/Departments </td>
   </tr>
     <tr>
  <td colspan="9">Call Management Centre (CMC) </td>
 </tr>
 <tr>
  <td>As the CMC I would like to keep track of all calls made so that I can refer back to the log in case of a complaint from a customer</td>
  <td>As the CMC I would like keep track of all sales and potential sales so that I can keep a running log of how much money is being made and also for any complaints made by customers and insurance</td>
  <td>As the CMC I would like to keep a list of RMs so that I can allocate them to customers suited to them best</td>
  <td>As the CMC I would like to keep track of holiday locations so that I can best match customers to their desired location</td>
  <td>As the CMC I would like to keep a log of customers so that I can help serve them better next time they call</td>
   </tr>
     <tr>
  <td colspan="9">Product Owner/Major Travel Company/Client </td>
 </tr>
 <tr>
  <td>As a Product Owner, I would like to have a customer database so that I can analyse the statistics of the calls </td>
  <td>As a Product Owner, I would like to have a call maintenance session every fortnight so that I can prevent problems from occurring </td>
  <td>As a Product Owner, I would like a list of calls that occurred on the day so that I can track any suspicious activity</td>
  <td>As a Product Owner, I would like to have an employee database so that I can identify their personal information as contacts</td>
  <td>As a Product Owner, I would like to hold weekly seminars so that I can summarise the activities that occurred</td>
   </tr>
</table>

# Stakeholders

| Stakeholders        | Explanation  |
| ------------- |:-------------:|
| Product Owner/Major Travel Company      | They are a stakeholder as they are the person who owns and funds the product. |
| Customers  | The system is targeted at smoothing the communication between Relationship Managers and Customers and therefore the needs and requirements of the customers are particularly important to consider. They are the ones using the product. |
| Managers (Inc. Relationship Managers) | Managers, particularly the Relationship Manager, will be using the system regularly. |
| Local Community | They are a stakeholder as they will be directly affected by the product. Whether they are or anren't customers, they will be affected by the product, especially through the streamlined travel the company will provide. |
| Developers | They develop the system and play a major role in deciding what is feasible within the timeframe. They ultimately control how the end product looks and feels. |
| Call Management Centre (CMC) | They are a section within the major travel company. This is where all RMs work, making the management centre a particularly important stakeholder with the new software. |

Customer User Stories
1. As a Customer, I want to be connected to the relationship manager so that I can inquire information about a travel package.
2. As a Customer, I want to be connected to the relationship manager in a timely manner so that I do not have to wait too long.

# Case Diagram
![image](https://user-images.githubusercontent.com/62222787/82164760-82609a80-98f5-11ea-8a3b-b9ab987afbca.png)

# Activity Diagram
![Create RM Profile AD](https://user-images.githubusercontent.com/62222776/82164363-9c00e280-98f3-11ea-91c6-b8b9bb1f2ca8.png)

# Approaches/Justification
In our approach to this information systems development project we have decided to use design thinking. Design thinking is an approach that involves considering what technological assets available and what business strategies are reasonable can be converted into customer value. The design thinking approach consist of 5 stages:
Empathise: In this stage we consider every stakeholder involved with the information system development project and try to regard every possible problem and wants they may have. In this case we identified all the stakeholders but did not utelise the interview method and made reasonable assumptions on the requirement document given to us. Furthermore we made empathy maps to get a deeper insight towards the specific stakeholder.

Define: In this stage we define the problems that have been identified through empathising with each stakeholder. We created user stories based on the assumptions and empathy maps. These user stories were then put into a user story map allowing us to prioritise the most important problems. 
 
Ideate: In this stage ideas are generated to solve the problems at hand and the best idea is used as the solution. We will use the point of view of our team to question how might we solve the issues we have gathered. We provide as many answers as possible and vote as a team on which solution is the best.

Prototype: In this stage an early version of the product is made to test the voted solution, get feedback on the prototyped solution, reduce assumptions and answer questions. In this phase we will propose work products and  models based on the solution that we had voted for.

Test: This is an iterative process where tests are done on the completed product. Results used in this phase are used to redefine problems and show the understanding of a user when they are using the product. In this phase we will test the product ourselves.

Case Diagrams
We have used case diagrams as one of our artifacts as it gives the simplist overview of the entities, relationships and cases.
Furthermore, it can be used as a communication tool to convey they development teams ideas to a person with less software development experience e.g. project owner.

Activity Diagrams
We have used activity diagrams as one of our artifacts as it gives an overview of the flow of data within a specific case diagram.
This will allow the development team to visualise what is the system needs.

# Development Methodology (Agile)
4. Explain the agile methodology, namely, Scrum you have used to carry out the procedure. In your explanation, ensure that you outline activities from Scrum that you use. 
Look at SES team charter
Make a backlog and user story diagram

8. Document in GitHub all your iteration and models as you progress
(update your work in github so its recorded)

# Competitive Advantages
7. Discuss the competitive advantages might be gained in developing the new information system. Identify and discuss the possible adverse effects for this Business if its information system project fails


6. Document your proposed work products and models. 


