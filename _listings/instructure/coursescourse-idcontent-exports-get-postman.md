{
  "info": {
    "name": "Instructure Canvas Courses API List content exports",
    "_postman_id": "fb5b62bf-79ef-4f0e-8d38-df667c63710e",
    "description": "List content exports.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "8b08f351-7415-4f9b-96c2-af53966cdf02",
          "name": "list-content-exports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/content_exports"
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
            "description": "List content exports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eebed1f8-c2fe-47b3-bc63-0ca6ab1f204d"
            }
          ]
        }
      ]
    }
  ]
}