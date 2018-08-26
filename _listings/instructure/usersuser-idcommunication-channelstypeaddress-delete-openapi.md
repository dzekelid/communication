---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Users API Delete a communication channel
  description: Delete a communication channel.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/self/communication_channels/{communication_channel_id}/notification_preferences:
    put:
      summary: Update multiple preferences
      description: Update multiple preferences.
      operationId: update-multiple-preferences
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preferences-put
      parameters:
      - in: query
        name: notification_preferences[X][frequency]
        description: The desired frequency for &lt;X&gt; notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
  /users/self/communication_channels/{communication_channel_id}/notification_preferences/notification:
    put:
      summary: Update a preference
      description: Update a preference.
      operationId: update-a-preference
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preferencesnotification-put
      parameters:
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for this notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
      - Notification
  /users/self/communication_channels/{communication_channel_id}/notification_preference_categories/category:
    put:
      summary: Update preferences by category
      description: Update preferences by category.
      operationId: update-preferences-by-category
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preference-categoriescategory-put
      parameters:
      - in: query
        name: category
        description: The name of the category
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for each notification in the category
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preference
      - Categories
      - Category
  /users/self/communication_channels/{type}/address/notification_preferences:
    put:
      summary: Update multiple preferences
      description: Update multiple preferences.
      operationId: update-multiple-preferences
      x-api-path-slug: usersselfcommunication-channelstypeaddressnotification-preferences-put
      parameters:
      - in: query
        name: notification_preferences[X][frequency]
        description: The desired frequency for &lt;X&gt; notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Type
      - Address
      - Notification
      - Preferences
  /users/self/communication_channels/{type}/address/notification_preferences/{notification}:
    put:
      summary: Update a preference
      description: Update a preference.
      operationId: update-a-preference
      x-api-path-slug: usersselfcommunication-channelstypeaddressnotification-preferencesnotification-put
      parameters:
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for this notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Type
      - Address
      - Notification
      - Preferences
      - Notification
  /users/{user_id}/communication_channels:
    get:
      summary: List user communication channels
      description: List user communication channels.
      operationId: list-user-communication-channels
      x-api-path-slug: usersuser-idcommunication-channels-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
    post:
      summary: Create a communication channel
      description: Create a communication channel.
      operationId: create-a-communication-channel
      x-api-path-slug: usersuser-idcommunication-channels-post
      parameters:
      - in: query
        name: communication_channel[address]
        description: An email address or SMS number
      - in: query
        name: communication_channel[token]
        description: A registration id, device token, or equivalent token given to
          an app whennregistering with a push notification provider
      - in: query
        name: communication_channel[type]
        description: The type of communication channel
      - in: query
        name: skip_confirmation
        description: Only valid for site admins and account admins making requests;
          If true, thenchannel is automatically validated and no confirmation email
          or SMS isnsent
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
  /users/{user_id}/communication_channels/communication_channel_id/notification_preferences:
    get:
      summary: List preferences
      description: List preferences.
      operationId: list-preferences
      x-api-path-slug: usersuser-idcommunication-channelscommunication-channel-idnotification-preferences-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
  /users/{user_id}/communication_channels/communication_channel_id/notification_preferences/{notification}:
    get:
      summary: Get a preference
      description: Get a preference.
      operationId: get-a-preference
      x-api-path-slug: usersuser-idcommunication-channelscommunication-channel-idnotification-preferencesnotification-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
      - Notification
  /users/{user_id}/communication_channels/communication_channel_id/notification_preference_categories:
    get:
      summary: List of preference categories
      description: List of preference categories.
      operationId: list-of-preference-categories
      x-api-path-slug: usersuser-idcommunication-channelscommunication-channel-idnotification-preference-categories-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preference
      - Categories
  /users/{user_id}/communication_channels/id:
    delete:
      summary: Delete a communication channel
      description: Delete a communication channel.
      operationId: delete-a-communication-channel
      x-api-path-slug: usersuser-idcommunication-channelsid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
      - Id
  /users/{user_id}/communication_channels/type/{address}:
    delete:
      summary: Delete a communication channel
      description: Delete a communication channel.
      operationId: delete-a-communication-channel
      x-api-path-slug: usersuser-idcommunication-channelstypeaddress-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
      - Type
      - Address
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---