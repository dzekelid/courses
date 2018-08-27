{
  "info": {
    "name": "Instructure Canvas Courses API Show module item",
    "_postman_id": "e77db4e4-0432-48b9-99d3-6b63dcc2447c",
    "description": "Show module item.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "3462c73c-b568-42d7-9476-65f4d3f2d4aa",
          "name": "list-module-items",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/modules/module_id/items"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "search_term",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "student_id",
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
            "description": "List module items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cfefefb-8915-45ea-b138-596ed5e1f43a"
            }
          ]
        },
        {
          "id": "2bb3d56c-aab8-464a-8589-4e965274667e",
          "name": "create-a-module-item",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/modules/module_id/items"
              ],
              "query": [
                {
                  "key": "module_item[completion_requirement][min_score]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[completion_requirement][type]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[content_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[external_url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[indent]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[new_tab]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[page_url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[position]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[title]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[type]",
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
            "description": "Create a module item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af7b81e7-97e3-46ed-abcf-edf95aa4dd40"
            }
          ]
        },
        {
          "id": "a54d87b2-513d-4823-bb58-e9b87012ea89",
          "name": "show-module-item",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/modules/module_id/items/:id"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "student_id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Show module item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74cd6a12-d05f-4d74-ab8d-b0782080e0c1"
            }
          ]
        },
        {
          "id": "71db8742-3390-4947-b5f4-e06473688a2f",
          "name": "delete-module-item",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/modules/module_id/items/:id"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete module item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9f8ef78-38a9-454e-b962-62fd4590643e"
            }
          ]
        }
      ]
    }
  ]
}