{
  "info": {
    "name": "Instructure Canvas Courses API List uncollated submission versions",
    "_postman_id": "903bab3c-2698-4f16-a3f5-aeb3fd883c15",
    "description": "List uncollated submission versions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "2ad7d3ae-1acb-42ef-a4a1-e51b143a8adc",
          "name": "details-for-a-given-date-in-gradebook-history-for-this-course",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/gradebook_history/date"
              ],
              "query": [
                {
                  "key": "date",
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
            "description": "Details for a given date in gradebook history for this course."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28dbd1ae-bf6d-4b14-8c2b-c3284183dfb9"
            }
          ]
        },
        {
          "id": "9bea17c9-d492-4caf-b3e7-ec31c55ab035",
          "name": "lists-submissions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/gradebook_history/date/graders/:grader_id/assignments/assignment_id/submissions"
              ],
              "query": [
                {
                  "key": "assignment_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "grader_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists submissions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "770e131d-3618-415f-a7b9-9de89e2077f6"
            }
          ]
        },
        {
          "id": "f29be3f9-540b-4c4c-826e-03ee81b1f036",
          "name": "days-in-gradebook-history-for-this-course",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/gradebook_history/days"
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
            "description": "Days in gradebook history for this course."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d12cd87f-d4e8-495c-960d-0f521ff934f6"
            }
          ]
        },
        {
          "id": "9e8dd55d-c826-40f9-8319-b7ec3e17e39c",
          "name": "list-uncollated-submission-versions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/gradebook_history/feed"
              ],
              "query": [
                {
                  "key": "ascending",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_id",
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
            "description": "List uncollated submission versions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "865143f9-005e-45e0-a81c-b69508a279f3"
            }
          ]
        }
      ]
    }
  ]
}