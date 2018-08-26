{
  "info": {
    "name": "Instructure Canvas Courses API List enrollments",
    "_postman_id": "91695213-3211-474e-a6aa-b3aae4d03dea",
    "description": "List enrollments.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "737f8b58-057f-433b-b5f0-9ca44e3e671f",
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
              "id": "49029d85-a4b9-482c-9207-8bbd1786d6c3"
            }
          ]
        }
      ]
    }
  ]
}