{
  "info": {
    "name": "Instructure Canvas Courses API Get a single assignment",
    "_postman_id": "e9b512a6-ddfc-4cf3-8c59-6d85bc09a481",
    "description": "Get a single assignment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "4db707e8-23fb-4e99-8b09-fdebcca58c7a",
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
              "id": "bfbf0bb0-fe4b-421f-b08d-074632b1cf14"
            }
          ]
        },
        {
          "id": "81cc5d9a-9814-4afa-96f4-17b12c8b5a48",
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
              "id": "592858cd-ce47-4d73-a379-63b8ada5d7ba"
            }
          ]
        },
        {
          "id": "5c58618b-d40f-43c9-a696-6e177a3ef83c",
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
              "id": "37329a3b-1604-4a5b-b556-9825a3f826d7"
            }
          ]
        },
        {
          "id": "37d61a23-03d1-45af-94ae-813ee70e76c4",
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
              "id": "1fcb5aa6-2605-4d51-bfd7-0ef92dc70d5a"
            }
          ]
        },
        {
          "id": "f7a83c8b-0ffb-4a2c-853b-c09a6503f309",
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
              "id": "f5621c2a-3e72-447b-a730-3160847c8297"
            }
          ]
        },
        {
          "id": "cf6fe270-2070-4a23-92bc-d14bc7e41e4f",
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
              "id": "b0b73a66-f14e-4ecf-9fa8-9232e192d801"
            }
          ]
        },
        {
          "id": "fb4154fd-e070-4bd8-9c1c-e51bd5af7590",
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
              "id": "f44401ca-b69e-4443-b3cb-858b49a347b5"
            }
          ]
        },
        {
          "id": "62e6b189-ccbe-4d2d-8807-e7ec928387b9",
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
              "id": "23d502f3-7925-45d7-9419-76235f71e72b"
            }
          ]
        },
        {
          "id": "0154bd8c-02fb-45c3-9232-c9ad66df40b4",
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
              "id": "b29f7dfd-58dd-4fb3-b86e-e0238f98559f"
            }
          ]
        },
        {
          "id": "a90a95b6-935a-4c13-bc4a-1bb6f96513ef",
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
              "id": "1eb4e8ae-1b83-47ea-95ff-d00fc6334340"
            }
          ]
        },
        {
          "id": "0cb65b78-43ed-41cf-86b7-d9ac91cfc38f",
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
              "id": "2a0f4a31-d708-4a48-971a-266c5c6b3d89"
            }
          ]
        },
        {
          "id": "db11757b-721b-4f8e-aa10-813fca5bd144",
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
              "id": "638e2ffb-5938-4cbe-a4da-2ad031f352a2"
            }
          ]
        },
        {
          "id": "faa2de10-51e2-4468-ace2-8252dbc9221f",
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
              "id": "81b8d093-b30b-430b-b23d-dbf65171380b"
            }
          ]
        },
        {
          "id": "70299949-02c3-43ba-8df0-563817f9cb3d",
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
              "id": "1cacfd2f-9000-4d95-a111-05f6335c6045"
            }
          ]
        },
        {
          "id": "962915c3-8535-4755-9bf6-ad26d271af55",
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
              "id": "2ea7504e-4f62-48e5-b176-44b23912113c"
            }
          ]
        },
        {
          "id": "bec7bcec-13c4-4517-837f-d9c0220870eb",
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
              "id": "189ab92a-52d5-4f3b-8de3-207439989394"
            }
          ]
        },
        {
          "id": "bcbb8f5c-9c95-4bf7-943b-eb4dbf731c03",
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
              "id": "6dc5348a-aa1e-4350-8e6f-40eb327c2946"
            }
          ]
        },
        {
          "id": "6c0b4d43-cfd0-4c09-b27f-3ce975a30ba7",
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
              "id": "11e4e542-45cc-4023-b3f5-1c2373d57cee"
            }
          ]
        },
        {
          "id": "4ad686d1-eb67-495f-95cb-5ca8e50d08f8",
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
              "id": "234b489b-a96f-4539-b1c8-21562726d8b5"
            }
          ]
        },
        {
          "id": "22e2935f-9980-4d4a-a4c4-babbb18f3161",
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
              "id": "e85b63a7-7887-497e-83dc-b39c2f26b925"
            }
          ]
        },
        {
          "id": "fa0548c7-386d-4513-b9e4-4cf6abed8e07",
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
              "id": "4aa24654-a1d7-4e5e-a27e-67fc5ed172de"
            }
          ]
        },
        {
          "id": "690bd022-9ed3-4cd3-b062-c4ea00c821b8",
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
              "id": "b652d44b-0202-4987-98f4-fe0c9b7dd0e1"
            }
          ]
        },
        {
          "id": "37a4081b-342b-4068-9f8b-2da6f6a57da9",
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
              "id": "5de85b21-9c93-4480-92b5-3836b07fd462"
            }
          ]
        },
        {
          "id": "b6123a7f-a4b8-4f0a-838b-5f6b7ac465e0",
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
              "id": "35531fc7-3df7-41c8-8bbb-d3f77c99e886"
            }
          ]
        },
        {
          "id": "7b20a37b-e01b-48bf-80ff-77e20c1ec84c",
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
              "id": "f175ee0a-4e13-42ad-bebe-3b4590b72ccf"
            }
          ]
        },
        {
          "id": "05fa0201-4a0d-4982-b643-de0b1d217636",
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
              "id": "fb6870d7-78e0-4beb-a022-2bd7f576f799"
            }
          ]
        },
        {
          "id": "4d8c413e-2129-45dc-b98b-609ccb88834c",
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
              "id": "6f3b0969-3297-440f-8475-3cecdb21d43b"
            }
          ]
        },
        {
          "id": "283d5da9-5dea-4360-9a43-22bec146a039",
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
              "id": "dffc2b71-ab4d-414c-b8c0-204f6df6dec1"
            }
          ]
        },
        {
          "id": "08c614b5-6e75-49f3-bd6f-d8df021144d6",
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
              "id": "fc7ec903-5d3a-435e-991b-43c54345dbc4"
            }
          ]
        },
        {
          "id": "abc6de0d-a852-4c81-8103-0924d204670b",
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
              "id": "7756c7da-e686-40f1-b44c-728b52acff46"
            }
          ]
        },
        {
          "id": "86e41946-9d76-406b-b02d-e13d9640197f",
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
              "id": "3ad2b14b-7d4f-4c21-a50e-1f1c7f930224"
            }
          ]
        }
      ]
    }
  ]
}