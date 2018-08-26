---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API List your courses
  description: List your courses.
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
  /courses:
    get:
      summary: List your courses
      description: List your courses.
      operationId: list-your-courses
      x-api-path-slug: courses-get
      parameters:
      - in: query
        name: enrollment_role
        description: Deprecated When set, only return courses where the user is enrolled
          withnthe specified course-level role
      - in: query
        name: enrollment_role_id
        description: When set, only return courses where the user is enrolled with
          the specifiedncourse-level role
      - in: query
        name: enrollment_type
        description: When set, only return courses where the user is enrolled as this
          type
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
      - Courses
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