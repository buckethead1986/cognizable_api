# Cognizance

## Overview

This is a Ruby on Rails JSON API for a front-end React project, Cognizable. The application is a clone of the game, Memory. Users sign in (non securely, merely to log high scores), choose a difficulty, and play a game of memory. Elapsed time and moves taken are logged, and high scores are updated (if you're within the top 5, one high score per user).

## Database Structure

The Rails backend JSON API uses a Postgres database and is deployed via Heroku.
Our React project interacts with this JSON API through get, post, and patch
requests.

Our database is structured with the following five models:

* Users

* Cards

All models have their own unique routes and are
rendered in JSON by the API.

## API Use

This API is public and the only thing that requires authorization is posting to
the user session in order to login. The rest of the information is accessible to
anyone who goes to a route on the following base url:
https://cognizance.herokuapp.com/api/v1/

This public accessibility is mirrored in our front-end application.
https://cognizable.herokuapp.com/
