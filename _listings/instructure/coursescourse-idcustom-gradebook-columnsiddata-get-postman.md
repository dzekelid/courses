{
  "info": {
    "name": "Instructure Canvas Courses API List entries for a column",
    "_postman_id": "fb54e12f-9efa-4036-911b-6e5bf41bdeb6",
    "description": "List entries for a column.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "79674dd4-b9be-4c37-b279-88ad44f9bfef",
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
              "id": "96551f88-3411-4e65-9044-7adc00855056"
            }
          ]
        },
        {
          "id": "43af6eb0-fd63-45d0-835c-68fc21291304",
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
              "id": "260d8f37-bc8c-43a0-bbbf-2c76e84b65ad"
            }
          ]
        },
        {
          "id": "28c5ca5a-4202-4d24-b195-5965aca78640",
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
              "id": "6041b9d1-116c-4271-945d-5e6e23675c02"
            }
          ]
        },
        {
          "id": "cab3484e-ae5c-48f6-a232-601896baaeac",
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
              "id": "fead0a7d-5e47-49e6-bf7c-c0640ada90f7"
            }
          ]
        },
        {
          "id": "174496da-c6e4-4aa2-8598-bdc4e6a948ab",
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
              "id": "f370fccf-0c13-42a3-a257-46d896ce83d6"
            }
          ]
        }
      ]
    }
  ]
}