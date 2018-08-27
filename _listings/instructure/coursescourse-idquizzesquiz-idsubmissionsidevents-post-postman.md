{
  "info": {
    "name": "Instructure Canvas Courses API Submit captured events",
    "_postman_id": "bd67f660-4747-457a-81a9-600770655f04",
    "description": "Submit captured events.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "96f90c66-db67-438d-ab9e-4b1e9975f3e9",
          "name": "retrieve-captured-events",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/quizzes/quiz_id/submissions/:id/events"
              ],
              "query": [
                {
                  "key": "attempt",
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
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve captured events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "130a69f8-7516-4dbf-9fb8-0b7828832333"
            }
          ]
        },
        {
          "id": "a978bac9-14f0-44ad-9340-1677eece5b10",
          "name": "submit-captured-events",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/quizzes/quiz_id/submissions/:id/events"
              ],
              "query": [
                {
                  "key": "quiz_submission_events",
                  "value": "%5B%7B%7D%5D",
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
            "description": "Submit captured events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3958a7a-2d5f-4949-a623-300805cdbbf3"
            }
          ]
        }
      ]
    }
  ]
}