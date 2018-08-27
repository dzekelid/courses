{
  "info": {
    "name": "Instructure Canvas Courses API Create a module item",
    "_postman_id": "c4cad3d6-db72-4569-8cf0-924354fad38d",
    "description": "Create a module item.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "cab82945-c7b7-485e-b2be-40d81904811e",
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
              "id": "80803dd5-2112-4add-b955-55ff02250cd1"
            }
          ]
        },
        {
          "id": "02181ec0-9faf-494d-93a7-2e8b7e0da0dc",
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
              "id": "a1591ec3-3bff-4c5a-b805-8b3510c1f16c"
            }
          ]
        }
      ]
    }
  ]
}