{
  "info": {
    "name": "Instructure Canvas Courses API Get a sessionless launch url for an external tool.",
    "_postman_id": "849f5089-ce93-41f6-a759-76e240c09932",
    "description": "Get a sessionless launch url for an external tool..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "e25d8dd0-00f3-4f3c-a9f5-92e5a985b250",
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
              "id": "930983e2-3da6-44a3-92cb-ef57fdc35aee"
            }
          ]
        },
        {
          "id": "69ef2d8e-c232-4a22-889c-1d33b61be61d",
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
              "id": "922d7fba-bc81-44a6-b041-087f0c21ff3a"
            }
          ]
        },
        {
          "id": "04629cbe-41c1-4d9c-a64c-990620a3b00d",
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
              "id": "67fe6368-1dde-4e08-86dc-c7b2355106c4"
            }
          ]
        },
        {
          "id": "b98ec636-a92d-474a-bb6b-377fb6895bb5",
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
              "id": "f9b99e46-6e3e-4ec2-919d-149b75235582"
            }
          ]
        },
        {
          "id": "a3a90f6b-4bfa-4de1-844c-4b65c3e0e298",
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
              "id": "c599188e-1c17-4e04-b5c0-c93bebc99a4b"
            }
          ]
        },
        {
          "id": "49a60e29-692b-452c-a07a-dbc78ce1f72d",
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
              "id": "2410cf34-bfab-4d17-baa9-815b1bc473ec"
            }
          ]
        },
        {
          "id": "eaeaee6f-3df5-47b8-a0af-03209ffcde01",
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
              "id": "918b61aa-7e3e-4ae6-8437-a7f782229908"
            }
          ]
        },
        {
          "id": "50010967-85c6-40d0-8f49-c4a28b927225",
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
              "id": "31a128ab-f2a2-4d94-8f65-995ec30767c7"
            }
          ]
        },
        {
          "id": "d7d719de-df0a-4ae5-812f-f91acfb7c664",
          "name": "get-a-sessionless-launch-url-for-an-external-tool",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/external_tools/sessionless_launch"
              ],
              "query": [
                {
                  "key": "assignment_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "launch_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
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
            "description": "Get a sessionless launch url for an external tool.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a2b5f38-2535-4cb2-9109-ffc61e26e48a"
            }
          ]
        }
      ]
    }
  ]
}