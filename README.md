# Read Me First
A task of Arkademy (Beginner Backend - Week 4), to create databases and CRUD features of 'Users', 'Tickets' or 'Movies', and 'Transactions'.
#### For the requirements of this task, Arkademy asked me to include a few things in this project :  
1.) Databases (all)  
2.) CRUD features (all)  
3.) Search (tickets)  
4.) Sort from the newest data (tickets & transactions)  
5.) Paginations  
6.) Push to GitHub repository (all)  
7.) Linter (Standard)  
8.) API's flowcharts (all)  
9.) Error handling (all)  
10.) A Postman's API Documentation (CRUD)  
11.) CORS  
12.) Env  
#### Then, what's included in this README.md?    
1.) Algorithms (user only)  
2.) Flowcharts (user only)  
3.) This project's overview/screenshots (all)  
4.) Postman's API Documentation (CRUD) => https://documenter.getpostman.com/view/14851668/Tz5jg1fd  

## 1.) Algorithms with Flowcharts (user only)
#### 1.1) CREATE
1.) Start.   
2.) First, take inputs from the user (real name, username, email, password).  
3.) After that, make some variables of user's input (realName, userName, userEmail, userPassword) with values from the body request of them (req.body).  
4.) Now, create a variable named "hashedUserPassword", that contains a value from variable "userPassword" then hashes it (in this case, I was using bCrypt to help me for the hashing process when an input came from the user).  
5.) Then, create a variable again named "newData" that'll be sent as a parameter to database query process, contains an object value with keys and values based by the user's first variables input in number 2 (realName, userName, userEmail, userPassword).  
6.) After that, create a function named "newUserData" with a paramater value passed from "newData", in this function we'll query the user's database and order it to insert the data into user's database.  
7.) Now, we make a statement for the result, if there's no error then give the result, else console an error message.  
8.) At last, execute the function newUserData(newData) and in no time the result will shown based on the statement in number 7 as JSON format.   
9.) End.  
#### 1.2) READ
1.) Start.  
2.) First, take GET or the READ request from the user (with no data input, ofc).  
3.) After that, we just need to query user's database with a line syntax that selecting all data from the database then returns all of them in JSON format.  
4.) Lastly, the result will shown to you, as easy as that!  
5.) End.  
#### 1.3) UPDATE
1.) Start.   
2.) First, take inputs from the user (targeted user's id to be updated, real name, username, email, password).  
3.) After that, make some variables of user's input (realName, userName, userEmail, userPassword) with values from the body request of them (req.body).  
4.) Now, create a variable named "hashedUserPassword", that contains a value from variable "userPassword" then hashes it (in this case, I was using bCrypt to help me for the hashing process when an input came from the user).  
5.) Then, create a variable again named "updatedData" that'll be sent as a parameter to database query process, contains an object value with keys and values based by the user's first variables input in number 2 (realName, userName, userEmail, userPassword).  
6.) After that, create a function named "updatedUserData" with a paramater value passed from "updatedData", in this function we'll query the user's database and order it to update the data into user's database based on the user's id.  
7.) Now, we make a statement for the result, if there's no error then give the result, else console an error message.  
8.) At last, execute the function updatedUserData(updatedData) and in no time the result will shown based on the statement in number 7 as JSON format.    
9.) End.  
#### 1.4) DELETE
1.) Start.  
2.) First, take input from the user (targeted id to be deleted).  
3.) After that, we just need to query user's database to delete the targeted data based on inputted user's id.  
4.) Lastly, the targeted data will be deleted, very simple right?    
5.) End.  

## 2.) Project's Overview / Screenshots (all)
#### 2.1) USERS  
![Create - Users](https://user-images.githubusercontent.com/77045083/110342396-ef4c4900-805d-11eb-8bd4-891b760e18ba.png)
![Read - Users](https://user-images.githubusercontent.com/77045083/110342402-f1160c80-805d-11eb-8f48-44a8e63e211e.png)
![Update - Users](https://user-images.githubusercontent.com/77045083/110342405-f2473980-805d-11eb-9475-15d51e33dae5.png)
![Delete - Users](https://user-images.githubusercontent.com/77045083/110342414-f410fd00-805d-11eb-99ee-2669354e6b5b.png)
#### 2.2) TICKETS  
![Create - Tickets](https://user-images.githubusercontent.com/77045083/110342935-8addb980-805e-11eb-8307-37bce724df91.png)
![Read - Tickets](https://user-images.githubusercontent.com/77045083/110342945-8d401380-805e-11eb-9536-55f4065fcfd3.png)
![Update - Tickets](https://user-images.githubusercontent.com/77045083/110343286-ee67e700-805e-11eb-81bb-f524a425188b.png)
![Delete - Tickets](https://user-images.githubusercontent.com/77045083/110342963-916c3100-805e-11eb-8764-8ecfbe8baeee.png)
#### 2.3) TRANSACTIONS  
![Create - Transactions](https://user-images.githubusercontent.com/77045083/110342996-9cbf5c80-805e-11eb-987c-76701e1b84b1.png)
![Read - Transactions](https://user-images.githubusercontent.com/77045083/110343006-9f21b680-805e-11eb-8ec2-6a989a8ccc9d.png)
![Update - Transactions](https://user-images.githubusercontent.com/77045083/110343015-a052e380-805e-11eb-8458-186ad3239d0b.png)
![Delete - Transactions](https://user-images.githubusercontent.com/77045083/110343023-a2b53d80-805e-11eb-9edd-fa2ebd86b252.png)