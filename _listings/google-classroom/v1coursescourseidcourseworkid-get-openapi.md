---
swagger: "2.0"
x-collection-name: Google Classroom
x-complete: 0
info:
  title: Google Classroom API Get Course Work
  description: |-
    Returns course work.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to access the
    requested course or course work, or for access errors.
    * `INVALID_ARGUMENT` if the request is malformed.
    * `NOT_FOUND` if the requested course or course work does not exist.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: classroom.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/courses:
    get:
      summary: Get Courses
      description: |-
        Returns a list of courses that the requesting user is permitted to view,
        restricted to those that match the request.

        This method returns the following error codes:

        * `PERMISSION_DENIED` for access errors.
        * `INVALID_ARGUMENT` if the query argument is malformed.
        * `NOT_FOUND` if any users specified in the query arguments do not exist.
      operationId: classroom.courses.list
      x-api-path-slug: v1courses-get
      parameters:
      - in: query
        name: courseStates
        description: Restricts returned courses to those in one of the specified statesThe
          default value is ACTIVE, ARCHIVED, PROVISIONED, DECLINED
      - in: query
        name: pageSize
        description: Maximum number of items to return
      - in: query
        name: pageToken
        description: nextPageTokenvalue returned from a previouslist call,indicating
          that the subsequent page of results should be returned
      - in: query
        name: studentId
        description: Restricts returned courses to those having a student with the
          specifiedidentifier
      - in: query
        name: teacherId
        description: Restricts returned courses to those having a teacher with the
          specifiedidentifier
      responses:
        200:
          description: OK
      tags:
      - Course
    post:
      summary: Create Course
      description: |-
        Creates a course.

        The user specified in `ownerId` is the owner of the created course
        and added as a teacher.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to create
        courses or for access errors.
        * `NOT_FOUND` if the primary teacher is not a valid user.
        * `FAILED_PRECONDITION` if the course owner's account is disabled or for
        the following request errors:
            * UserGroupsMembershipLimitReached
        * `ALREADY_EXISTS` if an alias was specified in the `id` and
        already exists.
      operationId: classroom.courses.create
      x-api-path-slug: v1courses-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Course
  /v1/courses/{id}:
    delete:
      summary: Delete Course
      description: |-
        Deletes a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to delete the
        requested course or for access errors.
        * `NOT_FOUND` if no course exists with the requested ID.
      operationId: classroom.courses.delete
      x-api-path-slug: v1coursesid-delete
      parameters:
      - in: path
        name: id
        description: Identifier of the course to delete
      responses:
        200:
          description: OK
      tags:
      - Course
    get:
      summary: Get Course
      description: |-
        Returns a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course or for access errors.
        * `NOT_FOUND` if no course exists with the requested ID.
      operationId: classroom.courses.get
      x-api-path-slug: v1coursesid-get
      parameters:
      - in: path
        name: id
        description: Identifier of the course to return
      responses:
        200:
          description: OK
      tags:
      - Course
    put:
      summary: Update Course
      description: |-
        Updates a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to modify the
        requested course or for access errors.
        * `NOT_FOUND` if no course exists with the requested ID.
        * `FAILED_PRECONDITION` for the following request errors:
            * CourseNotModifiable
      operationId: classroom.courses.update
      x-api-path-slug: v1coursesid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Identifier of the course to update
      responses:
        200:
          description: OK
      tags:
      - Course
  /v1/courses/{courseId}/courseWork:
    post:
      summary: Create Course Work
      description: |-
        Creates course work.

        The resulting course work (and corresponding student submissions) are
        associated with the Developer Console project of the
        [OAuth client ID](https://support.google.com/cloud/answer/6158849) used to
        make the request. Classroom API requests to modify course work and student
        submissions must be made with an OAuth client ID from the associated
        Developer Console project.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course, create course work in the requested course, share a
        Drive attachment, or for access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course does not exist.
        * `FAILED_PRECONDITION` for the following request error:
            * AttachmentNotVisible
      operationId: classroom.courses.courseWork.create
      x-api-path-slug: v1coursescourseidcoursework-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course
      responses:
        200:
          description: OK
      tags:
      - Course Work
  /v1/courses/{courseId}/courseWork/{id}:
    delete:
      summary: Delete Course Work
      description: |-
        Deletes a course work.

        This request must be made by the Developer Console project of the
        [OAuth client ID](https://support.google.com/cloud/answer/6158849) used to
        create the corresponding course work item.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting developer project did not create
        the corresponding course work, if the requesting user is not permitted
        to delete the requested course or for access errors.
        * `FAILED_PRECONDITION` if the requested course work has already been
        deleted.
        * `NOT_FOUND` if no course exists with the requested ID.
      operationId: classroom.courses.courseWork.delete
      x-api-path-slug: v1coursescourseidcourseworkid-delete
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: id
        description: Identifier of the course work to delete
      responses:
        200:
          description: OK
      tags:
      - Course Work
    get:
      summary: Get Course Work
      description: |-
        Returns course work.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course or course work, or for access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course or course work does not exist.
      operationId: classroom.courses.courseWork.get
      x-api-path-slug: v1coursescourseidcourseworkid-get
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: id
        description: Identifier of the course work
      responses:
        200:
          description: OK
      tags:
      - Course Work
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