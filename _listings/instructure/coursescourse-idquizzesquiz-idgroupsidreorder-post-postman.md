{
  "info": {
    "name": "Instructure Canvas Courses API Reorder question groups",
    "_postman_id": "5bc57db7-c5bd-4955-b4bd-61c022adfa14",
    "description": "Reorder question groups.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "16196214-bc05-4666-9d59-97e0dbcef560",
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
              "id": "8116c517-6b8d-4dd7-b098-185d5e0d1e57"
            }
          ]
        },
        {
          "id": "e33fb6cc-b2ab-40b4-906b-30e76dec1f37",
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
              "id": "f24f3d37-c49c-435d-9b7e-3125bcd86a93"
            }
          ]
        },
        {
          "id": "c9b43033-9695-4c4c-b6d8-74124a94b0f0",
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
              "id": "5e218a12-b209-42bd-8851-d0f93019a229"
            }
          ]
        },
        {
          "id": "e44ee66d-dd36-4dd0-8a1f-926c387696f4",
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
              "id": "500e1c75-377d-44b6-930c-8fe1ccd4139e"
            }
          ]
        },
        {
          "id": "dff7c6f2-feab-46d1-92c8-3cb75073caa2",
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
              "id": "e46e8156-03a8-473e-ac4d-a6573c4684bf"
            }
          ]
        },
        {
          "id": "cd70117a-abfa-4849-80d1-3c7cdb263938",
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
              "id": "3421f42d-0ba4-4d3d-aa75-39c530c984dd"
            }
          ]
        },
        {
          "id": "5b20836c-1c37-4881-ad8f-484871ee5177",
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
              "id": "0f8e857e-b645-40ad-8fdb-0ef5efb890e9"
            }
          ]
        },
        {
          "id": "8eaa5f43-e250-4b91-9ef4-357276c38ea1",
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
              "id": "1492d36c-c969-4492-aa0d-fa3de49667c5"
            }
          ]
        },
        {
          "id": "664e7a3a-540c-431b-924b-858de3e1dd57",
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
              "id": "214638ec-80de-429a-a346-af9925ec4b25"
            }
          ]
        },
        {
          "id": "7d5ccc3b-373e-444b-8adf-b38767b64ccd",
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
              "id": "e23728fc-463c-4e0e-be4e-fb08afc8c150"
            }
          ]
        },
        {
          "id": "9d4b7563-96b7-479c-8fa1-9060fad639eb",
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
              "id": "3c2b5a22-ca93-49a8-b459-cc1e277d0c18"
            }
          ]
        },
        {
          "id": "d5eae71e-d0fa-44dd-8280-62db6c037ab0",
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
              "id": "0afe4b34-4141-49f7-90dc-c256ef7f3774"
            }
          ]
        },
        {
          "id": "07a2e998-8637-493e-8a83-8164ea49d700",
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
              "id": "643127e1-6691-4101-9020-97a68c5c5ef4"
            }
          ]
        },
        {
          "id": "9bbddb0a-c83e-441f-8dce-8aa296cef0d1",
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
              "id": "684c5f55-fadd-4c3e-9675-bca5ebc59ee9"
            }
          ]
        },
        {
          "id": "16b7d345-9841-43a1-9835-8ef8fd8ec79f",
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
              "id": "49a2e47a-a6f5-4b15-8cb6-0d690b094fec"
            }
          ]
        },
        {
          "id": "a7d7c68b-84ee-45c6-ba9d-751b285d5d79",
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
              "id": "4d645c95-06fa-44e6-aa09-6a89b34d4f5b"
            }
          ]
        },
        {
          "id": "5305ec24-e4e1-451b-a085-c915ac5cba28",
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
              "id": "0af11c8f-11ad-4f30-bc64-6a91cee816da"
            }
          ]
        },
        {
          "id": "245a73bb-e833-4180-87d4-f9f84bfc1ec7",
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
              "id": "69f9b883-60c5-42c4-927f-f39debc75881"
            }
          ]
        },
        {
          "id": "b09abe89-424a-4222-875c-205481093af7",
          "name": "get-a-single-quiz-group",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single quiz group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "883f86f4-8607-4a28-a65b-83174a474628"
            }
          ]
        },
        {
          "id": "85958cb9-935d-48ec-9fc3-f814ebada356",
          "name": "update-a-question-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/quizzes/quiz_id/groups/:id"
              ],
              "query": [
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
            "description": "Update a question group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51dd9a70-687c-461d-bbf4-936b95c672c4"
            }
          ]
        },
        {
          "id": "71e3a268-bf55-4030-90f8-d63424d27712",
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
              "id": "bdb12a31-59d9-4678-a674-a8fed9fb6dad"
            }
          ]
        },
        {
          "id": "b86e4c13-7957-40b6-9238-fe5cfcb1bc18",
          "name": "reorder-question-groups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/quizzes/quiz_id/groups/:id/reorder"
              ],
              "query": [
                {
                  "key": "order[][id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "order[][type]",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reorder question groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d6caf87-0722-4c0b-976f-d47119dd2e23"
            }
          ]
        }
      ]
    }
  ]
}