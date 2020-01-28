# \(InProgress\)Proposal Functionality

**Summary:**  
This feature of Donut platform will enable individual developers to reach out to Open Source Organizations. Doing so will help developers and organizations in many different ways, lets see how developers can get benefit from this:

*  Consider an individual developer who is passionate about his/her project which he/she thinks is good enough and wants to showcase this project under any reputed organization.
* Consider a scenario where developer wants to reach out to a bigger crowd of developers seeking help in development or enhancement of the project.
* Or say someone has some crazy idea which he wants to propose under any Open Source Organization seeking help from them then this functionality will help the developer in such scenario.

## **Detailed Info:**

### User Facing Tasks:

* [ ] Build a Proposal page in Donut platform.
* [ ] Proposal page should have a markdown editor.
* [ ] Build draft functionality.
* [ ] Upon Submission of proposal show proposal tracker.
* [ ] The proposal tracker page should have comment functionality.

**Task 1: Build a proposal page in Donut platform:**  
This will be a page inside Donut platform which user will be able to access using the navigation panel. This page has to be built using Reactjs. You can refer to the designs\[1\] to build the page.

**Task 2: Embedding a markdown editor:**  
On this page the developer will be able to draft his proposal which will be submitted to Open Source Organizations. To start with this you can either embed an editor or build an editor which is totally dependent on you. The editor should support markdown syntax. The developer should be able to upload photos, attach documents/presentation related to the proposal.

**Task 3: Build draft and resume functionality for editor:**  
While the user is drafting the proposal the proposal should keep getting saved on regular intervals so that is the user closes the browser window or because of any other reasons the user leaves the page his progress keeps getting saved in Donut. User should also have option to save the proposal as draft and when the user returns to the page user can resume the proposal.

**Task 4: Build a proposal tracker:**  
This feature will help the user track the progress of the proposal and as which stage is the proposal currently on. This will only be visible to the user once the proposal has been submitted. We will have 4 stages of the proposal:  
Stage 1: Proposal Submitted  
Stage 2: Under Review  
Stage 3: More information required -&gt; This will be an optional stage and will be seen of the organization requests for more information from the user regarding the project. If the organization accepts the proposal then the tacker will jump to stage 4.  
Stage 4: Proposal accepted.

![Sample Image for proposal tracker](../../../../.gitbook/assets/assets_-lsv46f7uzuvdedvews0_-ltflz2mqkow25nhe1al_-ltfm3no_hb7me2lxeku_artboard-1.jpg)

**Task 5: Providing comment functionality on proposal page:**  
This functionality will be enabled only when the organization asks for more info regarding the proposal. To understand this more clearly think of a situation where in user has submitted a proposal for some FOSS organization. The organization after going through the proposal wants bit more info or wants to have more clarity on the idea then the tracked will show Stage: More information required. On this stage we need to have a comment functionality which will behave more like a thread where organization and user can interact and get thing more clear.

### Organization facing tasks:

* [ ] Send an email to admins of organization once a proposal has been submitted.
* [ ] Build feature where organization can access the proposal.
* [ ] Schedule a meeting with the user.

**Task 1: Send email to admins as soon as a proposal is submitted:**  
Admins of the organization should receive an email stating that a new proposal has been submitted and they go and have a check on the proposal. So you are supposed to build the email feature which will send email to the admins of the organizations. You also need to code the email template which will have dynamic data as per user.

**Task 2: Build functionality for admin dashboard to see the submitted proposals:**  
As the user submits the proposal the the admins of the organization should be able to see the submitted proposal. When admin clicks on one proposal it should open a new page in which the proposal will be displayed.  On this new page the admin should also be able to select if they want to proceed with the proposal or not.   
If Admin marks as more info required which is Stage 3 of the proposal tracker, in that case the admin should be able to add comments from the new page where the proposal opens up for review. Also, any comments added by the user should also be visible to admins on that page.  
If admins feels the idea or project is good and wants to proceed with it then they can change the state of the proposal to accepted state. As soon as the proposal gets accepted the user should a congratulation email says the propsal has been accepted.

**Task 3: Intergrate Jitsi for video calls:**  
To provide more flexibility in terms of interaction between admins and user. Admins can setup a meeting with the user. To provide this video call functionality you need to intergate Jitsi\[2\] with Donut platform.

