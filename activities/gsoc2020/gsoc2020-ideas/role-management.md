# Development of Admin Management mechanism for DONUT

### **Priority:** 

High

### **Description:**

 [**Donut Platform**](https://github.com/codeuino/Social-Platform-Donut) is a flexible open source **Social Network Kit that aims** to give you the customized social network, social intranet or huge social enterprise application for communities that really fits their needs.

Development of configuration mechanism is one of our newest additions to our installation frameworks of Donut Platform. Currently Donut is central hosted but aims to get bundled as FOSS/OSS tool. So, the task of this major project is to develop an **Admin Management System** that will allow individuals or community admins to setup for themselves. To simplify the configuration, these predefined modules will have the most common use cases with different options for modules and settings while setting up this environment.Few have been described below which would serve essential features as a separate modules:

1. Development of module for Configuration screens :

* **Screen 1:** Registering Admin account with information such as Admin name, Email, Username, Password, etc. For example check [**here**](https://www.tecmint.com/wp-content/uploads/2018/05/Create-New-Discourse-Account.png)
* **Screen 2:** Include Admin Account Confirmation through email. An email send to the Admin account, On confirmation should redirect them to the page of "Activate Account" which further leads to other setup.
* **Screen 3:** Welcoming Screen, that should allow to setup Community account.  For hint check [**here**](https://support.patreon.com/hc/article_attachments/360027026912/Image_2019-04-24_at_9.25.35_AM.png)
* **Screen 4:** Setting up Community profile and permissions like Community Name, Description,Welcoming Invites, Access \( Is community open to everyone or limited to invites,etc. \), Automated Invites, System Email setup, etc.
* **Screen 5:** This screen includes **View** are from User end that how the Admins want their platform to look like. This will have custom things like Theme Selection, Community Top bar \( Including Logos\), home page look, some other modules. **\(Important Part !\)**
* **Screen 6:** Includes the Thumbnail or the preview of the main page based upon the settings configured by Admin.

2. Development of Admin panel :

This will include building of Admin panel or dashboard which will be visible to them after configuring the Donut Platform on their server.

* Admins can add members to the community through Invites, also can invite other as an Admin/moderator due which all the same rights will be shared with the other person.
* Blocking users \( Giving access to block people\)
* Analytical representation \(This will help community Admins view stat for their posts, members joined, etc\)
* Giving Access to delete any post/comments,etc
* Giving them access to change modules in between any time through toggle or any other available options such as Theme change, Removing/Adding any other modules,
* Making a feature of "**Maintenance**". with this no user should be able to login/signup . they should see a particular page of maintenance. these rights should be given to only admins.
* Allowing to give them access for the "settings" of the community
* Activity logs \( This feature will describe about followings, comments, Upvote/Downvote, stare, pinned things\( posts/projects/events/etc\) on their dashboard.

{% hint style="warning" %}
**References:** [**Youtube Guide of Discourse SetUp**](https://www.youtube.com/watch?v=sjFlBgSiyCY) **,** [**How to bundle a software \| Tom's Guide**](https://forums.tomsguide.com/threads/how-to-bundle-software-in-one-installer.310629/) **,** [**Admin panel Templates**](https://colorlib.com/wp/admin-panel-templates/)
{% endhint %}

### **Required Skills/knowledge:**

* Good knowledge of databases
* languages such as NodeJs, JavaScript, React;
* Knowledge of visual representation
* Good Knowledge of Modules Bundling
* UI/UX experience is also required with unique approach.

### **Difficulty Level:** 

Moderate

### **Expected Outcome:** 

This project would result in formation of packaged setup of a Donut platform along side with Admin panel with new User Interface that would allow the Admins/Moderators to use it in their custom way.

### **Potential Mentors:**

 [**Jaskirat Singh**](https://github.com/jaskirat2000) , [**Devesh Verma** ](https://github.com/devesh-verma) and [**Vaibhav D. Aren**](https://github.com/vaibhavdaren)

