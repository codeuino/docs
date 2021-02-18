# GSoC 2021 Idea Page

**Welcome to our Google Summer of Code 2021 ideas page. As a student, you are welcome to pick any of the ideas listed below and start early in the community bonding process as well as learning a bit about our code if we get selected as a mentoring organization. And of course, we'd love you to stay around even if we are not invited to GSoC or if we cannot invite you as a student.**

Students can connect with the Org Admins, Mentors, and other community members through various communication channels given below:

* **Email:** **Jaskirat Singh** and **Siddharth Simharaju** **\(Org Admins\)**  


  Students and Mentors can join the slack discussion portal in order to carry discussions about their projects and interaction within the community.  

* **Slack Workplace** - [**http://slack.codeuino.org/**](http://slack.codeuino.org/)\*\*\*\*

All tasks on this page already indicate mentors for the task. New tasks on this page should be added only by those with the experience and time to invest in mentoring new developers.

**Make sure to Check out** [**Google Summer of Code 2021**](https://docs.codeuino.org/documentation/activities/google-summer-of-code-2021) **to know more about community participation in GSoC 2021.**

## **Table of Contents**

* [**IDEA 1: Refactoring and Improving Donut Platform Interaction**](https://docs.codeuino.org/documentation/activities/google-summer-of-code-2021/gsoc-2020-idea-page#idea-1-refactoring-and-improving-donut-platform-interaction)\*\*\*\*
* \*\*\*\*[**IDEA 2: Cross-Platform Hybrid Mobile Application for Donut**](https://docs.codeuino.org/documentation/activities/google-summer-of-code-2021/gsoc-2020-idea-page#idea-2-cross-platform-hybrid-mobile-application-for-donut)\*\*\*\*
* \*\*\*\*[**IDEA 3: Development of Event Management System inside Donut**](https://docs.codeuino.org/documentation/activities/google-summer-of-code-2021/gsoc-2020-idea-page#idea-3-development-of-event-management-system-inside-donut)\*\*\*\*
* \*\*\*\*[**IDEA 4: Visualizer Representation of User Activity through Heatmap**](https://docs.codeuino.org/documentation/activities/google-summer-of-code-2021/gsoc-2020-idea-page#idea-4-visualizer-representation-of-user-activity-through-heatmap)\*\*\*\*
* \*\*\*\*[**IDEA 5: Implementing Microservice architecture in Donut** ](https://docs.codeuino.org/documentation/activities/google-summer-of-code-2021/gsoc-2020-idea-page#idea-5-implementing-microservice-architecture-in-donut)

\*\*\*\*

## **IDEA 1: Refactoring and Improving Donut Platform Interaction**

### **Priority:**

High

### Description:

Donut is an open-source, feature-rich, highly flexible and privacy-friendly, social networking platform built for community-oriented collaboration in a customized way. It has been transitioning from development to a production phase, with a vision to have better scalability but it is required to evaluate through various testing, documentation, and elimination of all major level bugs which will allow an essential impetus to provide custom and friendly rich widgets and an expansive library of modules to make communication and collaboration easy and successful. So, it is required to refactor the whole existing codebase in order to build the powerful module system along with adding some minor features.

Few major directed points that need to be accomplished are:

* Maintaining design consistency across the whole application
* **Bug triaging** and **resolving** all pending bugs on backend and frontend repositories
* Restructuring code-base with introducing React Hooks and API's
* Writing unit test cases
* Making platform responsive
* Feature Addition: Implementation of the dark theme across the whole platform
* Deployment of Application:
  * Deployment of Docker Image to Docker Hub and AWS ECS/ other cloud providers
  * Setting up of clusters, server instances
  * Creating network load balancers
  * Adding SSL certification and handling cors.
* Monitoring Performance:

  *  Improving front-end performance by following the LightHouse measures like optimizing build    , minifying JS bundle size, lazy-loading, semantic elements etc.
  * Use of Performance Hooks API for Node.JS
  * Setting up Cloudwatch or similar tools on the cloud provider



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



### Expected Outcome

* A functional Android Mobile Application for Donut.
* Consistency across the web and mobile applications. 
* Bug fixes completion

### Potential Mentors





## **IDEA 3: Development of Event Management System inside Donut**

### **Priority:**

High

### Description:

The development of an online event configuration mechanism is one of our newest additions to our feature frameworks of the Donut platform. So, the task of this major project is to develop an Event  Management System with an integration of the Jitsi Meet platform that will allow individuals or community admins to set up themselves to host online events To simplify the configuration, the event management system will be divided into three different phases which are organizer space, speaker space, and audience space with various modules which will have the most common use cases while setting up this environment. 

Below is the development required within each space : 

**Organizer Space:**  
It will be a space where the organizer or admins will have control over the whole event management mechanism including the speakers, and audience.

* Admins can add members to the community spaces through Invites, also can invite others as an Admin/moderator due to which all the same rights will be shared with the other person.
* Blocking users \( Giving access to block people\).
* Add/Remove any independent modules like chat mechanism\(which will be used for live chat\).
* Showcase the backstage mechanism.
* Registrations - Designing the customized event's landing page which can be used to promote away and to sell tickets, manage registrations, and monitor signups from their own event dashboard.
* Giving Access to delete any post/comments, etc.
* Giving them access to change modules in between any time through toggle or any other available options such as Theme change, Removing/Adding any other modules.
* Making a feature of "Maintenance". with this no user should be able to login/signup . they should see a particular page of maintenance. These rights should be given to only admins.
* Allowing to give them access to the "settings" of the event mechanism for a community. 

**Speaker Space:**  
It will be a space which will be used by the speakers for giving the sessions. 

* They should have the mechanism to share their presentations.
* Access to the chats and comments by the audience and organizers in a separate way.
* Access to the Backstage settings - speakers line up, etc. 

**Audience Space:**  
It will be the general way to view the live or recorded events for the user.

* It should have the access to do networking with the people through chats or comments
* They will also have the access to see the event information, speakers line up 

**Note:** We have already some of the designs made for this project which can be found on [Figma](https://www.figma.com/file/iZvb7rLYRp3Di3wILVQ7V9/CodeUino-Donut?node-id=3194%3A6085). 

#### 

#### Steps to get started:

* Gain a good understanding of React Native, React
* Setup Donut and explore its different features, find bugs, and open issues.
* Get involved in the community and contribute to our code, fix bugs, or propose new features.
* Having a basic knowledge of platform-specific features and their implementations. 
* Writing tests using Jest \( for React \).



### Required Skills / Knowledge

* Excellent knowledge of JavaScript, NodeJs and React.
* Experience with unit testing. Experience with Jest or other testing frameworks.

**Technologies Involved:** React Native, React, NodeJs, JavaScript



### Expected Outcome

* This project will result in having an appropriate event management mechanism inside the donut platform which can be used by the communities to create engaging virtual events that can connect people around the globe.
* It will also have different management spaces for the organizers, speaker, and audience
* It will have an integration of the Jitsi platform

### Potential Mentors





## **IDEA 4: Visualizer Representation of User Activity through Heatmap**

### **Priority:**

High

### Description:

 A heat map is a graphical representation of data where values are depicted by color. Heat maps make it easy to visualize complex data and understand it at a glance and taking this into consideration this project states to implement the GitHub-like heatmap inside the donut platform which will give better insights to the respective users about their involvement inside the donut platform.

This heatmap will show up the user's following contribution through building blocks : 

* The number of posts, the user has interacted with.
* The number of Likes and comments 
* The number of projects uploaded
* The number of events organized/attended
* Some other functionalities

It should also include the separate contribution activity section which will consist of a detailed timeline of the user involvement inside the donut platform, including comments made, post co-authored, new ideas proposed inside proposal functionality. It is made publically where other people on the platform can see any user's contributions over time by clicking on a specific date calendar.

#### Steps to get started:

* Gain a good understanding of React Native, React.
* Setup Donut and explore its different features, find bugs, and open issues.
* Get involved in the community and contribute to our code, fix bugs, or propose new features.
* Understand the working of Github heatmap
* Understand the importance and implementation of the heatmap
* Having a basic knowledge of platform-specific features and their implementations. 



### Required Skills / Knowledge

* Excellent knowledge of JavaScript, NodeJs and React.
* Experience with unit testing. Experience with Jest or other testing frameworks.
* Understanding of heatmap integration and development

**Technologies Involved:** React Native, React, NodeJs, JavaScript



### Expected Outcome

* This instance will help to give the activity overview section on anyone’s profile, also giving access to external viewers to see more information about the types of contributions/involvements the specific user has interacted with within the donut platform.
* This feature will also allow viewers to filter the contribution graph and activity timeline for any user. 

### Potential Mentors



## **IDEA 5: Implementing Microservice architecture in Donut**

### **Priority:**

High

### Description:

Donut is an open source social networking platform. Currently backend of Donut is a monolith made in NodeJs. Since donut is a social networking platform it should be able to handle a large number of requests simultaneously and scale up or down depending upon the traffic. For an application like Donut, not all services experience the same traffic so we would like to be able to scale up or down individual services loosely linked through API interfaces. Hence, we plan to shift the backend to microservice architecture. This task would require a significant portion of the backend to be re-written in Typescript. Also since there are obvious performance limitations in JavaScript we would be rewriting some crucial frequently used services in GoLang. Ultimately we would expect Ansible packages to be created to automate to a fair extent the deployment of Donut with the new architecture on various cloud platforms. Also since the backend of Donut would significantly change by this task, detailed in depth documentation and a developer's guide should be written.

#### Steps to get started:

*  Gain good understanding of containers, container orchestration tools, micro service architecture and other related technologies.
* Setup Donut  and explore its different features, find bugs and open issues.
* Get involved in the community and contribute to our code, fix bugs or propose new features.
* Implementation of a small version of Donut with microservice architecture with few core services and creation of Ansible packages to automate it's deployment.
* Understanding the various components of Donut and coming up with an architecture for microservices.



### Required Skills / Knowledge

* Good knowledge of TypeScript and NodeJs.
* Experience with goLang.
* Some experience developing applications with microservice architecture.
* Fair amount of experience with containerization and container orchestration technologies like Docker and Kubernetes.
* Experience working with large codebases.
* Desire to learn about various open source best practices and adhere to them.
* Ability and passion for learning new concepts and technologies quickly and apply them on real world projects.

**Technologies Involved:** JavaScript, TypeScript, Microservice architecture, GoLang, Docker, Kubernetes, Helm, Prometheus, Ansible, Cloud services \(AWS, GCP, Azure\)



### Expected Outcome

* Completely functional bug free Donut with high availability and scalability made up of loosely coupled self contained microservices written in languages like GoLang and Typescript.
* Easily deployable Donut on major cloud platforms and for local development. It should be able to scale up or down automatically depending upon various metrics and perform optimally while requiring least amount of user intervention. Most of the tasks automated using Ansible and scripts. 

### Potential Mentors

