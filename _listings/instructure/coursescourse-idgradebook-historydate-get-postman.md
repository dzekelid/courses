{
  "info": {
    "name": "Instructure Canvas Courses API Details for a given date in gradebook history for this course",
    "_postman_id": "69258f19-9ab8-4305-9c28-7950b08eab95",
    "description": "Details for a given date in gradebook history for this course.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "5f9d7d5c-4fb2-4705-a1ad-5eec9539a032",
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
              "id": "0f4667a3-c52d-4ca3-adbd-359a68ee20f9"
            }
          ]
        }
      ]
    }
  ]
}