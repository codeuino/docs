# GSoC 2021 Idea Page

**Welcome to our Google Summer of Code 2021 ideas page. As a student, you are welcome to pick any of the ideas listed below and start early in the community bonding process as well as learning a bit about our code if we get selected as a mentoring organization. And of course, we'd love you to stay around even if we are not invited to GSoC or if we cannot invite you as a student.**

Students can connect with the Org Admins, Mentors, and other community members through various communication channels given below:

* **Email:** **Jaskirat Singh** and **Siddharth Simharaju** **\(Org Admins\)**  


  Students and Mentors can join the slack discussion portal in order to carry discussions about their projects and interaction within the community.  

* **Slack Workplace** - [**http://slack.codeuino.org/**](http://slack.codeuino.org/)\*\*\*\*

All tasks on this page already indicate mentors for the task. New tasks on this page should be added only by those with the experience and time to invest in mentoring new developers.

**Make sure to Check out** [**Google Summer of Code 2021**](https://docs.codeuino.org/documentation/activities/google-summer-of-code-2021) **to know more about community participation in GSoC 2021.**

## **Table of Contents**

\*\*\*\*[**IDEA 1: Refactoring and Improving Donut Platform Interaction**](https://docs.codeuino.org/documentation/activities/google-summer-of-code-2021/gsoc-2020-idea-page#idea-1-refactoring-and-improving-donut-platform-interaction)\*\*\*\*

\*\*\*\*

## **IDEA 1: Refactoring and Improving Donut Platform Interaction**

### **Priority:**

High

### Description:

Donut is an open-source, feature-rich, highly flexible and privacy-friendly, social networking platform built for community-oriented collaboration in a customized way. It has been transitioning from development to a production phase, with a vision to have better scalability but it is required to evaluate through various testing, documentation, and elimination of all major level bugs which will allow an essential impetus to provide custom and friendly rich widgets and an expansive library of modules to make communication and collaboration easy and successful. So, it is required to refactor the whole existing codebase in order to build the powerful module system along with adding some minor features.

Few major directed points that need to be accomplished are:

* Maintaining design consistency across the whole application
* **Bug triaging** and **resolving** all pending bugs on backend and frontend repositories
* Writing unit test cases
* Feature Addition: Implementation of the dark theme across the whole platform
* Deployment of Application:
  * Optimize build using Browserify/Webpack
  * Deployment of Docker Image to Docker Hub and AWS ECS/ other cloud providers
  * Setting up of clusters, server instances
  * Creating network load balancers
  * Adding SSL certification and handling cors.
  * Restructuring code base
* Monitoring Performance:

  * 
    Profiling of React App 

  * Use of Performance Hooks API for Node.JS
  * Setting up Cloudwatch or similar tools on the cloud provider. 



{% hint style="warning" %}
**References:** 
{% endhint %}

#### Steps to get started:

* Setup Donut and explore its different features.
* Write developer and user guides.
* Refactor code to follow standard conventions and best practices.
* Propose a new feature and implement it.
* Get involved in the community, review code, share ideas, open issues, and more.

### Required Skills / Knowledge

* Excellent knowledge of JavaScript, NodeJs and React.
* Experience with unit testing. Experience with Jest or other testing frameworks. 
* Fair technical documentation skills.
* Some experience with cloud services like AWS, Azure, and GCP. Experience setting up servers \( Like Enginx, Apache \), cloud storage services are preferable.
* Experience with Containerization\(Docker & Kubernetes\). 

**Technologies Involved:** React, NodeJs, Jest, Docker, Cloud \(AWS, GCP, Azure\), Kubernetes



### Expected Outcome

After the completion of this project, Donut will be able to transit towards the production phase with a new release and it will be deployed to a cloud service with fair scalability, properly handle requests from the web application and the to be developed mobile application.

### Potential Mentors



## **IDEA 2: Cross-Platform Hybrid Mobile Application for Donut**

\*\*\*\*

### **Priority:**

High

### Description:

Donut Platform is a highly flexible open**-**source Social Network Kit that aims to give you the customized social network, social intranet, or huge social enterprise application for communities that really fits their needs. Its frontend is made in React.JS and the backend is written in Node.JS. 

Major tasks in this project are :

* Creation of cross-platform Application.
  * Setting up of sample application
  * Going through the UI/UX Designs on Figma and maintaining the design consistency across the application
* Development of designed screens for different personas.
  * Signup/ Login Screen for normal users and admins, used for authentication. Also maintaining the external Google and Github OAuth.
  * Feed Screen: Used to fetch latest posts on a timeline 
  * Side nav bar: Contains links to all screens
  * User Profile Screen: Screen to show a user’s profile on the platform
  * Edit Profile: To able to edit a user’s profile contents
  * Insights Screen: Showcasing all the insights of a user which is seen from the web
  * New Posts, Projects, and Events: Screens to create new posts, projects, and events that can be posted on Donut 
  * Implementation of the organizational screen which gives the org admins any  rights to control the platform
* Implementation of Push Notifications
  * Understanding how push notifications work
  * Implementing push notifications using Firebase FCM/ Web Sockets 
* Adding location-based services to Donut.
* Deployment of the application
  * Writing test cases 
  * Uploading the app on Google Play Developer

#### Steps to get started:

* Gain a good understanding of React Native, React, and mobile application development.
* Setup Donut and explore its different features, find bugs, and open issues.
* Get involved in the community and contribute to our code, fix bugs, or propose new features.
* Implementation of sample mobile applications implementing existing donut features.
* Proposing new mobile app-specific features for donut and implementing proof of concepts.
* Having a basic knowledge of platform-specific features and their implementations. 
* Writing tests using Jest \( for React \).



### Required Skills / Knowledge

* Good knowledge of React Native and React. 
* Some experience with native Android and iOS development.
* UI / UX experience.
* Cloud Services like GCP/AWS/Azure.

  \*\*\*\*

**Technologies Involved:** React Native, React, Android, iOS, NodeJs, JavaScript



### Expected Outcome

* A functional Android Mobile Application for donut.
* Consistency across the web and mobile applications. 
* Bug fixes completion

### Potential Mentors



### 





