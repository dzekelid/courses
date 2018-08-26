{
  "info": {
    "name": "Instructure Canvas Courses API List group categories for a context",
    "_postman_id": "08d5827b-d879-4b6b-a508-65aa57224128",
    "description": "List group categories for a context.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "80662fa5-15b7-4286-90ed-1d040ffb920a",
          "name": "list-group-categories-for-a-context",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/group_categories"
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
            "description": "List group categories for a context."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ed22f86-9de3-4b3f-bf00-e81219eb560a"
            }
          ]
        }
      ]
    }
  ]
}