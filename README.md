# MILESTONE PROJECT 4: GAME GEEK
## NAME:  JAKE HARBOUR

## INTRODUCTION:

This project, Game Geek, is an e-commerce site selling games and game related products.
I got involved utilising the Django framework, which was new to me but very useful. 
I also used many other technologies that I have developed my skills in through other projects.

## UX

### AIMS:

The main aims of the project are as follows...

1)  To allow the user to register and create their own user profile
2)  To allow the user to buy gaming related products
3)  To allow the user to buy new game releases
4)  To allow users to buy gaming related clothes in their preferred size

The website should also be responsive so that it works across all devices and media sizes.  
It should be intuitive and easy for the user to use.

### USER STORIES:

To demonstrate the purpose of the website and the various ways it can/should be used 
I have created several user stories seen below...

Story 1:  As a gamer, I would like to shop for games on a console of my choice

Story 2: As a gamer, I would like to buy a new console to console exclusive games

Story 3:  As a new gamer, I would like to sort through the highest rated games to see what's popular

Story 4:  As a gamer, I would like to have a profile so that I can see my past orders

Story 5:  As a gamer, I would like to search for deals so that I can buy games cheaper than I can elsewhere

I believe that Game Geek delivers on all of these user stories and possesses the qualities that
gamers, beginner and experienced, will appreciate and find very useful.
### WIREFRAMES:

The wireframes (found in the wireframes folder) provide a good early 
indication of how I wanted the main pages of the site to look and feel.
Any changes in the final version submitted were done to either optimise responsiveness,
make the site more easily digestable or for aesthetic reasons. 

After consideration of names, approach and colour schemes I decided to make
game related decisions. For example, I chose a black, blue and red colour scheme,
as these are the colour most associated with the Mario Games which are universally recognised.
As a gamer myself I made these decisions so that the user can easily be enticed at a first glance.

My website will is divided into 5 apps, profile, products, home, bag, and checkout.

## FEATURES

### EXISTING FEATURES:

Feature 1: Admin is able to edit products by clicking on the edit button on either the products page
or the product detail page, taking them to a form to edit any one of the product details.

Feature 2: Admin able to deleta product by clicking on the delete button on either the 
products page or product detail page.

Feature 3: User is able to browse products and click on a specified product that takes them to 
the product detail page, finding out more about the product.

Feature 4: User is able to sort products by rating, a-z and z-a.

Feature 5: User is able to sort products by price lowest-highest and highest-lowest.

Feature 6: User is able to sort products by name of products, a-z and z-a.

Feature 7: User is able to sort products by category, a-z and z-a.

Feature 8: User is able to search through all products using the search bar,
keywords can match either name of products or words in the description of the product.

Feature 9: User profile allows users to save their personal billing/delivery information, 
making it so the checkout form will be pre-filled with their personal information.

Feature 10: User profile allows user to view previous orders, making it so you can see products bought.

Feature 11: User is sent an email after they have made an order so that they can view all order information there.


### FUTURE FEATURES:

Future Feature 1: Featured products - An extra page where users can view recently added and 
current trending games/games-related products.

Future Feature 2: Profile Customisation - User is able to customise their profile page including an avatar, page theme
and personal favourite games/genres so that they can be recommended products.

Future Feature 3: Game trailers/images - An extra field in the product detail page where the user can view images or videos of
gameplay or the specified game trailer. This will give the user extra information about the games and possibly improve sales.

## TECHNOLOGIES USED:

#### 1:  NAME - JQuery

LINK - https://jquery.com/

REASON - Jquery helps to streamline using JavaScript, especially when changes are happening 
on screen and also creates less code and easier readability.

#### 2: NAME - Google Fonts

LINK - https://fonts.google.com/

REASON - Used for the font of the website which is 'Rubik'.

#### 3: NAME - Font Awesome

LINK - https://fontawesome.com/

REASON - Font awesome has been used to make the website easier to navigate
and more visually appealing.

#### 7: NAME - Stripe

Link - https://stripe.com/gb/

Stripe was used to create payments when users make an order.

#### 8: NAME - Django 

Link - https://www.djangoproject.com/

Django is the framework I have used to create my site.  By using a combination
of views, urls, forms and models, the site is very easy to work on and has 
many built in features as standard that makes the whole process of building the 
site better and faster.

#### 9: NAME - Amazon Web Services 

I am using an AWS S3 bucket to store all static and user generated media files.

## WEBSITE TESTING:

Test 1: All links have been tested on all devices using Google Chrome developer tools.

Test 2: Payments were tested by going to the webhooks section in stripe and checking to see if
it succeeded, this was done several times to ensure it is consistently working.

Test 3: Changes to the website including pricing and products was tested by adding different items
in different combinations.

Test 4: Responsiveness was tested by viewing each page in all devices on Google Chrome developer tools
to ensure css is responding correctly and is readable enough.

## DEPLOYMENT:

I deployed my code using heroku which makes deployment very easy.

In order to do this I created a new app on the heroku site and linked to the app via the vscode terminal.  

I created a Procfile and requirements.txt file which I then pushed to heroku with the main files.  
These tell heroku that this is a web application and what tools in needs to load for the app to run correctly.

All commits have been made to the same master git branch.  

A number of config vars are required as follows...

HOSTNAME - The web address of the site - django uses this as a security measure 
to ensure the page is authorised to be accessed

DATABASE_URL - This is the address of the production postgres database, mine is 
a heroku addon postgres database

AWS_ACCESS_KEY_ID & AWS_SECRET_ACCESS_KEY - As my static and media files are set up to 
be held in an S3 bucket, both of these are required.

DISABLE_COLLECTSTATIC - This should be set to 1 to prevent any static and media files
being uploaded to heroku on each git push as they are hosted on AWS

EMAIL_ADDRESS & EMAIL_PASSWORD - As emails are sent via the site, a gmail address
and password is required with less secure apps access

SECRET_KEY - This is the key that django uses to verify the site

STRIPE_PUBLISHABLE_KEY & STRIPE_SECRET_KEY - These are required by stripe for a
user to make payments via checkout.html

## CREDITS:

Content - 

- Descriptions for the products were taken from their respective wikipedia articles or
if they did not have one then they were created originally.

- I used Carlo_alumni's README as a template for my own
so I would like to give credit and thank them for that.

- I followed the boutique ado project walkthorugh from the Code Institute
software development program to create my project, a lot of the code and some of the css
is from that project walkthrough.

Media - 

- All images have a URL that I have included in the product details
that link to the original image address with exception to the home background image,
here is the link for that https://wallpaperaccess.com/full/1896712.jpg

## AREAS FOR IMPROVEMENT:

I did not have a lot of available time to create this project so given more time to create 
a more fleshed out website, these are the things I would focus on the most:

1) Testing - In the future I would like to do more in-depth testing, I would like to dip into
a few different testing sites and extensions and generally find best practise for testing.

2) Styling - I am proud of the look of my website and styling choices, but in the future will
develop it further so that there is more use of the colour scheme, and to make the website flow 
a little better content-wise.

3) Content - As I had to manually input products, I did not have time to add too many products as it its very time consuming
and wanted to focus on the core functionality and styling, therefore there currently is quite a lack of available products.
In the future I would like to set up a method that makes adding products much more streamlined.


I enjoyed making this website and am proud of it, I hope you can enjoy it too!