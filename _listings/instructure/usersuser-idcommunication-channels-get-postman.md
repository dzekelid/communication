{
  "info": {
    "name": "Instructure Canvas Users API List user communication channels",
    "_postman_id": "4c51d024-bca2-48b2-83c8-c2c1df6f1324",
    "description": "List user communication channels.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "9d7f1bad-ef29-4aee-ab17-ef10137f9152",
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
              "id": "22fc48e1-d09c-4c9f-bbbd-00efc0c862be"
            }
          ]
        },
        {
          "id": "28c9aeda-a615-42ec-aff7-231b7a5bafa5",
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
              "id": "811f459e-ee1e-4ab7-a645-e40fe1ecb2cf"
            }
          ]
        },
        {
          "id": "5eb757a7-42a7-4270-8672-a10c2c6bbb08",
          "name": "update-preferences-by-category",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:communication_channel_id/notification_preference_categories/category"
              ],
              "query": [
                {
                  "key": "category",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
            "description": "Update preferences by category."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ac3c32c-97ad-4aa5-8d4d-d962db463854"
            }
          ]
        },
        {
          "id": "feecdc1b-d3d4-469f-91d9-13cdd110e0e2",
          "name": "update-multiple-preferences1",
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
              "id": "fa260a8c-05c9-42d2-98eb-0b5f8240f13e"
            }
          ]
        },
        {
          "id": "3bc7b12f-33c5-4b4f-8403-201a820b74bb",
          "name": "update-a-preference1",
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
              "id": "d80974ee-5398-4fd4-b86a-70d7d8b1656c"
            }
          ]
        },
        {
          "id": "28116231-549a-4f59-8f34-9750b1f8eee1",
          "name": "list-user-communication-channels",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels"
              ],
              "variable": [
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
            "description": "List user communication channels."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b24be57-78f4-414d-8353-fa7d225b3b25"
            }
          ]
        }
      ]
    }
  ]
}