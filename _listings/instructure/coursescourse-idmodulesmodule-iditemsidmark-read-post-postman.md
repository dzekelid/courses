{
  "info": {
    "name": "Instructure Canvas Courses API Mark module item read",
    "_postman_id": "df6bb276-2343-4d09-aac4-bc329fc432e6",
    "description": "Mark module item read.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "dc0e2d3b-9a50-46ba-b670-4b6ed3c69269",
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
              "id": "6796e83d-04b5-4e95-b00c-f5a408234f24"
            }
          ]
        },
        {
          "id": "9f4e364f-95ad-4fe3-b375-88e7a004e2ba",
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
              "id": "abeb1abc-4961-450e-9f60-4aae24d905fd"
            }
          ]
        },
        {
          "id": "4f2dc603-f776-4ab2-a860-5382cb006a99",
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
              "id": "4690f264-b9ac-4820-b6e3-1408105d6c92"
            }
          ]
        },
        {
          "id": "75a1101f-65ef-4aaa-a932-bbd2116279d3",
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
              "id": "f70ff216-cbac-4059-a357-7fc3f54be35f"
            }
          ]
        },
        {
          "id": "52d7fcfd-da2f-46e6-9781-ec2c34bc8945",
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
              "id": "aeb78a24-c212-4f2c-8a95-90a13a694961"
            }
          ]
        },
        {
          "id": "5b549044-c3a3-4dd4-892a-8afe76da2cee",
          "name": "mark-module-item-as-donenot-done",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/modules/module_id/items/:id/done"
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
            "description": "Mark module item as done/not done."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91fd8dff-e4cc-46a6-84b0-aeb041bc78cc"
            }
          ]
        },
        {
          "id": "19663722-e999-473e-bb4a-350eefa7ee1f",
          "name": "mark-module-item-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/modules/module_id/items/:id/mark_read"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Mark module item read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d580857-7b86-4666-a46b-c821136e6f3b"
            }
          ]
        }
      ]
    }
  ]
}