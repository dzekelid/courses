{
  "info": {
    "name": "Instructure Canvas Courses API List custom gradebook columns",
    "_postman_id": "fde74ba2-43b6-4d8c-b00b-efa595531592",
    "description": "List custom gradebook columns.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "fe0a2c7b-82da-4c5a-8e7a-f9947b77c05c",
          "name": "list-custom-gradebook-columns",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/custom_gradebook_columns"
              ],
              "query": [
                {
                  "key": "include_hidden",
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
            "description": "List custom gradebook columns."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "920e81b7-a964-4a5f-8e0a-24574c69ef4e"
            }
          ]
        }
      ]
    }
  ]
}