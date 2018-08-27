{
  "info": {
    "name": "Instructure Canvas Users API Update a preference",
    "_postman_id": "ebc169f5-dde5-4165-b50f-f62ce57de4e0",
    "description": "Update a preference.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "13c91485-8580-4593-9a4a-a78ca2b2963e",
          "name": "update-multiple-preferences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:communication_channel_id/notification_preferences"
              ],
              "query": [
                {
                  "key": "notification_preferences[X][frequency]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "communication_channel_id",
                  "value": "communication_channel_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update multiple preferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "263d94f2-a9e2-4060-855a-e0039eb09e8d"
            }
          ]
        },
        {
          "id": "35dd3c9e-2abe-4934-bba4-9c121a2bb719",
          "name": "update-a-preference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:communication_channel_id/notification_preferences/notification"
              ],
              "query": [
                {
                  "key": "notification_preferences[frequency]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "communication_channel_id",
                  "value": "communication_channel_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a preference."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91f46386-50f0-470d-a909-6f5602631fbb"
            }
          ]
        }
      ]
    }
  ]
}