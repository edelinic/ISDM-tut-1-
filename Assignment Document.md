# Project Objectives (Johan)
A major travel company has tasked us with developing an information system that improves the operation of their in-house call management centre. 
This system will automatically assign end customers to well informed relationship managers with appropriate knowledge of the destination and its traditions. 
This process is done based on the match between a customer's profile and a relationship managers profile and skill. 
A customers profile will be automatically made using a profiler tool and a relationship managers profile is made through a 10 minute questionnaire upon them being hired. 
*** A customer's profile includes information such as … . 
*** A relationship managers profile may include age, sex, culture, language proficiency, experience and product knowledge. 
*** During outbound calls the system automatically calls a customer according to a customer target list. 
This list consists of tuples of information in the form of <potential customer, Product proposed> and it is provided to a specific relationship manager. 
The system retrieves the customer details from the database and provides the relationship manager guidelines and a script to help provide improved service to the end customer. 
For Inbound calls a customer contacts the CMC which has its own private branch exchange to route calls. 
*** A customer will get a score from 1-10 based on the likelihood to purchase the product (e.g. repeat customers may have a higher score, customers from particular postcodes may have lower scores, etc..). 
A customer with higher scores is served first. 
*** Similarly a skill score is allocated to a relationship manager based on their previous call duration and profile. 
Customer is redirected to a relationship manager according to skills and best match. 
During busy times a customer is directed to an interactive voice response unit promoting them for options. 
It may ask a few questions before redirecting the customer to the automatic call distributor routing the call to the first available appropriate relationship manager.

Scope (Erina Delinicolas) (Includes assumptions)
1. RM Questionaire will be conducted at hiring to populate system, existing RMs will be required to complete questionaire
  *Most employees are comfortable with disclosing information about their age, sex and culture - however some fields should be optional and provide a netural value
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
7. Call Centres will be located in various countries across the world, therefore re-routing systems can see which regions/centres are online to most adequately redirect calls.
Staff assumed to be hired between business hours 9:00 - 17:00. 
8. System has a capacity of withstanding a maximum of 500 calls at a peak time, and less subsiquently based on Relationship Managers available at given time. 
9. Customers will be given a standard wait time of 15 minutes, and provided their place in queue. 
  * Existing statistics for average call time will be used in this function at first, but will become more accurate as RM use system
10. CMC system will be used in conjunction with existing systems, such as forms that RM already use to sell Travel Packages
11. Employees have knowledge of all travel packages available, along with a database they can quickly search during a call. 
Employees will be trained prior to new packages being available.
12. RM are able to see caller demographics/data on their screen automatically as they recieve call
13. RMs will be able to manually redirect calls to other hotlines, or other RMs if they dont feel they can adequatley service a customer

# Stakeholders
End Customer - They are a stakeholder as they are one of the end users that will be using the product.
Relationship Manager - They are a stakeholder as they are one of the end users that will be using the product.
Local community where product will be in use - They are a stakeholder as they will be directly affected by the product. 
Product owner - They are a stakeholder as they are the person who owns and funds the product.


Approaches (Week 9-10) 
3. Describe your approach from a Design Thinking principles perspective. 

# Development Methodology (Agile) (Week 4)
4. Explain the agile methodology, namely, Scrum you have used to carry out the procedure. In your explanation, ensure that you outline activities from Scrum that you use. 
Look at SES team charter
Make a backlog and user story diagram

# Assumptions
5. List assumptions you have made in the systems analysis. 
(everyone has to do at least 5)

# Proposed Models
UI “screens”


8. Document in GitHub all your iteration and models as you progress
(update your work in github so its recorded)

# Competitive Advantages
7. Discuss the competitive advantages might be gained in developing the new information system. Identify and discuss the possible adverse effects for this Business if its information system project fails


6. Document your proposed work products and models. 


