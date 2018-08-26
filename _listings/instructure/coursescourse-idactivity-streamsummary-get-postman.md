{
  "info": {
    "name": "Instructure Canvas Courses API Course activity stream summary",
    "_postman_id": "e8805098-b983-46f8-acff-0546dbe765c0",
    "description": "Course activity stream summary.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "31348f52-178f-4319-ab0f-bba6cf41a748",
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
              "id": "17c62bcf-14ed-46ae-87eb-3411aeed91ea"
            }
          ]
        },
        {
          "id": "7d8311d8-b166-467a-979d-fc433a9b885a",
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
              "id": "19057111-3a4a-49bc-b0c5-2592a93f9f14"
            }
          ]
        },
        {
          "id": "871b2977-01dc-40ce-a20f-faf0477d2c1a",
          "name": "course-activity-stream-summary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/activity_stream/summary"
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
            "description": "Course activity stream summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c48b67f-6e1b-46e8-9de0-4077e7532aa9"
            }
          ]
        }
      ]
    }
  ]
}