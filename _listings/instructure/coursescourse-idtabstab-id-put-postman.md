{
  "info": {
    "name": "Instructure Canvas Courses API Update a tab for a course",
    "_postman_id": "c48b247c-59f8-4355-8c25-9d23d7b7b9a2",
    "description": "Update a tab for a course.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "6d06c823-e9f2-4839-ad84-ea9a45345c15",
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
              "id": "bc85c2a0-84bf-448e-9748-4ae534f3e740"
            }
          ]
        },
        {
          "id": "179d7a73-24a6-4582-853f-658741201410",
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
              "id": "817817f5-76ad-4e1a-8141-d7b3f8bd5a6e"
            }
          ]
        },
        {
          "id": "21e27547-e462-4568-b58d-8bdc13e8153a",
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
              "id": "a7350ff6-8540-42d1-994a-ae84ea1e5ae8"
            }
          ]
        },
        {
          "id": "d9008a95-779c-4e26-8983-fe72d3eb102c",
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
              "id": "2c9dc08a-c4e0-4038-add6-e7dec26f661d"
            }
          ]
        },
        {
          "id": "4d946c49-7614-4836-981d-2b3474796d13",
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
              "id": "5929037c-f16e-40ce-9bf9-e23c0238cff8"
            }
          ]
        },
        {
          "id": "3d29cc15-b2e6-4e86-9dad-42d0a75094aa",
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
              "id": "5c6ac138-b747-413b-873f-f2e72e41d4aa"
            }
          ]
        },
        {
          "id": "148a1142-69e2-4fcc-a280-11a3427aa2a0",
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
              "id": "efd58685-7bd3-44fe-abc3-639a67fd146a"
            }
          ]
        },
        {
          "id": "659ab425-a892-43f1-985e-d5eb413e1799",
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
              "id": "8b5e620c-e938-4850-89e2-dffbe366c9c8"
            }
          ]
        },
        {
          "id": "55174bd2-8401-4804-86b2-7a0852c5003b",
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
              "id": "e891fb92-237d-461e-9ac0-9bd8056da9dc"
            }
          ]
        },
        {
          "id": "6016891d-6cbd-4020-903a-4858cc13d770",
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
              "id": "1098f458-545c-4666-93bd-f2ed10860ad4"
            }
          ]
        },
        {
          "id": "4029cdb5-a698-4550-8e93-ace60de212a0",
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
              "id": "c9671adb-0285-4969-a868-eb83e4b71c96"
            }
          ]
        },
        {
          "id": "b88bc6d7-f02a-4e76-85f7-551bfff38ba9",
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
              "id": "18bae343-ec93-42b7-a92b-7e67bbc85106"
            }
          ]
        },
        {
          "id": "e586ad3b-2478-43fb-b9b9-4ebef6ea890d",
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
              "id": "d635a8da-2691-432b-a0a3-3b22002eb235"
            }
          ]
        },
        {
          "id": "4f9a877c-e7bf-4449-9fd7-6bb08dee612e",
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
              "id": "c37f756c-684a-4b53-8648-61001aa6b606"
            }
          ]
        },
        {
          "id": "0f720f72-2475-42c1-b79b-22fa4ca9b5d9",
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
              "id": "c62976ba-9200-4e18-be22-a7317e5d3176"
            }
          ]
        },
        {
          "id": "d7c501ff-b4d3-4ad6-aec3-ad567734720b",
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
              "id": "67a1fcda-faa2-430e-8f0c-8d50f74bf410"
            }
          ]
        },
        {
          "id": "29e81a7f-cd44-4693-a12a-c6420117879c",
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
              "id": "81c84e06-b6b9-4ffe-a69f-f6f21dd88139"
            }
          ]
        },
        {
          "id": "696f5d99-d390-45ce-be1a-cb6272ccf1f5",
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
              "id": "1001c1c4-7288-4ac7-9cf6-49eec9a85124"
            }
          ]
        },
        {
          "id": "a0f5307a-9afe-491e-bcf4-8d32e53b5ee7",
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
              "id": "d421099e-c6d1-4df2-9dfe-cfae9a1f43e8"
            }
          ]
        },
        {
          "id": "3c7c59b7-0f93-4854-8b63-1cdb5388bbf7",
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
              "id": "8255a89e-0a6f-499e-83cc-fc4b17e147e1"
            }
          ]
        },
        {
          "id": "1cb67efa-8f69-471a-9701-4acb2a98046f",
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
              "id": "e81ec0d6-3844-418b-bfd1-8cce6960c0e3"
            }
          ]
        },
        {
          "id": "9cbd6454-5c11-49be-bca2-cd992f58398b",
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
              "id": "7e7453bb-9bd4-46ac-9bc3-a0292d414438"
            }
          ]
        },
        {
          "id": "b7890010-25fb-4402-a33f-8d39452c3d1c",
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
              "id": "c65bf6cd-b842-4b0d-96d9-63fded85ce73"
            }
          ]
        },
        {
          "id": "75c28cf7-81d1-4a23-9484-ab844b4356ea",
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
              "id": "2cf7c6a9-d118-4739-ac1c-06e7873972c5"
            }
          ]
        },
        {
          "id": "bad89977-394f-4da0-88d0-0d37f8fb0a03",
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
              "id": "5f17a991-bdcd-4bde-92e8-71326dc5d97c"
            }
          ]
        },
        {
          "id": "28e2a862-8d34-4abf-a3fe-ca9fedfb4e64",
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
              "id": "c1fd3ccd-5692-4af7-9e00-f00e503e8db5"
            }
          ]
        },
        {
          "id": "9e348cb4-481d-4510-86cb-0618150551ad",
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
              "id": "95762a2d-1a63-4563-87f7-7b4c998a9f02"
            }
          ]
        },
        {
          "id": "969c8f3c-4104-4f5e-88e4-18eb3363519c",
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
              "id": "77c6ded5-77ab-42d1-a34c-7aeb4c996f8c"
            }
          ]
        },
        {
          "id": "f72ad06c-9707-4d92-a560-b495cd9ee6ee",
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
              "id": "03199a8c-a41c-4aac-a42c-819a3cd1bf0a"
            }
          ]
        },
        {
          "id": "059813e1-c5ad-4479-be5a-ac70ab8ba30e",
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
              "id": "145774a4-10a8-4908-b619-3b087ea39ef7"
            }
          ]
        },
        {
          "id": "20556061-b76a-4f97-b9f7-6b48e7b8933d",
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
              "id": "7f32314e-f8e9-4e8b-835e-2178468da4e9"
            }
          ]
        },
        {
          "id": "541a3d84-d6f0-401d-a29a-386a7b3a808a",
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
              "id": "624ea9e5-48db-4803-98a6-07a830b0632d"
            }
          ]
        },
        {
          "id": "b800d909-de68-4f7a-b615-e1684ad2e059",
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
              "id": "74f09de1-1bcb-40d8-b3e1-acab4dbeabb6"
            }
          ]
        },
        {
          "id": "2229c0eb-57e3-4c66-927f-ef39f892d556",
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
              "id": "0158936c-1088-42ab-af07-8d4464c15505"
            }
          ]
        },
        {
          "id": "5f07d9ed-a8e8-40dc-8f18-f20f3edc03fb",
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
              "id": "2d5d7f7f-8806-4a21-9795-15f6893a7ff0"
            }
          ]
        },
        {
          "id": "8c447dd6-5836-4d31-8ee5-dd73c046bdd5",
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
              "id": "ad64840c-5b7d-44d3-82d7-15faf2ecbbe7"
            }
          ]
        },
        {
          "id": "8b6324e2-aec6-45c9-bc6e-beafdc05431d",
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
              "id": "6c626f03-c415-4a7d-a12e-6c06f0b9e9dd"
            }
          ]
        },
        {
          "id": "97eff062-ca56-405b-9981-e5eee4f115f9",
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
              "id": "1a2abaf2-264d-4184-80fd-ef48e5fd87df"
            }
          ]
        },
        {
          "id": "cd2774b5-f829-42b2-a9fb-a8f507231725",
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
              "id": "2e1cb2dd-4ea9-474e-be80-789a2a3729d3"
            }
          ]
        },
        {
          "id": "5990536b-e6f9-4655-8fd7-151cead3a2b3",
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
              "id": "b7ff48c6-14fc-47cc-a3c7-0ee0be834b45"
            }
          ]
        },
        {
          "id": "1a281254-be3e-44ab-9ffe-7f3ace046cc0",
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
              "id": "f2b7849f-6887-41d8-9bd2-e60116e7f0a5"
            }
          ]
        },
        {
          "id": "c649c00c-0c1e-461e-93e8-c782c584c02f",
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