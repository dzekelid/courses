{
  "info": {
    "name": "Instructure Canvas Courses API Retrieve captured events",
    "_postman_id": "b112da66-6bef-4caa-a6e1-ce29da4b01f5",
    "description": "Retrieve captured events.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "f4020015-2184-4228-9101-0aa3ae885ad1",
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
              "id": "cfcbae6b-db37-4052-9494-1b1bca87ccde"
            }
          ]
        }
      ]
    }
  ]
}