{
  "info": {
    "name": "Instructure Canvas Courses API Update column data",
    "_postman_id": "ce80b397-dd9d-436f-b9ac-1d5e1d6d5550",
    "description": "Update column data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "2179111f-8226-4e70-8387-a6600ea62463",
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
              "id": "a347539e-0b11-442c-9561-e7dff3040bbb"
            }
          ]
        },
        {
          "id": "53b7b7ae-65b2-4990-9e7d-debcf6f33f9b",
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
              "id": "a1987143-4ba1-438d-9327-616bba9ad6f0"
            }
          ]
        },
        {
          "id": "3b1c5ebc-56fc-47a4-9dd8-0f9de6028c1c",
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
              "id": "317fa855-b546-42b2-8cd7-3688f88ebca8"
            }
          ]
        },
        {
          "id": "8ea68fe2-0b8c-4b2d-b351-462a2d2c3054",
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
              "id": "924a50af-fdb6-4132-9619-e0d3d0e59eac"
            }
          ]
        },
        {
          "id": "083ad599-1062-4728-8f59-c56ea2e999f3",
          "name": "list-entries-for-a-column",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/custom_gradebook_columns/id/data"
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
            "description": "List entries for a column."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "136937bd-3395-4051-94cb-42bfc6bae189"
            }
          ]
        },
        {
          "id": "d84fc1e7-8184-49f3-880c-28cc70c0919e",
          "name": "update-column-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/custom_gradebook_columns/id/data/:user_id"
              ],
              "query": [
                {
                  "key": "column_data[content]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update column data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12157002-b9bf-436c-aa27-aa7dba96264a"
            }
          ]
        }
      ]
    }
  ]
}