# Location Blog

## Purpose of this site

This site has been created so that users can share and seek information about places to visit.  
Unregistered users can view a summary of the posts, to get a flavour of what the site does.  
Registered users can create posts, edit and delete their own posts.  They can also comment and like other peoples posts.


## User Experience


### User Goals


#### First Time User would like to:
- find out the purpose of the site and how to use it
- be able to easily navigate throughout the site
- see a list of posts to see if the site is something they would be interested in
- be able to register for a user account

#### Registered User would like to:
- be able to sign into my user account
- view posts and leave comments and likes
- create their own post
- edit and delete their own posts only
- be able to logout of my account to keep my account safe

#### Site Owner would like to:
- restrict access to non-registered users
- control users posts and comments for inappropriate use of the site. I have decided not to put in approval by superuser for adding posts and adding comments but instead have put a warning that the site admin will remove anything that is not in keeping with the sites ethos.

### User Stories

I used Guthub issues to record the following user stories:
 
- Manage posts - As a site admin I can create, read, update and delete posts so that I can manage the blog content.
- Pagination - As a site user I can view a paginated list of posts so that I can easily select a post to view.
- View likes - As a site user/ admin I can view the number of likes on each post so that I can see which is most popular.
- View post list - As a site user I can view a list of posts so that I can select one to read.
- View a detail post - As a signed in user I can click on a post so that I can read the full text.
- View comments - As a signed in user I can view comments on an individual post so that I can read the conversation.
- Account registration - As a site user I can register an account so that I can comment and like posts.
- Comment on a post - As a signed in user I can leave a comment on a post so that I can interact with the content.
- Like/unlike - As a signed in user I can like or unlike a post so that I can interact with the content.
- Create a post - As a signed in user I can create a new post so that I can share cool locations with other users.
- Edit posts - As a signed in user I can edit my posts so that i can update or correct information.
- Delete posts - As a signed in user I can delete my posts so that I can remove them from the website.
- Feedback messages - As a user I get messages back after I perform an action so that I know whether i have completed the action correctly.
- Landing page - As a site user I can go to the landing page so that I can see the purpose of the website.
- highlight active page - as a site user I can see the active page highlighted so that I know what page I am on.

### Wireframes

I have used balsamiq to create the following wireframes for both desktop and mobile devices.
- home page

[mobile home page](/documentation/wireframes/mobile_homepage.jpg)

[mobile home page with drop down navigation](/documentation/wireframes/mobile_with_drop_nav.jpg)

[mobile home page user signed in](/documentation/wireframes/mobile_home_drop_signedin.jpg)

[desktop home page](/documentation/wireframes/desk_home.jpg)

[desktop home page user signed in](/documentation/wireframes/desk_home_signedin.jpg)

- register page

[mobile register page](/documentation/wireframes/mobile_signup.jpg)

[desktop register page](/documentation/wireframes/desk_register.jpg)

- Login page

[mobile login page](/documentation/wireframes/mobile_login.jpg)

[desktop login page](/documentation/wireframes/desk_login.jpg)

- Post list

[mobile post list page](/documentation/wireframes/mobile_postlist_not_signedin.jpg)

[desktop post list page](/documentation/wireframes/desk_postlist_not_signed_in.jpg)

[mobile post list page user signed in](/documentation/wireframes/mobile_postlist_signed_in.jpg)

[desktop post list page user signed in](/documentation/wireframes/desk_postlist_signedin.jpg)

[mobile post list page author signed in](/documentation/wireframes/mobile_postlist_author.jpg)

- Post Detail

[mobile post detail page](/documentation/wireframes/mobile_postdetail.jpg)

[desktop post detail page](/documentation/wireframes/desk_postdetail.jpg)

- Create post page

[mobile post create page](/documentation/wireframes/mobile_create.jpg)

[desktop post create page](/documentation/wireframes/desk_create.jpg)

- Edit post page

[mobile post edit page](/documentation/wireframes/mobile_edit.jpg)

[desktop post edit page](/documentation/wireframes/desk_edit.jpg)

- Delete post page

[mobile post delete page](/documentation/wireframes/mobile_delete.jpg)

[desktop post edit page](/documentation/wireframes/desk_delete.jpg)

- Sign out page

[mobile signout page](/documentation/wireframes/mobile_signout.jpg)

[desktop signout page](/documentation/wireframes/desk_signout.jpg)

### Agile Development Tool


I am using an agile software development tool in the development of this website.  I am using Github projects, using a basic Kanban template.  I added automation so that as each new issue is added it adds it to the 'To Do' list for my project.  As I start working on each issue I move it to the 'In progress' column.  When the coding for each issues has been completed, the issue is then moved to the 'done' column.

![my kanban board](/documentation/images/kanban_1.png)

![my kanban board](/documentation/images/kanban_1.png)

## Existing Features

### Navbar and footer

#### Navbar

The navbar is plain and simple so that it is very easy for the user to read.  The name of the website is clear in the top left hand corner - Location Blog. There are links to Home, Posts, Register and Login pages for all users.   If the user is not signed in, the sign in and register links are visible on the navbar. 

![Navbar for not signed in user](/documentation/images/navbar.png)

If the user is signed in, then there is a Logout link visible.  Also if the user is signed in there is a message to say user name is currently signed in, to act as an extra visual to the user that they are signed in! 

![Navbar for signed in user](/documentation/images/navbar_signedin.png)

The page that is being viewed is highlighted in the navbar so that the user can see easily what page they are on.

In mobile view the navbar is collapsed into a hamburger icon, which when clicked shows the same information as in desktop view.

![Mobile Navbar](/documentation/images/hamburger.png)

![Mobile Navbar for not signed in user](/documentation/images/hamburger_not.png)

![Mobile Navbar for signed in user](/documentation/images/hamburger_signed.png)

#### Footer

The footer is very simple with minimal information, just displaying social media options.

![Footer](/documentation/images/footer.png)

### Register Page

When a user clicks the register button they are brought to the register page where they have to fill in their username, an email address but this is optional and their password, which they then have to confirm. Then click the button sign up. If the user has come to register instead of login, there is text to say if you have already an account click login. If the registration is successful the user is redirected back to the home page and a message just below the navbar will appear for 3 seconds to say successfully signed in as 'username'.

![Register](/documentation/images/register.png)

![message to say successfully signed in](/documentation/images/signedin.png)

### Login Page

If a user has already registered they can log into the site in the login page.  The user is asked for their username and password. If correct the user is redirected back to the home page to begin their viewing. A message will appear under the navbar for 3 seconds to say successfully signed in as 'username'.

![Login](/documentation/images/login.png)

![message to say successfully signed in](/documentation/images/signedin.png)

### Logout page

The user is asked are they sure they want to logout and then they can click the sign out button. the user is redirected back to the home page. a message will appear for 3 seconds under the navbar to say you have signed out.

![Logout](/documentation/images/logout.png)

![message to say successfully signed out](/documentation/images/signedout.png)

### Home Page

The home page consists of a hero image of a beautiful landscape, with the hero text of Location, Location, Location. Share your favourite places. Find new places.

![hero image](/documentation/images/hero_image.png)

Under the hero image, there is a short text to tell the user how this website works. If the user is not logged in they can only see the home page and the post list page. A signed in user can also see the post detail page, can like/unlike posts, can leave comments, can create their own post, can edit their own post and delete their own post. Finally their is a button for the user to get to the posts page.

![home information](/documentation/images/home.png)

### Posts Page

This page can be seen by both logged in and unlogged in users.  I wanted the unlogged user to get a look at what the blog offered so that they might then register and login. This page shows the title, location, authors name, date the post was created, image, how many likes and a short excerpt. If the author does not attach an image a stock picture is used.
In mobile view each post is the full width of the screen and the user can scroll down to see the other posts.
 
![mobile posts](/documentation/images/mobile_posts.png)

In desktop there are 6 posts per page, with 3 on the top row and 3 underneath.  If there are more than 6 posts there is a next button to look at the next page of posts and also a previous button to navigate back to the previous pages.

![desk posts](/documentation/images/desk_posts.png)

I have added the alt attribute on images for screen readers to make the site more accessible.
I have also capitalized the title and location so the page looks more uniform as we are relying on user input.

For logged in users only they can view all the detail posts.  For users not logged in the view button is not available to them. 

![able to see the view button](/documentation/images/view.png)

If the user is the author of the post they also have access to an edit and delete button.  The edit and delete buttons are only visible if the user that is signed in is the author of this post.

![able to see the edit & delete button](/documentation/images/all_buttons.png)

### Post Detail page

This page can only be accessed by logged in users. I have added alt atributes for the images for accessibility.
On mobile view the image is not displayed as it takes up too much room. There is a header banner which includes the title, location, author and date created.  Then under the banner is the content from the post.  Under the content there is a heart icon which acts as a button to allow the user to like or unlike the post.  If the heart is filled in red it means that this user has liked the post.  If the heart was just an outline in red it means this user has not liked this post.  There is logic in place that if a user has liked the post if they click the heart it will unlike the post. There is also a number beside the heart to show how many likes this post has. Also there is a comment icon again with a number to show how many comments.

![post detail](/documentation/images/title_detail.png)

This user has not liked this post as the heart is just an outline.

![post is unliked by this user](/documentation/images/unliked.png)

This user has liked this post as the heart is filled in with red.

![post is liked by this user](/documentation/images/liked.png)

Under this is the comments section, so it displays any comments that have been left on this post with the commenters name and date they left the comment.  Under this there is a simple form for the user to add a comment and submit it.  If the user clicks the submit button they have to have written something in the form or it gives a warning.  When the submit button is clicked the user is redirected back to the detail post and a message appears for 3 seconds to say thanks for leaving a comment.

![comment detail](/documentation/images/comment_detail.png)

![message to say successfully left comment](/documentation/images/comment.png)

### Create Post

If a signed in user clicks the 'Create Post' on the navbar it brings them to the create post page.  This is a form that the user has to fill in.  They must fill in the title, location and content fields, the image and excerpt are optional. The user will get warning messages if any of the required fields are not filled. If the user does not choose an image to add to their post a stock image will appear on the website.  If they do not put any text in the excerpt field, nothing will display for this post in the post list page.  

![create a post](/documentation/images/create_post.png)

When the user clicks the create button, they will be redirected back to the posts page. A message will appear just under the navbar to say successfully created a post.

![message to say successfully created post](/documentation/images/create.png)

### Edit Post

If a user clicks the edit button on the posts page, they will be brought to the edit post page.  This is very similar to the create page only this is populated with the information from the post that the user has tried to edit.  The user can then edit some or all of the post and then click the edit button. 

![edit a post](/documentation/images/edit_post.png)

The user will be redirected to the posts page.  A message will appear just under the navbar to say successfully edited the post.

![message to say successfully editted post](/documentation/images/edit.png)

### Delete Post

If a user clicks the delete button on the posts page for a post, they will be directed to the delete post page.  Here there is a button to 'go back' in case they accidently cam ehere and didn't mean to delete the post. this will bring them back to the posts page. The delete page checks to make sure that the user wants to delete the post - asking them are they sure? The name of the post that is about to be deleted is displayed. 

![delete post](/documentation/images/delete_post.png)

Then if the user clicks delete, the post is deleted and the user is redirected back to the posts page.  A message will appear just under the navbar to say that the post has been successfully deleted.

![message to say successfully deleted post](/documentation/images/delete.png)

### Super user/admin

I created a superuser/admin so that they can create, read, update and delete posts so that they can manage the blogs content.  They can remove any post or comment that is not in keeping with the ethos of the site.


## Design

The design is kept simple to let the location posts take centre stage.  Also to make it easy for users to navigate the site.

### Data Model

I needed two data models to amke this website work.  The first data model is the Post. This contains the information for the post.  I have a second data model for the comments which are linked to a post.

#### Location post model

| Key | Name | Type
|-----|----------------|------------------|
| | title (unique) | Char(200)
| | location | Char(50)
| foreign key | author | User Model
| | created_date | DateTime
| | updated_date | DateTime
| | content | TextField
| | featured_image | Cloudinary_image
| | excerpt | TextField
| many-to-many | likes | User Model
| label for url | slug (unique) | slugfield

#### Comment model

| Key | Name | Type
|--------|----------------|-------------------|
|foreign key | post | Post Model
| | name | Char(80)
| | body | TextField
| | created_on | DateTime

### Typography

The fonts I have selected are :  Nunito for the text and Roboto for the headings.  These have been selected as they are clear and simple.

### Images/color

I have kept the layout and colours simple. 


## Technologies used

### Languages

- HTML
- CSS
- Python

### Frameworks, libraries & programs

- Django
- Bootstrap
- Google Fonts
- Font Awesome for icons
- Github/Gitpod
- Cloudinary used to host static files
- Gunicorn as the server for Heroku
- Heroku used for cloud based deployment
- Summernote as editor
- Heroku Postgres for production database
- SqLite for local environment database
- Balsamiq for the wireframes


## Code Validation

### Html validation

To validate each of my html pages I inspected the page through devtools and viewed the page source and copied and pasted this into the W3C markup validation service.

for home page

![home page](/documentation/validation/html-validator-index.png)

for register page

![register page](/documentation/validation/html-validator-register.png)

for signin page

![sign in page](/documentation/validation/html-validator-login.png)

for signout page

![sign out page](/documentation/validation/html-validator-logout.png)

for post page

![post page](/documentation/validation/html-validator-postlist.png)

for post detail page

![post detail page](/documentation/validation/html-validator-postdetail.png)

for create post page

![create post page](/documentation/validation/html-validator-postcreate.png)

for edit post page

![edit post page](/documentation/validation/html-validator-postedit.png)

for delete post page

![delete post page](/documentation/validation/html-validator-postdelete.png)

### CSS Validation

I copied my style.css file into the W3C CSS validation service.

![css file](/documentation/validation/css-validator-locationblog.png)

### PEP8 Validation

I copied and pasted my python files into the PEP8 vslidator

for models.py file

![models.py](/documentation/validation/PEP8-models-py.png)

for forms.py file

![forms.py](/documentation/validation/PEP8-forms-py.png)

for urls.py file

![urls.py](/documentation/validation/PEP8-urls-py.png)

for views.py file

![views.py](/documentation/validation/PEP8-views-py.png)

for settings.py file

![settings.py](/documentation/validation/PEP8-settings-py.png)

for codeloco.urls.py file

![codeloco.urls.py](/documentation/validation/PEP8-codeloco-urls-py.png)


## Testing

### Manual testing

I checked each page (home, signup, login, logout, post, detail, create, edit, delete) to make sure everything looked ok at all screen sizes.

I am going to use the user stories as my structure for manually testing my project.
 
#1 manage posts
- as admin I can create a post
If I do not enter data in the required fields it gives a warning to add data to the required fields.  It is ok not to have data in the excerpt field. It is also ok to not include an image, if an image is not added by the admin/user a stock image will be included.

![showing warnings for required fields](/documentation/testing/admin_add_post_1.png)

when all required fields are filled and the post is saved, we get a success message and can see the new post.

![show success message and new post in list](/documentation/testing/admin_add_post_2.png)

- as admin I can read a post

Check in the website that the new post is there with correct data, including stock image.

![new post visible on website](/documentation/testing/admin_add_post_3.png)

- as admin I can update a post

Similar to create post in update if any of the required fields are not filled a warning is shown and fields that need filled are highlighted.

![warnings for update similar to create](/documentation/testing/admin_update_post_1.png)

when all required fields are filled a success message is given and I can see the updated

### Lighthouse

Testing of desktop for Home page

![lighthouse for desktop home page](/documentation/testing/light_desk_home.png)

Testing of desktop for post page

![lighthouse for desktop post page](/documentation/testing/light_desk_post.png)

Testing of desktop for detail page

![lighthouse for desktop detail page](/documentation/testing/light_desk_detail.png)

Testing of mobile for home page

![lighthouse for mobile home page](/documentation/testing/light_mob_home.png)

Testing of mobile for post page

![lighthouse for mobile post page](/documentation/testing/light_mob_post.png)

Testing for mobile for detail page

![lighthouse for mobile detail page](/documentation/testing/light_mob_detail.png)

### Bugs 

- not auto filling the slug field when user created a post - I needed to use slugify and then this worked.
- not pulling in the image when a user created a post - needed to add enctype='multipart/form-data to the form.
- some issues with accessibilty not a big enough contrast between the text and the background. I changed these to have a darker background and white text so that there was a bigger contrast.
- width attribute 100% giving an error in W3C html validator, couldn't find a way around this.

## Deployment, forking and making a clone

### Deployment to Heroku

Initial deployment:

I followed the 'I think therefore I blog' walkthrough to create a basic django project.  I used the code institute template. 
- I installed django and supporting libraries:
 I installed django, gunicorn, psycopg2, cloudinary.
I created the requirements.txt file.

- I created a new django project called 'codeloco' and a django app called 'blog'
I need to add blog to installed apps in settings.py.
After adding new app we need to migrate the changes to the database.

- I set the project to use Cloudinary and PostgreSQL database.
I created a heroku app called codeloco
I attached it to the database
I created an env.py file - this contains all the secret environmental variables. I need to reference this in settings.py file.
I connect to cloudinary and tell django to use cloudinary to store media and static files.
I set up for static and media at the bottom of settings.py file.
I need to tell django where our templates will be stored.
I need to add heroku host name into allowed hosts in settings.py file.
I need to create 3 directories at the same level as manage.py file for media, static and templates.
I need to create a Procfile this tells heroku how to run our project.

- I deployed the empty project to heroku
In Heroku in teh deploy tab.
I click Github.
I search for my repo.
Then scroll down and deploy branch.
Watch the build to check it was successful.
Then open app

When I had completed my testing in development, in the settings.py file I set DEBUG = False and added X_FRAME_OPTION = 'SAMEORIGIN'.
I git add ., then git commit git push.
In heroku I went into config vars and deleted the DISABLE_COLLECTSTATIC = 1
In the deploy tab in heroku, I deployed branch and watched the build to check it was successful. Then I opened the app and repeated all my testing to ensure this worked the same as my local testing.



### Forking the Github repository

By forking the GitHub Repository you will be able to make a copy of the original repository on your own GitHub account allowing you to view and/or make changes without affecting the original repository by using the following steps:

- Log in to GitHub and locate the GitHub Repository
- At the top of the Repository (not top of page) just above the "Settings" button on the menu, locate the "Fork" button.
- You should now have a copy of the original repository in your GitHub account.

### Making a local clone

- Log in to GitHub and locate the GitHub Repository
- Under the repository name, click "Clone or download".
- To clone the repository using HTTPS, under "Clone with HTTPS", copy the link.
- Open commandline interface on your computer
- Change the current working directory to the location where you want the cloned directory to be made.
- Type git clone, and then paste the URL you copied above.
- Press Enter. Your local clone will be created.


## Credits

- I used 'I think therefore I blog' to set up files, heroku app, cloudinary, environmental variables and github projects.
- I used github projects and kanban for user stories like 'I think therefore I blog'
- I used 'tails on trails' to help set out what I wanted for my project
- I got help with navigation from 'Tails on Trails'.
- I used card system from 'I think therefore I blog' for displaying posts.
- Ciara O'sullivan on slack for solving my slug problem when user creating post didn't create the slug field.
- I used the messages from 'I think therefore I blog'
- To help with crud functionality I used Dennis Ivy you tube video for to do list app
- To understand class based views explained well by Dennis Ivy
- I got help for showing active page on navbar from 'Favoureats'.
- I got my hero image from thetimes.co.uk.
- I found solution to my too long lines in settings.py in code.djangoproject.com/ticket/28163.
- i got structure of readme from JoGorska_alumni_lead


## Acknowledgements
- I would not have completed this project without the support and understanding of my family.
- Wonderful help and support from my cohort and facilitator Kasia.
- Help and support from my mentor Celestine Okoro.