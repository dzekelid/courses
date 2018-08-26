{
  "info": {
    "name": "Instructure Canvas Courses API Re-activate an enrollment",
    "_postman_id": "12cb4dbe-d5ab-4af4-b9e4-96524dd18d18",
    "description": "Re-activate an enrollment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "8c952164-8d1e-4b45-825b-947b821cd198",
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
              "id": "5b98def5-6c1d-42df-a8da-1d5dee262068"
            }
          ]
        },
        {
          "id": "afe0da1a-25d8-4156-9d98-14d46a1bd179",
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
              "id": "6a12bf02-fcbf-4f2b-8a68-d2c1591d1b4d"
            }
          ]
        },
        {
          "id": "ce3458b6-5d17-4e83-949d-7a7e90449cc9",
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
              "id": "ec1b8bcd-afb2-454f-8214-b7900f88f579"
            }
          ]
        },
        {
          "id": "1bc0de66-049e-49b1-ae3b-62bf78ae57be",
          "name": "reactivate-an-enrollment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/enrollments/id/reactivate"
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
            "description": "Re-activate an enrollment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "745f71ab-e03d-40e3-a4e2-1d2800d5f8c0"
            }
          ]
        }
      ]
    }
  ]
}