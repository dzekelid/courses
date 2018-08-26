---
swagger: "2.0"
x-collection-name: Learnifier
x-complete: 0
info:
  title: Learnifier Gets a participation by external id
  version: 1.1.0
  description: Gets a participation by external id.
host: learnifier.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /coursedesigns:
    get:
      summary: Lists all global course design templates
      description: Lists all global course design templates. Only api callers that
        have full access can call this method.
      operationId: coursedesigns.get
      x-api-path-slug: coursedesigns-get
      responses:
        200:
          description: OK
      tags:
      - Courses
  /extparticipation:
    get:
      summary: Gets a participation by external id
      description: Gets a participation by external id.
      operationId: extparticipation.get
      x-api-path-slug: extparticipation-get
      parameters:
      - in: query
        name: extid
        description: The external id of the participation
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Participation
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