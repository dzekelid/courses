{
  "info": {
    "name": "Instructure Canvas Courses API Create a Group Category",
    "_postman_id": "8d4a6343-0966-44f1-a225-7502d20067f6",
    "description": "Create a group category.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "74a301a0-58a4-40f5-bd1c-e31680677266",
          "name": "list-group-categories-for-a-context",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/group_categories"
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
            "description": "List group categories for a context."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5269e81a-1938-4b62-8ce2-0ae11f0be492"
            }
          ]
        },
        {
          "id": "f31aadc5-71a4-4bd5-9457-42f4a25f4b98",
          "name": "create-a-group-category",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/group_categories"
              ],
              "query": [
                {
                  "key": "auto_leader",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "create_group_count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group_limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "self_signup",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "split_group_count",
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
            "description": "Create a group category."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f932d47-388c-46f9-807e-3e9c02639539"
            }
          ]
        }
      ]
    }
  ]
}