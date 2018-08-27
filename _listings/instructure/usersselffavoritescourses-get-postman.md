{
  "info": {
    "name": "Instructure Canvas Users API List favorite courses",
    "_postman_id": "6a4ff16d-7189-450f-b293-8f5b2d198ad2",
    "description": "List favorite courses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "5ed78d90-9496-48a5-8c1b-391724708491",
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
              "id": "ed29f50a-1654-4d49-9ad3-70e12cc07ec0"
            }
          ]
        },
        {
          "id": "b78a9ecd-c1ae-4fa1-949f-ede2a582d0f6",
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
              "id": "d771b9ae-25ee-42f8-837e-782df34f9f5e"
            }
          ]
        }
      ]
    }
  ]
}