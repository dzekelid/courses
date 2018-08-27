{
  "info": {
    "name": "Instructure Canvas Courses API List external feeds",
    "_postman_id": "b555e530-d39a-4073-9456-21da5ef6d44b",
    "description": "List external feeds.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "158441b5-84c8-43f4-9d95-8d11f3447983",
          "name": "list-external-feeds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_feeds"
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
            "description": "List external feeds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5805453f-c2ce-4243-936a-9949e78dd0ce"
            }
          ]
        }
      ]
    }
  ]
}