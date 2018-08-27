{
  "info": {
    "name": "Instructure Canvas Sections API Redirect to the assignment override for a section",
    "_postman_id": "82c2cfd1-b5ec-4ed8-9971-5b0051edc0e3",
    "description": "Redirect to the assignment override for a section.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sections",
      "item": [
        {
          "id": "c04cbaaf-a07d-4b3c-9a4b-7120839786df",
          "name": "redirect-to-the-assignment-override-for-a-section",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "sections/:course_section_id/assignments/assignment_id/override"
              ],
              "variable": [
                {
                  "id": "course_section_id",
                  "value": "course_section_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Redirect to the assignment override for a section."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "809f4b7c-9405-432d-9072-36e5c071926b"
            }
          ]
        }
      ]
    }
  ]
}