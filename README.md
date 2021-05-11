# Project Name: News Portal


### Project Description
A Java/Spark application with a rest REST API for querying and retrieving scoped news and information. News, articles and posts are available to all users without navigating into any department, and others that are housed or classified within departments.

<img src="/news_portal.png">

### Setup Instructions

* To run the application, first install the java development kit from `https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html`
* Install gradle.
* Next clone the project using `$ git clone https://github.com/deepeters/douglas-fir` to your preferred folder.
* In the command prompt, navigate to cloned folder and use the following command to run the app `$ gradle run`
* Open the browser and enter the address `localhost:4567`

* * Install PostgreSQL. for help installing ==> https://www.youtube.com/watch?v=-LwI4HMR_Eg
  * Open up your terminal and type the following commands(only works if postgreSQL is installed)
  
          psql
          
          CREATE DATABASE newsportal;
          
          \c newsportal;
          
          CREATE TABLE departments ( id SERIAL PRIMARY KEY, name VARCHAR, description VARCHAR, size int );
          
          CREATE TABLE news ( id SERIAL PRIMARY KEY, news_type VARCHAR, department_id INT, user_id INT, title VARCHAR, description VARCHAR );
          
          CREATE TABLE staff ( id SERIAL PRIMARY KEY, name VARCHAR, staff_position VARCHAR, staff_role VARCHAR );
          
          CREATE TABLE users_departments ( id SERIAL PRIMARY KEY, user_id INT, department_id INT );
          
          CREATE DATABASE newsportal_test WITH TEMPLATE newsportal;


# Contact Information:
### Author: [DENNIS NJENGA](https://github.com/deepeters)

         Email: dennis@dennis.com
         Phone: +254712345678

### Technology Used
1. Java
2. HTML
3. CSS

### Frameworks Used
1. Gradle
2. Spark
3. Maven
4. Junit
5. Handlebars

### Libraries Used
1. Bootstrap
2. Material Design Bootstrap.

### LICENSE: [MIT LICENSE](https://raw.githubusercontent.com/deepeters/news-portal/master/LICENSE)