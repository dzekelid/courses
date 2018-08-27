{
  "info": {
    "name": "Instructure Canvas Courses API Get a single external tool",
    "_postman_id": "32a5e16e-53af-4e26-af2f-c75ad5032116",
    "description": "Get a single external tool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "ec391be4-e49f-43dc-b457-dfe889a6065b",
          "name": "list-external-feeds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_feeds"
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
            "description": "List external feeds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02aae2a1-2ea5-4645-89f5-4fb8ea995464"
            }
          ]
        },
        {
          "id": "72af1bdb-8719-4e9e-b964-b9e85c95fce8",
          "name": "create-an-external-feed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_feeds"
              ],
              "query": [
                {
                  "key": "header_match",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "verbosity",
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
            "description": "Create an external feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d16bf88d-7778-4e24-968c-cacb84c5bbbe"
            }
          ]
        },
        {
          "id": "88a9517a-62c8-4bfd-9150-46e39889addc",
          "name": "delete-an-external-feed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_feeds/external_feed_id"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an external feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1bb46f3-f089-4cdf-a8eb-93687b8e72b3"
            }
          ]
        },
        {
          "id": "c25ac74c-7cf9-47aa-836b-d10baf0d5daa",
          "name": "list-external-tools",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_tools"
              ],
              "query": [
                {
                  "key": "search_term",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "selectable",
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
            "description": "List external tools."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20890fc4-e069-4d0a-93c7-338bb304f586"
            }
          ]
        },
        {
          "id": "10641d33-e08d-412d-9f50-52f41d172cad",
          "name": "create-an-external-tool",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_tools"
              ],
              "query": [
                {
                  "key": "account_navigation[enabled]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "account_navigation[text]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "account_navigation[url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "config_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "config_url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "config_xml",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "consumer_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "course_navigation[default]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "course_navigation[enabled]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "course_navigation[text]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "course_navigation[url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "course_navigation[visibility]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "custom_fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "domain",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "editor_button[enabled]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "editor_button[icon_url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "editor_button[selection_height]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "editor_button[selection_width]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "editor_button[url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "icon_url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "not_selectable",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "privacy_level",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "resource_selection[enabled]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "resource_selection[icon_url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "resource_selection[selection_height]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "resource_selection[selection_width]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "resource_selection[url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "shared_secret",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_navigation[enabled]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_navigation[text]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_navigation[url]",
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
            "description": "Create an external tool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f10e9a84-3ab2-481d-a62b-e8d31eed6cf8"
            }
          ]
        },
        {
          "id": "f98e9562-3200-4c60-ad0c-4ae19a118b52",
          "name": "get-a-single-external-tool",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_tools/external_tool_id"
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
            "description": "Get a single external tool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db687846-72b6-433a-aa12-d5fd79990729"
            }
          ]
        },
        {
          "id": "dc6c88b1-066c-4427-81ee-bc0bc02bdea9",
          "name": "delete-an-external-tool",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_tools/external_tool_id"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an external tool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "067b4704-7335-4a8c-8beb-6083c7df9320"
            }
          ]
        }
      ]
    }
  ]
}