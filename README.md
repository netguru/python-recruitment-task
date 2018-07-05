# Django task

Hey there!

This is the first task in recruitment process for the position of Python Developer at Netguru. Read the instructions carefully and send us back the link with solution.

### Specification

We’d like you to build simple REST API for us - a basic movie database interacting with external API. Here’s full specification of endpoints that we’d like it to have:

* `POST /movies`:
  * Request body should contain only movie title, and its presence should be validated.
  * Based on passed title, other movie details should be fetched from http://www.omdbapi.com/ (or other similar, public movie database) - and saved to application database.
  * Request response should include full movie object, along with all data fetched from external API.
* `GET /movies`:
  * Should fetch list of all movies already present in application database.
  * Additional filtering, sorting is fully optional - but some implementation is a bonus.
* `POST /comments`:
  * Request body should contain ID of movie already present in database, and comment text body.
  * Comment should be saved to application database and returned in request response.
* `GET /comments`:
  * Should fetch list of all comments present in application database.
  * Should allow filtering comments by associated movie, by passing its ID.

### Rules & hints

* Your're goal is to implement REST API in Django, however you're free to use any third-party libraries and database of your choice - sharing your reasoning behind choosing them is welcome!
* At least basic tests of endpoints and their functionality are obligatory. Their exact scope and form is left up to you.
* The application's code should be kept in a public repository so that we can read it, pull it and build it ourselves. Remember to include README file or at least basic notes on application requirements and setup - we should be able to easily and quickly get it running.
* Written application must be hosted and publicly available for us online - we recommend [Heroku](https://heroku.com).

**Good luck! If you have any questions feel free to ping us!**