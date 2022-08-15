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
- control users posts and comments for inappropriate use of the site. I have decided not to put in approval by superuser for adding posts and adding comments but instead put terms and conditions of use by the user ****

### Agile Development Tool


I am using an agile software development tool in the development of this website.  I am using Github projects, using a basic Kanban template.  I added automation so that as each new issue is added it adds it to the 'To Do' list for my project.  As I start working on each issue I move it to the 'In progress' column.  When the coding for each issues has been completed, the issue is then moved to the 'done' column.

#### User Stories


I have the following user stories:
 
- Manage posts - As a site admin I can create, read, update and delete posts so that I can manage the blog content.
- Pagination - As a site user I can view a paginated list of posts so that I can easily selecta post to view.
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



### Features


#### all Pages


##### Navbar

- Links to Home, **post list, register and sign in/out pages. The home and post list pages are visible to and can be accessed by any user.  If the user is not signed in, the sign in and register links are visible on the navbar. If the user is signed in then there is a sign out link visible.  Also if the user is signed in there is a message to say user name is currently signed in, to act as an extra visual to the user that they are signed in!
Navbar for not signed in user

Navbar for signed in user

- the navbar collapes for mobile views

##### Footer
- clear links for the user to go to facebook, twitter, instagram and youtube.

##### Home Page
##### Post list
##### Post detail
##### Sign In form
##### Register Page
##### sign out page
##### Create Post
##### Edit Post
##### Delete Post

### Wireframes
- home page
- Post list
- Post Detail
- sign in page
- register page
- create post page
- edit post page
- delete post page
- sign out page



## Data Model

There are two models for the database: a post model and a comment model

### Location post model

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

### Comment model

| Key | Name | Type
|--------|----------------|-------------------|
|foreign key | post | Post Model
| | name | Char(80)
| | body | TextField
| | created_on | DateTime


## Design

The design is kept simple to let the location posts take centre stage.  Also to make it easy for users to navigate the site.

### Typography

the fonts selected are : *** for the text and *** for the headings.  These have been selected as they are clear and simple.

### Images

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
- Github
- Cloudinary used to host static files
- Gunicorn as the server for Heroku
- Heroku used for cloud based deployment
- Summernote as editor
- Heroku Postgres for production database
- SqLite for local environment database
- Balsamiq for the wireframes


## Testing
### Code Validation
#### Html validation
#### CSS Validation
#### PEP8 Validation
#### Lighthouse
Validator checks HTML, CSS, Python
URL validator???

### Manual testing

#### Responsiveness 
Check each page looks good and is easily navigated at all screen sizes.

#### Testing user stories



## Deployment

Initial deployment
I followed the 'I think therefore I blog' walkthrough to create a basic django project.  I used the code institute template. 
- I installed django and supporting libraries
- I created a new django project called 'codeloco' and a django app called 'blog'
- I set the project to use Cloudinary and PostgreSQL
- I deployed the empty project to heroku

## super user

I created a superuser so that they can create, read, update and delete posts so that they can manage the blogs content.

## Credits

- I used 'I think therefore I blog' to set up files, heroku app, cloudinary, environmental variables and github projects
- I used 'tails on trails' to help set out what I wanted for my project
- I used card system from I think therefore I blog for displaying posts
- Ciara O'sullivan on slack for solving my slug problem when user creating post
- messages from i think therefore I blog
- crud functionality from Dennis Ivy you tube video for to do list app
- class based views explained well by dennis Ivy
## Acknowledgements
- I would not have completed this project without the support and understanding of my family.
- Wonderful help and support of my cohort and facilitator Kasia.
- Help and support from my mentor Celestine Okoro.

