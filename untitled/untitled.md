---
description: This contains all the proposed ideas for GSOC'19
---

# GSOC-2019-Ideas

**Welcome to our Google Summer Of Code 2019 ideas page. As a student, you are welcome to pick any of the ideas listed below and start early in the community bonding process as well as learning a bit about our code if we get selected as a mentoring organization. And of course, we'd love you to stay around even if we are not invited to GSoC or if we cannot invite you as a student.**

Students can connect with the Mentors through various communication channels given below:

* **SLACK Discussion platform:** [**Join to interact with community!**](http://slack.codeuino.org)\*\*\*\*
* **IRC channel:** [**\#codeuino on freenode**](http//irc.freenode.net/codeuino) 
* **Contact Email:** [gsoc@codeuino.org](mailto:gsoc@codeuino.org)

All tasks on this page already indicate mentors for the task. New tasks on this page should be added only by those with the experience and time to invest in mentoring new developers.

Check out [**Google Summer of Code 2019 with Codeuino**](https://docs.codeuino.org/documentation/untitled) to know more about community participation.

## **1. Development of modules with new UI/UX**

**Priority:** High

**Description:**

Developing configuration mechanism is one of our newest additions to our installation frameworks of [**DONUT Platform**](https://github.com/codeuino/Social-Platform-Donut). The task of this major project is to develop a minimum of 12 different Modules for the social environment \([**DONUT platform**](https://github.com/codeuino/Social-Platform-Donut)\) along with a good looking User Interface architecture. To simplify the configuration, these predefined modules will have the most common use cases with different options for modules and settings while setting up this environment. Few have been described below which would serve essential features but make sure you meet the minimum criteria \(12\) for these.

1.\) Defining the Security Settings

* External users can register \(show registration form on login\)
* Allow access for non-registered users to public content \(guest access\)

2.\) Setup independent Modules for following:

* Notification \( This widget will show upcoming notifications on the dashboard \)[**Issue to work**](https://github.com/codeuino/Social-Platform-Donut/issues/13)
* Tasks Manager \( This will help to form tasks/assigns tasks/track tasks \)
* building Forms that will help users to post their projects/events/articles/etc
* Formatting Tool \( It will Help in formatting the content which can be written to post something \)
* Most Active Projects/People/posts/articles \(Defining most active people and most viewed projects \)

3.\) Sample data Content

* This part will consists of developing Dashboards for organization and Users differently depending upon who signed up. [**Issue to work**](https://github.com/codeuino/Social-Platform-Donut/issues/27)
* Developing "Pages" just like we have in [**Facebook**](http:www.facebook.com) \( This is the main part of the project as it will help the users or community to develop pages for their "project"/"events"/internships or any other related things in order to showcase it in profound way\)

**These modules should be developed with appropriate User Interface\(i.e. front-end part\) as well as back-end code with better User Experience.** [**Know more about Donut here**](http://www.codeuino.org/projects.html)

**References:**

* [**What exactly modules mean-Guide by Digital Ocean**](https://www.digitalocean.com/community/tutorials/how-to-write-modules-in-python-3)
* [**Modules from Drupal**](https://www.drupal.org/project/project_module)
* [**Plugins from Elgg that can help to know more about modules**](https://elgg.org/plugins)
* [**Some modules example by Terasology**](https://forum.terasology.org/forum/modules.55/)

**Required Skills/Knowledge:**

* Good knowledge of Modules with packaging
* languages such as Python, Node Js, JavaScript, HTML, and CSS. 
* UI/UX experience is also required with unique approach.

**Difficulty:** High

**Expected Outcome:**

This project would result in formation of packaged modules with new User Interface that would help the users and various communities to get predefined things configured on initial installing or setting up.

**Potential Mentors:**

* [Jaskirat SIngh](https://github.com/jaskirat2000), IRC Nickname: jaskiratsingh, SLACK name: @jaskirat, email: juskirat2000@gmail.com
* [Devesh Verma](https://github.com/devshiva619), IRC Nickname: devesh\_verma, SLACK name: @devesh, email: deveshverma619@gmail.com
* [Vaibhav Aren](https://github.com/vaibhavdaren), IRC Nickname: vaibhavdaren, SLACK name: @vaibhavdaren, email: vaibhavdaren@gmail.com
* [Pratul kumar](https://github.com/Pratul1997), IRC Nickname: Pratul1997, SLACK name: @pratul1997, email: pratulkumar1997@gmail.com
* [Ifeanyi Ekperi](https://github.com/ifeanyiekperi), IRC Nickname: ifeanyi\_, SLACK name: @ifeanyiekperi, email: imattew3@gmail.com
* [Uphaar Dubey](https://github.com/capedcrusader23), IRC Nickname: uphaar dubey SLACK: @Ccrusader, email:uphaar23dubey@gmail.com

### **2. Categorization system using tags in DONUT PLatform along with module development to retrieve analytics and export it in CSV/PDF format**

**Priority:** High

**Description:**

The [**DONUT Platform**](https://github.com/codeuino/Social-Platform-Donut) contains the notification feature which helps users to accommodate things in easy way. So the task of this project is to develop a mechanism for **"tags"** [**Explanation of tags in posts by WordPress**](https://en.support.wordpress.com/posts/tags/)**.** These tags will provide a useful way to group related posts together and and to quickly tell readers what a post is about and where to redirect or highlight the particular post more. The mechanism should be developed in such a way that users can make their own tags or can also select from predefined tags\(this needs to be built\) which gets automatically saved at one place that can be called as tag cloud and while submitting any posts it should get redirected to the appropriate users/groups which contains the similar tags.The tag cloud needs to be built which can store all the tags. When someone viewing your blog/project/article/any other post, clicks on one of defined Tag links, a Tag archive page with all the posts belonging to that Tag, should be displayed should also get displayed.

**Lets Understand this with example**

Assume that **"X"** user signs up on the DONUT platform. Once the **"X"** user has defined all the details about himself, then he would be asked to select some tags from the tags cloud which describes him the best and here, **"X"** user chooses "Designer", "Nodejs" and "Html". this tells us from the description of the tags in the tags cloud that this **"X"** user is a "Designer" and knows languages like "Nodejs" and "Html".On pursuing further these tags get stored for him.

Now assume other user **"Y"**, suppose "Y" user is already logged into this platform. **"Y"** user writes a post as project/article/blog or any other thing related to feeds on it, before he publishes, he would be asked to choose some tags from the "Tags Cloud". Suppose the **"Y"** user choose "Nodejs" tag from it. **Here, we see that user "X" and "Y" has "Nodejs" common in them.** So on publishing the post by user **"Y"**, the particular project would be redirected to the **"X"**\(because they both contain common tags\), **According to the tags description user "X" would be able to review the thing.**

**"X" and "Y" can be users as well as communities.**

Few things to be considered while developing the tags module as:

* Minimum of 50 predefined tags are required with different colors.
* Users can also make custom tags
* Some required items can be inspired from [**here**](https://codex.wordpress.org/Posts_Tags_Screen)
* Should be well formatted in the table in the "tags cloud" with tag name and descriptions required.
* giving access to the users to delete custom made tags as well as edit custom made tags.

Another objective is to develop a module using APIs with which communities admins will be able to gather meaningful insights from the various conversation happening in various phases of the DONUT platform. But, sometimes, it becomes difficult for the admin to personally go through all the Activities that are happening within the channels of this platform like people posting various things, tagging and introducing new projects, etc. This is where an analytics tool could save the day for admins. This project aims at developing a module to retrieve and show meaningful information to admins which could help them remain updated with all the happenings within the community. This should result in the formation of a Summary sheet which can also be notified through emails to them.

Following are the basic feature which should be supported by the analytics module:

* Admin should be able to track all the members within the community
* Users privacy should be kept secure and safe and no one other than community admin should be able to access any conversation
* The data should be collected and organized in the proper way to extract meaningful information. It should also help admin to understand community members behavior and trigger automation workflows
* The analysis should show key trends, how many members are active and are responding which should help him make a future decision.
* The report should be updated in real-time. 
* Admin should be able to export the report generated in CSV/PDf format.  
* The proper user interface should be used to make the report attacking and readable.    

**Required Knowledge:**

* Good knowledge about data analytics and commonly used analytics tool
* Prior experience with Data analytics or data collection
* Technologies required: Python, HTML, CSS, Python Libraries like numpy, Matplotlib etc.
* Converting analytics report in PDF or CSV format
* Prior experience of NLP and semantic analysis will be an added advantage 

**References:**

* [**Reference 1 by tag modules by WordPress**](https://en.support.wordpress.com/posts/tags/)
* [**Reference 2**](https://codex.wordpress.org/Posts_Tags_Screen)
* [Slack analytics](https://slack.com/apps/category/At0G5YTKU2-analytics)
* [Exporting workspace data from Slack](https://get.slack.help/hc/en-us/articles/201658943-Export-your-workspace-data)
* [Chatbot Analytics](https://chatbotsmagazine.com/advanced-chatbot-analytics-and-sentiment-analysis-part-1-17a8e674d7e1?gi=1ad039e47b54)

**Required Skills/Knowledge:**

* Good knowledge of Modules with packaging
* languages such as Python, Node Js, JavaScript, HTML, and CSS.
* Good knowledge about data analytics and commonly used analytics tool
* Prior experience with Data analytics or data collection
* Technologies required: Python, HTML, CSS, Python Libraries like numpy, Matplotlib etc.
* Converting analytics report in PDF or CSV format
* Prior experience of NLP and semantic analysis will be an added advantage 

**Difficulty:** Moderate

**Expected Outcome:**

This tag module will help users to review group related posts together and to quickly tell readers what a post is about by supporting them in their projects if needed. Tags also make it easier for people to find content as well as describe your own tag in better way.

**Potential Mentors:**

* [Jaskirat SIngh](https://github.com/jaskirat2000), IRC Nickname: jaskiratsingh, SLACK name: @jaskirat, email: juskirat2000@gmail.com
* [Prateek Chanda](https://github.com/prateekiiest), IRC Nickname:prateekiiest, SLACK name: @prateekiiest, email:prateekkol21@gmail.com;
* [Devesh Verma](https://github.com/devshiva619), IRC Nickname: devesh\_verma, SLACK name: @devesh, email: deveshverma619@gmail.com
* [Vaibhav Aren](https://github.com/vaibhavdaren), IRC Nickname: vaibhavdaren, SLACK name: @vaibhavdaren, email: vaibhavdaren@gmail.com
* [Pratul kumar](https://github.com/Pratul1997), IRC Nickname: Pratul1997, SLACK name: @pratul1997, email: pratulkumar1997@gmail.com
* [Uphaar Dubey](https://github.com/capedcrusader23), IRC Nickname: uphaar dubey SLACK: @Ccrusader, email:uphaar23dubey@gmail.com
* [Pranjal Kumar](https://github.com/pranjalkumar), email:pranjalkumar8228@gmail.com, slack name:@pranjal

### **3. Improve the user experience of the Admin Dashboard with a module that automatically publishes scheduled social posts**

**Priority:** Medium

**Description:**

The [**DONUT Platform**](https://github.com/codeuino/Social-Platform-Donut) already contains dashboard for users only but with new mission and aim DONUT platform can be used by an individual user as well as by the community. This project defines the purpose to give more profound look to the Admins dashboards for the **"users"** and **"community"** differently. More and better user interface and user experience required that could fulfill the requirements for the users and community admins.

Since for the community, only a single user can register/sign up for their community, so the community admin\( person who register/signs up\)should have all the access. Few things/features described below.

* Admins can add members to the community.
* Blocking users \( Giving access to block people\)
* Analytical representation \(This will help community view stat for their posts which can be shown through popularity/most viewed,etc \)
* Contribution on various projects by making the APIs and integrating with the Github.
* Project/Articles/blogs and other feeds posted by community
* Comments made by people on any community post
* Profile with all details \(Giving access to delete any post\)
* Allowing to give them access for the "settings" of the community
* Activity logs \( This feature will describe about followings, comments, Upvote/Downvote, stare, pinned things\( posts/projects/events/etc\)

You are welcome to add more features that can improve the UI/UX and result in good outcome. [**Look here at this example to see some UIs for dashboard**](https://wrapbootstrap.com/themes/admin)

User Dashboard should includes the following things:

* User profile \(with appropriate settings feature\)
* Activities log \( This feature will describe about followings, comments, Upvote/Downvote, stare, pinned things\( posts/projects/events/etc\)
* Groups \( Create, invite and manage your own groups \)
* blocking other users

[**DONUT Platform**](https://github.com/codeuino/Social-Platform-Donut) is an open source social networking platform that gives you the privilege of having your own social platform and use it in a custom way. So the purpose of this project is to develop a module that would help users to draft their posts in advance which can be posted accordingly and automatically after it has been scheduled with appropriate timing.

**For instance**, if "X" user wants to publish his project/post on "Y date/day", then he will write their posts in advance in this tool and schedule it with appropriate timings/day/date. On particular "Y date/day" this post would automatically get published. This will help to save time and increase efficiency.

The other part of this project is to integrate other social handles like **"**[**Facebook**](http://www.facebook.com)**", "**[**Twitter**](http://www.twitter.com)**", "**[**LinkedIn**](https://www.linkedin.com)**", "**[**YouTube**](https://www.youtube.com)**"** with the DONUT platform so that post can be shared on other social handles too.

**Note:** This project requires additional minimum 10 features for both users as well as organisations apart from the above described ones. Creativity would be really appreciable and be taken into consideration.

Initial dashboard code can be seen [**here**](https://github.com/codeuino/frontened/blob/master/User-dashboard.html)

**References:**

* [**\#Reference 1 - Some good looking UI/UX of dashboard**](https://wrapbootstrap.com/themes/admin)
* [**\#Reference 2 - Guide explaining the structuring of the dashboard**](https://www.geckoboard.com/blog/building-great-dashboards-6-golden-rules-to-successful-dashboard-design/)
* [**\#Reference 3 - Open Source guide describing the components of a dashboard**](https://www.predictiveanalyticstoday.com/open-source-dashboard-software/)
* [**\#Reference 4 - Dashbuilder**](http://dashbuilder.org/)
* [**Reference 5 - Google analytical**](https://analytics.google.com/analytics/web/provision/?authuser=0#/provision)
* [**\#Reference 6 - Hootsuit which is paid and non-open source guides about it**](https://hootsuite.com/)

**Required Skills/Knowledge:**

* Good knowledge of databases
* languages such as NodeJs, Html CSS, Bootstraps, JavaScript, React;
* Knowledge of visual representation
* Good knowledge of databases
* languages such as NodeJs, Html CSS, Bootstraps, JavaScript, React;
* Knowledge of visual representation

**Difficulty:** Moderate

**Expected Outcome:**

This project would reward back with more user-friendly and better User experience dashboard along with a tool that will help users to save their post as a draft and share them anytime or automatically through Reminders.

**Potential Mentors:**

* [Aishwarya Srivastava](https://github.com/SriAish), IRC Nickname: SriAish, SLACK name: @SriAish, email: aishsrivastava1998@gmail.com
* [Vaibhav Aren](https://github.com/vaibhavdaren), IRC Nickname: vaibhavdaren, SLACK name: @vaibhavdaren, email: vaibhavdaren@gmail.com
* [Jaskirat SIngh](https://github.com/jaskirat2000), IRC Nickname: jaskiratsingh, SLACK name: @jaskirat, email: juskirat2000@gmail.com
* [Devesh Verma](https://github.com/devshiva619), IRC Nickname: devesh\_verma, SLACK name: @devesh, email: deveshverma619@gmail.com
* [Uphaar Dubey](https://github.com/capedcrusader23), IRC Nickname: uphaar dubey SLACK: @Ccrusader, email:uphaar23dubey@gmail.com

### **4. Integration of Task Management tool in DONUT platform**

**Priority:** Medium

**Description:**

The purpose of this project is to integrate task management tool for DONUT platform which will provide admins of the communities to organize the workflow using the concept of generating cards to showcase task. By making use of **Task Management tool** admins will be able to organise different types of tasks that has been achieved/to be achieved/in progress.

Also, Task Management tool will have progress monitoring charts, to explain this in a better way the progress tracking will help in monitoring the development cycle of the projects. Using the progress tracking feature contributors will be well aware of the deadlines to finish a particular task. Also this will help better management of the communities.

Following are the things that an integrated Task Management tool should have:

* Automating the work flow \( This will set up triggering events to save time on project management that can move tasks into the right columns accordingly.\)
* Representing the progress made with the help of visualization
* Project boards are made up of issues and notes that are categorized as cards in columns of your choosing. These can drag and drop or use keyboard shortcuts to reorder cards within a column, move cards from column to column, and change the order of columns.
* Creating notes within columns with appropriate **formatting tool** 
* Able to add task reminders, references to issues and pull requests from any repository on GitHub, or to add information related to the project board.
* Allowing selecting things with the help of **checklist** added
* Notifying assignee through email if any comment made or tagged.

**Note:** This project can be achieved by integration of task managment tools from [**Github**](https://help.github.com/articles/about-project-boards/)**,** [**Trello**](https://trello.com/) and other tools that can result in same outcome.

**Reference:**

* [**\#Reference 1 - Project Board Engineering**](https://projectboard.engineering.com/?r=hu7txl)
* [**\#Reference 2 - GitHub Project Board**](https://help.github.com/articles/about-project-boards/)
* [**\#Reference 3 - Trello**](https://trello.com/)

**Required Skills/Knowledge:**

* Good knowledge of Integration
* Knowledge of working in project boards of GitHub and Trello
* languages such as NodeJs, Html CSS, Bootstraps, JavaScript, React;
* Knowledge of visual representation

**Difficulty:** Moderate

**Expected Outcome:**

With integrated tool communities would be able to track progress and will able to generate task for members.

**Potential Mentors:**

* [Aishwarya Srivastava](https://github.com/SriAish), IRC Nickname: SriAish, SLACK name: @SriAish, email: aishsrivastava1998@gmail.com
* [Vaibhav Aren](https://github.com/vaibhavdaren), IRC Nickname: vaibhavdaren, SLACK name: @vaibhavdaren, email: vaibhavdaren@gmail.com
* [Devesh Verma](https://github.com/devshiva619), IRC Nickname: devesh\_verma, SLACK name: @devesh, email: deveshverma619@gmail.com
* [Uphaar Dubey](https://github.com/capedcrusader23), IRC Nickname: uphaar dubey SLACK: @Ccrusader, email:uphaar23dubey@gmail.com

### **5. Integration of Chat functionality in DONUT Platform**

**Priority:** Medium

**Description:**

Communication is an important part of the development cycle and for an efficient product, it's important that all the team members can communicate and coordinate accordingly. This is why we wish to provide a proper communication channel for developers where they can discuss about any new development in their project, can share their ideas with their team members or even plan a team meeting. This project aims at integrating various chat platforms like [**Slack**](https://slack.com/), [**Gitter**](https://gitter.im/), and [**IRC**](https://webchat.freenode.net/) with the **DONUT** platform. Since **DONUT** is an open source platform, community leaders and team leaders should be able to create a channel or add or remove members from the channel. This project would require integration through making APIs.

Following the basic feature which should be supported by the chat platform:

* Secure Integration with various chat platforms like Slack, Gitter, and IRC using their APIs
* User experience should be a top priority while developing the chat functionality so that even a new developer finds is very easy
* User privacy should be a top priority 
* Team leaders or organization Leaders should be able to create a different channel where they could add to remove members
* Notification feature in case of an emergency message with the group of which a particular user is a part of, either via text message or email.
* To perform meaningful analytics across various chat platforms and an efficient way to manage them
* Video communication platforms should also be integrated as an additional feature for effective team meetings. 
* The efficient way to handle the large traffic in case of video communication 

Some of the widely used chat platforms \(textual\) which need to be integrated are as follows :

* [**Slack**](https://slack.com/)
* [**Gitter**](https://gitter.im/)
* [**Flock**](https://flock.com)
* [**Telegram**](https://web.telegram.org/)
* [**Rocket Chat**](https://rocket.chat/)

**Note:** The above-mentioned communication platforms are just the examples and any new platforms can also be added and integrated

**Required Knowledge:**

* Good Knowledge about integration 
* Prior experience of working with any chat functionalities.
* Understanding the security concern and way to tackle them
* Prior working experience with WebRTC 
* Technologies required: HTML, CSS, JavaScript, Redux, NodeJS, WebRTC

**Difficulty:** Moderate

**References:**

* [**Integrating Slack using API**](https://api.slack.com/)
* [**Integrating Gitter using API**](https://sidecar.gitter.im/)
* [**Developing a video communication platform**](https://webrtc.ventures/2018/02/learn-how-to-build-a-video-conference-app-and-not-die-trying/)

**Expected Outcome:**

With the integration of proper communication channel, the communities should be able to communicate and coordinate any project.

**Potential Mentors:**

* [Pranjal Kumar](https://github.com/pranjalkumar), email:pranjalkumar8228@gmail.com, slack name:@pranjal 
* [Uphaar Dubey](https://github.com/capedcrusader23), IRC Nickname: uphaar dubey SLACK: @Ccrusader, email:uphaar23dubey@gmail.com

