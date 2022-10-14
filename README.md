# Location Blog

## Purpose of this site

This site has been created so that users can share and seek information about places to visit.  
Unregistered users can view a summary of the posts and get a flavour of what the site does.  
Registered users can create, edit and delete their own posts.  They can also comment and like other people's posts.

![am i responsive](/documentation/testing/location_responsive.png)

## User Experience


### User Goals


#### First Time User would like to:
- find out the purpose of the site and how to use it
- be able to easily navigate throughout the site
- see a list of posts to see if the site is something they would be interested in
- be able to register for a user account

#### Registered User would like to:
- be able to sign into their user account
- view posts and leave comments and likes
- create their own post
- edit and delete their own posts only
- be able to logout of their account to keep their account safe

#### Site Owner would like to:
- restrict access to non-registered users
- control users posts and comments for inappropriate use of the site. I have decided not to put in approval by superuser/admin for adding posts and adding comments but instead have put a warning that the site admin will remove anything that is not in keeping with the site's ethos


### User Stories


I used Github Issues to record the following user stories:
 
- Manage posts - As a site admin I can create, read, update and delete posts so that I can manage the blog content.
- Pagination - As a site user I can view a paginated list of posts so that I can easily select a post to view.
- View likes - As a site user/ admin I can view the number of likes on each post so that I can see which is most popular.
- View post list - As a site user I can view a list of posts so that I can select one to read.
- View a detail post - As a signed in user I can click on a post so that I can read the full text.
- View comments - As a signed in user I can view comments on an individual post so that I can read the conversation.
- Account registration - As a site user I can register an account so that I can comment and like posts.
- Comment on a post - As a signed in user I can leave a comment on a post so that I can interact with the content.
- Like/unlike - As a signed in user I can like or unlike a post so that I can interact with the content.
- Create a post - As a signed in user I can create a new post so that I can share locations with other users.
- Edit posts - As a signed in user I can edit my posts so that I can update or correct information.
- Delete posts - As a signed in user I can delete my posts so that I can remove them from the website.
- Feedback messages - As a user I get messages back after I perform an action so that I know whether I have completed the action correctly.
- Landing page - As a site user I can go to the landing page so that I can see the purpose of the website.
- Highlight active page - as a site user I can see the active page highlighted so that I know what page I am on.
- Profile - as a logged in user I can view and edit my profile so that I can keep it up to date.


### Agile Development Tool


I am using an agile software development tool in the development of this website.  I am using Github Projects, using a basic Kanban Template.  I added automation so that as each new issue is added, it adds it to the 'To Do' list for my project.  As I start working on each issue I move it to the 'In progress' column.  When the coding for each issue has been completed, the issue is then moved to the 'done' column.

![my kanban board](/documentation/images/kanban_1.png)

![my kanban board](/documentation/images/kanban_2.png)


### Wireframes


I have used Balsamiq to create the following wireframes for both desktop and mobile devices.
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



## Existing Features


### Navbar and Footer


#### Navbar

The navbar is plain and simple so that it is very easy for the user to read.  The name of the website is clear in the top left hand corner - Location Blog. There are links to Home, Posts, Register and Login pages for all users.   If the user is not signed in, the sign in and register links are visible on the navbar. 

![Navbar for not signed in user](/documentation/images/navbar.png)

If the user is signed in, then there is a Logout link visible.  Also if the user is signed in there is a message to say user name to act as an extra visual to the user that they are signed in! There is also a Profile link that the user can go in and view their profile.

![Navbar for signed in user](/documentation/images/navbar_signedin.png)

The page that is being viewed is highlighted in the navbar so that the user can see easily what page they are on.

In mobile view the navbar is collapsed into a hamburger icon, which when clicked shows the same information as in desktop view.

![Mobile Navbar](/documentation/images/hamburger.png)

![Mobile Navbar for not signed in user](/documentation/images/hamburger_not.png)

![Mobile Navbar for signed in user](/documentation/images/hamburger_signed.png)

#### Footer

The footer is very simple with minimal information, just displaying social media options.  When the icons are clicked, they open in a new tab so that the user still has my web site open.

![Footer](/documentation/images/footer.png)


### Register Page


I have used Allauth for register, login and logout.

When a user clicks the register button they are brought to the register page where they have to fill in their username, an email address but this is optional and their password, which they then have to confirm. Then the user can click the button to sign up. If the user has come to register instead of login, there is text to say if you have already an account click login. If the registration is successful the user is redirected back to the home page and a message just below the navbar will appear for 3 seconds to say successfully signed in as 'username'.

![Register](/documentation/images/register.png)

![message to say successfully signed in](/documentation/images/signedin.png)


### Login Page


If a user has already registered they can log into the site in the login page.  The user is asked for their username and password. If correct the user is redirected back to the home page to begin their viewing. A message will appear under the navbar for 3 seconds to say successfully signed in as 'username'.

![Login](/documentation/images/login.png)

![message to say successfully signed in](/documentation/images/signedin.png)


### Logout page


The user is asked are they sure they want to logout and then they can click the sign out button. The user is redirected back to the home page. A message will appear for 3 seconds under the navbar to say you have signed out.

![Logout](/documentation/images/logout.png)

![message to say successfully signed out](/documentation/images/signedout.png)


### Profile Page

When the user has signed in they have an option on the navbar to click Profile link which brings them to their profile page.  I have put security mesures to make sure that the user is logged in and if not they are redirected to the login page.

![Profile page](/documentation/images/profile_view.png)

At the bottom of the profile page the user has the option of returning to the home page or to edit their profile.

### Edit Profile Page

The user has the option of changing their profile image and changing their favourite place. Again there is security to prevent non logged in users gaining access to this page.

![Edit Profile page](/documentation/images/profile_edit.png)

### Home Page


The home page consists of a hero image of a beautiful landscape, with the hero text of Location, Location, Location. Share your favourite places. Find new places. Underneath is a button to redirect to the posts page. I changed the hero image to be a webp format to improve performance loading the page.

![hero image](/documentation/images/hero_image.png)

Under the hero image, there is a short text to tell the user how this website works. 

![home information](/documentation/images/home.png)

If the user is not logged in they can only see the home page and the post list page. A signed in user can also see the post detail page, can like/unlike posts, can leave comments, can create their own post, can edit their own post and delete their own post.
I have added security to prevent non logged in users trying to access these pages through typing the urls.

### Posts Page


This page can be seen by both logged in and unlogged in users.  I wanted the unlogged user to get a look at what the blog offered so that they might then register and login. This page shows the title, location, authors name, date the post was created, image, how many likes and a short excerpt. If the author does not attach an image a stock picture is used.
In mobile view each post is the full width of the screen and the user can scroll down to see the other posts.
 
![mobile posts](/documentation/images/mobile_posts.png)

In desktop there are 6 posts per page, with 3 on the top row and 3 underneath.  If there are more than 6 posts there is a next button to look at the next page of posts and also a previous button to navigate back to the previous pages.

![desk posts](/documentation/images/desk_posts.png)

I have added the alt attribute on images for screen readers to make the site more accessible.
I have also capitalized the title and location so the page looks more uniform as we are relying on user input.

For logged in users only, they can see a view button so that they can view all the detail posts.  I thought about making the image clickable to direct to the detail page but I thought there would be a lot of repetitive code with having to check if the user was logged in too. So I just left it as the view button. For users not logged in the view button is not visible/available to them. 

![able to see the view button](/documentation/images/view.png)

If the user is the author of the post they also have access to an edit and delete button.  The edit and delete buttons are only visible if the user that is signed in is the author of this post.

![able to see the edit & delete button](/documentation/images/all_buttons.png)

After testing and getting feedback I have put a message at the top of the posts page to tell users that have not logged in that they need to log in to read the full detailed post.  I have also included the link to login.  This message is not visible for users that have logged in.

![message to login to see full post](/documentation/images/login_message.png)

I have amended the post to only show the date and not the date and time. I felt the date was enough to display.


### Post Detail Page


This page can only be accessed by logged in users. I have added alt atributes for the images for accessibility.
On mobile view the image is not displayed as it takes up too much room. There is a header banner which includes the title, location, author and date created.  Then under the banner is the content from the post.  Under the content there is a heart icon which acts as a button to allow the user to like or unlike the post.  If the heart is filled in red it means that this user has liked the post.  If the heart was just an outline in red it means this user has not liked this post.  There is logic in place that if a user has liked the post if they then click the heart again it will unlike the post. There is also a number beside the heart to show how many likes this post has. Also there is a comment icon again with a number to show how many comments.
There is a back to posts button so the user can easily navigate back to the posts page.
I have added security to prevent non logged in users accessing the view by typing the url.

![post detail](/documentation/images/title_detail.png)

This user has not liked this post as the heart is just an outline.

![post is unliked by this user](/documentation/images/unliked.png)

This user has liked this post as the heart is filled in with red.

![post is liked by this user](/documentation/images/liked.png)


Under this is the comments section, so it displays any comments that have been left on this post with the commenters name and date they left the comment.  Under this there is a simple form for the user to add a comment and submit it.  If the user clicks the submit button they have to have written something in the form or it gives a warning.  When the submit button is clicked the user is redirected back to the detail post and a message appears for 3 seconds to say thanks for leaving a comment. The comment that the user has just submitted should appear on the page.

![comment detail](/documentation/images/comment_detail.png)

![message to say successfully left comment](/documentation/images/comment.png)

Similar to the post list I have amended the detail post and the comment to only display the date and not the time.


### Create Post


If a signed in user clicks the 'Create Post' on the navbar it brings them to the create post page.  This is a form that the user has to fill in.  They must fill in the title, location and content fields, the image and excerpt are optional. The user will get warning messages if any of the required fields are not filled. If the user does not choose an image to add to their post a stock image will appear on the website.  If they do not put any text in the excerpt field, nothing will display for this field in the post list page.  

![create a post](/documentation/images/create_post.png)

When the user clicks the create button, they will be redirected back to the posts page. A message will appear just under the navbar to say successfully created a post.

![message to say successfully created post](/documentation/images/create.png)

After testing and getting feedback I have put in a brief explanation of the excerpt field - brief description.  This is to help the user in filling in the form.

![explanation of excerpt](/documentation/images/excerpt.png)

I have added security to prevent non logged in users accessing this page by typing the url. If they are not logged in they will be redirected back to the login page.

### Edit Post


If a user clicks the edit button on the posts page, they will be brought to the edit post page.  This is very similar to the create page only this is populated with the information from the post that the user has tried to edit.  The user can then edit some or all of the post and then click the edit button. 

![edit a post](/documentation/images/edit_post.png)

The user will be redirected to the posts page.  A message will appear just under the navbar to say successfully edited the post.

![message to say successfully editted post](/documentation/images/edit.png)

I have added security to prevent non logged in users accessing this page and being able to edit an other persons post.  If a non logged in user tries to access the edit page they will get a forbidden message.

### Delete Post


If a user clicks the delete button on the posts page for a post, they will be directed to the delete post page.  There is a button to 'go back' in case they accidently came here and didn't mean to delete the post. This will bring them back to the posts page. The delete page checks to make sure that the user wants to delete the post - asking them are they sure? The name of the post that is about to be deleted is displayed. 

![delete post](/documentation/images/delete_post.png)

Then if the user clicks delete, the post is deleted and the user is redirected back to the posts page.  A message will appear just under the navbar to say that the post has been successfully deleted.

![message to say successfully deleted post](/documentation/images/delete.png)

I have added security to prevent non logged in users accessing this page by typing the url.  If they are not the author and not logged in they will get a forbidden message.

### Super user/admin


I created a superuser/admin so that they can create, read, update and delete posts so that they can manage the blogs content.  They can remove any post or comment that is not in keeping with the ethos of the site.


## Design



The design is kept simple to let the location posts take centre stage.  Also to make it easy for users to navigate the site.


### Data Model


I needed two data models to make this website work.  The first data model is the Post. This contains the information for the post.  I have a second data model for the comments which are linked to a post. I have added a profile model, with some information about the user. The profile is created when the user registers.

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

#### Profile model

|Key | Name | Type
|---------|----------------|-------------------|
| 1 to 1 | User | User Model
| | Image | Cloudinary_image
| | Favourite_place | Textfield


### Typography


The fonts I have selected are :  Nunito for the text, Roboto for the headings and Cedarville Cursive for the brand.  These have been selected as they are clear and simple.


### Images/color


I have kept the layout and colours simple. I have used a darker shade of blue for the navbar and footer, pulled from the hero image.  I have used a brighter blue to highlight the page that is open on the navbar and have used this color again on the posts page for the author flash.  I have use a slightly differnet blue for the header in the details page.


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

for profile page

![profile page](/documentation/validation/html-validator-profile.png)

for profile edit page

![profile edit page](/documentation/validation/html-validator-profileedit.png)

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


I copied and pasted my python files into the PEP8 validator

for blog>admin.py

![blog.admin.py](/documentation/validation/PEP8-admin-py.png)

for blog>models.py file

![blog.models.py](/documentation/validation/PEP8-models-py.png)

for blog>forms.py file

![blog.forms.py](/documentation/validation/PEP8-forms-py.png)

for blog>urls.py file

![blog.urls.py](/documentation/validation/PEP8-urls-py.png)

for blog>views.py file

![blog.views.py](/documentation/validation/PEP8-views-py.png)

for codeloco>settings.py file

![codeloco.settings.py](/documentation/validation/PEP8-settings-py.png)

for codeloco>urls.py file

![codeloco.urls.py](/documentation/validation/PEP8-codeloco-urls-py.png)

The online pep8 validator was unavailable when I was checking my profile files and the changes I had made to blog>views.py so I ran python3 -m flake8 and fixed errors that showed up. 

## Testing



### Manual Testing


I checked each page (home, signup, login, logout, post, detail, create, edit, delete) to make sure everything looked ok at all screen sizes using devtools.  I also got family and friends to test my site on their different devices.

I am going to use the user stories as my structure for manually testing my project.  This testing was carried out on my development website and the fully deployed site on heruko.

#2 manage posts

- as admin I can create a post

If I do not enter data in the required fields it gives a warning to add data to the required fields.  It is ok not to have data in the excerpt field. It is also ok not to include an image, if an image is not added by the admin/user a stock image will be included.

![showing warnings for required fields](/documentation/testing/admin_add_post_1.png)

When all required fields are filled and the post is saved, we get a success message and can see the new post.

![show success message and new post in list](/documentation/testing/admin_add_post_2.png)

- as admin I can read a post

Check in the website that the new post is there with correct data, including stock image.

![new post visible on website](/documentation/testing/admin_add_post_3.png)

- as admin I can update a post

Similar to create post in update if any of the required fields are not filled a warning is shown and fields that need to be filled are highlighted.

![warnings for update similar to create](/documentation/testing/admin_update_post_1.png)

When all required fields are filled a success message is given and I can see the updated post.

![updated post visible and success message](/documentation/testing/admin_update_post_2.png)

Checked on website to check updated data is there.

![updated post on website](/documentation/testing/admin_update_post_3.png)

- as admin I can delete a post

When the admin selects the post they want to delete, select action - delete and then clicks go, the admin is asked are they sure they want to delete this post. They have the option of going back or deleting the post.

![are you sure you want to delete](/documentation/testing/admin_delete_1.png)

When the post is successfully deleted you get a success message and the post is deleted

![successful delete](/documentation/testing/admin_delete_2.png)

Also I want admin to be able to delete a comment, if a user has put up a comment that needs to be removed.
So similar to the post delete, they select the comment, set action to delete and click go.

![select comment for delete](/documentation/testing/admin_delete_3.png)

Asked if they are sure they want to delete, exactly same as delete post and they just need to confirm. Get a message to say comment successfully deleted.

![successfully deleted comment](/documentation/testing/admin_delete_4.png)

Check on website to ensure that comment has been deleted.

![check comment deleted on website](/documentation/testing/admin_delete_5.png)

#1 pagination

- as a site user I can view a paginated list of posts

By clicking the posts button on the navbar or the call to action button on the hero image I can view a paginated list of posts. On desktop there are 6 posts per page, 3 in the first row and 3 underneath, there is a next button at the bottom of the page to go to the next page.  On the next page there is a back button to return to the first page.
On a mobile device there is one post, the full width of the screen but still 6 posts per page and again the navigation between the pages with next and prev buttons.

![pagination](/documentation/testing/pagination.png)

#3 view likes

- as a site user I can view the number of likes on each post - both logged in and non logged in users can see the number of likes on the post list page.

![view likes on a post](/documentation/testing/view_likes.png)

#4 view post list

- as a logged in user I can view a list of posts so I can select one to view.  Being able to select one to view, the detail view is only available to logged in users, so the view button is not displayed for non logged in users.

![view post list](/documentation/testing/view_post_list.png)

Check that a non logged in user can not see the view button.

![no view button](/documentation/testing/noview_button.png)

#5 open a post

- as a logged in site user I can view the full post

![can view detail](/documentation/testing/view_detail.png)

Check that clicking the back to posts button takes the user back to the posts page - yes

Check to make sure not logged in user cannot access the detail view if they are not logged in. they are redirected to login page - yes

#6 view comments

- as a logged in user I can view comments on posts.  The posts should be in chronological order starting with the earliest comment.

![can view comments](/documentation/testing/view_comments.png)

#7 account registration

- as a site user I can register so that I can comment and like posts.

For register, checks with user if they already have an account and if so they can click login which redirects them to the login page.  

Allauth checks if the username has been used before.

![user already exists](/documentation/testing/user_exists.png)

Checks that a username has been entered.

![user entered](/documentation/testing/must_enter_username.png)

Checks that a password must be entered.

![password entered](/documentation/testing/must_enter_password.png)

Also checks that the password is long enough.

![password short](/documentation/testing/password_short.png)

For login, checks that the user has an account and if not redirects them to register page.

Warning if username not entered.

![username must be entered](/documentation/testing/si_enter_user.png)

Warning if password not entered

![password must be entered](/documentation/testing/si_enter_pass.png)

Warning if the user isn't a registered user

![user must be registered](/documentation/testing/user_not_right.png)

When user logs in properly their username appears in the navbar, as a reminder that they are logged in- yes

For logout, checks that the user wants to log out.

![check logout](/documentation/testing/check_logout.png)

Check when logged out the username does not appear on the navbar - yes

#8 comment on a post

- as a logged in user I can leave a comment on a post.

Check that the user logged in matches the name - posting as.

![check posting is user](/documentation/testing/leave_comment.png)

User must enter something in the comment text field or there is a warning

![must enter comment](/documentation/testing/must_enter_comment.png)

Check that after submitting comment the user gets redirected back to the detail post that they commented on and their new comment should be there.

![check comment is there](/documentation/testing/comment_added.png)

#9 like/unlike

- as a logged in user I can like / unlike posts

If the red heart is an outline the user has not liked this post.

![user not liked post](/documentation/testing/not_liked.png)

If the user clicks on the heart, the user will be redirected back to the detail post they have just liked and the heart should be filled in.

![user liked post](/documentation/testing/liked_post.png)

Also increases the number of likes.  The same user cannot like the same post multiple times.  If they click to like a post they have already liked it will unlike it.

#10 create post

-as a logged in user I can create a post

Create post on the navbar is only visible to logged in users. When the create post button is clicked it takes the user to 'Add a location Post' page.
The user cannot enter an empty form, user gets a warning.

![create post warning](/documentation/testing/create_post_warn.png)

Similar to the admin adding a post, all the required fields need to have something entered or the form will not be entered.  There must be something entered in the title, location and content fields. The user does not have to enter an image, if no image is entered then a stock image is added to the post for display in the website. The user does not have to add something in the excerpt field, in the model I have defined this field as blank=True.

When the create button is clicked, the user should be redirected back to the posts page and their post should be visible.

![check post created](/documentation/testing/post_created.png)

Check that information entered on the create page is correct in the new post - yes

Check that if no image was selected then the stock image is showing - yes

Check if the user selects an image this image is showing - yes

Check that not logged in user can access this page and they are redirected to login page - yes

#11 edit post

- as a logged in user I can edit my own post

The edit button is only available on the post page if the user is the author of the post - yes 

When the edit button is clicked, the user is redirected to the 'Edit Location Post' page - yes

Check that the fields are auto filled with the information from the post that the user wants to edit - yes.
Again, if any field is deleted from a required field a warning is given to the user.

![edit post warning](/documentation/testing/edit_post_warn.png)

When edit is clicked the user should be redirected to the posts page - yes

The post should be visible on the posts page with the fields that were edited changed - yes

![edit check](/documentation/testing/edit_check.png)

If not logged in user tries to access this page via url they are redirected to the login page -yes

#12 delete post

- as a logged in user I can delete my own post.

The delete button should only be visible on a post if the author is the user - yes

When the delete button is clicked, the user is redirected to the 'Delete post' page. - yes

![delete post page](/documentation/testing/delete_post_page.png)

This page checks that the user definitely wants to delete this post. 

The title of the post to be deleted is shown on the delete page - yes

There is a go back button in case the user has made a mistake.  This should bring the user back to the posts page - yes

If the user wants to delete this post they click delete. The user is redirected to the posts page and the post should not be shown - yes

If a not logged in user tries to access the delete page via url they are redirected to login page - yes

#13 feedback messages

- as a user I will get feedback after every action

All messages appear just under the navbar, I have set them to disappear after 3 seconds, the user can also delete the message before the 3 seconds by clicking on the X.

Check the messages delete after 3 seconds - yes

Check that the user can delete the message by clicking the X - yes

When the user registers.

![register message](/documentation/testing/register_mess.png)

When a user logs in.

![login message](/documentation/testing/login_mess.png)

When a user logout.

![logout message](/documentation/testing/logout_mess.png)

When a user creates a post.

![create message](/documentation/testing/create_mess.png)

When a user edits a post.

![edit message](/documentation/testing/edit_mess.png)

When a user deletes a post.

![delete message](/documentation/testing/delete_mess.png)

When a user leaves a comment.

![comment message](/documentation/testing/comment_mess.png)

When a user edits their profile

![profile message](/documentation/testing/profile_message.png)

#14 landing page

- as a user I can see what the website is for from the landing page.

When I open the website on the browser it goes to the landing page or index page - yes

The landing page has a hero image of a beautiful place.

There is a button for users to look at the posts, when this button is clicked the user is redirected to the posts page - yes

Under the hero image is a brief overview of the site.

All the navigation buttons work and redirect to the correct page - yes

#15 highlight active link

- as a user the page that I am looking at is highlighted on the navbar.

When on the home page

![highlight home](/documentation/testing/high_home.png)

When on the posts page

![highlight posts](/documentation/testing/high_posts.png)

When on the register page

![highlight register](/documentation/testing/high_reg.png)

When on the login page

![highlight login](/documentation/testing/high_login.png)

When on the logout page

![highlight logout](/documentation/testing/high_logout.png)

#16 view and edit profile

- as a user I can view and edit my profile

Check that when a user logs in the profile link is visible on the navbar - yes

Check on mobile view too - yes

Check if not logged in user tries to access the profile page they get redirected to the login page - yes

Check that the home button redirects correctly to the home page - yes

Check that the edit profile button brings user to edit profile page - yes

Check that edits to profile page are saved and can be viewed - yes


#17 small changes added through testing

- make footer links work - yes

- only display date not date & time in post list, post detail and comments - yes

- message at top of post list page to tell non logged in user that they have to login to read the full post - yes

- above message does not show for logged in users - yes

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

- not pulling in the image when a user created a post - needed to add enctype='multipart/form-data' to the form.

- some issues with accessibilty, not a big enough contrast between the text and the background. I changed these to have a darker background and white text so that there was a bigger contrast.

- on delete page, when a post was successfully deleted the user was redirected to the home page instead of the posts page - changed the url in the link to point to the post_list.



## Deployment, forking and making a clone



### Deployment to Heroku


Initial deployment:

I followed the 'I think therefore I blog' walkthrough to create a basic django project.  I used the code institute template. 
- I installed django and supporting libraries:
I installed django, gunicorn, psycopg2, cloudinary with pip3 install django gunicorn dj_database_url psycopg2 dj-3-cloudinary-storage
I created the requirements.txt file with pip3 freeze > requirements.txt

- I created a new django project called 'codeloco' and a django app called 'blog'.
django-admin startproject codeloco
python3 manage.py startapp blog
I need to add blog to installed apps in settings.py.
After adding new app we need to migrate the changes to the database.
python3 manage.py migrate

- I set the project to use Cloudinary and PostgreSQL database.
I created a heroku app called codeloco.
I attached it to the database, in resource tab searched for postgres and attached. Then in config vars copy the text beside DATABASE_URL

I created an env.py file - this contains all the secret environmental variables. I need to reference this in settings.py file. Added env.py to the .gitignore file.
In the env.py file import os library.
add os.environ["DATABASE_URL"] = copied string from heroku
add os.environ["SECRET_KEY"] = make up randon key -add this secret key to heroku config vars
I connected to cloudinary and tell django to use cloudinary to store media and static files.
add os.environ["CLOUDINARY_URL"] = "cloudinary://<insert-your-url>" - add this to heroku config vars
in heroku config vars add DISABLE_COLLECTSTATIC with value 1 - this has to be removed before final deployment
I set up for static and media at the bottom of settings.py file.
I needed to tell django where our templates will be stored.
I needed to add heroku host name into allowed hosts in settings.py file.
I needed to create 3 directories at the same level as manage.py file for media, static and templates.
I needed to create a Procfile this tells heroku how to run our project.

- I deployed the empty project to Heroku.
In Heroku in the deploy tab,
I click GitHub,
I search for my repo,
Then scroll down and deploy branch.
I watched the build to check it was successful and
then opened the app.
I have included a env.sample file which is a copy of my env.py file without the secret information.  This is to show what secret keys are required.

When I had completed my testing in development, in the settings.py file I set DEBUG = False and added X_FRAME_OPTION = 'SAMEORIGIN'.
I git add ., then git commit and git push.
In Heroku I went into config vars and deleted the DISABLE_COLLECTSTATIC = 1
In the deploy tab in Heroku, I deployed branch and watched the build to check it was successful. Then I opened the app and repeated all my testing to ensure this worked the same as my local testing.


### Forking the GitHub Repository


By forking the GitHub Repository you will be able to make a copy of the original repository on your own GitHub account allowing you to view and/or make changes without affecting the original repository by using the following steps:

- Log in to GitHub and locate the GitHub Repository.
- At the top of the Repository (not top of page) just above the "Settings" button on the menu, locate the "Fork" button.
- You should now have a copy of the original repository in your GitHub account.


### Making a local clone


- Log in to GitHub and locate the GitHub Repository.
- Under the repository name, click "Clone or download".
- To clone the repository using HTTPS, under "Clone with HTTPS", copy the link.
- Open commandline interface on your computer.
- Change the current working directory to the location where you want the cloned directory to be made.
- Type git clone, and then paste the URL you copied above.
- Press Enter. Your local clone will be created.


## Credits



- I used 'I think therefore I blog' to set up files, Heroku app, Cloudinary, environmental variables and GitHub Projects.
- I used GitHub Projects and Kanban for user stories like 'I think therefore I blog'
- I used 'tails on trails' to help set out what I wanted for my project
- I got help with navigation from 'Tails on Trails'.
- I used card system from 'I think therefore I blog' for displaying posts.
- Ciara O'sullivan on slack for solving my slug problem when user creating post didn't create the slug field.
- I used the messages from 'I think therefore I blog'
- To help with crud functionality I used Dennis Ivy Youtube video for to do list app.
- Class based views was explained well by Dennis Ivy.
- I got help for showing active page on navbar from 'Favoureats' by Siobhan Gorman.
- I got my hero image from thetimes.co.uk.
- I found the solution to my too long lines in settings.py in code.djangoproject.com/ticket/28163.
- I followed structure of readme from JoGorska_alumni_lead.
- I used bootstrap links from 'I think therefore I blog'.
- I used 'I think therefore I blog' for the bases of my footer.
- I used the stock picture from wallpapersafari.com.
- I got the post pictures from - destimap.com, alany.com, istockphoto, coldwellbankercork.ie, discoverireland.ie, dreamtime.com, facebook.com, oceandivers.com, cork-guide.ie, eoceanic.com and mountainviews.ie


## Acknowledgements



- I would not have completed this project without the support and understanding of my family.
- Wonderful help and support from my cohort and facilitator Kasia.
- Help and support from my mentor Celestine Okoro.