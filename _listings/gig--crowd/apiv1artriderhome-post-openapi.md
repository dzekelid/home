---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Art Rer Home
  version: 1.0.0
  description: Post art rer home.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/art/rider/home:
    get:
      summary: Get Art Rer Home
      description: Get art rer home.
      operationId: getApiV1ArtRerHome
      x-api-path-slug: apiv1artriderhome-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Art
      - Rer
      - Home
    post:
      summary: Post Art Rer Home
      description: Post art rer home.
      operationId: postApiV1ArtRerHome
      x-api-path-slug: apiv1artriderhome-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Art
      - Rer
      - Home
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