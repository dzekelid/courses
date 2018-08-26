{
  "info": {
    "name": "Instructure Canvas Courses API Update a custom gradebook column",
    "_postman_id": "f3e4975f-a700-49af-bc19-85f7a4da8774",
    "description": "Update a custom gradebook column.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "8d2ff89c-ba86-4738-a6e7-8b1a66e786c5",
          "name": "list-custom-gradebook-columns",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/custom_gradebook_columns"
              ],
              "query": [
                {
                  "key": "include_hidden",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List custom gradebook columns."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ca83565-081f-4827-9af4-4cf7d25f5595"
            }
          ]
        },
        {
          "id": "9b8a7b8a-828c-448a-b4c0-21047753041f",
          "name": "create-a-custom-gradebook-column",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/custom_gradebook_columns"
              ],
              "query": [
                {
                  "key": "column[hidden]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "column[position]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "column[teacher_notes]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "column[title]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a custom gradebook column."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9332b6aa-a536-4b1f-a037-2293750e5612"
            }
          ]
        },
        {
          "id": "3f29aaad-d69a-4be5-9c11-749d77c6141a",
          "name": "update-a-custom-gradebook-column",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/custom_gradebook_columns/id"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a custom gradebook column."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80b9e27e-2013-4ea0-9fcd-d7a9f17295be"
            }
          ]
        },
        {
          "id": "61d9310f-fc94-4361-90ea-734a62017a8f",
          "name": "delete-a-custom-gradebook-column",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/custom_gradebook_columns/id"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a custom gradebook column."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7c6b82f-50f7-4972-84fd-6dc1a55e2fa7"
            }
          ]
        }
      ]
    }
  ]
}