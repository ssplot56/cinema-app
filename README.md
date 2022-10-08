#  Cinema - app 

### Project description:
> This is web-application that represent service for 
> buying cinema tickets. The app implemented using n-tier
> architecture, built with the Hibernate framework and the 
> Spring framework, connected to MySQL database and complies
> with SOLID standard. 
> 
> Here you can register and then log in to the service, buy 
> a ticket by selecting the required session, or view already 
> purchased tickets.

### Features: 
> Two roles: user and administrator and 
> different CRUD operations that depend on the role:
- __Everyone__:
  - ability to register, login and logout;
- __Admin & user__:
  - display list of cinema-halls / movies / available movie-sessions;
- __As admin__:
  - create / update a cinema-hall / movie / movie-session;
  - delete movie-session;
  - display info about the user by his email;
- __As user__:
  - display info about the user`s orders / shopping cart;
  - adding tickets to shopping cart;
  - completing orders;

### Structure:
> The project consists of three layers:
* __Controller__ - provides for the processing of user requests
* __DAO__ - provides all database operations;
* __Service__ - provides all the business-logic;

> Relationships in the database:
> 
> ![](image/relationships.png)

### Application was built with:
* Java 11;
* Apache Maven 3.8.6;
* Apache Tomcat 9.0.65;
* Hibernate;
* Spring framework (web, security);
* HQL
* MySQL;

### How to launch project:
1. Clone this project.
2. Create new schema in MySQL.
3. In the resources folder open db.properties file 
and configure the connection with your data.

   `src/main/resources/db.properties`
4. Check pom.xml. Іf there are errors - fix them.
5. Configure your tomcat and run application.