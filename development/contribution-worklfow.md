# Contribution Worklfow

### Contribution Approach

We love pull requests from everyone! We follow the standard Git workflow of **`fork`** 👉 **`change`** 👉 **`pull request`** 👉 **`merge`** 👉 **`update fork`** 👉**`change`** ... \(**repeat forever**\). If you are new to open source, we recommend GitHub's excellent guide on "[How to Contribute to Open Source](https://opensource.guide/how-to-contribute/)". In addition, please feel free to reach out to any of the maintainers or other community members if you are struggling; we are here to help you learn!

Before getting started, please make sure you've read the **README** of the respective project repository to get a primer on our project.

### Opening an Issue

If you're experiencing an issue with any project or have a question you'd like help answering, please feel free to open an issue in the respective repository of the project. To help us prevent duplicates, we kindly ask that you briefly search for your problem or question in our issues before opening a new one.

Please note that if you open a bug report and your issue does not follow our template, we cannot help you until you have provided us all the relevant information in that format. Respectfully, we do not have the time to try and recreate an error given with minimal or no context, so by providing this information you are helping us help you! You will see this template when you open an issue; click on "Bug Report" and it will be populated with descriptions of what to put in each section. Replace the descriptions with your comments to the best of your ability, and please include screenshots and error logs if applicable.

### Contributing to Source Code

 Help is always welcome, be it any form, whether it is working on the documentation process or solving an issue. It is the best way to get along with the community. You can view all the issues on our GitHub Organization.  
  
**Important !!** You need to be logged in before you follow the issues link. They will give you a glimpse of what it’s like to work with us and what the workflow is like.

#### Cloning the GitHub repository

The git clone command is used to copy an existing Git repository from a server to the local machine. To clone our git repository follow these steps in your terminals\(This is just an example of website repo\):-

```text
git clone https://github.com/Codeuino/website-www.Codeuino.org.git
cd website-www.codeuino.org /
```

Now pick an issue that isn’t assigned and which you would like to fix. Leave a comment that you would like to work on that particular issue. This way we don’t have multiple people working on the same issue at the same time. After this, you can start working on it.

{% hint style="info" %}
**NOTE:** You should never work on an issue without being assigned. Also take up the issue, only when you know what the problem is and how to solve it.
{% endhint %}

#### Forking and Testing the Modifications

You should first fork the repository by visiting the official repository of Codeuino and clicking on the button Fork. This step is needed only once.

 **Important !!** It is important that you DO NOT make your changes on the master branch of your forked repository as you cannot have two pull requests using the same branch name. Therefore, if your fork’s master has been used in a pull request and you decide to work on a different issue you will have to branch eventually. Differently, every new commit that you make on your master branch will get attached to the initial pull request and that will result in altering the purpose of that request.

#### Branching

You can create a branch per set of changes. To do that run:

```text
$ git checkout -b branchname
```

where your branch name can be anything other than master. The scope is your forked repository. The branch name will be shown on the pull request. Before pushing the pull request, you must test your changes with some concrete examples.

#### Sending the Pull request

Now that your commit has been sent to your fork, it is time to create a Pull Request. You can do this by accessing your fork on GitHub and clicking the New Pull Request.

{% hint style="info" %}
**NOTE:** Comments are always welcomed, as the readability of the code becomes easy for the other developers.
{% endhint %}

**Creating a Pull Request:-** If you've forked a repository and made changes to the fork, you can ask that the upstream repository accept your changes by creating a pull request.

{% hint style="info" %}
**NOTE:** To open a pull request in a public repository, you must have write access to the head or the source branch or, for organization-owned repositories, you must be a member of the organization that owns the repository to open a pull request.
{% endhint %}

* Navigate to the original repository you created your fork from.
* To the right of the Branch menu, click **New pull request.**
* Type a title and description for your pull request.
* If you do not want to allow anyone with push access to the upstream repository to make changes to your PR, deselect **Allow edits from maintainers.**
* Click **Create pull request.**

{% hint style="warning" %}
**Source Citation:** This page has been inspired from the [**CHAOSS Contributing Workflow page**](https://chaoss-project.gitbook.io/community-handbook/development/contributing-worfkflow).
{% endhint %}

