# Final-Project
Final Project OOPS - Ecommerce Application
**How to run the application**
Step-1 You need to unzip the project & load it in any IDE (eclipse / IntelliJ). I have created this using eclipse.
Step-2 Now, update the project using Maven build tool.
Step-3 Now, Run the Application (Right click Project name > Run as > Java Application)

**A Tomcat server will be started on which project will be hosted**

This project is created using springboot & h2-database to save all application related data.
 In order to login to database , Go to > **http://localhost:8080/h2-console**
 All parameters will be pre-filled in the database sheet, press connect to connect to the database.
 Database related all properties are mentione din application.properties file in the project.
After connecting to database, run these scripts to manually add user roles while running application first time :

1. insert into roles(id,name) values
(1,'ROLE_ADMIN'),
(2,'ROLE,USER')

After this query, you can create new users in the application.

 Once you are connected, you'll be able to see all Tables which are created for this ecommerce application.

 You can find the home page : **http://localhost:8080**

 This is the main Homepage of the application.

 I have implemented Authentication functionality for login-logout using Cutom Authentication & Google OAuth2Authentication.
 Google OAuth2 related properties are mentione din application.properties file.

 I have added my own auth credentials on line 15,16 in application.properties file, you can use these or create your own also following this tutorial : https://support.google.com/cloud/answer/6158849?hl=en

 After setting up google OAuth authentication, 

 You can login to application using **Sign-in with google** button 

 You can use the following URLs to add categories, products in the database :

 http://localhost:8080/admin/categories/ - To add categories in the database
 http://localhost:8080/admin/products/ - To view all products from the database
 http://localhost:8080/admin/categories/add - To add specific category
 http://localhost:8080/admin/product/1 - will show the product with id =1.
