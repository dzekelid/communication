{
  "info": {
    "name": "Instructure Canvas Users API Get a preference",
    "_postman_id": "b4926b4d-4e9d-4b5a-9722-44f7b7bbe145",
    "description": "Get a preference.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "17c741bf-dd61-4d7e-9d28-afe2ea2cba32",
          "name": "update-multiple-preferences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:type/address/notification_preferences"
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
                  "id": "type",
                  "value": "type",
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
              "id": "5328ce28-be2a-4879-a385-63a6a2b51d48"
            }
          ]
        },
        {
          "id": "fb0b9260-b608-40df-8a12-3fc5cb4fa14d",
          "name": "update-a-preference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:type/address/notification_preferences/:notification"
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
                  "id": "type",
                  "value": "type",
                  "type": "string"
                },
                {
                  "id": "notification",
                  "value": "notification",
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
              "id": "58c9d1e7-10ae-4e26-8ac1-1d9847d6fd90"
            }
          ]
        },
        {
          "id": "b5cd1e4c-5a36-41bc-a7d5-9915b8612770",
          "name": "delete-a-communication-channel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels/type/:address"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a communication channel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22853484-2229-418d-901e-f7ae7682f375"
            }
          ]
        },
        {
          "id": "32d2ba81-5f28-4d52-8dd5-2719823d5fcc",
          "name": "list-preferences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels/type/:address/notification_preferences"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List preferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a568fea-d1ab-469d-aa8b-cdbfeecb1425"
            }
          ]
        },
        {
          "id": "c8b7d723-3420-4be4-850e-d8cd244e20b7",
          "name": "get-a-preference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels/type/:address/notification_preferences/notification"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a preference."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0fb8251b-59aa-4a38-a497-209e166692bc"
            }
          ]
        }
      ]
    }
  ]
}