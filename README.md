# Lifeshare | Portfolio Project 5

![Am I responsive](/readme-imgs/responsive.jpg)

[Live site for frontend](https://lifeshare.herokuapp.com/)

[Live site for backend](https://drf-api-sam.herokuapp.com/)
#
## Project Goals
- Design an interactive Front-End web application using HTML, CSS and advanced JavaScript, based on component composition and separation of concerns.
   - For more information see [Front-End Repository](https://github.com/FullstackSammy/lifeshare)
- Explain the key role that specialist Front-End developers perform in modern software development/delivery terms.
- Create an Application Programming Interface (current repository) for comsumption by 3rd party applications.
   - Create Unique models.
      - Number of models created four, two in contacts and two in imessages.
- Create an Interactive Front-End application that consumes API data.
#
## Key role of a Front-End developer
- The key-role of a Front-End developer is to build a set of clean, user friendly and reusable resources/pages, that independent of one another can be reused, even in other projects, and updated without refreshing the whole page it's view on. 
#
## Difference for the User when using React compaired to vanilla JavaScript
- Since React JS is built up of components that are reusable on several "pages", it's more intuitive for the user. They don't have to learn to "drive the car" with each new page they visit on the platform, and the whole page doesn't reload which would paus the user flow.
#
## Planning
#
- The current direction for this project is to follow the walkthrough given by Code Institute and some own unique designs.
#
## Technologies and Libraries
### Languages used
- [Django Rest Framework](https://www.django-rest-framework.org/) 

- [HTML](https://www.w3schools.com/html/html_intro.asp)

- [CSS](https://www.w3schools.com/css/css_intro.asp)

- [React JS](https://reactjs.org/)

### Databases and server gateways
- [ElephantSQL](https://www.elephantsql.com/)
  - As database in Heroku


### Frameworks, tools and libraries
#### Back-End
- [Django Rest Framework](https://www.django-rest-framework.org/)
- [Psycopg2](https://pypi.org/project/psycopg2/)
   - PostgreSQL database adapter for python
- [JSON Web Tokens](https://jwt.io/)
   - Http-safety, web-tokens for kepping user logged in, authentication etc.
#### Front-End
- [React JS](https://reactjs.org/)
- [JSON Web Tokens](https://jwt.io/)
    - Web-tokens for kepping user logged in, authentication etc.
- [React Bootstrap](https://react-bootstrap-v4.netlify.app/)
   - Specilaize Bootstrap framework with React components
- [React Router](https://v5.reactrouter.com/web/guides/quick-start)
   - Assist in switches, routes and links for React apps.
### Cloud storage and deployment services
- [Cloudinary](https://cloudinary.com/)
- [Heroku](https://www.heroku.com/)
#
## Demographics
- The intended user for this API is someone who wants to build a Front-End application consistent with the below stated User Goals.
- Lifeshare is intented for a demographic that likes social media, but want a warmer and calmer space to interact with other people, more personable.
#
## User Feautures
### Navigation & Authentication
- Navigation: As a user I can view a navbar from every page so that I can navigate easily between pages
- Routing: As a user I can navigate through pages quickly so that I can view content seamlessly without page refresh
- Authentication - Sign up: As a user I can create a new account so that I can access all the features for signed up users
- Authentication - Sign in: As a user I can sign in to the app so that I can access functionality for logged in users
- Authentication - Logged in Status: As a user I can tell if I am logged in or not so that I can log in if I need to
- Authentication - Refreshing access tokens: As a user I can maintain my logged-in status until I choose to log out so that my user experience is not compromised
- Navigation: Conditional rendering - As a logged out user I can see sign in and sign up options so that I can sign in/sign up
- Avatar: As a user I can view user's avatars so that I can easily identify users of the application
#
### Profile
- Profile page: As a user I can view other users profiles so that I can see their posts and learn more about them
- Most followed profiles: As a user I can see a list of the most followed profiles so that I can see which profiles are popular
- User profile - user stats: As a user I can view statistics about a specific user: bio, number of posts, follows and users followed so that I can learn more about them
- Follow/Unfollow a user: As a logged in user I can follow and unfollow other users so that I can see and remove posts by specific users in my posts feed
- View all posts by a specific user: As a user I can view all the posts by a specific user so that I can catch up on their latest posts, or decide I want to follow them
- Edit profile: As a logged in user I can edit my profile so that I can change my profile picture and bio
- Update username and password: As a logged in user I can update my username and password so that I can change my display name and keep my profile secure
#
### Post
- Post page: As a user I can view the posts page so that I can read the comments about the post
- Edit post: As a post owner I can edit my post title and description so that I can make corrections or update my post after it was created
- Create a comment: As a logged in user I can add comments to a post so that I can share my thoughts about the post
- Comment date: As a user I can see how long ago a comment was made so that I know how old a comment is
- View comments: As a user I can read comments on posts so that I can read what other users think about the posts
- Delete comments: As an owner of a comment I can delete my comment so that I can control removal of my comment from the application
- Edit a comment: As an owner of a comment I can edit my comment so that I can fix or update my existing comment
### Likes
- Create posts: As a logged in user I can create posts so that I can share my images with the world!
- View a post: As a user I can view the details of a single post so that I can learn more about it
- Like a post: As a logged in user I can like a post so that I can show my support for the posts that interest me
#
### Home Page
- View most recent posts: As a user I can view all the most recent posts, ordered by most recently created first so that I am up to date with the newest content
- As a user, I can search for posts with keywords, so that I can find the posts and user profiles I am most interested in.
- View liked posts: As a logged in user I can view the posts I liked so that I can find the posts I enjoy the most
- View posts of followed users: As a logged in user I can view content filtered by users I follow so that I can keep up to date with what they are posting about
- Infinite scroll: As a user I can keep scrolling through the images on the site, that are loaded for me automatically so that I don't have to click on "next page" etc
#
## Design
### Wireframes
The structure was taken from Code Institutes walkthrough project. The final design is by myself and I decided to use this color pallate:
![Colors](/readme-imgs/color.jpg)
#
## Testing in development
- A logged out User can only view items
- A logged out User can log in or register an account
- All testing is done on multiple users
#
### Profiles
- Testing creating a profile
- Testing editing profile: 
         - Bio
         - Image
         - Username
         - Password
     - Successfull
- Testing Follow and Unfollowing other Users
    - Following from 'Most Followed Users'
    - Following from Profile page
- Testing items followers and following change when following and unfollowing a User
- A User can view other Users profiles
- A User can only access the edit and delete tools on the Profile page they own.
- The posts from the Users a User follows appear on the Feed-page
- If user logs out from edit profile-page, user is transported to home-page
- if user tries to access edit profile-page from logged out, they are transported to home-page
#
### Post
- A logged in user can create posts with a chosen image or with a default image
- If title is not filled in error thrown: "This field may not be blank"
- If image not chosen error thrown
- If image is to big byte-wise error thrown
- If image is to big pixel-wise error thrown
- If cancel create post user is transported to home page
- If logged user tries to acces create post-page, they are transported to logged out home-page

#
### Comments
- A User can view their own and other Users posts
   - In that view they can comment that post
   - If a User created a comment, they can then edit or delete that comment
   - If a user did not create a comment, they can only view the comment
   - If the owner of the commented post, deletes that posts, the comments are deleted as well
- The comment-count changes when the number of comments change
- No empty comment is accepted, error thrown
#
### Likes
- A User can like and unlike other Users posts
- A User can not like their own post
- A User can only like a post if they haven't already liked it
- A users liked posts appear on the Like-page
- The like-count changes when the number of likes change-
- If a user logs out from Liked-page, they are transported to home page

#
### General Testing
- Tested the:
     - Collaps of the NavBar
     - NavBar in different views
     - Responsiveness of the layout down to 320px.
     - upload of images to Cloudinary from UI
     - Login
        - error thrown if wrong username
        - error thrown if wrong password
        - error thrown if no username
        - error thrown if no password
     - Register
        - error thrown if no username
        - error thrown if username is taken
        - error thrown if no password and confirmed password
        - error thrown if password and confirm password doesn't add upp
     - Saving data to Back-End
     - Editing data in Back-End from Front-End, updated_at is updated in Back-End
     - No broken links found
     - testing responsiveness with [AmIResponsive](https://ui.dev/amiresponsive?url=https://lifeshare.herokuapp.com/)
#
## Bugs in development
- Added README-files to fast and hindered installment of dependencies
   - Delete all files that could interfere
   - Install dependencies
   - Recreate README-files
- Problem uploading images for Users
   - bug solved by adding back default image to posts/models.py in the Back-End
- While developing the Front-End part of this project I couldn't get post_count, following_count and follow_count to work in the profile.
   - These fields where not added to profiles/serializers.py in the Back-End. 
   - Added items and bug resolved.
#
## Set up repository
- Start with a new empty repo
   - Since there are items from the full-template that can interfere with React.
   - choose a name with all lower case letters
   - Create repository
   - Add items to do
   - Create project
   - Add items to project
#
## Set up project in GitPod
- Launch repository to GitPod and let build finish to minimize risk of disturbance to automatic setup
- Enter command: "npx create-react-app . --template git+https://github.com/Code-Institute-Org/cra-template-moments.git --use-npm"
   - To install correct dependencies
   - All dependencies needed are now installed.
- npm start
   - to test if React is compiled successfully
#
## Initial Deployment
- After the [set up in GitPod](#set-up-project-in-gitpod), make the initial deployment to Heroku.
- In Heroku:
    - Front-End app
        - Create a new app called lifeshare
        - connect to lifeshare repository in GitHub
        - Launch app to create a url
        - After connection up the Front-End and the Back-End, relaunch page with API database
    - BackEnd app
        - In Config Vars
            - Add CLIENT_ORIGIN and https://lifeshare.herokuapp.com/ as value to give deployed page access to API database
            - Add CLIENT_ORIGIN_DEV and https://3000-fullstacksamm-lifeshare-nf2nfc1ycgy.ws-eu82.gitpod.io/ as value (this changes over time and is a known bug, solution is an update of the Config Vars when needed)
#
## Final Deployment
- In Heroku.
    - After pushing the last version to GitHub, from GitPod.
        - Under the tab deploy, deploy latest branch, ensure successfull build.
        - Open app
        - Test all feautures in deployed version to make sure it's the same as the preview.
#
## Credits
## Thank you
- Antonio for always being there and being a fantastic mentor.
- Tutors at Code Institute
- Code Institute Slack-channel community for being the good and funny bunch of people I need!


### Content credits
- The biggest credit has to go Code Institute, I followed the Walkthroughs given, and developed a little on top of it.

### Media
- Every media image that was used, came from free resource [Unsplash](https://unsplash.com/)

#
* [Back to top](#)
#