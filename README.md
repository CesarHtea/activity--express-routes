# Express Routes

## Implement `Router` function from Express

### Setup Instructions

###### In terminal

```sh
# (1) navigate to your activities directory
$ cd ~/Documents/muktek/activities

# (2) Clone the repo and save it into activity--express-routes
$ git clone https://github.com/agzeri/starter-repo--express-routes.git activity--express-routes

$ cd activity--express-routes

# (3) Install all dependencies
$ npm install
```

###### In File

#### (1) Create a `routes` folder

#### (2) Inside `routes` folder, create a `apiRouter` file

#### (3) Import `Router` from Express.JS framework
_Don’t forget to export the module._

##### (4) Create four routes to handle RESTful services

```
GET     /api/courses
POST    /api/courses
PUT     /api/courses/{id}
DELETE  /api/courses/{id}
GET     /api/courses/{id}

GET     /api/instructors
POST    /api/instructors
DELETE  /api/instructors/{id}
GET     /api/instructors/{id}

GET     /api/students
GET     /api/students/{id}
POST    /api/students
```

```js
# Courses

[{
  id: 1,
  name: "Introduction to JavaScript",
  length: "15 hours"
}, {
  id: 2,
  name: "React.js Fundamentals",
  length: "25 hours"
}]
```

```js
# Instructors

[{
  id: 1,
  name: "Mr R"
}, {
  id: 2,
  name: "Tyler"
}, {
  id: 3,
  name: "John Die"
}]
```

```js
# Students

[{
  id: 1,
  name: "Damian Allende"
}, {
  id: 2,
  name: "Cesar Hernandez"
}, {
  id: 3,
  name: "Ingrid Garcia"
}, {
  id: 4,
  name: "Maribel Navia"
}]
```

###### Hint 1: For DELETE and PUT requests, you can play responding with a message like: "Making a DELETE/PUT request on {course/instructor/students} endpoint with id: «value»"

###### Hint 2: For GET requests, return all data and filter if it’s necessary (GET individual endpoints)

##### (5) Configure in `app.js`  the `apiRouter` file

**Test all routes using Postman.**

## Explorer Mode

* Send actual data to `POST /api/courses` endpoint.
  + To do this, you’ll need to capture data from body request. Read more about [here](https://expressjs.com/en/4x/api.html#req.body).
