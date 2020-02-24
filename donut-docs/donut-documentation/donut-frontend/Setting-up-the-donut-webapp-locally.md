# Setting up the donut frontend potion locally.

 **Forking The Repository**

The first step of setting the donut frontend locally is to fork the original repository. This creates a copy of that repository under your own account enabling you to begin working with the code. The rights to public repositories will be such that you can view the code, but not directly commit into the repository or create branches. This allows the project owners to control changes within their codebase. 

The forking step creates a copy to which you do have permission to commit and branch on and you can consider this your working copy of the project. You can make changes and commits here, safe in the knowledge that you will not affect the main repository.

In order to fork the  donut frontend repository visit [here](https://github.com/codeuino/social-platform-donut-frontend)

![](https://i.imgur.com/bWLML1u.png)

**Cloning the forked repository**

In order to clone the forked repository visit fork of the donut repository under "your repositories" section and click on the “Clone or download” which will open a UI showing the Git URL. A button to the right hand side of the URL allows you to copy it into your clipboard.

![](https://i.imgur.com/2UyN3KV.png)
There are various graphical tools you can use to work with Git repositories but for simple procedures, the command line is often fastest.

Open a command window and navigate to the path where you would like to clone the repository.
Use the following command to begin a clone:
```
git clone https://github.com/<your github username>/social-platform-donut-frontend.git
```
Once the command completes you will have a new folder containing the cloned repository. We can validate this by running the “dir” command.  We can then move into that directory using the "cd " command.

![image of command line](https://i.imgur.com/QsQy4Sg.png)

**Setting up a remote upstream**

The next step is to set up a remote. Remotes simply represent paths or URLs to other versions of your repository. In our case, as we cloned from our fork on GitHub a default remote will have been setup for us called origin. This origin allows us to push and pull code from our forked repository hosted on GitHub. We can list the currently configured remotes on our machine using the “git remote” command.

Pushing and pulling from your own fork is very useful and this will be how you will work with the project most often. However, when working on that code, you’ll want to be starting from the most recent version of the code from the main donut-frontend repository. That code may have been updated and changed since you first made your fork. In order to get access to that latest code, we’ll setup a second remote which points to the main donut-frontend repository. We will not have commit rights there, so we cannot push changes, however, we will be able to fetch the latest commits that have occurred.

To create a new remote we use the “git remote add” command, passing in a name for the new remote and the URL as arguments. In our case since we want the second remote to point towards the original donut-frontend repository we will use the follwing command. It's possible to name the remote anything you like, but the convention is to name it "upstream".

```
git remote add upstream https://github.com/codeuino/social-platform-donut-frontend.git
```

**Installing the dependencies and running our local version of donut-frontend**

The next step is to install the required dependencies to our newly created donut-frontend app. This could be done by running the following command in the terminal.

```
npm install
```

The npm install command will install all the project dependencies mentioned in the package.json file.  
Once all the dependencies are completely installed the final step is to run our local instance using the following command.

```
npm start
```

Now visit the [http://localhost:3000](http://localhost:3000) using your favorite browser to see your very own donut-frontend app in action!