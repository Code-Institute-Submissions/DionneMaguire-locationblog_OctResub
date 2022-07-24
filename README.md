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

### User Stories

I am using an agile software development tool in the development of this website.  I am using Github projects, using basic Kanban template.  I added automation so that as each new issue is added it adds it to the 'To Do' list for my project.  As I start working on each issue I move it to the 'In progress' column.  When the coding for each issues has been completed, the issue is then moved to the 'done' column.


## Features

- Responsiveness




## Data Model

### Location post

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

### Comment Post

| Key | Name | Type
|--------|----------------|-------------------|
|foreign key | post | Post Model
| | name | Char(80)
| | body | TextField
| | created_on | DateTime

## technologies used

### languages

- HTML
- CSS
- Python

### frameworks, libraries & programs

- Django
- Bootstrap
- Google Fonts
- Font Awesome
- Github
- Cloudinary
- Heroku


### testing

Validator checks HTML, CSS, Python
URL validator???


## deployment

Initial deployment
I followed the 'I think therefore I blog' walkthrough to create a basic django project.  I used the code institute template. 
- I installed django and supporting libraries
- I created a new django project called 'codeloco' and a django app called 'blog'
- I set the project to use Cloudinary and PostgreSQL
- I deployed the empty project to heroku


