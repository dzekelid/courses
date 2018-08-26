{
  "info": {
    "name": "Instructure Canvas Courses API Get available quiz IP filters.",
    "_postman_id": "f5a8b181-10d7-423f-b5c6-eb800889a2e9",
    "description": "Get available quiz ip filters..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "b45aa31a-9abe-4eb6-a69d-f8c5a4c6b0f9",
          "name": "get-available-quiz-ip-filters",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/quizzes/quiz_id/ip_filters"
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
            "description": "Get available quiz ip filters.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6566a012-2982-43c7-87c5-773fb49f09ae"
            }
          ]
        }
      ]
    }
  ]
}