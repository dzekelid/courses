{
  "info": {
    "name": "Instructure Canvas Courses API Update a topic",
    "_postman_id": "476d5b65-50a8-429c-80da-5e0930534138",
    "description": "Update a topic.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "f404dda9-6561-4c34-9e76-93eb6d5b04ad",
          "name": "list-your-courses",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/courses?enrollment_role=%7B%7D&enrollment_role_id=%7B%7D&enrollment_type=%7B%7D&include=%5B%7B%7D%5D&state=%5B%7B%7D%5D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List your courses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea10a3ef-2ed0-44bd-b2dd-f46c40902b0a"
            }
          ]
        },
        {
          "id": "d67ddb05-b3de-482e-8a1a-8fee76992f47",
          "name": "course-activity-stream",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/activity_stream"
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
            "description": "Course activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "418afc9f-aac3-4dbe-a849-9cab43225fe0"
            }
          ]
        },
        {
          "id": "ee48fbec-f2dc-4bbe-9fc5-66c708e1a3e7",
          "name": "course-activity-stream-summary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/activity_stream/summary"
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
            "description": "Course activity stream summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d43c7b43-468e-44dd-8bd2-fc3ed9f5bd63"
            }
          ]
        },
        {
          "id": "6df31f2e-b898-443d-90f6-0597ca0b1d89",
          "name": "get-courselevel-participation-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/analytics/activity"
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
            "description": "Get course-level participation data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82491c96-7e97-4485-9f0f-89b95fccf6bd"
            }
          ]
        },
        {
          "id": "72fb9d2f-dbc9-4914-aeca-34fd50d94922",
          "name": "get-courselevel-assignment-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/analytics/assignments"
              ],
              "query": [
                {
                  "key": "async",
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
            "description": "Get course-level assignment data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2d288c0-a54b-4f33-9126-fee74441b1be"
            }
          ]
        },
        {
          "id": "03a5339f-e823-43fc-aea6-3c3e9c5c4d28",
          "name": "get-courselevel-student-summary-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/analytics/student_summaries"
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
            "description": "Get course-level student summary data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5966573e-2cf6-485a-b4d9-713016862697"
            }
          ]
        },
        {
          "id": "cf0191d3-5463-4828-8983-2ccf0abb6c77",
          "name": "get-userinacourselevel-participation-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/analytics/users/student_id/activity"
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
            "description": "Get user-in-a-course-level participation data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "039a3106-5b86-4f58-b20e-3adae79b3255"
            }
          ]
        },
        {
          "id": "e2f8ffa2-e578-462b-8fdb-99a2a51dc3f9",
          "name": "get-userinacourselevel-assignment-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/analytics/users/student_id/assignments"
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
            "description": "Get user-in-a-course-level assignment data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42dd6c05-5e93-45a8-948b-57a0537f7e9b"
            }
          ]
        },
        {
          "id": "252d8774-bbdc-4c79-9431-4738c7a62557",
          "name": "get-userinacourselevel-messaging-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/analytics/users/student_id/communication"
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
            "description": "Get user-in-a-course-level messaging data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d111e48-a8bb-4322-9953-190e93f739e7"
            }
          ]
        },
        {
          "id": "2871e9e2-8f26-40e5-873f-11a328ea7753",
          "name": "list-assignments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments"
              ],
              "query": [
                {
                  "key": "bucket",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "needs_grading_count_by_section",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "override_assignment_dates",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search_term",
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
            "description": "List assignments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9376248d-d372-4ed9-871d-0beb6118a5d3"
            }
          ]
        },
        {
          "id": "c66c50a3-a8d5-42fd-b6c8-8f2e10a396ae",
          "name": "create-an-assignment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments"
              ],
              "query": [
                {
                  "key": "assignment[allowed_extensions",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "assignment[assignment_group_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[assignment_overrides",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "assignment[automatic_peer_reviews]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[description]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[due_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[external_tool_tag_attributes]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[grade_group_students_individually]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[grading_standard_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[grading_type]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[group_category_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[integration_data]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[integration_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[lock_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[muted]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[notify_of_update]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[only_visible_to_overrides]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[peer_reviews]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[points_possible]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[position]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[published]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[submission_types",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "assignment[turnitin_enabled]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[turnitin_settings]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[unlock_at]",
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
            "description": "Create an assignment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1850abb8-df46-4d51-9e73-80a3c8e709bc"
            }
          ]
        },
        {
          "id": "c7cf083a-9521-498d-9a1a-dedaf8e14710",
          "name": "list-gradeable-students",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/gradeable_students"
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
            "description": "List gradeable students."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed652b15-b73f-49e5-ad7b-14de86ba894d"
            }
          ]
        },
        {
          "id": "cb904b41-84c3-4812-8ba5-63e622e86e2a",
          "name": "list-students-selected-for-moderation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/moderated_students"
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
            "description": "List students selected for moderation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79c530ae-24a2-44cb-940c-e9f1c8c1d3e7"
            }
          ]
        },
        {
          "id": "807027e6-2202-4d6e-baaa-46624f4df46a",
          "name": "select-students-for-moderation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/moderated_students"
              ],
              "query": [
                {
                  "key": "student_ids",
                  "value": "%5B%7B%7D%5D",
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
            "description": "Select students for moderation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eff7bf4b-4bc2-4615-9633-8a5d7b644014"
            }
          ]
        },
        {
          "id": "0c97d613-c98e-400f-b368-d43e40157616",
          "name": "list-assignment-overrides",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/overrides"
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
            "description": "List assignment overrides."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f2775b6-5ccd-4c63-8089-2d9d91b36ec3"
            }
          ]
        },
        {
          "id": "d3f650a7-ce46-4df9-9103-562404d340ca",
          "name": "create-an-assignment-override",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/overrides"
              ],
              "query": [
                {
                  "key": "assignment_override[course_section_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment_override[due_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment_override[group_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment_override[lock_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment_override[student_ids",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "assignment_override[title]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment_override[unlock_at]",
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
            "description": "Create an assignment override."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80d6f7b7-abbe-44a9-9565-181597d6ff7f"
            }
          ]
        },
        {
          "id": "2b88ad42-64ee-455b-9507-605a40e28c1b",
          "name": "get-a-single-assignment-override",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/overrides/:id"
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
            "description": "Get a single assignment override."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "134d1530-61ca-499b-aa4f-0985a5edc56c"
            }
          ]
        },
        {
          "id": "12104731-c70c-482a-b0fa-18249213027c",
          "name": "update-an-assignment-override",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/overrides/:id"
              ],
              "query": [
                {
                  "key": "assignment_override[due_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment_override[lock_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment_override[student_ids",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "assignment_override[title]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment_override[unlock_at]",
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
            "description": "Update an assignment override."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "501816bb-4a95-4046-b78c-7e26dd315542"
            }
          ]
        },
        {
          "id": "d4c1352a-a2e8-46c2-bc80-4a7d5e0a3c5f",
          "name": "delete-an-assignment-override",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/overrides/:id"
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
            "description": "Delete an assignment override."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fc5a077-bc7e-4f3d-8341-0176de677e77"
            }
          ]
        },
        {
          "id": "fa4857a5-9a66-4970-8651-9e4444c631d0",
          "name": "get-all-peer-reviews",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/peer_reviews"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
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
            "description": "Get all peer reviews."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba606b5a-4ac2-4121-a8ca-7b08e71e35cf"
            }
          ]
        },
        {
          "id": "107123fe-4b92-468c-9e76-0f237b759197",
          "name": "publish-provisional-grades-for-an-assignment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/provisional_grades/publish"
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
            "description": "Publish provisional grades for an assignment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f36c6d16-6852-491e-a2ee-64b8c729a32e"
            }
          ]
        },
        {
          "id": "2b6b6b02-7086-4f29-a94f-b7b4fd58947d",
          "name": "show-provisional-grade-status-for-a-student",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/provisional_grades/status"
              ],
              "query": [
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
            "description": "Show provisional grade status for a student."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57f0c283-3e04-46e1-af6c-022ee827f4d3"
            }
          ]
        },
        {
          "id": "b2740e87-287e-4ccf-8a07-9fae018de715",
          "name": "copy-provisional-grade",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/provisional_grades/:provisional_grade_id/copy_to_final_mark"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                },
                {
                  "id": "provisional_grade_id",
                  "value": "provisional_grade_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Copy provisional grade."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad7ed3d1-6b3d-475c-878c-44e666d2d313"
            }
          ]
        },
        {
          "id": "7a89a8e4-5cbb-42f0-9a42-afa2ad56ad9b",
          "name": "select-provisional-grade",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/provisional_grades/:provisional_grade_id/select"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                },
                {
                  "id": "provisional_grade_id",
                  "value": "provisional_grade_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Select provisional grade."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f3f5f86-58ed-41d4-9318-c58e84b0877c"
            }
          ]
        },
        {
          "id": "89e9d723-a6ea-4eeb-8d54-342c2046df94",
          "name": "list-assignment-submissions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/submissions"
              ],
              "query": [
                {
                  "key": "grouped",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
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
            "description": "List assignment submissions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ad6e2c1-f61f-476b-a887-73915c5f458b"
            }
          ]
        },
        {
          "id": "9efe9d92-a5f4-45d1-8dec-20bcd4eacd4b",
          "name": "submit-an-assignment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/submissions"
              ],
              "query": [
                {
                  "key": "comment[text_comment]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "submission[body]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "submission[file_ids",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "submission[media_comment_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "submission[media_comment_type]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "submission[submission_type]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "submission[url]",
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
            "description": "Submit an assignment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7981137a-503e-4c56-bbfd-f9f37bcf64a4"
            }
          ]
        },
        {
          "id": "a4a11598-e656-4664-a607-9e91ce47375c",
          "name": "grade-or-comment-on-multiple-submissions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/submissions/update_grades"
              ],
              "query": [
                {
                  "key": "grade_data[student_id][file_ids",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "grade_data[student_id][group_comment]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "grade_data[student_id][media_comment_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "grade_data[student_id][media_comment_type]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "grade_data[student_id][posted_grade]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "grade_data[student_id][rubric_assessment]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "grade_data[student_id][text_comment]",
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
            "description": "Grade or comment on multiple submissions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4960ccab-89e7-42e9-8a12-1fc6a3611c5a"
            }
          ]
        },
        {
          "id": "d1a3bf92-00d8-4d46-a442-8811a0fc9188",
          "name": "get-all-peer-reviews1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/submissions/:submission_id/peer_reviews"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
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
                  "id": "submission_id",
                  "value": "submission_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all peer reviews."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc7b49d1-584a-4bf1-ab4e-1b79236225f1"
            }
          ]
        },
        {
          "id": "156fbd68-4493-4c24-a0dd-8e30f6501869",
          "name": "create-peer-review",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/submissions/:submission_id/peer_reviews"
              ],
              "query": [
                {
                  "key": "user_id",
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
                  "id": "submission_id",
                  "value": "submission_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create peer review."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0f89c04-b476-4aa0-ba13-1ae4edbd051d"
            }
          ]
        },
        {
          "id": "be55ab02-2ddb-4024-8ffa-8374026c117f",
          "name": "create-peer-review",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/submissions/:submission_id/peer_reviews"
              ],
              "query": [
                {
                  "key": "user_id",
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
                  "id": "submission_id",
                  "value": "submission_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Create peer review."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08a9eca1-99f9-4773-91d2-a67b591b5208"
            }
          ]
        },
        {
          "id": "a7461cfc-9a55-4026-b48b-04aaeda9b31e",
          "name": "get-a-single-submission",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/submissions/:user_id"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
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
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single submission."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40d66a30-c908-4cc3-a696-99aff604e84a"
            }
          ]
        },
        {
          "id": "7bba35ac-0d61-45d0-998e-f66cb0b3e15d",
          "name": "grade-or-comment-on-a-submission",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/submissions/:user_id"
              ],
              "query": [
                {
                  "key": "comment[file_ids",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "comment[group_comment]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "comment[media_comment_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "comment[media_comment_type]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "comment[text_comment]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include[visibility]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rubric_assessment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "submission[excuse]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "submission[posted_grade]",
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
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Grade or comment on a submission."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d303856-8201-4bbd-88cf-2740074512c0"
            }
          ]
        },
        {
          "id": "1af22a49-1ed8-4cbd-b668-0c1939b672d1",
          "name": "upload-a-file",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/submissions/:user_id/comments/files"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload a file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c94b2dfa-741c-4941-9c79-b673b49b5208"
            }
          ]
        },
        {
          "id": "6b302ede-df39-487b-bc0f-61fdc4064127",
          "name": "upload-a-file1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/submissions/:user_id/files"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload a file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4400a7f4-8b6d-45c7-9af8-4b0e31ccb858"
            }
          ]
        },
        {
          "id": "416df41f-d2a7-412b-b80e-162300f0a83f",
          "name": "mark-submission-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/submissions/:user_id/read"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Mark submission as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc66d100-b946-42cb-8efc-d6944fc19b37"
            }
          ]
        },
        {
          "id": "b3a2a6b0-7da6-495a-ba25-f23900fbcbbf",
          "name": "mark-submission-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/assignment_id/submissions/:user_id/read"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Mark submission as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27f17b92-7b7f-4e7a-a1f8-59c7fd13de7a"
            }
          ]
        },
        {
          "id": "448a077c-91f6-42e8-bfc1-7289269a020d",
          "name": "get-a-single-assignment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/id"
              ],
              "query": [
                {
                  "key": "all_dates",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "needs_grading_count_by_section",
                  "value": "%7B%7D",
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
            "description": "Get a single assignment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1140e2bb-450c-4485-8168-4855798d881f"
            }
          ]
        },
        {
          "id": "409d0a19-4401-4c02-8908-b67d87684358",
          "name": "edit-an-assignment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/id"
              ],
              "query": [
                {
                  "key": "assignment[allowed_extensions",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "assignment[assignment_group_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[assignment_overrides",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "assignment[automatic_peer_reviews]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[description]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[due_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[external_tool_tag_attributes]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[grade_group_students_individually]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[grading_standard_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[grading_type]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[group_category_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[integration_data]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[integration_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[lock_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[muted]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[notify_of_update]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[only_visible_to_overrides]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[peer_reviews]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[points_possible]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[position]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[published]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[submission_types",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "assignment[turnitin_enabled]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[turnitin_settings]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment[unlock_at]",
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
            "description": "Edit an assignment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ddabc63-d485-4681-a8a6-e5ddba871ca4"
            }
          ]
        },
        {
          "id": "6ac61eec-ea89-43d6-9629-b785885ff7b5",
          "name": "delete-an-assignment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignments/id"
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
            "description": "Delete an assignment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f35bfa5f-455e-456b-8d9c-63cc6f49181f"
            }
          ]
        },
        {
          "id": "8f9d5fc4-9ff0-42be-9283-f4ee06d3bdb4",
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
              "id": "d1d60731-4dfc-4697-aea8-82f52eb2f31d"
            }
          ]
        },
        {
          "id": "a3d90e1f-9245-48b2-a112-19a7750d3e9d",
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
              "id": "eafadf85-8251-4853-8623-99422ab66f39"
            }
          ]
        },
        {
          "id": "fdde6a30-5dae-466d-beb8-ed8669e457f8",
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
                  "ke