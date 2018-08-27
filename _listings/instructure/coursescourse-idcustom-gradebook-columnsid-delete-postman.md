{
  "info": {
    "name": "Instructure Canvas Courses API Delete a custom gradebook column",
    "_postman_id": "b5e0aa4e-ef95-463a-b5e0-47dc8d61727c",
    "description": "Delete a custom gradebook column.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "48e269dc-502a-4b97-8d64-75d587021317",
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
              "id": "4815a859-968f-425d-9031-988bd0f5ca82"
            }
          ]
        },
        {
          "id": "a556af05-a49a-44d2-adc5-e2aff2f3cde8",
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
              "id": "029e19c1-e626-4d8a-868b-6bb8bf7a9d54"
            }
          ]
        },
        {
          "id": "d6ddeef9-b324-4f5d-8a93-ea1e323d1ebc",
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
              "id": "24cf68d6-f046-4633-a842-a68dc29bff18"
            }
          ]
        }
      ]
    }
  ]
}