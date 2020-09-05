# Contributing to the donut frontend.

**Choosing an issue**

The first step when contributing to donut-frontend is to visit the project site and find an issue you would like to work on and which you think is suitable for your skillset. From the project homepage on GitHub, you can click the Issues tab to navigate to a list of the open issues.


![enter image description here](https://i.imgur.com/ncLCy84.jpg)

After choosing an issue from the issues tab, click on that particular issue to view more details about it. The issue details page provides the full information about the issue. Usually, the top comment will include details of the bug or the feature that is needed. Issues can be raised by anyone and as a result, the level of detail may not always be sufficient to understand the problem or requirement. The project owners and core contributors try to view new issues and triage them. This involves verifying the issue being reported is valid and where necessary, providing some further details or guidance. If it’s not clear what is needed from an issue, you can leave a comment to ask questions about it. If you have an idea for a solution, but want to run it past the project team before starting, work, you can leave a comment for that too. Issues are a good place for open discussions like this.


**Working on an issue**

When beginning work on an issue locally, the first thing you’ll need to do is to create a branch for that piece of work. There are many Git UI tools that allow you to create a branch, for this demo we’ll use the command line. To create and checkout a branch you can use a single command.

```
git checkout -b <branchname>
```

This command allows us to specify a name for our new branch and immediately check it out so we can work on it. It's common to name the branch with the issue number. For example if we are working on the issue #223, it would be a good idea to name the branch,


```
git checkout -b 223
```

Once we are on our new branch we can make changes to the code which addresses the issue. When we have made the required changes that address a particular issue, we need to commit that code to our branch. We can use the “git status” command to view the changes since our last commit.

```
git status
```

We then use the “git add” command to stage the changes for the next commit. It's possible to add the files one by one by specifying their relative path afterward. For example, if we want to add the corrections.js file in the same directory,

```
git add corrections.js
```

However, if you want to stage all the files that have been changed, it's also possible with the following command.
```
git add *
```
Next, we will commit our staged changes using the “git commit” command. In this case we can use the following example:
```
git commit -m "Fix readme typo"
```

The -m option allows us to specify a message for our commit. It’s good practice to try and provide a succinct, but descriptive message for your commits. This helps a reviewer understand at a high level what was addressed in each commit.

At this point, we have made and committed out changes local to our development machine. Our final step is to push the changes to our fork of the master repository up on GitHub. We can do that using the “git push” command. We need to specify the name of the remote that we want to push to and the name of the branch we want to push up. 
 ```
 git push origin 223
 ```
 
Now the changes we have made are pushed into our fork in GitHub. The final step is to make a pull request. A **pull request** (PR) is a method of submitting contributions to an open development project. It occurs when a developer asks for changes committed to an external repository to be considered for inclusion in a project's main repository after the peer review.

In order to make a pull request, visit the forked repository on GitHub. On the top right hand side a button will now be there mentioning that a pull request is ready to be made.

![enter image description here](https://i.imgur.com/bTN9On5.jpg)
Click on the "compare and pull request" button to make the pul request!
