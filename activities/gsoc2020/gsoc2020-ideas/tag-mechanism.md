# Developing a module with a Tag Cloud with a post check mechanism

### **Priority:** 

Medium

### **Description:**

 The [**DONUT Platform**](https://github.com/codeuino/Social-Platform-Donut) contains the notification feature which helps users to accommodate things in easy way. So the task of this project is to develop a mechanism for **"tags" \(**[**Explanation of tags in posts by WordPress**](https://en.support.wordpress.com/posts/tags/)**\)** as an independent "**Tags Cloud**"and check and sort out similar posts from user end. These tags will provide a useful way to post users related to quickly tell readers what a post is about and where to redirect or highlight the particular post more. The mechanism should be developed in such a way that users can make their own tags or can also select from predefined tags\(this needs to be built as a kind of panel/store\) which gets automatically saved at one place and can be called as tag cloud and while submitting any posts it should get redirected to the appropriate users/groups which contains the similar tags. The tag cloud needs to be built which can store all the tags. When someone viewing your blog/project/article/any other post, clicks on one of defined Tag links, a Tag archive page with all the posts belonging to that Tag, should be displayed.

Other part of this project is develop a "**Post Check**" mechanism which will help the user writing the post to check from similar posts and allow to do some actions on the similar post.

**Tag prediction: -** In addition of the above idea, it is possible to predict the tags based on the content of the articles/posts using some ML algorithms \(Supervised Learning\). So that when user creates the post/article then he/she will have some auto-predicted tags as a suggestion along with option of adding custom tags.

**Approach:-** Firstly pre-process the data \(i.e posts/articles content\) and accordingly train the ML model and after that use the classifications algorithms to predict the tags.

**Understand tag-prediction with an example:**

Suppose a user has created the article/post whose content is something like this:

**"**GSOC stands for Google Summer of Code, a 3 to 4-month long program for students studying in any university all across the globe. Google started this program long back in 2005 aiming to promote the open source culture among the college and university students. During this program, a student works with an open source community or organization of his/her choice for around 3 to 4 months on a project.**"**

So for the above post the predicted tag should be like: "**GSOC**", "**Open Source**", "**Google**" and it should be displayed in the **Add tag field**, so if it seems irrelevant to the user then he can remove that and add their custom tag. \( Something like this: [click](https://raw.githubusercontent.com/olahol/react-tagsinput/HEAD/example/demo.gif) \)

**Lets understands this with an example**

**PART 1:** Assume that **"X"** user signs up on the DONUT platform. Once the **"X"** user has defined all the details about himself, then he would be asked to select some tags from the tags cloud which describes him the best and here, **"X"** user chooses "Designer", "Nodejs" and "Html". this tells us from the description of the tags in the tags cloud that this **"X"** user is a "Designer" and knows languages like "Nodejs" and "Html". On pursuing further these tags get stored for him.

Now assume other user **"Y"**, suppose "Y" user is already logged into this platform. **"Y"** user writes a post as project/article/blog or any other thing related to feeds on it, before **he/she** publishes, he would be asked to choose some tags from the "Tags Cloud". Suppose the **"Y"** user choose "Nodejs" tag from it. **Here, we see that user "X" and "Y" has "Nodejs" common in them.** So on publishing the post by user **"Y"**, the particular project would be redirected to the **"X"**\(because they both contain common tags\), According to the tags description user **"X"** would be able to review the thing.

PART 2: Suppose that **"X"** user writes some post, so before publishing it. He would be shown similar posts that either matches with the **"Title"** or **"Post Content"**. So clicking on any, he would be able to "Add/comment/share/Add reasons". This will help avoid replication of content as well.

{% hint style="warning" %}
**References:** [**Tag module by WordPress**](https://en.support.wordpress.com/posts/tags/) **,** [**Tag Screens by WordPress**](https://en.support.wordpress.com/posts/tags/)
{% endhint %}

### **Required Skills/knowledge:**

* Good knowledge of databases
* Good Knowledge of Back-end
* languages such as NodeJs, JavaScript, React;
* For tag-prediction: Python, ML, Supervised learning \(Beginners - Intermediate\)
* Knowledge of front-end as well for developing a tag dashboard

### **Difficulty Level:** 

Moderate

### **Expected Outcome:** 

This project would result in development of a tag mechanism with an appropriate dashboard where one can "Create/Edit/Manage/Delete" with proper settings option.

### **Potential Mentors:**

[**Jaskirat Singh**](https://github.com/jaskirat2000) , [**Devesh Verma** ](https://github.com/devesh-verma) and [**Vaibhav D. Aren** ](https://github.com/vaibhavdaren)



