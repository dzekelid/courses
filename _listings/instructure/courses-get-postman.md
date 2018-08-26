{
  "info": {
    "name": "Instructure Canvas Courses API List your courses",
    "_postman_id": "6e0f84d3-f7f4-453b-8710-f9a87a3e21d9",
    "description": "List your courses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "0c71ea1a-b392-4452-a441-5df8afdb1e2a",
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
              "id": "a92806bb-8db8-48f2-8dcd-0a6c43a0d62d"
            }
          ]
        }
      ]
    }
  ]
}