# Pull Request manager API  within Codebadge

### **Priority:**

High

### **Description:**

#### **Summary**

In Codebadge, presently all the badge allotment computation are taking place on the basis of comment count. We want to create a smarter approach to give each user its token of appreciation. Moreover CRON jobs approach which is being followed at present is pretty slow and hence need to optimise it. Trello dashboard being an awesome tool to manage Issue and pull requests is something we would like to take into consideration as a platform to manage the tasks and issues. The task to be performed under this project are:-

* Creating a Webhook which fires when a pull request is made on the project. This webhook link shall be provided to the admin at the time of adding an organization to his/her dashboard.
* Admin dashboard interact with Trello to check the award points if already set on trello cards.
* These awarded points must be updated in users section in the database. Remember maintainer’s merge commit shall not be awarded any point to the maintainer.
* If the trello dashboard has no such points in the card default points shall be awarded to the user which shall be decided by badge and point allotment api\(which is a separate project\).
* All the point updated that are made shall reflect in db.
* Update badges on the basis of total points
* Moving trello dashboard as per pull request merge usingv machine learning classification.
* Pull request award points must be visible for user on the respective pull request.
* Extra award points for an open issue.

### **Required Skills/knowledge:**

* Good knowledge of databases
* languages such as NodeJs, python for machine learning
* experience of using github apis
* Good Knowledge of Modules Bundling
* Good Knowledge of making restful API services

### **Difficulty Level:** 

Moderate

### **Potential Mentors:**

[**Jaskirat Singh**](https://github.com/jaskirat2000) and [**Vaibhav D. Aren**](https://github.com/vaibhavdaren)

