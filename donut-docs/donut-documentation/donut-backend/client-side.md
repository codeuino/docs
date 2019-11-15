# Client-Side

## Introduction <a id="introduction"></a>

Donut has two different directories for client and server, for server side guide refer [Server Side](server-side.md).

The frontend of the project is set up using Vue 3, and design is setup using Vue Bootstrap and Vuetify. Every view in the project has a separate components in the views directory, which contains shared components in the components directory, the objective of this is to bring modularity in the project.

Stay careful, on updating any shared components may bring changes to other views as well.

## File Structure <a id="file-structure"></a>

```text
.+-- dist+-- .node_modules+-- public|   +-- img|       +-- icons|   +-- favicon.ico|   +-- index.html|   +-- manifest.json|   +-- robots.txt|   +-- service-worker.js+-- src|   +-- assets|       +-- test_data|       +-- config.js|   +-- components|   +-- views|   +-- plugins|   +-- services|   +-- store|   +-- App.vue|   +-- main.js|   +-- registerServiceWorker.js|   +-- router.js+-- tests|   +-- unit+-- .browserslistrc+-- .editorconfig+-- .eslintignore+-- .eslintrc.js+-- .gitignore+-- babel.config.js+-- .package-lock.json+-- .package.json+-- .postcss.config.js+-- README.md+-- vue.config.js
```

## Design <a id="design"></a>

The designs are setup to be responsive even for the 2K screens, the design is minimal and light intended for professionals and organisations. User interface is created using Bootsrap, Vue Bootstrap and Vuetify and grid system is followed throughout the system. Vue is based on single page application design, so frontend design is setup for such requirements.

**For each view, sub components are added on the grid system and reused at different places, so stay careful on making changes.**

#### **Screenshots** <a id="screenshots"></a>

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LmNu7h893q6uE4kRHHp%2F-LmO0ZtIO-rhtyGYnxbA%2F-LmO8cORn64E1QkZe_PJ%2FScreenshot%20from%202019-08-16%2012-07-31.png?alt=media&token=ac526e6c-fff0-474b-8346-003d56ef7800)

Feed

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LmNu7h893q6uE4kRHHp%2F-LmO0ZtIO-rhtyGYnxbA%2F-LmO8fwS7Bx_sAjdQREz%2FScreenshot%20from%202019-08-16%2012-07-56.png?alt=media&token=cf3db5ab-bbf4-4f03-af22-454f280efd91)

Profile

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LmNu7h893q6uE4kRHHp%2F-LmO0ZtIO-rhtyGYnxbA%2F-LmO8iMucqhGHaagSxQS%2FScreenshot%20from%202019-08-16%2012-08-12.png?alt=media&token=3edf2db9-ab67-40c8-bc0e-7df436a36b34)

Settings

**Please refer before contributing:**

## Modules <a id="modules"></a>

### Navigation Bar <a id="navigation-bar"></a>

The application provides two navigation bar, one on top and other on left side.

The upper navigation bar is setup to provide navigation to announcement and also display custom navbar name set up by user on registration. This navbar is managed using state variable `isLogged`, which displays navbar whether user is logged in or not.

Whereas, the side navbar is for actual navigation, client can navigated over every views using this navbar, `user id` and `user type` using computed functions which fetches from session data and injects to the components.

#### Screenshots <a id="screenshots-1"></a>

​

#### Code Snippets <a id="code-snippets"></a>

```text
​
computed: {    getNavbarName () {      return this.$session.get('navbarName')    },    id () {      return this.$session.get('UserID')    },    isLogged () {      return this.$store.state.isLogged    }  },
```

_The computed functions inject session data to navigation bar template._

### Login/Signup <a id="login-signup"></a>

#### Login <a id="login"></a>

Donut provides login page for user and organisation to login, and also provides Oauth login functionality using Google and Github, the Login page has sub-component `Login.vue`

This views imports Typewriter module which displays type writing heading effect and login module uses vue-google-oauth2, frontend validation, location service and subscriptions for providing login feature.

The sub modules provides following feature:

* **Location Service:** The modules fetches user current location using fetch API and sends to server for providing better user experience.
* **Frontend Validation:** This modules provides validation on user input and disables and enables login button accordingly using computed functions.
* **Subscription:** This module creates subscription object and sends to server for providing web push notification service to user.
* **vue-google-oauth2:** This module is used to provide google oauth feature to the users, the module using promises to fetch user details to client which moreover send to server on login.

#### Signup <a id="signup"></a>

Donut provides signup feature where user can created a account using third party oauth or simply signup with their email account, password and name, these details are stored in application as state, which are accessed in second step and send to server.

The signup procedure consist of two steps, first step user has to input email and password and in second they have to input type, location, bio and github link.

```text
this.addSignupData({            email: this.email,            password: this.password,            name: this.name          })
```

**Screenshots**

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LmNu7h893q6uE4kRHHp%2F-LmUp_8x7E81cj89glE7%2F-LmUr5J0G8FSfZYdxc9U%2FScreenshot%20from%202019-08-17%2019-24-41.png?alt=media&token=f79f9636-5e51-4993-9b1c-65bb9b09b86b)

Signup Page 1

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LmNu7h893q6uE4kRHHp%2F-LmUp_8x7E81cj89glE7%2F-LmUr5J7Q5aICspZehoO%2FScreenshot%20from%202019-08-17%2019-24-57.png?alt=media&token=85857578-30f5-47c2-ba55-7884dfc443f2)

Signup Page 2

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LmNu7h893q6uE4kRHHp%2F-LmUp_8x7E81cj89glE7%2F-LmUrOIptKbveNGGNQNO%2FScreenshot%20from%202019-08-17%2019-26-18.png?alt=media&token=2b819db4-eef1-4feb-81f4-6851281dfcf3)

Login Page

### Feed <a id="feed"></a>

The following module provides news feed to the user where user can see to projects, events and posts of others, this module has three subcomponents and data is injected into them using props. In the application, there are three feeds, main feed, project feed and event feed. The side navigation access `user_id` using vue-session.

**The subcomponents are:**

* Side Navigation
* Feed Group
* Recents

The feed group has another sub components Project, where post, project or event data is inject and displayed.

The feed group also contains create buttons, which display models to add new project, posts and events.

```text
<SideNavigation/><FeedGroup :postsArray="posts"/><Recent/>
```

**Screenshots**

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LmNu7h893q6uE4kRHHp%2F-LmUp_8x7E81cj89glE7%2F-LmUuP0NN92fP8pI5o8V%2FScreenshot%20from%202019-08-17%2019-39-07.png?alt=media&token=d512fa6c-568f-4c4f-85a9-8c1364321441)

Main Feed

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LmNu7h893q6uE4kRHHp%2F-LmUp_8x7E81cj89glE7%2F-LmUuMtgy-WtN8aFSobh%2FScreenshot%20from%202019-08-17%2019-39-13.png?alt=media&token=dc1b58e0-fce3-4784-b841-6cce04c4b43e)

Project Feed

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LmNu7h893q6uE4kRHHp%2F-LmUp_8x7E81cj89glE7%2F-LmUuMtjJLg40k3Gi0ii%2FScreenshot%20from%202019-08-17%2019-39-16.png?alt=media&token=d6fb3ca5-2035-4e31-9eae-426734e7b16a)

Event Feed

### **Profile** <a id="profile"></a>

This module lets user to look over other's profile and see their projects as well, this module is setup using two sub-components, User Details and Feed Group, and the data is injected into them using props.

The user detail also has a toggle button, which let user to follow or unfollow other user, but they can't follow themselves. On clicking toggle button, it emits the signal to parent component to update backend.

```text
if (this.Userfollowing) {

        this.$emit('FollowerIncoming', 0) // Decrease Follower List and remove the currentUSer        this.Userfollowing = !this.Userfollowing      } else {        this.$emit('FollowerIncoming', 1) // Decrease Follower List and remove the currentUSer        this.Userfollowing = !this.Userfollowing      }
```

```text
computed: {    followingCount () {      return this.user.followingList.length    },    followerCount () {      return this.user.followersList.length    },    differentPerson () {      return this.$route.params.id !== this.user.id    },    isUserFollowing () {      return this.Userfollowing    }  }​
```

Make sure, the parent component sends data to backend.

#### Screenshots <a id="screenshots-2"></a>

​

### Dark Mode <a id="dark-mode"></a>

The module's purpose is to make application low light compatible by changing colour scheme to dark.This components toggles the state value `DarkMode` which toggles every component of application. Every component has build in if statement to push the dark theme class into whenever DarkMode toggles to true.

```text
:class="$store.state.darkMode ? 'bg-dark' : '' "
```

Don't add same class name for dark mode in parent and child components as parent style properties will overwrite it.

**Screenshots**

### **Settings** <a id="settings"></a>

This module provides user to access settings, i.e Profile Setting and Integration Setting.

This module consist of three sub component which display settings according to settings state in the application, the first sub component Setting Menu lets user to toggle over Profile Setting and Integration Setting.

```text
SettingState: { // These are for which view is active in setting module    isPActive: true,    isIActive: false  },
```

#### Profile Settings <a id="profile-settings"></a>

This sub component indents user to access their profile settings and update it easily, it includes a form which is editable so user can change their details easily.

**Integration Settings**

This sub component allows user to change their integration setting, including here user can import projects from github and save them in Donut as own projects.

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LmNu7h893q6uE4kRHHp%2F-LmZ5kIsD1JeOXklop6-%2F-LmZ6BbweeqZIYpA2UK6%2FScreenshot%20from%202019-08-18%2015-13-20.png?alt=media&token=d89950aa-50fb-48db-8d11-4f445dfdb291)

Profile Settings

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LmNu7h893q6uE4kRHHp%2F-LmZ5kIsD1JeOXklop6-%2F-LmZ6Fokhp1Ez156RGKv%2FScreenshot%20from%202019-08-18%2015-13-43.png?alt=media&token=5ef585c8-2e3a-4d10-aede-99949215a8c3)

Integration Settings

### Landing Screen <a id="landing-screen"></a>

This module, provides a landing page template for **organisation** only. Landing page can be seen by any users, if landing page is not setup yet, a 404 page will be displayed.

If landing page is not setup and admin tries to access it, a setup form will be displayed where admin can setup.

The logic is handled by a single state variable `error` .

### Liked Projects <a id="liked-projects"></a>

This module displays projects liked by user, it has two sub modules used Side Navigation and Feed Group, server injects liked projects data from server to the liked project feed which is therefore injected to Feed Group module.

### Card Components <a id="card-components"></a>

Card components are required to display to projects, posts and events and each type of content has different kind of card, which is fetched using `v-if` statements.

**Code snippets**

```text
// Card for displaying Projects

<div v-if="post.pname" class="post-card" :class="$store.state.darkMode ? 'content-dark' : 'content-light' ">              <div class="lead float-right pr-3 pt-3 post-tag">Project</div>              <div class="post-header">                <img src="https://image.flaticon.com/icons/svg/17/17004.svg" alt="">                <h3>{{post.authorName}}</h3>              </div>              <div class="post-title">                <router-link :to="`/project/${post._id}`"><h4>{{post.pname}}</h4></router-link>              </div>              <p class="post-description">{{post.description}}</p>              <div class="post-img">                <img :src="post.image" alt="">              </div>              <div class="userResp">                <div class="row mb-4 user-btn">                  <i class="fas fa-thumbs-up col-2 pt-2" :class="{'Blue': isThumbsUpActive}" @click="toggleVote"></i>                  <i class="fas fa-thumbs-down col-2 pt-2" :class="{'Blue': isThumbsDownActive}" @click="toggleVote"></i>                  <i class="fas fa-share pt-2 col-2"></i>                </div>                <div class="comment-container">                  <form @submit="addComment">                      <input type="text" class="form-control comment" placeholder="Add Comment" v-model="Currentcomment" @submit="addComment">                  </form>                </div>              </div>
```

### **Store and Sessions** <a id="store-and-sessions"></a>

The application manages application level state as well as some data in session, including user preferences and authentication token respectively.

Sessions are only set up on successfully login, and user preferences are set to default and can be only updated using build in mutations and actions.

Vue sessions does not provide two way binding so keep in mind before injecting it to any component.

States sets to default on refresh so make sure to use router link on page navigation.

```text
export default {  token: null,  isLogged: false,  position: null,  userDetails: null,  SettingState: { // These are for which view is active in setting module    isPActive: true,    isIActive: false  },  IDofShare: null,  Portfolio: {},  darkMode: false,  Todos: [],  temp: {},  // On deployment make sure you change this accordingly  BaseURL: 'http://localhost:3000'}
```

​

