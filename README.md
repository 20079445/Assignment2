# Assignment 2 - Web API.

Name: John Murphy

## Features.

A bullet-point list of the ADDITIONAL features you have implemented in the API **THAT WERE NOT IN THE LABS** (or modifications to existing features)

 + endpoint Top rated movies
 + endpoint Now Playing
 + functional login
 + functional register
 + new people mongodb collection


## Setup requirements.

[ Outline any non-standard setup steps necessary to run your app locally after cloning the repo.]

## API Configuration

Describe any configuration that needs to take place before running the API. For example, creating an `.env` file and what variables to put in it. Give an example of how this might be done.

REMEMBER: DON'T PUT YOUR OWN USERNAMES/PASSWORDS/AUTH KEYS IN THE README OR ON GITHUB, just placeholders as indicated below:

______________________
NODEENV=development
PORT=8080
HOST=localhost
mongoDB=placeholder URL
seedDb=true
secret= placehodler secret
REACT_APP_TMDB_KEY= placeholder key
______________________

## API Design
Give an overview of your web API design, perhaps similar to the following: 

- /api/movies | GET | Gets a list of movies 
- /api/movies/{movieid} | GET | Gets a single movie 
- /api/movies/{movieid}/reviews | GET | Get all reviews for movie 
- /api/movies/{movieid}/reviews | POST | Create a new review for Movie
- /api/genres | GET | Gets a list of genres
- /api/genres/{movieid} | GET | Gets the genres of a specific movie by id
- /api/users | GET | Gets a list of all users
- /api/users | Post | Creates new users
- /api/people | GET | Gets a list of actors
- /api/people/{peopleid} | GET | Gets a actors details by id

If you have your API design on an online platform or graphic, please link to it (e.g. [Swaggerhub](https://app.swaggerhub.com/)).

## Security and Authentication

Give details of authentication/security implemented on the API (e.g. passport/sessions). Indicate which routes are protected.
All routes are protected except the homepage and login/register pages.
Movies, People, Users, Genres are all protected by passport authentication.

## Integrating with React App

Describe how you integrated your React app with the API. List the views that use your Web API instead of the TMDB API. Describe any other updates to the React app from Assignment One.

There are manu updates from assignment one, two new endpoints in Top rated and Now Playing also i got login and tegister to officially work. There is now backend help for my frontend app with added secuirity in the form of if you are not logged in you cannot view any other page but the homepage or it will force you to login. Also i am now pulling from my own web api instead of TMDB api which makes my app alot less reliant on TMDB and able to stand on its own better.

## Independent learning (if relevant)

Briefly explain any non-standard features developed for the app.   

Creating the mongodb collection myself was hard and confusing, fidning all the data points needed for the model and data for people. Then getting the web api to actually take in the data properly and have it on the mongodb collections was a bit of work too. 
