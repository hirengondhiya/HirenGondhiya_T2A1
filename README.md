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

Agile Project management is a way of project delivery in which project is delivered in iterations. At the end of each iteration agile team delivers a working product which can be tested and is improved over previous iteration by adding new features and/or, improving previously delivered features. Due to continuous delivery approach it helps the end client to understand how the end product will look like and the team gets continuous feedback from the customer which leads to realistic understanding of the requirements. In this way the issues and gaps in the requirements are picked up in early stages of the project before they become serious risks to completion of the project.

**Core Values**

As per [Work front - The Beginners’ Guide to Agile Project Management Methodology](https://www.workfront.com/blog/the-beginners-guide-to-agile-project-management-methodology) there are four core values that guides any agile team

1. Individuals and interactions over processes and tools

    The first core value focusses on all the involved stackholders which includes representatives not only from the customer but also whole of the team involved in delivery of the project. As per agile philosophy the humans involved in the project should interact directly in order to quickly solve the issues instead of focusing on formal processes and tools.

2. Working software over comprehensive documentation

    In line with first core value of informal interaction over formal processes, the second value focusses more on delivering a working application over building detailed formal documentation.
    
3. Customer collaboration over contract negotiation

    This principle stresses on involvement of customer to make the project delivery successful by meaningful collaboration between the project delivery team and the customer.

4. Responding to change over following a plan
    
    This priciple requires the project team to be flexible in responding to the changes instead following a fixed plan that may not be suitable for change in the environment.

There are many different frameworks which follows the core values of agile project management. Two the more popular ones are Scrum and Kanban.

References:
 - https://searchcio.techtarget.com/definition/Agile-project-management
 - https://www.atlassian.com/agile/project-management
 - https://www.workfront.com/blog/the-beginners-guide-to-agile-project-management-methodology
 - https://www.pmi.org/learning/library/agile-project-management-scrum-6269
 - https://www.dummies.com/careers/project-management/agile-project-management-for-dummies-cheat-sheet/

## Q4

Provide an overview and description of a standard source control process. WC 100-200

---

In a multi-person team environment where a number of developers and other contributors are collaborating together to implement an application, the Source Control process helps to maintain the integrity of application code and other resources.

The application that is used to implement the Source Control process is categorized as a Source Code Management (SCM) Application. There are two popular approaches to Source Control 
1. Centralized and,
2. Distributed. 

In a centralized system, such as Microsoft TFS, all resources are controlled centrally and hence the user of the system is required to be connected to the SCM software to maintain the integrity of the code. 

In a distributed SCM system, source control application resides at individual developer's machine and then changes are synced to a central code base as and when required.

In general, standard source control process works as follows,
1. Each Developer gets a copy of the source code from a central codebase to their local development environment.
2. They make changes to code in their local environment.
3. When any of a developer is ready, s/he syncs the changes back to the central codebase. If there are any conflicts due to other developer's work that was synced to the central codebase after the developer acquired its copy of the code, then the SCM system flags the conflicts. In this scenario, the developers need to collaborate together to merge the conflicting changes.

References
1. https://www.atlassian.com/git/tutorials/source-code-management
2. https://aws.amazon.com/devops/source-control/
3. https://www.linuxnix.com/what-is-source-code-management-or-version-control/
4. https://www.oshyn.com/blogs/2012/06/version-control-systems-distributed-vs-centralized

## Q5

Provide an overview and description of a standard software testing process. WC 100-200

---

Software Testing Process is required to verify that the system performs as per specifications in different kind of scenarios and it also handles unspecified scenarios without crashing.

There are many different approaches, types, levels, techniques of software testing, such as Black box testing, White box testing, Manual Testing, Automated, Unit testing, Integration testing, System testing, Regression Testing, Functional Testing, Non-functional testing, Performance Testing, Accessiblity testing etc.. Based on the budget, Goals of the testing, impact on the business, and the requirements a mix of different approaches and techniques are used for testing.

The most basic testing that is used in modern development is unit testing. Where automated test cases are created by the developer to make sure changes to the code implements new functionality correctly as well as does not adversely impact previously implemented functionality. However unit testing alone can not be used for Quality Assurance purposes, so other approches are also used in conjuction.

A General Software Testint process involves following steps,
1. Understanding testing requirements and setting quality goals.
2. Building a test strategy to meet all the requirements and goals.
3. Planning to implement the test strategy including test case creation.
4. Test execution which involves executing test cases and reporting errors. This step is performed many times until desired quality is achieved.
5. Release. In release stage the software application is released to the users along with report of all the known issues and bugs.

References:
1. https://www.tutorialspoint.com/software_testing/software_testing_quick_guide.htm
2. https://reqtest.com/testing-blog/the-a-to-z-guide-to-the-software-testing-process/
3. https://www.testbytes.net/blog/software-testing-process/
4. https://en.wikipedia.org/wiki/Software_testing
5. https://www.toolsqa.com/software-testing/test-process-in-software-testing/
6. https://www.softwaretestinghelp.com/what-is-actual-testing-process-in-practical-or-company-environment/



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
1. **Bubble Sort**: 
Bubble sort works by comparing each element of the list to the next element in the list until the list is sorted (no swap required). In this method, on each iteration, the lower value elements of the list bubble up on top of higher value elements and hence it gets the name bubble sort.

    Following pseudo code explains the steps that are required to sort an array of numbers with n number of elements using the Bubble sort algorithm.

    - For index i= 0 to n-1 repeat following steps,
        - Set value of Swap = false.
        - For index j = 0 up to n-2-i do the following,
          - If array[j] > array[j+1] 
            - swap the elements in order and, 
            - set the value of the swap to true.
        - if the value of the swap is still false end the loop.

    Efficiency of Bubble sort:
  
    - Best case: Best case scenario for sorting is when the list is already sorted in this case Bubble sort requires one full pass to detect that the array is sorted, that means efficiency in the best case is O(n)
    - Worst case: In worstcase scenario bubble sort needs to traverse through the list approximately n * n times, that means efficiency in worst case is O(n^2).

2. Merge Sort: 

    Merge Sort is divide and conquer form of algorithm. This algorithm recursively divides the list into halves until each list contains only one item and then recursively merges the divided lists into larger sorted lists until all of the divided lists are merged back into a single sorted list.

    Following pseudo code explains the steps that are required implement Merge sort to sort an array of numbers with n number of elements.

    Method: MergeSort(input: array)
      - Set length= length of the array
      - If length > 1
        - set middle= length/2
        - divide the array into left and right as
          - left = array[0..middle]
          - right = array[middle+1..length-1]
        - Call merge sort on left and right array to get new sorted left and right array
          - Call new_left = MergeSort(left)
          - Call new_right = mergeSort(right)
        - Merge the sorted left and right array into a sorted array and return it back to the calling method
      - else
        - return the array

    Performance: 
    The efficiency of the Merge sort is O(n Log n)

    Though the merge sort takes the same number of iterations in bestcase or worstcase scenarios, its efficiency value is realiazed when sorting large number of items.

If we compare efficiency of the above two sort algorithms it is evident that in case of lower number of the items in the list the performance of the algorithm would be equivalent however when working with large number of list items Merge sort out performs the bubble sort.

References:
1. https://www.geeksforgeeks.org/bubble-sort/
2. https://en.wikipedia.org/wiki/Bubble_sort
3. https://www.tutorialspoint.com/data_structures_algorithms/bubble_sort_algorithm.htm
4. https://www.hackerearth.com/practice/algorithms/sorting/bubble-sort/tutorial/
5. https://en.wikipedia.org/wiki/Merge_sort
6. 


## Q13

Identify and explain the workings of TWO search algorithms and discuss and compare their performance/efficiency (i.e. Big O). WC 300-500

---

1. Linear Search:

    Linear search is the simplest and the most intituitive form of search algorithm. Given a list of n items it works by comparing the search item one by one with each of the items in the list in a linear fashion, starting from the first item in the list. The algorithm stops when the item is first time encountered in the list or the end of the list is reached. 

    - **Efficiency:**
      
      Using Big O the efficiency of the Linear Search is expresed as O(n).

      Since the algorithm works by searching items one by one in linear fashion, in best case when the search item is found at the first position it requires only one look up operation and in the worst case if the search item is not found or if it's at the last position in the list it takes n look up operations. 

      This implies that in worst case scenario the time taken by algorithm increases as the number of items in the list increases.

2. Binary Search:

    The Binary Search algorithm is another divide and conquer search algorithm. For this algorithm to work it requires a sorted list of items. The algorithm works by looking up for the search item at middle position of the list. If the search item is not found then it recursively looks up for the item in left half of the list if the search item's value is less than the item at the middle position or otherwise it recursively searches for the item in right half of the list. The algorithm keeps dividing the list into halves as described above until the search item is found or when the list can not be divided any further.

     - Efficiency:

        The efficiency of the Binary search in worst case is O(log n). This means that the time taken by the algorithm exponentially reduces as the number of the items in the list increases.

When comparing between the Linear search and the Binary search algorithm, the Binary search performs better when searching in large lists of the items.

References:
1. https://www.geeksforgeeks.org/linear-search/
2. https://www.tutorialspoint.com/data_structures_algorithms/linear_search_algorithm.htm
3. https://www.studytonight.com/data-structures/linear-search-algorithm
4. https://en.wikipedia.org/wiki/Linear_search

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

  I have done research on Airbnb, which as per wikipedia is, "is an online marketplace for arranging or offering lodging, primarily homestays, or tourism experiences". Following answers each part of the question.

- a) What software is used by the app?
  
    As per information on [stackshare](https://stackshare.io/airbnb/airbnb) Airbnb uses a lot of different kind of software application but the most relevant applications to their website are
    - Javascript
    - React
    - React Native
    - Native Navigation
    - Sass
    - CSS
    - Ruby
    - Rails
    - nginx
    - MySQL
    - Amazon RDS
    - Amazon EC2
    - Amazon S3
    - GitHub
    - New Relic
    - Webpack
    - Vagrant
    - Jest

- b) What hardware is used by the app?

  As per [AWS case study of Airbnb](https://aws.amazon.com/solutions/case-studies/airbnb-case-study/), most of Airbnb's hardware is virtualized and hosted on [AWS](https://aws.amazon.com/). AWS works based on Infrastructure As A Service (IAAS) model. In this model the provider leases its physical computing resources for example servers as a virtual server which can be accessed and managed through internet service.
  
  Due to the huge number of simultaneous customers being served by Airbnb it uses about 200 servers which are nothing but two hundred instances of Amazon EC2. To optimally distribute the requests, coming from the large number of users, among the 200 servers it uses Elasti Load Balancing service provided by AWS. To store the data, generated from various requests, Airbnb uses Amazon RDS, which is a relational database service from AWS. To store various kinds of files for example, backups, pictures of properties and users, etc..., it uses Amazon Simple Storage service which is a kind of cloud file storage service.

  As per the [AWS case study of Airbnb](https://aws.amazon.com/solutions/case-studies/airbnb-case-study/), most of Airbnb's infrastructure is hosted on [AWS](https://aws.amazon.com/). Due to the huge number of simultaneous customers being served by Airbnb, it uses about 200 servers which are nothing but two hundred instances of Amazon EC2. To optimally distribute the requests, coming from a large number of users, among the 200 servers it uses Elasti Load Balancing service provided by AWS. To store the data, generated from various requests, Airbnb uses Amazon RDS, which is a relational database service from AWS. To store various kinds of files, for example, backups, pictures of properties and users, etc..., it uses Amazon Simple Storage service which is a kind of cloud file storage service.

  There are many other IAAS services offered by AWS that are used by Airbnb for data analytics, Monitoring, and Operations but above are the core services that are used to host the website.

- c) Describe the interaction of technologies within the app

  As explained earlier, Airbnb uses many technologies however different kind of functions performed by these technogies can be divided mainly into three categories
  
  1. Front End
    
      Airbnb uses React to implement front end of its website which can be accessed through any web browser.

      Airbnb also has its mobile version of the app for android and ios platform, which is built with React Native. React native is used to render UI on the screen of the mobile devices. It makes the app platform agnostic since React is ultimately a javascript. Sass is used within the for stying the app. Native navigation is used within React Native apps, to manage presentation of and transition between the screens.

      Webpack is used to compile React, Sass code into javascript and css respectively. It is also used to minify the compiled code which helps in faster loading of the site.

  2. Backend
    
      Airbnb uses Ruby on Rails to interact with the database and then respond to the data requests made by front end of the app. This way it implements separation of concerns between backend and front end for different platforms.

      Nginx (engine-ex) webserver is used by Airbnb to serve its front end React website  and the Ruby on Rails backend apis.

  3. Hosting
     Airbnb uses AWS for its computing needs instead of owning its own physical servers it uses the servers in AWS datacenters offered through AWS service. To run the Rails application and to serve the http requests through Nginx it uses AWS EC2 instances. The MySQL databases are hosted on Amazon RDS instances and the large number of files are stored on Amazon S3.

- d) Describe the way data is structured within the app

  Airbnb uses MySQL database hosted on Amazon RDS. MySQL is a relational database management system and hence the data in MySQL is structured in form of two dimentional tables similar to the way data is structured in an Excel spreadsheet. Each entity and the relationship between the entities tracked by the Airbnb is stored as table inside the database. Relational database management systems uses SQL (Structured Query Language) to manipulate the data within the tables.

  Hosting the the MySQL on Amazon RDS reduces a lot of database adminstration tasks such backup automation, database security setup, Database replication in multiple regions etc..

- e) Identify entities which must be tracked by the app

  Based on the features provided by Airbnb following entities must be tracked by the app.

  1. User

      To store user login information.

  2. User Profile
    
      To store user information such as Name, Gender, Contact details, etc...

  4. Property
    
      To store Property information such as Address, Features offered, House Rules
  5. Room
      
      To store details of amenities in each room.
  6. Bed
      
      To store different kind of bed details.
  7. Amenities
      
      To store details of common amenities each property offers.
  8.  Schedule
      
      To store details of period when property is available to lease and the rate for each period.
  9. Review
      
      To store review of the property.
  10. Booking
      
      To store booking information.

  11. Images (User and Property)
      
      To store details of the image which can belong to a property or a user.

- f) Identify the relationships and associations between the entities you have identified in part (e)

  1. User: 
      - A User has one User Profile.
  2. User Profile
      - A User Profile belongs to a User entity
      - A User Profile has many Properties
      - A User Profile has one Image (Profile image)
  3. Property
      - A Property belongs to a User Profile
      - A Property has many Rooms
      - A Property has many Amenities through AmenitiesProperty join table
      - A Property has many Schedules
      - A Property has many Reviews through Bookings
      - A Property has many Bookings
      - A Property has many Images
  4. Room
      - A Room belongs to a Property
      - A Room has many Beds through BedsRoom join table
  5. Bed
      - A Bed has many Rooms through BedsRoom join table
  6. BedsRoom
      - A BedsRoom belongs to a Room
      - A BedsRoom belongs to a Bed
  7. Amenities
      - An amenity has many Properties through AmenitiesProperty join table
  8. Schedule
      - A Property Schedule belongs to a Property
  9. Review
      - A Review belongs to a Property through Booking (that was made for the property)
  10. Booking
      - A booking belongs to a Property (the booked property)
      - A booking belongs to a User (who made the booking)
      - A booking has a review
  11. Image
      - Polymorphic relation with User Profile and Property
      

- g) Design a schema using an Entity Relationship Diagram (ERD) appropriate for the database of this website (assuming a relational database model).

![Airbnb ERD Diagram](images/air-bnb-erd.svg)