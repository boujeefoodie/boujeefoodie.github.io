# Table of Contents
* [About Boujee Foodie](#about-boujee-foodie)
  * [Approach](#approach)
  * [Use Case Ideas](#use-case-ideas)
  * [Beyond the Basics](#beyond-the-basics)
* [Installation](#installation)
* [Application Design](#application-design)
  * [Directory structure](#directory-structure)
* [Development History](#development-history)
  * [Milestone 1: Mockup development](#milestone-1-mockup-development)
* [Contact Us](#contact-us)

# About Boujee Foodie
The problem: There are many food choices on campus: campus center, food trucks, Manoa Gardens, Paradise Palms, vending machines, and so forth. Let’s say you have a desire for chinese food today for lunch. What places on campus are serving chinese food menu items today? Alternatively, let’s say that you love the fresh salmon fillet at Campus Center, but that dish is only served once every few weeks. How do you find out on the day that it’s available?

The solution: The Boujee Foodie app enables you to login on your phone and determine:
  * What specific menu items will be available today at campus center locations;
  * What food is available right now.
  * When a style of food you love is available today.

Links:

Galaxy App: [http://boujeefoodie.meteorapp.com/#/](http://boujeefoodie.meteorapp.com/#/)

GitHub Repo Page: [https://github.com/boujeefoodie](https://github.com/boujeefoodie)

GitHub Project Management Page: [https://github.com/boujeefoodie/boujeefoodie/projects](https://github.com/boujeefoodie/boujeefoodie/projects)

# Guided Tour

Boujee Foodie Portal is deployed via Galaxy with this link: [http://boujeefoodie.meteorapp.com/#/](http://boujeefoodie.meteorapp.com/#/)

After clicking the link, you will be in the landing page which is show below

- boujee foodie landing page

You will need to create an account. You can do this by clicking the login at the top right corner and then clicking sign up.

![](images/signup.png)

Please enter a valid email and password.

Once logged in you will be greeted with the landing page again, but with more options in the top menu.

- Landing Page User Image

As a user, you will have the option of viewing the restaurants that are available around UH.

You will be able to see the name, address, images, description and price range of each restaurants in this page.

![](images/ListRestaurant.png	)

If you are an Admin User, your navigation bar will have more functions than a regular user

- Landing Page Admin Image

Admins have an option to add restaurant to website. Admins will have to input the restaurants name, description, an link to the restaurants image, a description about the restaurant and the price range in the indicated by amount '$' out of three being one being the cheapest and 3 being expensive.

![](images/AddRestaurantAdmin.png)

Admins also have the power to edit the restaurant page in case restaurants change their hours.

![](images/ListRestaurantAdmin.png)


# Installation

First, [install Meteor](https://www.meteor.com/install).

Second, [download a copy of Boujee Foodie](https://github.com/boujeefoodie/boujeefoodie/archive/master.zip), or clone it using git.
  
Third, cd into the app/ directory and install libraries with:

```
$ meteor npm install
```

Fourth, run the system with:

```
$ meteor npm run start
```

If all goes well, the application will appear at [http://localhost:3000](http://localhost:3000).

# Application Design

## Directory structure

The top-level directory structure contains:

```
app/        # holds the Meteor application sources
config/     # holds configuration files, such as settings.development.json
.gitignore  # don't commit IntelliJ project files, node_modules, and settings.production.json
```

This structure separates configuration files (such as the settings files) in the config/ directory from the actual Meteor application in the app/ directory.

The app/ directory has this top-level structure:

```
client/
  lib/           # holds Semantic UI files.
  head.html      # the <head>
  main.js        # import all the client-side html and js files. 

imports/
  api/           # Define collection processing code (client + server side)
    base/
    interest/
    profile/
  startup/       # Define code to run when system starts up (client-only, server-only)
    client/        
    server/        
  ui/
    components/  # templates that appear inside a page template.
    layouts/     # Layouts contain common elements to all pages (i.e. menubar and footer)
    pages/       # Pages are navigated to by FlowRouter routes.
    stylesheets/ # CSS customizations, if any.

node_modules/    # managed by Meteor

private/
  database/      # holds the JSON file used to initialize the database on startup.

public/          
  images/        # holds static images for landing page and predefined sample users.
  
server/
   main.js       # import all the server-side js files.
```

# Development History

## [Milestone 1](https://github.com/boujeefoodie/boujeefoodie/projects/1): Mockup development

This milestone started on the 5th of April 2019 to 11th of April 2019

The goal of Milestone 1 was to create a set of HTML pages to provide a mockup for the pages that will be in our application. This mockup was developed as a Meteor app. We then later deployed this mockups into Galaxy.

* Deployment of Application in [Galaxy](http://boujeefoodie.meteorapp.com/#/)

Mockups for the following pages were implement during M1:

Home Page:

![](images/homepage.png)

Sign In:

![](images/SignIn.jpg)

Landing Page:

![](images/LandingPage.jpg)

List Restaurants:

![](images/ListRestaurant.png)


## [Milestone 2](https://github.com/boujeefoodie/boujeefoodie/projects/2)

Our goal for Milestone 2 was to add functionality to the Mockups that were created in Milestone 1. We also added an admin in order to keep the website organized.

Updated Home/Landing Page:

Add Restaurant:

![](images/AddRestaurantAdmin.png)

Edit Housing:

![](images/EditRestaurant.png)

Add Review:




Add Review: 
# Contact Us

Jetro Butac: jetro@hawaii.edu

Ryan Li: ryanli80@hawaii.edu

Kevin Liu: liukevin@hawaii.edu

Jonathan Tu: jltu@hawaii.edu
