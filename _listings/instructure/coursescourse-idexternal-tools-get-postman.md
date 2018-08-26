{
  "info": {
    "name": "Instructure Canvas Courses API List external tools",
    "_postman_id": "aedb14fb-e33b-480d-88cf-d65849ae964f",
    "description": "List external tools.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "b2749954-3e8c-490b-a976-35b4a6d14ea0",
          "name": "list-external-feeds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_feeds"
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
            "description": "List external feeds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c05bf91c-58cc-459b-b82d-ce184df38e6b"
            }
          ]
        },
        {
          "id": "5dff63ed-64b9-4b5c-a24a-4ac9b2f84ec0",
          "name": "create-an-external-feed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_feeds"
              ],
              "query": [
                {
                  "key": "header_match",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "verbosity",
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
            "description": "Create an external feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36d78b14-144f-4658-bfa9-2ea48b6cf415"
            }
          ]
        },
        {
          "id": "098170bc-f97a-4d97-b216-fd536055e532",
          "name": "delete-an-external-feed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_feeds/external_feed_id"
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
            "description": "Delete an external feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8e5e8be-693b-4449-9e08-dc858b8588e1"
            }
          ]
        },
        {
          "id": "ec156e97-9bf9-4956-ba84-8e436fd1f339",
          "name": "list-external-tools",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_tools"
              ],
              "query": [
                {
                  "key": "search_term",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "selectable",
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
            "description": "List external tools."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "daa7a4bc-9b61-45f1-8236-b47765320b41"
            }
          ]
        }
      ]
    }
  ]
}