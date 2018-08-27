{
  "info": {
    "name": "Instructure Canvas Courses API Create an external tool",
    "_postman_id": "c2a92a09-65a9-4303-9498-218e3d1dae82",
    "description": "Create an external tool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "9cdad046-b0d0-4491-9fdc-6c2cd7c71c0f",
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
              "id": "9bb07f73-86f6-4e9e-99e5-83ae5604a5e7"
            }
          ]
        },
        {
          "id": "13c497ae-8a43-4f1a-a0d7-c09b51091ce9",
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
              "id": "33df5a26-380d-4d9e-80ec-3178a4816407"
            }
          ]
        },
        {
          "id": "a2978c37-9c55-49d2-85b9-07c7397e152a",
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
              "id": "ac79f17f-e4ce-4804-8b80-b0e21db34741"
            }
          ]
        },
        {
          "id": "6fd77fdc-e560-4051-836d-9748ea33e351",
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
              "id": "d312611c-b7ff-416d-a051-688790978e43"
            }
          ]
        },
        {
          "id": "d5ccef0e-b476-4e7e-87b1-65415fe0678e",
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
              "id": "1af6b8bc-d7f1-45c2-9d3f-8d9d5e293c66"
            }
          ]
        }
      ]
    }
  ]
}