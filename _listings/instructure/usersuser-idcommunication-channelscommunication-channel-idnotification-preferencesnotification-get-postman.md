{
  "info": {
    "name": "Instructure Canvas Users API Get a preference",
    "_postman_id": "0f67690e-0b9a-466e-b056-6cfe371abf38",
    "description": "Get a preference.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "9eff09f5-b6db-48b2-ac4e-2b3b7e505a6d",
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
              "id": "c971e3cd-ba58-497a-8249-ba93242b0dc7"
            }
          ]
        },
        {
          "id": "bed773db-3f21-4302-9741-111babe9b1f4",
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
              "id": "41771281-ee30-48f2-bf46-5d6f52f9b7ce"
            }
          ]
        },
        {
          "id": "e370177b-c8b4-4f34-8297-a8c55be0f473",
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
              "id": "34d5ab2a-f4e8-4865-b0ed-595c075b0998"
            }
          ]
        },
        {
          "id": "b8087fbf-77de-4840-8b8f-247dd267bcad",
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
              "id": "a118cec0-95e8-4d5b-94a7-a6532bb3715b"
            }
          ]
        },
        {
          "id": "703e1297-7e4a-4167-90ec-a2625f7d7307",
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
              "id": "f293fa10-58a9-4bc2-ae50-1cb98b730465"
            }
          ]
        },
        {
          "id": "b66ec8d3-182a-46b5-8284-73b0e5dbb82d",
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
              "id": "ffa441f9-f64d-4b2d-81cf-a28ed920786a"
            }
          ]
        },
        {
          "id": "fb9b6f97-4c84-420e-b90d-70e2f475dc5b",
          "name": "create-a-communication-channel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels"
              ],
              "query": [
                {
                  "key": "communication_channel[address]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "communication_channel[token]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "communication_channel[type]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip_confirmation",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
            "description": "Create a communication channel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e855deab-8e18-4fb6-a5c8-e7bef32350c1"
            }
          ]
        },
        {
          "id": "17602481-4d2d-4b69-be37-2640b6b4981a",
          "name": "list-preferences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels/communication_channel_id/notification_preferences"
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
            "description": "List preferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "918ba926-1e6e-4278-83c8-38ed04dd3926"
            }
          ]
        },
        {
          "id": "ddc1b56d-ce24-487b-8776-7c67cd114730",
          "name": "get-a-preference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels/communication_channel_id/notification_preferences/:notification"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "notification",
                  "value": "notification",
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
              "id": "02c26fae-97b9-45ec-89a2-dd650d1837d0"
            }
          ]
        }
      ]
    }
  ]
}