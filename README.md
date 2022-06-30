# MongoDB-autocomplete-search
Auto-Completing Movie_Search_App Project Overview

The goal of this project is to learn how to instantaneously search a massive MongoDB database from inside of an Auto-Completing Movie Finder App. A lot of websites do this to help you figure out what you are typing as you go. In this project, typing in the search will give you a list of the main cast as well as the poster. 

<p align="center">
  <img width="600" height="310" src="./autocompleteApp.gif">
</p>

## Installation

1. Clone repo
2. run `npm install`

## How It's Made:

**Tech used:** HTML, CSS, JavaScript, Express, MongoDB

As soon as you start typing you'll notice it will start giving you some results in a dropdown and as you keep typing its going to keep giving you updated results.

## Optimizations

**Creating JSON search index** to import sample datasets and as a result make it easier to search on a specific field that we have indexed. The search index used to apply to MongoDB movies collection is below;

`{
    "mappings" : {
        "dynamic" : false,
        "fields" : {
            "title" : [
                {
                    "foldDiacritics": false,
                    "maxGrams": 7,
                    "minGrams": 3,
                    "tokenization": "edgeGram",
                    "type": "autocomplete"
                }
            ]
        }
    }
}`

## Lessons Learned:

**Using npm install dotenv** which allows us to create a separate environment location where we can set things to various variables and then use them in our code but still hide/obscure them from GitHub. In that case, it is useful for us here because we are going to obscure our connection string to MongoDB so that nobody can go up get our connection information to our database.


**Using CORS** to bypass the error we get in our browser when we want to connect our app to our server and viceversa.

## Examples:
Take a look at these couple examples that I have in my own portfolio:

**Random Quote Generator:** https://mooseki.github.io/JS-Random-Quote-Generator-Project/

**Picture-in-Picture:** https://github.com/mooseki/JS-Picture-In-Picture-Project.git

**Joke Teller:** #
