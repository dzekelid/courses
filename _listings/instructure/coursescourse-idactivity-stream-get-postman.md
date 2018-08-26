{
  "info": {
    "name": "Instructure Canvas Courses API Course activity stream",
    "_postman_id": "9750e453-8799-4f6d-8297-c871d2fd6fb0",
    "description": "Course activity stream.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "c4381c16-d04d-46ba-9879-113cea4aef28",
          "name": "list-your-courses",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/courses?enrollment_role=%7B%7D&enrollment_role_id=%7B%7D&enrollment_type=%7B%7D&include=%5B%7B%7D%5D&state=%5B%7B%7D%5D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List your courses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "afa371c4-3f6d-4903-9b60-ee668f00babc"
            }
          ]
        },
        {
          "id": "d1f8b39e-f09c-43d2-a67c-0614b0ced4dc",
          "name": "course-activity-stream",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/activity_stream"
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
            "description": "Course activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f6812e1-6a4a-4948-ace1-2ade2299982d"
            }
          ]
        }
      ]
    }
  ]
}