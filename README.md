# Noni Full Stack Developer Coding Challenge

## Objective

To create a note taking app using Laravel and VueJS.

## Insructions

You are going to use a pre-configured dockerized application to create a simple CRUD application. Laravel is used on the back-end Vuejs is used on the front end as a SPA.

_Note: There is already JWT authentication implemented for the app._

**TODO:** The application should allow you to create, edit, and delete delete notes. Notes will be save to the database. Notes will have a title, content, and created_at displayed on the front end.

1.  Save the created notes in the database
2.  Create the necessary table with Laravel migrations
3.  Create all require restful routes to achieve the CRUD functionality
4.  Create required Front End components to access the API you created
5.  Authenticated user needs to be able to view all notes, create new notes, edit existing notes, and delete notes.
6.  Create phpunit tests for the new feature

## Grading Scheme

Functionality: Out of 10

UX/Design: Out of 10

DB Design: Out of 5

Validation: Out of 10

Coding Style: Out of 10

Testing: Out of 5


Include front-end and back-end validation.
Feel free to use your creativity and design skills to make the existing site design your own.

## Setup

The project comes with a dockerized development environment and should include everything you need to get working right away.

This setup requires that you have docker and docker-compose installed on your system.

**Docker installation instructions here:**
[https://docs.docker.com/compose/install/](https://docs.docker.com/compose/install/)

**Copy Laravel environment file**
(While in project root)

```
cp .env.example .env
```

**Copy Docker environment files**

```
cd docker

cp env-example .env
```

**Run docker containers**

```
docker-compose up
```

**Enter workspace container**

```
docker-compose exec --user=laradock workspace bash
```

**Install dependencies and build existing database**

```
composer install
npm install
php artisan key:generate
php artisan migrate --seed
```

**Build app**

```
npm run watch
```

The application should now be available at http://localhost

## Submission

Create a pull request on Github. Name the branch as {firstname}-{lastname}-submission.
