{
  "info": {
    "name": "Learnifier Lists all global course design templates",
    "_postman_id": "f8f0291b-d667-4b27-926e-73e003fdefe7",
    "description": "Lists all global course design templates. Only api callers that have full access can call this method.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "6739d530-8e38-41b0-8981-6f8166ad330f",
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
              "id": "a0327182-ed1f-4407-9efa-74de50952b45"
            }
          ]
        }
      ]
    }
  ]
}