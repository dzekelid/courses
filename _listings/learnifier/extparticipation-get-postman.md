{
  "info": {
    "name": "Learnifier Gets a participation by external id",
    "_postman_id": "6bb4b0ad-5e38-4ae1-9049-24eb401f5edd",
    "description": "Gets a participation by external id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "b4c73758-d612-4d02-a67d-4e877889ae78",
          "name": "coursedesigns.get",
          "request": {
            "url": "http://learnifier.com/coursedesigns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all global course design templates. Only api callers that have full access can call this method."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "357dbe6f-110a-4044-8c7c-80e976ace38a"
            }
          ]
        },
        {
          "id": "7e91479d-cb90-4f47-a091-b9e2318aff90",
          "name": "extparticipation.get",
          "request": {
            "url": "http://learnifier.com/extparticipation?extid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a participation by external id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2de15ffc-6927-45bc-90f3-ddc72e53c55e"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "0968b4e2-5ac6-4636-a056-43d7bd302704",
          "name": "extorgunit.get",
          "request": {
            "url": "http://learnifier.com/extorgunit?extid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the organization unit with the specified external id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85b83776-2dc4-4924-bf68-7e0e12766ad3"
            }
          ]
        }
      ]
    }
  ]
}