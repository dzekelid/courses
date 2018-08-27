{
  "info": {
    "name": "Instructure Canvas Users API Add course to favorites",
    "_postman_id": "a19a88c8-fec2-4d30-adad-d2cd7ba9fc58",
    "description": "Add course to favorites.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "8a199fd7-ec43-445f-bb45-d07783b25e46",
          "name": "list-favorite-courses",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/courses",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List favorite courses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "662cfbea-f9bf-4f9a-b6a4-65d2576102f0"
            }
          ]
        },
        {
          "id": "59b360a9-c977-423c-a7f3-b9a53132fc59",
          "name": "reset-course-favorites",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/courses",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Reset course favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e97ded87-5d54-404a-90d5-a3de019773fc"
            }
          ]
        },
        {
          "id": "176930e0-8350-4fbf-baf6-a91aa359c6e0",
          "name": "add-course-to-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/courses/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add course to favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72069698-7112-49e9-9dc7-eb6cee03adc3"
            }
          ]
        },
        {
          "id": "31716135-fcff-4389-a066-3e9468cf3a0d",
          "name": "remove-course-from-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/courses/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove course from favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "709c0f1f-ac55-4022-93a9-77628c6a5d67"
            }
          ]
        }
      ]
    }
  ]
}