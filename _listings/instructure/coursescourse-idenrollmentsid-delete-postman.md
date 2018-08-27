{
  "info": {
    "name": "Instructure Canvas Courses API Conclude or inactivate an enrollment",
    "_postman_id": "3f3f8849-ec55-45fc-b47b-adf89b40c5e3",
    "description": "Conclude or inactivate an enrollment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "3c47d0b2-c381-4cbd-85cc-f6605764b288",
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
              "id": "20d76e65-088d-48c8-816d-4d5fd48f939b"
            }
          ]
        },
        {
          "id": "3f16578d-887a-4779-8fee-8978e74ac7c2",
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
              "id": "3dfe879e-6421-4088-9c10-2c0c45a4286d"
            }
          ]
        },
        {
          "id": "bcdf49cc-fdd7-4acd-8cb8-10faeb15277e",
          "name": "conclude-or-inactivate-an-enrollment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/enrollments/id"
              ],
              "query": [
                {
                  "key": "task",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Conclude or inactivate an enrollment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35bfb3c0-ae3a-42a7-bc14-a2a3099fb41e"
            }
          ]
        }
      ]
    }
  ]
}