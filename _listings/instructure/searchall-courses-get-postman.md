{
  "info": {
    "name": "Instructure Canvas Utility APIs List all courses",
    "_postman_id": "5b7e3ef9-d7e0-4884-881b-34a5e098ffd3",
    "description": "List all courses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Api",
      "item": [
        {
          "id": "8e53ffff-66cf-4596-95eb-931103156dec",
          "name": "retrieve-assignments-enabled-for-grade-export-to-sis",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "api/sis/accounts/:account_id/assignments"
              ],
              "query": [
                {
                  "key": "course_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ends_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "starts_before",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve assignments enabled for grade export to sis."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e49fd33-3875-46d2-88db-c160a340244e"
            }
          ]
        },
        {
          "id": "2f1b5a17-d9c4-4145-8a20-00c941477da2",
          "name": "retrieve-assignments-enabled-for-grade-export-to-sis1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "api/sis/courses/:course_id/assignments"
              ],
              "query": [
                {
                  "key": "account_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ends_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "starts_before",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve assignments enabled for grade export to sis."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da5cdfb7-da43-42ef-986a-e58bacfc2d83"
            }
          ]
        }
      ]
    },
    {
      "name": "Collaborations",
      "item": [
        {
          "id": "291cf3b0-87af-4bc4-84a1-9785749bc18a",
          "name": "list-members-of-a-collaboration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "collaborations/:id/members"
              ],
              "variable": [
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
            "description": "List members of a collaboration.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ddf3416-204a-4732-8f88-5ef659f78a1b"
            }
          ]
        }
      ]
    },
    {
      "name": "Comm",
      "item": [
        {
          "id": "7d547aad-c38a-4acf-beec-297ca417b7be",
          "name": "list-of-commmessages-for-a-user",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/comm_messages?end_time=%7B%7D&start_time=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of commmessages for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb1f2fcc-b539-4e70-a89d-d5f4fbfb9532"
            }
          ]
        }
      ]
    },
    {
      "name": "Course",
      "item": [
        {
          "id": "a17713c7-7582-4a80-bca9-947603b8e5c7",
          "name": "list-accounts-for-course-admins",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/course_accounts",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List accounts for course admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffa0ab8a-4b53-4dfb-8bed-3b2f5e5f60fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Error",
      "item": [
        {
          "id": "050df8f3-9cc9-4fa4-bb15-2d07bc36dad6",
          "name": "create-error-report",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/error_reports?error[comments]=%7B%7D&error[email]=%7B%7D&error[http_env]=%7B%7D&error[subject]=%7B%7D&error[url]=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create error report."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25c02bf8-35ed-4eb2-9ef5-8ccb930a45bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Jwts",
      "item": [
        {
          "id": "20e937ed-13b6-4855-bdc9-562cb7ae7b7a",
          "name": "create-jwt",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/jwts",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create jwt."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13d3c396-3f93-435b-84a2-c80089d710d7"
            }
          ]
        }
      ]
    },
    {
      "name": "Outcomes",
      "item": [
        {
          "id": "f38b60bf-78d0-494c-bc17-4c3d92ab9512",
          "name": "show-an-outcome",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "outcomes/:id"
              ],
              "variable": [
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
            "description": "Show an outcome."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "639070dc-30ea-4d27-b94b-59e0c0e58ff0"
            }
          ]
        },
        {
          "id": "7b9c5828-c2b6-4708-bce4-b891992cb40a",
          "name": "update-an-outcome",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "outcomes/:id"
              ],
              "query": [
                {
                  "key": "calculation_int",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calculation_method",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "display_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "mastery_points",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ratings[][description]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ratings[][points]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "vendor_guid",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
            "description": "Update an outcome."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59cc63ec-39f1-4afd-a59e-1bf561dfb273"
            }
          ]
        }
      ]
    },
    {
      "name": "Progress",
      "item": [
        {
          "id": "e3abe554-d35d-4a11-b829-c766850df51a",
          "name": "query-progress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "progress/:id"
              ],
              "variable": [
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
            "description": "Query progress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7ad3441-2c49-4afe-af3e-d0cc8e4ba3b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "ff38d3a9-1ef7-4d85-a22b-842f0fa35378",
          "name": "list-all-courses",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/search/all_courses?open_enrollment_only=%7B%7D&public_only=%7B%7D&search=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all courses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e730b5ab-5d45-461e-9937-936206532e06"
            }
          ]
        }
      ]
    }
  ]
}