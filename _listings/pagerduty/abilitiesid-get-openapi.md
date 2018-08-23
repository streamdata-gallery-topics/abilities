---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 0
info:
  title: PagerDuty Test an ability
  version: 1.0.0
  description: Test whether your account has a given ability.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /abilities:
    get:
      summary: List abilities
      description: List all of your account's abilities, by name.
      operationId: list-all-of-your-accounts-abilities-by-name
      x-api-path-slug: abilities-get
      responses:
        200:
          description: OK
      tags:
      - Abilities
  /abilities/{id}:
    get:
      summary: Test an ability
      description: Test whether your account has a given ability.
      operationId: test-whether-your-account-has-a-given-ability
      x-api-path-slug: abilitiesid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Abilities
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