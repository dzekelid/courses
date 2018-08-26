{
  "info": {
    "name": "Instructure Canvas Courses API List topic entries",
    "_postman_id": "f6c77a7c-0065-4e12-b2ad-0ef3db9adaf7",
    "description": "List topic entries.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "c208765e-b56b-40c5-9482-db5ed12c7893",
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
              "id": "5fac6e70-1629-4785-85e5-efd4501f6303"
            }
          ]
        },
        {
          "id": "849b445c-d618-4865-b254-2017e7826753",
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
              "id": "a95ca53a-776b-4231-a6d7-21f2515c3d6c"
            }
          ]
        },
        {
          "id": "232b041a-9a99-400d-88af-aaf2b5f7d331",
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
              "id": "25aaa23f-af7e-416c-b531-4bd2aee23738"
            }
          ]
        },
        {
          "id": "2b72394b-765c-4f84-86b4-fa7ab2b4761c",
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
              "id": "f0f9648e-b1bc-49ac-8427-14f762161a5b"
            }
          ]
        },
        {
          "id": "7d591334-7d66-4949-9677-6c386b3cbf38",
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
              "id": "93d9a95c-a868-43d6-a2de-85d39d70a446"
            }
          ]
        },
        {
          "id": "3565eff7-0206-46d4-abd1-9e5df12f1e11",
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
              "id": "83063af0-69ce-4919-949d-5aa1632f7b67"
            }
          ]
        },
        {
          "id": "dc406fe4-7bcc-4146-8517-0087acc68247",
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
              "id": "4b89dec3-eb66-4719-b699-156591596e89"
            }
          ]
        },
        {
          "id": "ae41816e-d153-4efd-9d1a-493cd16beff2",
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
              "id": "f0d48509-509c-4d09-96eb-8a63d0203dc2"
            }
          ]
        },
        {
          "id": "7a82ae46-580f-446b-8ebd-b7a70a065d30",
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
              "id": "04bead21-853b-4de0-872b-6f67e4d7c802"
            }
          ]
        },
        {
          "id": "00bf26c1-a3f9-45ce-a325-0c19c411b8c6",
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
              "id": "0a9ca05d-2b48-4054-ab9f-da6a8f2b246b"
            }
          ]
        },
        {
          "id": "a1f72f61-0fd0-4fae-9c8d-822624425805",
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
              "id": "9db9d374-02e5-42ee-8c01-933da83191b9"
            }
          ]
        },
        {
          "id": "29738b2f-3e55-463d-bf0d-515218b54f91",
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
              "id": "8ccb1161-9de2-4066-9e00-5ed681e194b6"
            }
          ]
        },
        {
          "id": "c0badcda-0eb8-4d79-9a99-d42ca339ef1c",
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
              "id": "0b3e2bd2-9d77-45ac-af5c-966a72536595"
            }
          ]
        },
        {
          "id": "0d21d831-7981-45d7-a69b-f74e46a9ac56",
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
              "id": "4c96cb53-aa0f-4904-ab5e-7e1eb88c1639"
            }
          ]
        },
        {
          "id": "3afd4391-e17c-4a90-8adc-e82db2e3fcf5",
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
              "id": "75955ebc-41d6-448e-8c04-fa4bcbe62d43"
            }
          ]
        },
        {
          "id": "1a66d5a1-c1ca-433d-bca7-656e625eefd2",
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
              "id": "d447ab53-e538-4cb9-abc4-2dd93a486542"
            }
          ]
        },
        {
          "id": "30737ef9-57af-48de-9724-07413ce5342b",
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
              "id": "589728c9-5a02-4a71-a748-efa3380ed9d8"
            }
          ]
        },
        {
          "id": "b56dd6c3-49a3-42e5-b77c-4b60427db6f0",
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
              "id": "65fd6743-56e9-4829-97e9-334c401aee92"
            }
          ]
        },
        {
          "id": "8c58a837-c9dc-430a-8086-b48aa6d2ee3a",
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
              "id": "681e5b9c-f39c-480e-b20c-8816209b0b73"
            }
          ]
        },
        {
          "id": "85402eae-69a4-4b0a-8153-d2668fe07829",
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
              "id": "22b12b66-f1e4-4718-9d6b-410c0cc89aec"
            }
          ]
        },
        {
          "id": "f6eab816-790c-4913-bc22-d1e20133132c",
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
              "id": "56311e90-003a-4487-a108-b5743f42e23f"
            }
          ]
        },
        {
          "id": "bf5e9b31-7d2a-4716-b0fd-839c05b1cf54",
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
              "id": "7b6e9594-4039-4f7e-b94f-59195d15e5de"
            }
          ]
        },
        {
          "id": "c690d76f-caad-4f6a-9128-b723586bee20",
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
              "id": "80e63e74-c5ca-4763-88d0-fcac5eca80db"
            }
          ]
        },
        {
          "id": "a55397b8-d59b-45b4-9fa1-f751b32cf42e",
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
              "id": "ad32c5ac-d269-4198-98c9-06477874674a"
            }
          ]
        },
        {
          "id": "53e7c45f-8f7f-4668-bf03-a62576b46c67",
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
              "id": "c9fc9ded-06ff-4928-bfa1-f95175f02a06"
            }
          ]
        },
        {
          "id": "09d679cf-6582-4650-947b-7a728ad09c2f",
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
              "id": "53f52857-6d8d-4f80-8c48-ca8b1a8b3a79"
            }
          ]
        },
        {
          "id": "819d4d6c-fe5b-4992-80bc-eac962ad6a0e",
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
              "id": "299fd8ea-7f38-41d3-821c-1f5b4a6503e5"
            }
          ]
        },
        {
          "id": "c085ac9c-116e-4b38-8a83-06dd19e8555d",
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
              "id": "92794be9-7e05-404c-8125-7cc09b094a7b"
            }
          ]
        },
        {
          "id": "6389e5fc-4d9c-4dc4-94ca-be906239abec",
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
              "id": "32658c56-0a2a-4c8c-b475-8df18a216f09"
            }
          ]
        },
        {
          "id": "fe5591eb-1666-4e00-a0b2-354e8024e6d3",
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
              "id": "f3bc9eff-1b38-4e35-8276-93b9673c065a"
            }
          ]
        },
        {
          "id": "39b3cae3-2825-492b-899e-0e450529558b",
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
              "id": "7849c62e-3072-4499-ba4c-18c5de387661"
            }
          ]
        },
        {
          "id": "7437de92-df2a-4328-9725-8d921f180381",
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
              "id": "50664bcb-3c5f-40e7-bbf4-4fad236e9656"
            }
          ]
        },
        {
          "id": "c68a5513-8234-4dd5-a328-a5131fa0a67d",
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
              "id": "1aa5713a-4f4d-4f3e-b9d6-0941d5ef1b6b"
            }
          ]
        },
        {
          "id": "2256049e-3099-4137-818a-b5e6326849ee",
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
              "id": "9254aef0-aaed-45c1-9609-344ca618bee1"
            }
          ]
        },
        {
          "id": "68c9633b-7d75-453f-82ca-09d8ab04ba60",
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
              "id": "337f4514-4a88-457d-b030-4668ce175994"
            }
          ]
        },
        {
          "id": "39e74f2d-627e-42a2-b9c2-e96b5aa19b90",
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
              "id": "a261ec57-ee5d-4999-852b-15ad58f9dd68"
            }
          ]
        },
        {
          "id": "8ee13a19-6ece-45d9-a61d-1aca402ec3ed",
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
              "id": "cde5b92b-b157-4e1e-b61c-7647781f6b30"
            }
          ]
        },
        {
          "id": "f334a2ee-05a2-4bd4-9c41-5a2e743053ee",
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
              "id": "ff47369a-0c1b-41a8-9fac-d4d58aa413f5"
            }
          ]
        },
        {
          "id": "a3e04aed-44ac-439b-a744-e5db16e96bef",
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
              "id": "5c3023e9-665d-4236-afc1-c63d31d0580a"
            }
          ]
        },
        {
          "id": "56dd3a8d-bcb2-4093-ad77-fe121489004c",
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
              "id": "9a4c1853-365c-4328-ba83-6ef305290073"
            }
          ]
        },
        {
          "id": "f42b5482-fd57-4c82-adbe-33f5048d62e2",
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
              "id": "9a51c273-6e6b-44de-9052-9ff78c9e439a"
            }
          ]
        },
        {
          "id": "90f2d6b6-e348-42f6-8c92-43c8ab45a9b3",
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
             