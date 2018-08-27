{
  "info": {
    "name": "Instructure Canvas Users API List assignments for user",
    "_postman_id": "08c4f9ff-ed43-4269-808b-6c6a4b17590f",
    "description": "List assignments for user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "6619bd66-416b-43fd-b98e-9431adbdf050",
          "name": "list-assignments-for-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/courses/course_id/assignments"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List assignments for user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56700066-e4c4-48e0-9035-fe1ec2633391"
            }
          ]
        }
      ]
    }
  ]
}