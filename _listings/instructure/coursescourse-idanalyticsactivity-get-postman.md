{
  "info": {
    "name": "Instructure Canvas Courses API Get course-level participation data",
    "_postman_id": "31bb6386-f4e9-4633-9fd7-f309c570dd48",
    "description": "Get course-level participation data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "5c6d930c-f738-4267-85ad-a7e42acddc11",
          "name": "get-courselevel-participation-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/analytics/activity"
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
            "description": "Get course-level participation data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81af8105-5c80-4c35-8ce0-efb3f8e1f112"
            }
          ]
        }
      ]
    }
  ]
}