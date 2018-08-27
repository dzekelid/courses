swagger: "2.0"
x-collection-name: Learnifier
x-complete: 1
info:
  title: Learnifier
  version: 1.1.0
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