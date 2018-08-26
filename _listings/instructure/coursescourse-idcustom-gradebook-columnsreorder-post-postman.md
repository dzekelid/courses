{
  "info": {
    "name": "Instructure Canvas Courses API Reorder custom columns",
    "_postman_id": "7f6fdbad-a588-4b4c-9e21-2f4f073481da",
    "description": "Reorder custom columns.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "4a4dca6a-cf9b-4ac7-ac05-5de368cb4a1c",
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
              "id": "e2f04ace-1967-47ee-9a2c-efd2794bfa07"
            }
          ]
        },
        {
          "id": "e9041cb3-5d61-4d56-b951-200cdd8a3fad",
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
              "id": "a4458808-af1a-4431-b5e6-506d9e06b918"
            }
          ]
        },
        {
          "id": "0d364ed7-cd06-4a6a-90a6-edf4e4309679",
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
              "id": "0016f6b1-0000-45ca-ad88-b769ad4aac51"
            }
          ]
        },
        {
          "id": "6bb40ed9-a723-4e81-a52a-1e707a9f330c",
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
              "id": "8d7ccb36-7e4b-494b-bb7b-ef283c3a2da1"
            }
          ]
        },
        {
          "id": "288a252e-005c-40d4-b1c6-4684adc07cf8",
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
              "id": "bf8cb0e1-e8d9-433e-821e-9c62f1a6ed1c"
            }
          ]
        },
        {
          "id": "6dc75518-86d0-4a1a-9a2b-a6d67d7c3db2",
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
              "id": "36a28dc1-ed27-4a6f-a497-82a412c8e645"
            }
          ]
        },
        {
          "id": "da8cbf54-3869-4eea-bbdd-d2ec8acafc82",
          "name": "reorder-custom-columns",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/custom_gradebook_columns/reorder"
              ],
              "query": [
                {
                  "key": "order",
                  "value": "%5B%7B%7D%5D",
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
            "description": "Reorder custom columns."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9be05785-3e08-488a-ba5e-cec1bd7faf57"
            }
          ]
        }
      ]
    }
  ]
}