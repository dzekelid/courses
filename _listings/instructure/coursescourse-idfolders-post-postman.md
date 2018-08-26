{
  "info": {
    "name": "Instructure Canvas Courses API Create folder",
    "_postman_id": "3d733682-d8a0-404a-806a-60b46a2da836",
    "description": "Create folder.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "ab709769-1f3e-42ef-8ce2-af291d6f1a28",
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
              "id": "86601d6c-f2af-4da9-aca4-ebb066c4ef58"
            }
          ]
        },
        {
          "id": "5a9a351b-3107-450d-a81e-a38fdcebee58",
          "name": "create-folder",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/folders"
              ],
              "query": [
                {
                  "key": "hidden",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "locked",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lock_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "parent_folder_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "parent_folder_path",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "unlock_at",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create folder."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbaa8d1c-9f97-424a-b485-dbc00058db6b"
            }
          ]
        }
      ]
    }
  ]
}