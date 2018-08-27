{
  "info": {
    "name": "Instructure Canvas Courses API Edit an external tool",
    "_postman_id": "07c90200-6e3d-46c4-b07f-d474d41fb83b",
    "description": "Edit an external tool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "ff8a7947-3e79-4655-b9b3-59bea19fa72c",
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
              "id": "6d69c421-d7a8-4f82-b40b-94120b4c2873"
            }
          ]
        },
        {
          "id": "1837940f-b8d0-4d84-a7fc-582b468cb3ff",
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
              "id": "17a64132-3034-4319-98cc-772e6356aa3a"
            }
          ]
        },
        {
          "id": "60184b6b-83cc-4475-99ad-9c6dab0e163f",
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
              "id": "a67f0c12-f607-4241-b4d4-da095747da9b"
            }
          ]
        },
        {
          "id": "354f5bb9-c77d-45a0-bd81-4140fe30ca6e",
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
              "id": "38af4ae8-e383-4014-8103-deec552938dc"
            }
          ]
        },
        {
          "id": "8db6d28e-8321-43ad-896b-86c3a9685f6f",
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
              "id": "3278ff69-02b8-4475-953f-3df431501919"
            }
          ]
        },
        {
          "id": "ed3e4853-bb17-4f41-8ed4-eae0dc505e8f",
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
              "id": "261d338c-5393-4129-9b84-212d373a274c"
            }
          ]
        },
        {
          "id": "3693cecb-7ce5-450b-9b04-53a72a8b099a",
          "name": "edit-an-external-tool",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Edit an external tool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f743c4c-0a2f-428c-9290-a5cbce828e2c"
            }
          ]
        },
        {
          "id": "f9265da2-25d7-40de-92b1-748d5da42d28",
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
              "id": "98b5323c-fa2f-4309-ae25-555576625558"
            }
          ]
        }
      ]
    }
  ]
}