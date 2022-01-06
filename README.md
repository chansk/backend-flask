# Backend with Flask

This is a backend application built with Flask with some of the typical
situations encountered during the development.

https://www.youtube.com/playlist?list=PLab_if3UBk98jBTmyxShFVirMbgfFYu8W

## Chapter 1

In this first video, I've created a Flask project, I've added the necessary
dependencies and structured the folders.

For this, I've used the Poetry to create the project and add the dependencies.
Then, I've created some simple endpoints to test my application.

To structure the endpoints, I've also used the Blueprints.


## Chapter 2

In this second video, I show different methods to authenticate a request into
a Flask application.

I start using a Basic Authentication and then JWT. Both authentication are
validated with the library flask-httpauth using decorators.

To protect endpoints with any kind of authentication, I only need to add the
adequate decorator to the endpoint signature.


## Chapter 3

In this third video, I will configure the database connection with SQLAlchemy.
Flask and SQLAlchemy work very well together. The database connection can direclty
be injected in the Flask application and SQLAlchemy will read it.

I will also create some entities to show the most common relationships: one-to-one,
one-to-many, many-to-one and many-to-many.

Here is the command I've used to create the database in the video:
```
docker run -d -e POSTGRES_HOST_AUTH_METHOD=trust -e POSTGRES_USER=sergio -e POSTGRES_PASSWORD=my-password -e POSTGRES_DB=backenddb -p 5432:5432 postgres:13
```

