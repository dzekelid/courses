{
  "info": {
    "name": "Instructure Canvas Courses API Set extensions for student quiz submissions",
    "_postman_id": "f16a2fee-d33e-4e97-8f07-2fbcd33ad5cb",
    "description": "Set extensions for student quiz submissions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "781e77b2-b7a3-4cfc-8f46-1c8e228cf671",
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
              "id": "308f2787-2560-48df-8006-4e8848dfe922"
            }
          ]
        }
      ]
    }
  ]
}