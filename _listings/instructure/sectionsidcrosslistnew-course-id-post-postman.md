{
  "info": {
    "name": "Instructure Canvas Sections API Cross-list a Section",
    "_postman_id": "6e7d4f8b-a7c7-427a-9a78-c425bb8b451e",
    "description": "Cross-list a section.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sections",
      "item": [
        {
          "id": "aa4495fa-e4db-4e66-ba02-5ff9f66a455b",
          "name": "decrosslist-a-section",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "sections/:id/crosslist"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "De-cross-list a section."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ba47746-5f9d-4b59-ab56-2e4e46b0e0e0"
            }
          ]
        },
        {
          "id": "b6f8c933-5a30-4f18-9503-4a469514dce1",
          "name": "crosslist-a-section",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "sections/:id/crosslist/new_course_id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Cross-list a section."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77845152-6d68-4286-ad3d-da8f0d816fb4"
            }
          ]
        }
      ]
    }
  ]
}