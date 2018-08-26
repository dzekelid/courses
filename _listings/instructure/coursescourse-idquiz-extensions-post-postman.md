{
  "info": {
    "name": "Instructure Canvas Courses API Set extensions for student quiz submissions",
    "_postman_id": "618ae4b9-6d4a-42c3-99a9-3969b21c5dfa",
    "description": "Set extensions for student quiz submissions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "1b3ce68d-679e-4aae-8d8a-87a6662f27c1",
          "name": "set-extensions-for-student-quiz-submissions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/quizzes/quiz_id/extensions"
              ],
              "query": [
                {
                  "key": "extend_from_end_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "extend_from_now",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "extra_attempts",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "extra_time",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "manually_unlocked",
                  "value": "%7B%7D",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set extensions for student quiz submissions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d8c76b2-2c2e-423b-9260-8ea002af6c16"
            }
          ]
        },
        {
          "id": "91117cb4-e455-4ea6-a42c-a18b1b388ab1",
          "name": "set-extensions-for-student-quiz-submissions1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/quiz_extensions"
              ],
              "query": [
                {
                  "key": "extend_from_end_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "extend_from_now",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "extra_attempts",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "extra_time",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "manually_unlocked",
                  "value": "%7B%7D",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set extensions for student quiz submissions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "042f1953-2378-45f8-beef-2995eb9dec46"
            }
          ]
        }
      ]
    }
  ]
}