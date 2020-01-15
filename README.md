# T2A1 Workbook - by Hiren Gondhiya

```
ACME Corporation is looking for devs with an understanding of Rails. 
The following set of questions relate to this RfQ-requirement.
```

## Q1

**Describe the architecture of a typical Rails application. WC 200-300**

---

A typical Ruby on Rails application follows Model, View, Controller (MVC) architecture. MVC is one of many design patterns that provides a well-defined structure for the development of software applications.

 As the name suggests in a typical MVC application there are mainly three important components as described below,

- Model: 
  
  In the MVC application Model is responsible for the storage of data and the business logic of the application. A Rails model follows the Active Record design pattern, in which the model is responsible for not only the storage of the data but also interacting with database application for the persistence of the data.

- View:

  In MVC a View is responsible for the representation of information and interaction with the end-user. In rails, application Views are typically hybrid HTML files with some embedded Ruby code. It contains all of the presentation and client-side validation logic. 

- Controller:

  In an MVC application Controller is the glue that binds the Model with Views. Whenever a browser requests a particular URL it is the controller that is responsible for calling the Models to retrieve or store the data and then hand it over to the view for presentation.

The MVC design pattern has many advantages few of them are listed below,

- Maintainability: 

  As explained above an MVC application has different components to deal with different parts of the application logic. This results in the separation of concerns. Due to this a programmer can easily change or update different parts of the application without affecting others.

- Supports Test-Driven Development (TDD):

  Since Model and View are independent of each other the UI logic and Business Logic of an MVC application can be tested independently. This helps in creating independent unit tests which are the foundation of Test Driven Development.

- Parallel Development:

  In an MVC application since UI and Business logic is built separately, it supports parallel development of the application logic by specialist backend and frontend programmers independent of each other.



## Q2

Identify a database commonly used in web applications (including Rails) and discuss the pros and cons of this database. WC 150-250

---

There are plenty of database management systems used for different kind of web applictions. One of the popular open source option is PostgreSQL. 

PostgreSQL is open source database management system. It can be easily used to work with web applications including the ones built using Ruby on Rails.

Below are the advantages and disadvantages of PostgreSQL,

- Advantages
  - Opensource: As mentioned earlier PostgreSQL is an opensource database with community of dedicated developers who are not only continuously improving and adding new features but also provides detailed documentation on how to work PostgreSQL. This results in very well supported production grade database system with zero licensing costs.
  - High SQL Compliance: PostgreSQL achieves very high degree of SQL compliance. PostgreSQL implements 160 out of 179 full core SQL:2011 compliant features as well as it also implements a number of optional SQL features.
  - Customizable: PostgreSQL can be customized based on the needs of the application to support additional custom features.
  - Very High Data integrity: PostgreSQL implements multiversion concurrency control algorithm to maintain integrity of the stored data. This results in consistent data 
  - Highly Fault Tolerant: PostgreSQL implements write ahead loging feature. Due to this feature its fault tolerance is very high.
- Disadvantages
  - Memory Intensive: PostgreSQL creates a new process for each user connection, which results in a lot of memory requirement when there are thousands of simulataneous user connections made to the database system. Based on popularity and purpose of the web application it can have few hundred to several thousand users connecting to the database to retrieve the information. In this situation it may lead to very high memory usage.

  - Very few management clients: Though PostgreSQL has existed for years it is becoming more popular very recently. Due to the lack consistent interest in PostgreSQL by organizations very few management clients are available to manage PostgreSQL databases.
  - Learning Curve: Due to a large number features supported by PostgreSQL it requires some learning curve to understand and master installation and configuration of the system.


```
ACME Corporation is very big on project management, documentation and process. This will be a key metric in their decision to award the project. The following set of questions relate to this RfQ-requirement.
```

## Q3

Discuss the implementation of Agile project management methodology. WC 200-300	

---

## Q4

Provide an overview and description of a standard source control process. WC 100-200

---

## Q5

Provide an overview and description of a standard software testing process. WC 100-200

---

```
Having suffered several cyber attacks in the past and resultant remedial audits ACME Corporation takes compliance, security and privacy very seriously. The following set of questions relate to this RfQ-requirement.
```

## Q6

Discuss and analyse requirements related to information system security. WC 100-200

---

## Q7

Discuss common methods of protecting information and data. WC 100-200

---

## Q8

Research what your legal obligations are in relation to handling user data. WC 100-200

---

```
ACME Corporation has specifically requested the app to be based on a relational database. The next set of questions relate to this RfQ-requirement.
```

## Q9

Describe the structural aspects of the relational database model. Your description should include information about the structure in which data is stored and how relations are represented in that structure. WC 100-200

---

## Q10

Describe the integrity aspects of the relational database model. Your description should include information about the types of data integrity and how they can be enforced in a relational database. WC 100-200

---

## Q11

Describe the manipulative aspects of the relational database model. Your description should include information about the ways in which data is manipulated (added, removed, changed, and retrieved) in a relational database. WC 100-200

---

```
The efficiency of an app (i.e. site) and the algorithms used are of the utmost importance. The next set of questions relate to this RfQ-requirement.
```

## Q12

Identify and explain the workings of TWO sorting algorithms and discuss and compare their performance/efficiency (i.e. Big O). WC 300-500

---

## Q13

Identify and explain the workings of TWO search algorithms and discuss and compare their performance/efficiency (i.e. Big O). WC 300-500

---

```
Companies (including ACME Corporation) value previous project experience and case studies. The following set of questions relate to this RfQ-requirement.
```

## Q14

Conduct research into a marketplace website (app) and answer the following parts:  
  - What software is used by the app?
  - What hardware is used by the app?
  - Describe the interaction of technologies within the app
  - Describe the way data is structured within the app
  - Identify entities which must be tracked by the app
  - Identify the relationships and associations between the entities you have identified in part (e)
  - Design a schema using an Entity Relationship Diagram (ERD) appropriate for the database of this website (assuming a relational database model).

  WC 50-100 per part

  ---

  