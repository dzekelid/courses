{
  "info": {
    "name": "Instructure Canvas Courses API Enroll a user",
    "_postman_id": "2a76d615-0337-4111-a31f-4042b0f79194",
    "description": "Enroll a user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "59d44edf-4ccd-4b94-9f20-a190446b9e17",
          "name": "list-enrollments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/enrollments"
              ],
              "query": [
                {
                  "key": "grading_period_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "role",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "user_id",
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
            "description": "List enrollments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c71a7e0e-4f06-4f63-a667-2ae28f414b10"
            }
          ]
        },
        {
          "id": "25c3ee5c-edd3-48bb-8882-e4c0012d523d",
          "name": "enroll-a-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/enrollments"
              ],
              "query": [
                {
                  "key": "enrollment[course_section_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "enrollment[enrollment_state]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "enrollment[limit_privileges_to_course_section]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "enrollment[notify]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "enrollment[role]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "enrollment[role_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "enrollment[self_enrolled]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "enrollment[self_enrollment_code]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "enrollment[type]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "enrollment[user_id]",
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
            "description": "Enroll a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6df76c5f-fa6e-4df6-8f6e-cbb20bde511e"
            }
          ]
        }
      ]
    }
  ]
}