# MongoDB-autocomplete-search
Movie_Search_App Project Overview

The goal of this project is to learn how to instantaneously search a massive MongoDB database from inside of an Auto-Completing Movie Finder App. A lot of websites to this to help you figure out what you are typing as you go. In this project, typing in the search will give you a list of the main cast as well as the poster. 

**Link to project:** https://mooseki.github.io/JS-Infinity-Scroll-Project/

![alt tag](http://placecorgi.com/1200/650)

## How It's Made:

**Tech used:** HTML, CSS, JavaScript, Unsplash Image API

As soon as you start typing you'll notice it will start giving you some results in a dropdown and as you keep typing its going to keep giving you updated results.    
The images are photos fetched from the unsplash image API and we are tracking the moment all the images are loaded in order to dynamically hide our loading animation. It is one long column of images with a margin on the left and right. As we scroll closer to the bottom, if you watch the scroll bar on the right, you are going to see it jump up when the next network request is made and we are fetching more images to give a totally seamless experiance. 

If we hover over an image we can see a description and if we click on the image we can see that image on the unsplah website so that we can see the author or download the photo if we want. Lastly, if we open up our dev tools, we can see it is mobile responsive as well, so instead of having big margin on the left and right in a mobile device, we just have a 10 pixel margin all the way around to so that it will look great on mobile as well. 


## Optimizations

**Using developer tools to improve performance** of the website because not every user has good internet connection. To improve user experience and have good SEO ranking we do analysis by going to 'Network' where we can see that it is taking forever to load many photos at once. Based on that, we can learn that the easiest thing to do here, for example, is to just grab one item instead of 30 photos and then loading up the page.


## Lessons Learned:

**Creating custom animated loading icon** using a website called Loading.io. They have a very easy to use interface where you can adjust a number of different settings and output in a number of different formats using the free or paid options provided. This is a great opportunity to add my own personal style to any project like a custom color theme that matches a certain brand. Eventually, I can download the custom image as an animated SVG image. SVG uses coordinates in 2D space to create lines and shapes with the main benefit being that the file sizes are smaller and I can make an SVG any size and it would look just as sharp when we zoom.


**Using Unsplash API** to set up the functionality of our project which allows us to return high quality random images and that will allow us to showcase our infinite scroll functionality.

## Examples:
Take a look at these couple examples that I have in my own portfolio:

**Random Quote Generator:** https://mooseki.github.io/JS-Random-Quote-Generator-Project/

**Picture-in-Picture:** https://github.com/mooseki/JS-Picture-In-Picture-Project.git

**Joke Teller:** #

