{
  "info": {
    "name": "Instructure Canvas Courses API Delete an external tool",
    "_postman_id": "e0a53b98-8ca2-4f97-9d0b-923162857a5f",
    "description": "Delete an external tool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "cdbfee5b-011e-4ec5-9f70-764a5ee19a68",
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
              "id": "9a0030da-d3f0-4676-9eed-4769095a5bcd"
            }
          ]
        },
        {
          "id": "bd400646-30e6-40dd-b86d-9eeba71205dc",
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
              "id": "2c5fe20e-25fd-4dcb-8920-f9019bcebced"
            }
          ]
        },
        {
          "id": "ac01f6f9-9c5e-46dc-9825-781f7df20411",
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
              "id": "6fe8fd12-4485-4c7c-a415-868b4342c290"
            }
          ]
        },
        {
          "id": "97f6ff3c-1951-4eb4-9480-bfc6a0f8aa21",
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
              "id": "55562226-c62c-42f4-88ff-6efc339013fe"
            }
          ]
        },
        {
          "id": "1ce22195-1b25-4ea3-b24c-f80acb4ce19f",
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
              "id": "49beb870-2b06-4708-b77e-5c6733479b9d"
            }
          ]
        },
        {
          "id": "2e23e258-c1f9-4cc2-9a11-0743605733f9",
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
              "id": "5e62eacc-9178-4c33-9c90-365af6878bb2"
            }
          ]
        }
      ]
    }
  ]
}