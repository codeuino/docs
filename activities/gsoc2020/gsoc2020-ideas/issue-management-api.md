# Issues, Pull request and Comment Management API inside Codebadge

### **Priority:**

High

### **Description:**

**This project includes 3 parts as described below:**

**ISSUE MANAGEMENT API SYSTEM**

In Codebadge, presently all the badge allotment computation are taking place on the basis of comment count. We want to create a smarter approach to give each user its token of appreciation. Moreover CRON jobs approach which is being followed at present is pretty slow and hence need to optimist it. Trello dashboard being an awesome tool to manage Issue and pull requests is something we would like to take into consideration as a platform to manage the tasks and issues. The task to be performed under this project are:-

* Creating a Webhook which fires when a issue is made on the project. This webhook link shall be provided to the admin at the time of adding an organization to his/her dashboard.
* Admin dashboard interact with Trello to add a new card on related section by using classification algorithm of machine learning.
* Trello award points are set at issue card on trello which are awarded using badge and point allotment system.
* Issue award points must be visible on github issue section.
* Card must be moved or deleted respectively whenever needed on the basis of development. Awards must be updated in case of shift.
* Auto assigning issue on the basis of past issue solutions.
* Update database schema wherever required with an efficient schema design.
* Reward point updates in database for issue and updating badges on basis of points.

**COMMENT MANAGEMENT API SYSTEM**

* Creating a Webhook which fires when a comment is made on the issues/pull request. This webhook link shall be provided to the admin at the time of adding an organization to his/her dashboard.
* The comment must be analysed and decided how much the issue is relocatable to the issue topic using machine learning.
* Reaction of other users shall award extra points for positive comment and reduction in case of negative comment/ reaction.
* Admin and maintainer positive reactions and mentions must awarded with extra points. positive reactions must be reflected in the same way.
* Comments must suggest the maintainer some contributor in case of issue. The person who has the most relocatable comment must be suggested and shall be displayed on issue section.
* Inappropriate comments or language must be awarded a penalty.

**PULL REQUEST MANAGER API SYSTEM**

* Creating a Webhook which fires when a pull request is made on the project. This webhook link shall be provided to the admin at the time of adding an organization to his/her dashboard.
* Admin dashboard interact with Trello to check the award points if already set on trello cards.
* These awarded points must be updated in users section in the database. Remember maintainer’s merge commit shall not be awarded any point to the maintainer.
* If the trello dashboard has no such points in the card default points shall be awarded to the user which shall be decided by badge and point allotment api\(which is a separate project\).
* All the point updated that are made shall reflect in db.
* Update badges on the basis of total points
* Moving trello dashboard as per pull request merge usingv machine learning classification.
* Pull request award points must be visible for user on the respective pull request.
* Extra award points for an open issue.

{% hint style="warning" %}
**References:** [**Text similarity using Corpus**](https://www.site.uottawa.ca/~diana/publications/tkdd.pdf) **,** [**Trello Webhooks**](https://developers.trello.com/page/webhooks)
{% endhint %}

### **Required Skills/knowledge:**

* Good knowledge of databases
* languages such as NodeJs, python for machine learning
* experience of using GitHub apis
* Good Knowledge of Modules Bundling
* Good Knowledge of making Restful API services

### **Difficulty Level:** 

Moderate

### Expected Outcome:

This project would result in the improvement in the badge allotment system of Codebadge project by evaluating the quality of issue which will allow admin to judge the progress of the project in the better way.

### Potential Mentors:-

[**Jaskirat Singh**](https://github.com/jaskirat2000) and [**Vaibhav D. Aren**](https://github.com/vaibhavdaren)

