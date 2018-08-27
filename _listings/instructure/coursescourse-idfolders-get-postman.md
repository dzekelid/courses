{
  "info": {
    "name": "Instructure Canvas Courses API List all folders",
    "_postman_id": "d3095903-7d5e-4d8e-86ab-f4f206bdf0e5",
    "description": "List all folders.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "8d387e80-67b2-4e27-99e2-7fded7b375bf",
          "name": "list-all-folders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/folders"
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
            "description": "List all folders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41460d50-f79f-4503-9717-48524f5fe5bf"
            }
          ]
        }
      ]
    }
  ]
}