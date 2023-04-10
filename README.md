## [23-SP-COMP-294-Project](https://github.com/FranklinCSPracticum/2023_W_Team5_Kaitlyn)
COMP294 was a class designed to push students through the process of group development. Issues and branches were handled on github. I've attached the details of the project. In this repository I've added all the code that I worked on with a bit of details on what they did. At one point the website worked but was disconnected from the database.

# Login page
Bog standard login page, with input fields for username and password with a login and register button. Axios is used to store validated user data while users browse the site. Users enter credentials, and those credentials are sent to the backend. The method validateLogin() takes the credentials, compares it to all users in the database, if a user with credentials matching the passed ones is found then a true is returned to the frontend. Register just links to the register page. Invalid login attempts notify user that they have invalid login credentials.

# FriendsList + removeFriend
On the frontend I built a friendsList that displays a list of friends sorted alphabetically. There is also a remove button which will remove a friend from the list. The friend entity has a friends string, this string contains all of the userIds of friends associated with a given user. The frontend user sends to the backend the userId of the logged in user. In the backend the function getFriendsList() pulls the friends string associated with the user, builds an array List from friends, replaces userId's with associated usernames, sorts alphabetically, and sends that back to the frontend to be displayed. The removeFriend() method is initiated when a user clicks the remove button. The button sends the userId associated with the index of the button, the friendList of the logged in user is pulled up, the friend userId to be removed is removed from the string, then the string is rebuilt and put back into the database.

## MovieDB Web Application
In this project the team will build a web application for rating movies and sharing their reviews with friends. Users will be able to create accounts, sign in, and view their collection of movies, along with their ratings and the ratings their friends have given. If they are interested in seeing the details of an individual movie, such as the summary and discussions among their friends, they will be able to select the movie and see those details. They will also be able to add movies to their library. 

## Technology Stack
* Database: MySQL
* Middleware: Java with Spring Boot and JPA, using Gradle as the build tool
* Frontend: HTML5, CSS3, and JavaScript using the React framework

## Team members
* Kaitlyn Stackhouse - Team Lead
* Kyle Boldman - Senior Developer
* Brysen Meyer - Junior Developer
* Brandon Rivera - Junior Developer
* Matt Miller - Junior Developer
* Bushra Clark - Junior Developer

Link to full repo: https://github.com/FranklinCSPracticum/2023_W_Team5_Kaitlyn
