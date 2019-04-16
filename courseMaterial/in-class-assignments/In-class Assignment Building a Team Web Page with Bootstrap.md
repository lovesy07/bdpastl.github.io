# In-class Assignment: Build a Team Web Page with Bootstrap

####Overview

This exercise will require students to work in teams of 4-5 student in order to build a team web page. This document will provide step by step instructions as well as links to helpful resources. As always, classroom instructors will be available to provide assistence and answer questions.

#### Learning Objectives

* Increase familiarity with html and css
* Learn how to build a project in VS Code
* Increase familiarity with Bootstrap
* Learn how to collaborate with team members

#### Helpful links

* [Bootstrap Cheatsheet (short)](http://creativealive.com/wp-content/uploads/2014/01/bootstrap3-cheatsheet.pdf)

* [Bootstrap Cheatsheet (long)](https://bootstrapcreative.com/resources/bootstrap-3-css-classes-index/)
* [Bootstrap Icons Cheatsheet](https://glyphicons.bootstrapcheatsheets.com/)
* [Free website backgrounds](https://unsplash.com/collections/491836/website-backgrounds)

#### Instructions

######Getting Started

1. __Create a Projects Folder__: Create a folder on your computer called `Projects`. You will use this folder for this assignment as well as assignments in the future. If you already have a `Projects` folder, ignore this step and use that folder for today's assignment.

2. __Create Your Project Folder and index.html__: Inside your `Projects` folder create a new folder and call it `my-team-site`. Within the `my-team-site` folder create a file and name it `index.html`.

3. __Open the template in VS Code__: Start by opening VS Code. Next click `File` then `Open...`. This should open a window for navigating through the folders and files on your computer. Find the folder called `my-team-site` and select it. Then click `Open`. VS Code has a built in file explorer on the left hand side. At the moment `index.html` is the only file in this project. Double click on it to open the file.

4. __Add Bootstrap to index.html__: Add the following code to `index.html`:

   ```html
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <meta charset="utf-8" />
       <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
   
       <!-- Latest compiled and minified CSS -->
       <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
   
       <!-- Optional theme -->
       <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">
   
       <title>My Team Site</title>
       <meta content='width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0' name='viewport' />
     </head>
     <body id="my-page">
       <h1>
         Hello World!!!
       </h1>
     </body>
   
     <!-- Latest compiled and minified JavaScript -->
   	<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
     <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
   </html>
   ```

5. __Preview Your Site in the Browser__: In the VS Code file explorer, right click on `index.html` and then click `Copy Path`. Open up a web browser, paste what you just copied into the address bar, and then hit `Enter`. This should take you to your team web page and words __Hello World!!!__ should be displayed in your browser. At any point going forward, you should be able to see saved changes to your project in the browser by simply clicking the refresh button or using the `ctrl-R` keyboard shortcut.

###### Build

1. __Navbar__: At the top of the `body` html element in `index.html`, create a `div` element with the classes `navbar`,`navbar-default` and `navbar-fixed-top`. Within this `div` element, create another `div` element  with the class `container`. Within this `div` element, create another `div` element with class `navbar-header`. Within this `div` element add the following code:

   ```html
   <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar-collapse" aria-expanded="false">
     <span class="sr-only">Toggle navigation</span>
     <span class="icon-bar"></span>
     <span class="icon-bar"></span>
     <span class="icon-bar"></span>
   </button>
   <a class="navbar-brand" href="#my-page">Your Team Name Here</a>
   ```

   

   Replace `Your Team Name Here` with your team's name.  You now have a navbar. We will return to it later in this assignment when we have content to navigate to.

2. __Jumbotron__: Under your navbar add a new `div` element with the classes `jumbotron` and `Jumbotron-fluid`. Within this `div` add an `h1` element followed by an `h2` element, each with the class `text-center`. In the `h1` element put your team name as its content. In the `h2` put a team slogan or catchphrase.

3. __Background Image__: Although we have styling provided to us by bootstrap, we can still add our own stylesheets. Start by creating a folder within your project called `assets`. Within the assets folder, create two folders called `css` and `img`. Now we need to find an image online. [CLick Here](https://unsplash.com/collections/491836/website-backgrounds) to find free background images. Download the image of your choice and move it into the `img` folder that you just created in your project. Then rename the file to `my-background.jpg`. Now create a new file in the css folder called `my-site.css` and add the following code to that file:

   ```
   .jumbotron {
     height: 100vh;
     width: 100%;
     background-image: url("../img/my-background.jpg");
     background-size: cover;
     color: white;
     display: flex;
     flex-direction: column;
     justify-content: center;
   }
   ```

   Now go ahead and test it out in your browser. You'll notice that nothing has changed. This is because we aren't using the style sheet that you just created. You can do this by adding the following code to line 12 of index.html:

   ```html
   <link rel="stylesheet" href="./assets/css/my-site.css">
   ```

   Now test your code again by refreshing your web browser.

4. __Goodbye World__: The Hello World code that we put in at the beginning is no longer necessary. Remove the following lines of code:

   ```html
   <h1>
     Hello World!!!
   </h1>
   ```

5. __About Section__: Lets add an about section to the team site to tell our fans a little about our team. To do this we will need to create a new `div` element with an id of `about` and a class called `section`. Within this `div` element, create another `div` element with classes `container` and `container-fluid`. Within this `div` create another `div` element with the class `row`. Within this div we will now be able to utilize all of the `col` classes in Bootstrap. Add content here as the team sees fit. The only requirements are the Bootstrap grid system must be used and there must be text and an image.

6. __Our Team Section__: The final section is meant to showcase the individual team members. The html structure should be very similar to the about section. However, instead of having a `div` with an id of `about`, the id should be `our-team`. Like the previous section, it should utilize the bootstrap grid system.

7. __Navbar part II__: Inside of the html for the navbar there exists a `div` with a class of `container`. This `div` has one child at the moment. Add the following code as a second child component:

   ```html
   <div class="collapse navbar-collapse" id="navbar-collapse">
     <ul class="nav navbar-nav navbar-right">
       <li>
         <a role="button" href="#about">About</a>
       </li>
       <li>
         <a role="button" href="#our-team">Our Team</a>
       </li>
     </ul>
   </div>
   ```

   Refresh your browser and you will see that your navbar now has two new buttons. Clicking these buttons should navigate you to the correspondingpart of the page.

8. __Extra Styling__: Review your website and modify `my-site.css` to make it look the way you want .

   

###### Deploy (optional)

Host your new website on Github.io