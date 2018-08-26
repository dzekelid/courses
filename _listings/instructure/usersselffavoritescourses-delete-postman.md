{
  "info": {
    "name": "Instructure Canvas Users API Reset course favorites",
    "_postman_id": "1da2dffb-9f77-434e-b2a7-7e2e16cc5b0b",
    "description": "Reset course favorites.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "0603605c-21ca-40d8-b650-1254ebc68fe5",
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
              "id": "d8d7d857-6665-4a8f-9142-b7a793b29751"
            }
          ]
        }
      ]
    }
  ]
}