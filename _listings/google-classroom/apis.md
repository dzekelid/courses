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
created: "2018-08-26"
modified: "2018-08-26"
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