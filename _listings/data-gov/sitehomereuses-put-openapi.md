---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Put Site Home Reuses
  description: Set the homepage reuses editorial selection
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/home/datasets/:
    get:
      summary: Get Site Home Datasets
      description: List homepage datasets
      operationId: getSiteHomeDatasets
      x-api-path-slug: sitehomedatasets-get
      responses:
        200:
          description: OK
      tags:
      - Site
      - Home
      - Datasets
    put:
      summary: Put Site Home Datasets
      description: Set the homepage datasets editorial selection
      operationId: putSiteHomeDatasets
      x-api-path-slug: sitehomedatasets-put
      parameters:
      - in: body
        name: payload
        description: Dataset IDs to put in homepage
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Site
      - Home
      - Datasets
  /site/home/reuses/:
    get:
      summary: Get Site Home Reuses
      description: List homepage featured reuses
      operationId: getSiteHomeReuses
      x-api-path-slug: sitehomereuses-get
      responses:
        200:
          description: OK
      tags:
      - Site
      - Home
      - Reuses
    put:
      summary: Put Site Home Reuses
      description: Set the homepage reuses editorial selection
      operationId: putSiteHomeReuses
      x-api-path-slug: sitehomereuses-put
      parameters:
      - in: body
        name: payload
        description: Reuse IDs to put in homepage
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Site
      - Home
      - Reuses
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