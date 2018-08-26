{
  "info": {
    "name": "Instructure Canvas Courses API Get module item sequence",
    "_postman_id": "0f05443c-9aaf-4255-bfa5-bb79767d2781",
    "description": "Get module item sequence.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "4ac8ecc6-1f64-4a2c-9828-bcb1cfcc5724",
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
              "id": "b144eabd-1c2a-413d-a130-6b9702f9d496"
            }
          ]
        },
        {
          "id": "7122c169-b210-4abe-8a98-1b8cd52e4a5f",
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
              "id": "57d9ad91-d55f-42c2-bcbd-1c3830226598"
            }
          ]
        },
        {
          "id": "5ddd2321-391e-4c05-925b-cdd2fbf4ca1d",
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
              "id": "dff8a878-7ab9-4c4f-b932-48617cd598c5"
            }
          ]
        },
        {
          "id": "3aabfc4c-a0ac-4987-a54c-4d099f027325",
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
              "id": "a2cf1528-6c88-42ae-9ac2-d549b9119f99"
            }
          ]
        },
        {
          "id": "5619ceb9-b780-47a7-aedd-ec60ce47620b",
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
              "id": "d1a2a49c-8e50-4528-a35c-96efd63c46d0"
            }
          ]
        },
        {
          "id": "b7b5e463-455e-4844-860b-894d142bcd8b",
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
              "id": "7fcd13ca-5ea5-4788-b8b7-74840a29affc"
            }
          ]
        },
        {
          "id": "e63f84d2-fd83-4004-8c8a-28e15da55071",
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
              "id": "d140414b-e307-4bf4-b02c-a941f778b2ed"
            }
          ]
        },
        {
          "id": "ff533841-84be-45d9-8886-1dad3d70e200",
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
              "id": "48c2b763-c5a8-4061-a33c-d0efde0cb9b2"
            }
          ]
        },
        {
          "id": "daf2fdd0-c274-4dd8-b06f-5899a9a6ded2",
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
              "id": "ba490785-83c0-403f-ab09-81d9f5fed246"
            }
          ]
        },
        {
          "id": "6e293641-0433-4ebf-b26c-af2d93d57bc7",
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
              "id": "5dad8363-dfab-4cc9-8b79-9909264da0b0"
            }
          ]
        },
        {
          "id": "e1408a53-c5b0-4e1d-8798-108b634db1b5",
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
              "id": "46050921-8dc1-4bf8-9c79-c5b4faaab4e8"
            }
          ]
        },
        {
          "id": "3a6d2688-c3ab-4054-ae03-7cc25a71431b",
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
              "id": "f450bcde-84a3-434e-92ee-e490b8bf46f5"
            }
          ]
        },
        {
          "id": "6d5c9e2e-5b35-479d-ae32-783fee5c79c3",
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
              "id": "fb29656a-c619-45fe-adc2-09289a9f8fdb"
            }
          ]
        },
        {
          "id": "0b307839-d644-45a2-8e91-b232ae417b88",
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
              "id": "beee971e-dfdb-409e-9db6-3e5c14e43afb"
            }
          ]
        },
        {
          "id": "f22cc585-4612-484d-8f03-f503dc9894e3",
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
              "id": "e2a5fa2c-4a24-4f5f-8944-745fe53a446c"
            }
          ]
        },
        {
          "id": "00d539e7-538c-463f-a816-36f293cec57c",
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
              "id": "f4deb1d4-4845-4c6a-b981-97837ea0c907"
            }
          ]
        },
        {
          "id": "8e2c1bf8-6389-4a86-b3e4-2a6ac533b704",
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
              "id": "5bfbac5d-182f-4703-af93-442be42baf11"
            }
          ]
        },
        {
          "id": "b6a607db-74ea-4079-a826-7b3403b9c662",
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
              "id": "7a10c457-31fe-406b-9b09-bc1155afc51d"
            }
          ]
        },
        {
          "id": "4d1f97ea-2f14-45d5-b8f6-d8f49975875b",
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
              "id": "b6dc147d-7547-42b9-9de0-15895067e6d8"
            }
          ]
        },
        {
          "id": "d0db244d-c656-49f8-8956-abbff848b0a5",
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
              "id": "22b54eca-2492-42a9-9b6e-2dd20a97cab7"
            }
          ]
        },
        {
          "id": "4b57b129-0711-4a32-b5ff-35e1a15d19b7",
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
              "id": "970710c2-3423-4cec-9236-1aa7ac09764e"
            }
          ]
        },
        {
          "id": "2d7c8a3b-0056-42f4-b2e7-b32de484a072",
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
              "id": "3e75a98c-f0e8-427c-ac3a-b097229248be"
            }
          ]
        },
        {
          "id": "1f702a3b-7647-4d8a-87fc-866b34c4de46",
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
              "id": "ef61a4b5-4a92-4a63-9902-4cec5c07ce13"
            }
          ]
        },
        {
          "id": "3c1466dc-19ec-40ba-8c9c-33c8a44ce7f6",
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
              "id": "d7a0ad6e-ab7c-4e2b-9a0e-66ee3d8c0359"
            }
          ]
        },
        {
          "id": "ccbb1e71-3c5c-4608-ab64-95defd48eca9",
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
              "id": "7669324f-1858-4f30-870c-1d8d4effdcb4"
            }
          ]
        },
        {
          "id": "ed165757-d1a7-4284-9b7d-5c36afe00f4a",
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
              "id": "d5208aab-aa90-41cd-9aa4-55726ceda2d4"
            }
          ]
        },
        {
          "id": "00501e6d-60b3-4cb2-ba49-78f1859f50a3",
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
              "id": "f6253c0a-28aa-40f7-b64b-5cb43d12e30f"
            }
          ]
        },
        {
          "id": "bd303b91-8184-40bb-8a6f-0ff0dc329218",
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
              "id": "7bb9c1ef-c230-4e50-854d-375f9ebbaefa"
            }
          ]
        },
        {
          "id": "e557eacc-90a7-4d13-b348-3341ef524b58",
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
              "id": "3836f7d4-15cb-44b0-8c15-87bc331f0a22"
            }
          ]
        },
        {
          "id": "cf7087cc-85bd-49f6-94df-9388ee502d75",
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
              "id": "0fde644b-aa8e-4b2c-be2f-da8fcf353924"
            }
          ]
        },
        {
          "id": "29ae22ab-8c24-407b-ab92-ed31db9feb1a",
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
              "id": "215852fe-8d56-4767-8c3e-1365e22fe451"
            }
          ]
        },
        {
          "id": "c631d9fc-1db4-4663-94fa-34448aefe8e9",
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
              "id": "1fb6fcf2-1e33-4ea5-952c-edfd94499e8d"
            }
          ]
        },
        {
          "id": "d45e7fe5-1f9c-4836-8f8d-b7372f3c7cfd",
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
              "id": "c931868d-bbb5-4dce-a752-1d4a123ff887"
            }
          ]
        },
        {
          "id": "e4f36cf9-ef03-43d0-a1eb-e1d7cc11f2b9",
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
              "id": "0a69bb60-6355-46da-9987-1ff2e24a19aa"
            }
          ]
        },
        {
          "id": "1c24cc40-7ed6-4921-bb63-25b005ee27fa",
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
              "id": "941656e4-ab0d-4a26-8b0c-159df5e8cf76"
            }
          ]
        },
        {
          "id": "4f2f28b7-5eba-4f9c-a2d4-85cdb6126276",
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
              "id": "f2033063-ad3b-441e-aa5c-7d4d517e34de"
            }
          ]
        },
        {
          "id": "52d670d7-4eee-4d9d-8606-af23e75d39ba",
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
              "id": "c7517be6-a309-4fda-9919-c5da333e8355"
            }
          ]
        },
        {
          "id": "afca1271-2878-4050-996c-5876d7c7ff0e",
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
              "id": "a5983fbb-02cf-4cf4-8a7e-d3195e4cfeea"
            }
          ]
        },
        {
          "id": "15111c45-4dda-484f-900c-a92b2d0255b3",
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
              "id": "9f641b0b-0bdd-4145-989e-d6ed5ffe8e21"
            }
          ]
        },
        {
          "id": "8a6d1be8-154c-4f9f-8d86-a3eb109955ac",
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
              "id": "e9548b01-06b1-47b9-b6f9-6967f86cac56"
            }
          ]
        },
        {
          "id": "d5bb8a73-dcef-4602-bec7-d9c2d2fd1712",
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
              "id": "3386aa22-8542-4b87-b667-30bfbf44e8eb"
            }
          ]
        },
        {
          "id": "b23dd878-37f8-4b31-93ce-c94cbfd06ce2",
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
 