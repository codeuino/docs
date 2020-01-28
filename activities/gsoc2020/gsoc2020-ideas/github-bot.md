# Displaying Github Activity Data in Donut Platform

* Bot Functionalities:
  * Issues\[open/close/comment/assign/unassign/assignedUsers\]
  * pr\[open/close/comment/review\]
  * Share Issue on Donut as a post
  * Reply to comments through Donut platform
* While enabling the bot 
  * Send a request to admin
    * Then select repos to enable the bot

TODO: build a simple bot to check the complexity.  


### Summary

Build a GitHub bot which users can install from GitHub marketplace\[1\] and configure the bot on selected repositories / all repositories based on users choice. After successful installation, the bot should send details of activities happening in the repositories on which bot is configured. Here repository activities refer to actions done by any user. 

### **Detailed Info:**

**TASK 1:** The main purpose of this bot is to show github activity inside Donut platform. This feature will help users stay updated with all types of activities happening in the repository on which the bot has been configured. ****Donut platform will have a dedicated page to show github activities which users can access after logging in where they will able to see every activity that happens on github repos.         

**Github activities to be sent to Donut platform:**

* Actions performed on issues:
  * Issue created
  * Issue closed
  * Comment on an issue
* Actions performed on pull requests:
  * Pull request opened
  * Pull request closed
  * Comment on a pull request

**TASK 2:** Build a dedicated page for github activity as shown in the design. Activity data received should be stored in database and then displayed on the page.

**TASK 3:**  Build sharing functionality, such that every activity which is displayed on the activity page, user should be able to share any activity as a post.

### **Expected Outcome:**

* The user should be able to install this bot on repositories they wish to.
* The bot should send activity data\(mentioned in Detailed info section\) to donut platform.
* Display the received data in proper format as show in the design.
* User should be able to share any activity as a post.

The bot will be sending activity data to donut platform where the activities will be displayed

**References:**

\[1\]: [https://github.com/marketplace](https://github.com/marketplace)                                                                  \[2\]:You can make use of [probot](https://probot.github.io/).

### Tech Stack:

* Nodejs
* Reactjs
* MongoDB

### **Required Skills/knowledge:**

* Good knowledge of databases
* Good knowledge of Back-end
* Languages such as NodeJs, JavaScript, React

### **Difficulty Level:**   Moderate

### **Potential Mentors:** 

* [**Jaskirat Singh**](https://github.com/jaskirat2000)  
* [**Devesh Verma**](https://github.com/devesh-verma)

