{
  "info": {
    "name": "Instructure Canvas Courses API Update a module item",
    "_postman_id": "a4f29c27-300b-4b33-b7de-0a4c1880aa88",
    "description": "Update a module item.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "b67875d4-9ad5-4ad6-b7f6-3a9692492986",
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
              "id": "d0669ea4-e7fe-45fa-8316-418bc3ad111b"
            }
          ]
        },
        {
          "id": "76685070-a507-4484-a8f5-9f22da91ce45",
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
              "id": "7d741e2d-af0d-48ca-9d4e-3e9c36388a73"
            }
          ]
        },
        {
          "id": "9e8475b3-3d59-427d-8643-679edf4a32af",
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
              "id": "1bcbdafe-f295-4f32-853b-8bf9ca061fee"
            }
          ]
        },
        {
          "id": "a87b7f9f-a20a-408c-a766-44734f621ea5",
          "name": "update-a-module-item",
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
                  "key": "module_item[module_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[new_tab]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[position]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[published]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "module_item[title]",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a module item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a03a8a45-ff63-4f98-9cc4-dec5e66b0657"
            }
          ]
        },
        {
          "id": "7ba88964-6505-44fd-bfe9-853e97e36e0c",
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
              "id": "cd753ed8-df4a-449b-ad5e-30211d904da9"
            }
          ]
        }
      ]
    }
  ]
}