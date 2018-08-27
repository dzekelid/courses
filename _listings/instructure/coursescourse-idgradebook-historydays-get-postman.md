{
  "info": {
    "name": "Instructure Canvas Courses API Days in gradebook history for this course",
    "_postman_id": "f68fc48c-d31f-4732-9469-096e82cb50fa",
    "description": "Days in gradebook history for this course.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "cbea2d11-cace-463b-b4ed-b4964644b91d",
          "name": "details-for-a-given-date-in-gradebook-history-for-this-course",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/gradebook_history/date"
              ],
              "query": [
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details for a given date in gradebook history for this course."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09460eb3-f001-44dd-83eb-ae307ed8b400"
            }
          ]
        },
        {
          "id": "cc223724-6028-4ba0-b461-bc1e6accc605",
          "name": "lists-submissions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/gradebook_history/date/graders/:grader_id/assignments/assignment_id/submissions"
              ],
              "query": [
                {
                  "key": "assignment_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "grader_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists submissions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "473b53a0-c099-499c-87e2-01ad23cb9e2b"
            }
          ]
        },
        {
          "id": "3e32b82c-99cf-480a-8a72-e4981a034107",
          "name": "days-in-gradebook-history-for-this-course",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/gradebook_history/days"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Days in gradebook history for this course."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b56d085-b3b8-4d50-84dc-db62ea4814df"
            }
          ]
        }
      ]
    }
  ]
}