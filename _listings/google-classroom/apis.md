---
name: Google Classroom
x-slug: google-classroom
description: Google Classroom is mission control for your classes. As a free service
  for teachers and students, you can create classes, distribute assignments, send
  feedback, and see everything in one place. Instant. Paperless. Easy.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Courses
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/apis.md
specificationVersion: "0.14"
apis:
- name: Google Classroom - Get Courses
  x-api-slug: v1courses-get
  description: |-
    Returns a list of courses that the requesting user is permitted to view,
    restricted to those that match the request.

    This method returns the following error codes:

    * `PERMISSION_DENIED` for access errors.
    * `INVALID_ARGUMENT` if the query argument is malformed.
    * `NOT_FOUND` if any users specified in the query arguments do not exist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1courses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1courses-get-openapi.md
- name: Google Classroom - Create Course
  x-api-slug: v1courses-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1courses-post-openapi.md
- name: Google Classroom - Delete Course
  x-api-slug: v1coursesid-delete
  description: |-
    Deletes a course.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to delete the
    requested course or for access errors.
    * `NOT_FOUND` if no course exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursesid-delete-openapi.md
- name: Google Classroom - Get Course
  x-api-slug: v1coursesid-get
  description: |-
    Returns a course.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to access the
    requested course or for access errors.
    * `NOT_FOUND` if no course exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursesid-get-openapi.md
- name: Google Classroom - Update Course
  x-api-slug: v1coursesid-put
  description: |-
    Updates a course.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to modify the
    requested course or for access errors.
    * `NOT_FOUND` if no course exists with the requested ID.
    * `FAILED_PRECONDITION` for the following request errors:
        * CourseNotModifiable
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursesid-put-openapi.md
- name: Google Classroom - Create Course Work
  x-api-slug: v1coursescourseidcoursework-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursescourseidcoursework-post-openapi.md
- name: Google Classroom - Delete Course Work
  x-api-slug: v1coursescourseidcourseworkid-delete
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursescourseidcourseworkid-delete-openapi.md
- name: Google Classroom - Get Course Work
  x-api-slug: v1coursescourseidcourseworkid-get
  description: |-
    Returns course work.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to access the
    requested course or course work, or for access errors.
    * `INVALID_ARGUMENT` if the request is malformed.
    * `NOT_FOUND` if the requested course or course work does not exist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursescourseidcourseworkid-get-openapi.md
- name: Google Classroom - Get Courses
  x-api-slug: v1courses-get
  description: |-
    Returns a list of courses that the requesting user is permitted to view,
    restricted to those that match the request.

    This method returns the following error codes:

    * `PERMISSION_DENIED` for access errors.
    * `INVALID_ARGUMENT` if the query argument is malformed.
    * `NOT_FOUND` if any users specified in the query arguments do not exist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1courses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1courses-get-openapi.md
- name: Google Classroom - Create Course
  x-api-slug: v1courses-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1courses-post-openapi.md
- name: Google Classroom - Delete Course
  x-api-slug: v1coursesid-delete
  description: |-
    Deletes a course.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to delete the
    requested course or for access errors.
    * `NOT_FOUND` if no course exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursesid-delete-openapi.md
- name: Google Classroom - Get Course
  x-api-slug: v1coursesid-get
  description: |-
    Returns a course.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to access the
    requested course or for access errors.
    * `NOT_FOUND` if no course exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursesid-get-openapi.md
- name: Google Classroom - Update Course
  x-api-slug: v1coursesid-put
  description: |-
    Updates a course.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to modify the
    requested course or for access errors.
    * `NOT_FOUND` if no course exists with the requested ID.
    * `FAILED_PRECONDITION` for the following request errors:
        * CourseNotModifiable
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursesid-put-openapi.md
- name: Google Classroom - Create Course Work
  x-api-slug: v1coursescourseidcoursework-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursescourseidcoursework-post-openapi.md
- name: Google Classroom - Delete Course Work
  x-api-slug: v1coursescourseidcourseworkid-delete
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursescourseidcourseworkid-delete-openapi.md
- name: Google Classroom - Get Course Work
  x-api-slug: v1coursescourseidcourseworkid-get
  description: |-
    Returns course work.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to access the
    requested course or course work, or for access errors.
    * `INVALID_ARGUMENT` if the request is malformed.
    * `NOT_FOUND` if the requested course or course work does not exist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursescourseidcourseworkid-get-openapi.md
- name: Google Classroom - Get Courses
  x-api-slug: v1courses-get
  description: |-
    Returns a list of courses that the requesting user is permitted to view,
    restricted to those that match the request.

    This method returns the following error codes:

    * `PERMISSION_DENIED` for access errors.
    * `INVALID_ARGUMENT` if the query argument is malformed.
    * `NOT_FOUND` if any users specified in the query arguments do not exist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1courses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1courses-get-openapi.md
- name: Google Classroom - Create Course
  x-api-slug: v1courses-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1courses-post-openapi.md
- name: Google Classroom - Delete Course
  x-api-slug: v1coursesid-delete
  description: |-
    Deletes a course.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to delete the
    requested course or for access errors.
    * `NOT_FOUND` if no course exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursesid-delete-openapi.md
- name: Google Classroom - Get Course
  x-api-slug: v1coursesid-get
  description: |-
    Returns a course.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to access the
    requested course or for access errors.
    * `NOT_FOUND` if no course exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursesid-get-openapi.md
- name: Google Classroom - Update Course
  x-api-slug: v1coursesid-put
  description: |-
    Updates a course.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to modify the
    requested course or for access errors.
    * `NOT_FOUND` if no course exists with the requested ID.
    * `FAILED_PRECONDITION` for the following request errors:
        * CourseNotModifiable
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursesid-put-openapi.md
- name: Google Classroom - Create Course Work
  x-api-slug: v1coursescourseidcoursework-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursescourseidcoursework-post-openapi.md
- name: Google Classroom - Delete Course Work
  x-api-slug: v1coursescourseidcourseworkid-delete
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursescourseidcourseworkid-delete-openapi.md
- name: Google Classroom - Get Course Work
  x-api-slug: v1coursescourseidcourseworkid-get
  description: |-
    Returns course work.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to access the
    requested course or course work, or for access errors.
    * `INVALID_ARGUMENT` if the request is malformed.
    * `NOT_FOUND` if the requested course or course work does not exist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/courses/master/_listings/google-classroom/v1coursescourseidcourseworkid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.civic.information.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.classroom.stack.network
- type: x-button
  url: https://developers.google.com/classroom/guides/sharebutton
- type: x-developer
  url: https://developers.google.com/classroom/
- type: x-getting-started
  url: ""
- type: x-issues
  url: https://code.google.com/a/google.com/p/apps-api-issues/issues/list?can=2&q=label%3AAPI-Classroom
- type: x-website
  url: https://classroom.google.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---