Project: HTML/CSS
===

For this mini-project, you'll deconstruct an existing web page and rebuild it. Don't worry if the links don't go anywhere and the search box doesn't do anything when you submit it. The goal is to start thinking about how elements get placed on the page and roughly how they get styled and aligned. For some of you, this may be the first time you've actually tried to "build" something in HTML (very exciting!).

Using the browser's developer tools (right clicking something on the page and clicking "inspect element" will get you there) will be your best friend. Build the page in a .html text file and open it in your browser to check it out (or try using CodePen or jsfiddle.net).

Try These Before Starting
---

These skills will be helpful for you when you start building. Either try them yourself or at least make sure you know how to do it:

+ Two ways to move a div around on the page
+ Stick a div onto the bottom or top of the page
+ Identify the background color of an existing webpage
+ Grab the URL for an image from an existing webpage
+ Center an element horizontally
+ Identify three ways you can include your CSS styles in a page
+ Understand how to use classes and ids to target CSS at specific elements on the page
+ Build a very basic form (even if it doesn't "go" anywhere)
+ Setting Up Your Project's Github Repository

As mentioned in the introduction to git, you'll want to organize all your projects like a portfolio and link them to GitHub so it can be seen by others.

+ Create a new repo for this project on GitHub.com.
+ Then move that repository on to your local machine. The command should look like: git clone https://github.com/YourUserName/YourRepoName    
+ Now cd into the project directory that is now on your local machine; setup your README.md file and write a brief introduction for what the current project is and what skills you have demonstrated once you have completed it. (You can do this as a self-reflection at the end of the project which is a good way to revise what you have learned.)

When you're building your project, you will probably end up doing several git add + git commit cycles before being ready to push it up to Github with git push origin master.

If you have entered git push origin master and typed out your username and password, if you refresh your GitHub page, you should see new files added onto GitHub.

Okay, that's enough Git for the moment -- time to actually build stuff!

Easy Version: Build the Google.com homepage
----
(the simple one with just a search box).

Inside your project folder, create your index.html file

1. Tips:
 +  DONT BE A PERFECTIONIST! You're just trying to make it look like google.com, not actually function like it and it doesn't have to be spaced exactly the same way to the pixel. Any dropdown menus or form submissions or hover-highlighting should be ignored.
 + USE GOOGLE! You'll probably run into roadblocks where you can't figure out how to do something so do what all good devs do... Google it!
 +  If you're frustrated with trying to get buttons or inputs to style the way you want (for instance, they seem to just not respond to any styles), look into the css property -webkit-appearance: none; or -moz-appearance if you're using Firefox.
2. Start with just putting the main elements on the page (the logo image and search form), then get them placed horizontally. You can either download the Google logo or link directly to its URL on the web in your <img> tag.
3. Next do the navbar across the top, first building the content and then trying to position it. [Check out how to build a horizontal CSS navbar](https://www.w3schools.com/css/css_navbar.asp) if you're lost.
+ Finally, put in the footer, which should be very similar to the top navbar.
+ In general, do as much on your own as you can before relying on the developer tools (or viewing the page's source code) to help you along.
+ Push your project to Github using the instructions above!
4. Challenge: rebuild the page using Bootstrap!

Difficult Version (optional): Build the Google.com search results page
---

You should be able to reuse much of your code from before if you started with that project. Again, don't worry about links to nowhere and forms that won't submit and hard coding the search results (which you'll have to do of course), just focus on placement and order of items on the page.

Note: All the classes and id's and names of elements that you inspect on Google's home page are nonsensical strings (like <div class='srg'>). This is because the code was **Minified** ([see the Wikipedia entry here](https://en.wikipedia.org/wiki/Minification_(programming))), which removes or shortens unnecessary characters and names to help the page load faster. The HTML (or Javascript or CSS) file will be smaller but the browser can still read it just fine.

> You can obviously do any website you like, it doesn't actually have to be Google. 

Viewing your project on the web
------
If you want to show your work (the project) to others, or submit a solution below, you will need to publish your site so that others can access it from the web, rather than just on your local machine. The good news is that if you have your project on github (as described above) doing this is incredibly simple. 


### Use github-pages

Github allows you to publish web projects directly from a github repository. Doing this will allow you to access your project from your-gh-username.github.io/your-github-repo-name

There are a couple of ways to go about doing this, but the simplest is this:

+ make sure that the main html file of your project is called index.html. If it is not, you will need to rename it.
+ go to your github repo on the web and click the Settings button
+ scroll down until you find the GitHub Pages section
+ change the Source from none to master branch and click Save.
+ it may take a few minutes (the GitHub website says up to 10) but your project should be accessible over the web from your-gh-username.github.io/your-github-repo-name (obviously substituting your own details in the link).

Project DOM
===

Now that you have your flashy Google or Apple web site clone, it's time to add some functionality to it.

Once you have a solid enough grasp of DOM manipulation, try the following challenges:

+ clicking anywhere on the background, should change the background image or color
+ hovering over the main title should change its size
+ for every link: clicking should trigger an alert stating that you clicked that link
+ try to submit a form. By default the submission is send to the back-end, but in this case you'll need to "hijack" the submission somehow.
+ have a div ( or another block element) dissapear and reappear by clicking a button/hovering over it
  + challenge: add an animation (like fade)
+ challenge: by using only JS clicking on the search button (or whatever is equilavent on the Apple page) should empty the home page and display a page with search results (hard coded).
+ challenge: create a user login form. When a user logs in, his/her/its name should be displayed somewhere in the navbar + the option to log out. The user's login info should somehow be saved in the browser, even after refreshing the page! (hint: look into HTML5 local storage...). Similarly, when a user logs out, the user's login info should be deleted and the navbar should have the option to log in.
+ Challenge: you could use HTML5 GeoLocation to display your current location. This will return geographical coordinates. If you want an even bigger challenge, you could include the Google Maps API to have your current address displaye in human readible form.
+ Challenge: try to make a "real" Google search. The submit form should take everyting you've put in the input and redirect it to the real google search.  
  + Even more challengy: use ajax to retrieve the data!