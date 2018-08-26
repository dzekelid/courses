{
  "info": {
    "name": "Instructure Canvas Courses API Delete a question group",
    "_postman_id": "d696f328-b31b-4b40-97d1-51f1433456e9",
    "description": "Delete a question group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "30b3dc52-3e6f-4b27-b320-a89bbb436c59",
          "name": "list-assignment-groups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignment_groups"
              ],
              "query": [
                {
                  "key": "grading_period_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "override_assignment_dates",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "scope_assignments_to_student",
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
            "description": "List assignment groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d20624d-f252-4d5d-9603-b1d785ffb731"
            }
          ]
        },
        {
          "id": "7151a686-3ef2-4bf7-869f-265dc1e0054d",
          "name": "create-an-assignment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignment_groups"
              ],
              "query": [
                {
                  "key": "group_weight",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rules",
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
            "description": "Create an assignment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5e2b9f0-8848-48b7-a63a-7e07373e00de"
            }
          ]
        },
        {
          "id": "63ad74de-fa09-47c1-963e-5301f2092773",
          "name": "get-an-assignment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignment_groups/assignment_group_id"
              ],
              "query": [
                {
                  "key": "grading_period_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "override_assignment_dates",
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
            "description": "Get an assignment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb590328-8a1c-4e6d-aad6-0a93e2cacfb7"
            }
          ]
        },
        {
          "id": "a286f0ba-7459-4e30-bd6f-22c89b8c115b",
          "name": "edit-an-assignment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignment_groups/assignment_group_id"
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
            "description": "Edit an assignment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d74f4cbf-315c-480a-ab64-ea325e1c402c"
            }
          ]
        },
        {
          "id": "bbd271c6-54b7-40e3-ad53-bd30f78c4c70",
          "name": "destroy-an-assignment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignment_groups/assignment_group_id"
              ],
              "query": [
                {
                  "key": "move_assignments_to",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Destroy an assignment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b870710e-6f3f-4e09-9a84-96d5db09d3db"
            }
          ]
        },
        {
          "id": "dc5c052a-f3b4-45b0-9f61-21c3724003ef",
          "name": "list-the-groups-available-in-a-context",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/groups"
              ],
              "query": [
                {
                  "key": "only_own_groups",
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
            "description": "List the groups available in a context.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25360bfb-9af7-4593-a229-2dffd256377e"
            }
          ]
        },
        {
          "id": "2441bfde-c47e-407a-9d27-595480963c46",
          "name": "get-all-outcome-groups-for-context",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/outcome_groups"
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
            "description": "Get all outcome groups for context."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f18a38a2-b4fe-4635-9bc0-f32dbc7a0d4c"
            }
          ]
        },
        {
          "id": "1d2df675-e902-4a3b-b5a1-73a927e7cdcc",
          "name": "show-an-outcome-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/outcome_groups/id"
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
            "description": "Show an outcome group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05b0bb30-f5f4-4da6-be5a-5dcd5a270979"
            }
          ]
        },
        {
          "id": "5b14cba4-0d0e-4412-bf5c-91e4d22a5f35",
          "name": "update-an-outcome-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/outcome_groups/id"
              ],
              "query": [
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "parent_outcome_group_id",
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
            "description": "Update an outcome group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5dc06847-2491-43e1-894e-bc033b0ae6af"
            }
          ]
        },
        {
          "id": "b8d05f25-ca2a-43ea-b6d8-aa5a056ae4fd",
          "name": "delete-an-outcome-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/outcome_groups/id"
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
            "description": "Delete an outcome group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36098529-180d-48fb-a51d-0cb03b538a88"
            }
          ]
        },
        {
          "id": "223f274a-4bad-4762-9318-0afe6d9c6c61",
          "name": "import-an-outcome-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/outcome_groups/id/import"
              ],
              "query": [
                {
                  "key": "source_outcome_group_id",
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
            "description": "Import an outcome group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60e150f0-0d14-4e3b-a0e9-90b729b7cbd7"
            }
          ]
        },
        {
          "id": "d6ec0931-a4e4-4bfd-8274-4e2d46dafa2c",
          "name": "list-linked-outcomes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/outcome_groups/id/outcomes"
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
            "description": "List linked outcomes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7c0bc0a-8069-4999-8731-840a8dba8566"
            }
          ]
        },
        {
          "id": "98f6097c-0517-43f7-bbb8-fff28950141c",
          "name": "createlink-an-outcome",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/outcome_groups/id/outcomes"
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
                  "key": "outcome_id",
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
            "description": "Create/link an outcome."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f6ad625-030e-494c-842e-7c98e9c3212a"
            }
          ]
        },
        {
          "id": "9c2b370c-bc65-4fb4-b665-c1d05d78463d",
          "name": "createlink-an-outcome",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/outcome_groups/id/outcomes/:outcome_id"
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
                  "id": "outcome_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Create/link an outcome."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13ab1236-3c2e-4f5f-99c5-0585b5b165a0"
            }
          ]
        },
        {
          "id": "1f52af21-0422-48b0-92b8-4ebe4e3cc5c0",
          "name": "unlink-an-outcome",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/outcome_groups/id/outcomes/:outcome_id"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                },
                {
                  "id": "outcome_id",
                  "value": "outcome_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unlink an outcome."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db62c36e-9baa-47ac-8378-63bdf3d3debf"
            }
          ]
        },
        {
          "id": "82446625-ab29-4f1c-94f3-fad25dfb1411",
          "name": "list-subgroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/outcome_groups/id/subgroups"
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
            "description": "List subgroups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51d1c164-d180-449d-b8f6-8203fe395399"
            }
          ]
        },
        {
          "id": "7e51c2ef-5c31-4579-88df-02416c44ecb8",
          "name": "create-a-subgroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/outcome_groups/id/subgroups"
              ],
              "query": [
                {
                  "key": "description",
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
            "description": "Create a subgroup."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37b90b1f-d73b-447e-8477-9327f7309d5d"
            }
          ]
        },
        {
          "id": "ea524ed5-d5ab-427a-9cc0-dcd25dbba2bf",
          "name": "create-a-question-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/quizzes/quiz_id/groups"
              ],
              "query": [
                {
                  "key": "quiz_groups[][assessment_question_bank_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "quiz_groups[][name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "quiz_groups[][pick_count]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "quiz_groups[][question_points]",
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
            "description": "Create a question group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "828d4817-1450-4e79-9409-52d54daf9b4a"
            }
          ]
        },
        {
          "id": "445f243c-b711-45a9-981e-cdf6bf72e35c",
          "name": "delete-a-question-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/quizzes/quiz_id/groups/:id"
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
            "description": "Delete a question group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca3d1570-f5a8-4efd-a1a2-5c94e4a67e9d"
            }
          ]
        }
      ]
    }
  ]
}