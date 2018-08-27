{
  "info": {
    "name": "Instructure Canvas Courses API Delete module item",
    "_postman_id": "d300277c-9b7f-4559-b477-a2b3dc509200",
    "description": "Delete module item.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "7f67f2b3-96cb-4023-9b17-e1fe30d93ae0",
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
              "id": "dd57478a-f20a-4c9c-94fd-fd59ad0b5015"
            }
          ]
        },
        {
          "id": "98811829-a366-4076-b34b-a78612ff2c00",
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
              "id": "3b0e756a-1eb7-4802-a255-48e2b33da9e2"
            }
          ]
        },
        {
          "id": "de4281c5-e873-4274-8765-62cf50d5e086",
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
              "id": "0c763dac-3138-451d-93c8-607bc831c584"
            }
          ]
        }
      ]
    }
  ]
}