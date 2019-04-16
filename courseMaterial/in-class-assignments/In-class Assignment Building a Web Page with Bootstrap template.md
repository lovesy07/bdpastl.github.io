# In-class Assignment: Building a Web Page with Bootstrap Template

####Overview

This exercise will require students to work in teams of 4-5 student in order to build a web page from a Bootstrap template. This document will provide step by step instructions as well as links to helpful resources. As always, classroom instructors will be available to provide assistence and answer questions.

#### Learning Objectives

* Learn about Bootstrap templates
* Increase familiarity with Bootstrap
* Learn how to collaborate with team members

#### Helpful links

* [Bootstrap Cheatsheet (short)](http://creativealive.com/wp-content/uploads/2014/01/bootstrap3-cheatsheet.pdf)

* [Bootstrap Cheatsheet (long)](https://bootstrapcreative.com/resources/bootstrap-3-css-classes-index/)
* [Bootstrap Icons Cheatsheet](https://glyphicons.bootstrapcheatsheets.com/)
* [Free website backgrounds](https://unsplash.com/collections/491836/website-backgrounds)

#### Instructions

######Getting Started

1. __Download the Gaia Bootstrap Template__: Todays assignment will leverage a bootstrap template. [Click here](https://www.creative-tim.com/product/gaia-bootstrap-template#) to navigate to the site where you can download the Gaia template.  After the download is complete, unzip it. This will result in a folder called `gaia-bootstrap-template-master`. Move this folder into your `Projects` folder.
2. __Open the template in VS Code__: In VS Code, click `File` then `Open...`. This should open a window for navigating through the folders and file on your computer. Find the folder called `gaia-bootstrap-template-master` and select it. Then click `Open`.
3. __Explore the contents of your new project__: VS Code has a file explorer for navigating your project in the left panel. Take a few moments to explore the contents of the project. At the top level, you will notice a folder called `assets` and three files titled `freebie.html`, `LICENCE.md`, and `README.md`. The `assets` folder contains all of the necessary css, js, fonts, and images for your project. Rename `freebie.html` to `index.html` by right clicking on it and then clicking `Rename`. The `index.html` file is where we will be doing most of our work today.
4. __Preview your web page locally in your web browser__: In the VS Code file explorer, right click on `index.html` and then click `Copy Path`. Open up a web browser, paste what you just copied into the address bar, and then hit `Enter`. You should now see your web page in the default state as provided by the Gaia template. Go back to VS Code. In `index.html` , line 77 and replace the word `Gaia` with your team name. Then save your project, navigate back to your web browser, and refresh the page. You should see that the page has changed and includes your team name.

###### Build

1. __Change the title__: Go to line 10 of `index.html`. Replace the contents within the `<title>` element with whatever you want the title of your page. What do you think will be the result of this?

2. __Change the background image__: You may want to change the background of your web page. Start by going to lines 70-72. The code should look like this: 

   ```html
   <div class="image"
      style="background-image: url('assets/img/header-1.jpeg')">
   </div>`
   ```
   Notice that there is a string that says `'assets/img/header-1.jpeg'`. If you recall there is a folder called `assets` in the project. If you open the `assets` folder in the VS Code file explorer, you will see a folder called `img`. If you open the `img` folder, you will find a file called `header-1.jpeg`. This is the file that contains the background image for your web page. Using [this link](https://unsplash.com/collections/491836/website-backgrounds), find an alternative background and download its file. Then place the downloaded file in the `assets/img/` folder. Lastly, modify lines 70-72 so that they refer to the new image file.

3. __Be Creative__: Transform this website in any way that you'd like. Have fun and be creative.

###### Deploy (optional)

Host your new website on Github.io

