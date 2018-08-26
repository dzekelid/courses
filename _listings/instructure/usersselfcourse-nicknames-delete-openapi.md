---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Users API Clear course nicknames
  description: Clear course nicknames.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/self/favorites/courses:
    delete:
      summary: Reset course favorites
      description: Reset course favorites.
      operationId: reset-course-favorites
      x-api-path-slug: usersselffavoritescourses-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
    get:
      summary: List favorite courses
      description: List favorite courses.
      operationId: list-favorite-courses
      x-api-path-slug: usersselffavoritescourses-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
  /users/self/favorites/courses/{id}:
    delete:
      summary: Remove course from favorites
      description: Remove course from favorites.
      operationId: remove-course-from-favorites
      x-api-path-slug: usersselffavoritescoursesid-delete
      parameters:
      - in: query
        name: id
        description: the ID or SIS ID of the course to remove
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
      - Id
    post:
      summary: Add course to favorites
      description: Add course to favorites.
      operationId: add-course-to-favorites
      x-api-path-slug: usersselffavoritescoursesid-post
      parameters:
      - in: query
        name: id
        description: The ID or SIS ID of the course to add
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
      - Id
  /users/{user_id}/courses:
    get:
      summary: List courses for a user
      description: List courses for a user.
      operationId: list-courses-for-a-user
      x-api-path-slug: usersuser-idcourses-get
      parameters:
      - in: query
        name: include[]
        description: 'u201cneeds_grading_countu201d: Optional information to include
          with each Course'
      - in: query
        name: state[]
        description: If set, only return courses that are in the given state(s)
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Courses
  /users/{user_id}/courses/course_id/assignments:
    get:
      summary: List assignments for user
      description: List assignments for user.
      operationId: list-assignments-for-user
      x-api-path-slug: usersuser-idcoursescourse-idassignments-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Courses
      - Course
      - Id
      - Assignments
  /users/self/course_nicknames:
    delete:
      summary: Clear course nicknames
      description: Clear course nicknames.
      operationId: clear-course-nicknames
      x-api-path-slug: usersselfcourse-nicknames-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
    get:
      summary: List course nicknames
      description: List course nicknames.
      operationId: list-course-nicknames
      x-api-path-slug: usersselfcourse-nicknames-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
  /users/self/course_nicknames/{course_id}:
    delete:
      summary: Remove course nickname
      description: Remove course nickname.
      operationId: remove-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
    get:
      summary: Get course nickname
      description: Get course nickname.
      operationId: get-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
    put:
      summary: Set course nickname
      description: Set course nickname.
      operationId: set-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-put
      parameters:
      - in: query
        name: nickname
        description: The nickname to set
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---