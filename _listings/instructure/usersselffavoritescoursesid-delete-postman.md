{
  "info": {
    "name": "Instructure Canvas Users API Remove course from favorites",
    "_postman_id": "2f03bfe3-f863-4b59-9bbc-6fc4d8c02208",
    "description": "Remove course from favorites.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "5e13965c-7878-4ab8-b59a-b98ef020030d",
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
              "id": "47866dfe-e90d-4e8c-b074-4902d5c849e4"
            }
          ]
        },
        {
          "id": "44d561da-12e2-45d9-8b21-6df2aef1977f",
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
              "id": "5de624a0-b7cc-4587-afb8-7e27fe6d3fd3"
            }
          ]
        },
        {
          "id": "e08ebebf-394b-48ca-a8d7-a83f483335c5",
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
              "id": "fd3bc564-7f93-4c1a-8c1d-54e0c2dd6c3e"
            }
          ]
        }
      ]
    }
  ]
}