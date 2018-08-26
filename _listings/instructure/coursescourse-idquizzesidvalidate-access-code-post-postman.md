{
  "info": {
    "name": "Instructure Canvas Courses API Validate quiz access code",
    "_postman_id": "53d57e38-5663-44ea-b830-64cef0bd5384",
    "description": "Validate quiz access code.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "3a23cffc-9c44-47c4-afd5-f8d7df574856",
          "name": "validate-quiz-access-code",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/quizzes/id/validate_access_code"
              ],
              "query": [
                {
                  "key": "access_code",
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
            "description": "Validate quiz access code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d59f20ef-e7e6-433f-850c-a95944d4560c"
            }
          ]
        }
      ]
    }
  ]
}