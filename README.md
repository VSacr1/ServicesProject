## Index 
0. [Project Definition](#0-Project-Definition)
1. [Architecture](#1-Architecture)
2. [How To Run](#2-How-To-Run)

# 0. Project Definition
As a user you can register for an account online. Once you have registered you should recieve a confirmation email which will give you a hyperlink to activate your account; allowing you to log in to the dashboard via the login page. This was created using Docker-compose, npm and nginx. 

# 1. Architecture 

![Serverdiagram](/Serverdiagram.jpg)

From the diagram above we can see how each of the docker files communicate with each other. 

**Clients run on port 8080**

**Servers run on port 3000**

**MongoDB run on port 3000**

# 2. How To Run
 * Nodejs - frontend 
 * Vuejs - frontend
 * MongoDB - database
 * Nginx.conf - web server

 1. Make a new google cloud virtual machine and git clone this project. 
 
 2. Install Docker on to the virtual machine 
 
 3. Change the .env file IP address to the external ip of the virtual machine
 
 4. Enter the file with the cd command and run docker-compose -d up. This will build and compile all the docker files inside this folder. 
 
 5. Once that is all running head to http://localhost/authentication/login

*Localhost = the ip of the virtual machine*
