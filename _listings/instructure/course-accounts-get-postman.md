{
  "info": {
    "name": "Instructure Canvas Utility APIs List accounts for course admins",
    "_postman_id": "e067719d-d00e-4ff5-a338-939b8d4e3cb3",
    "description": "List accounts for course admins.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Api",
      "item": [
        {
          "id": "49a1d6aa-fb69-4e92-8c77-a24d5e706cb1",
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
              "id": "3d0e2245-5536-4da5-b8b4-c63d32d69757"
            }
          ]
        }
      ]
    },
    {
      "name": "Course",
      "item": [
        {
          "id": "1fd34e39-dae5-401d-9513-b9329dcaf1af",
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
              "id": "1b0ac8ce-0c14-4c02-ae93-7bea5b230973"
            }
          ]
        }
      ]
    }
  ]
}