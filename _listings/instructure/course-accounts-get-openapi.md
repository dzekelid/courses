---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Utility APIs List accounts for course admins
  description: List accounts for course admins.
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
  /api/sis/courses/{course_id}/assignments:
    get:
      summary: Retrieve assignments enabled for grade export to SIS
      description: Retrieve assignments enabled for grade export to sis.
      operationId: retrieve-assignments-enabled-for-grade-export-to-sis
      x-api-path-slug: apisiscoursescourse-idassignments-get
      parameters:
      - in: query
        name: account_id
        description: The ID of the account to query
      - in: query
        name: course_id
        description: The ID of the course to query
      - in: query
        name: ends_after
        description: When searching on an account, restricts to courses that end after
          this daten(if they have an end date)
      - in: query
        name: starts_before
        description: When searching on an account, restricts to courses that start
          before thisndate (if they have a start date)
      responses:
        200:
          description: OK
      tags:
      - Api
      - Sis
      - Courses
      - Course
      - Id
      - Assignments
  /search/all_courses:
    get:
      summary: List all courses
      description: List all courses.
      operationId: list-all-courses
      x-api-path-slug: searchall-courses-get
      parameters:
      - in: query
        name: open_enrollment_only
        description: Only return courses that allow self enrollment
      - in: query
        name: public_only
        description: Only return courses with public content
      - in: query
        name: search
        description: Search terms used for matching users/courses/groups (e
      responses:
        200:
          description: OK
      tags:
      - Search
      - ""
      - Courses
  /course_accounts:
    get:
      summary: List accounts for course admins
      description: List accounts for course admins.
      operationId: list-accounts-for-course-admins
      x-api-path-slug: course-accounts-get
      responses:
        200:
          description: OK
      tags:
      - Course
      - Accounts
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