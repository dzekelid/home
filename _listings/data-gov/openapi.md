---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 1
info:
  title: Data.gov API
  description: the-data-gov-catalog-is-powered-by-ckan-a-powerful-open-source-data-platform-that-includes-a-robust-api--please-be-aware-that-data-gov-and-the-data-gov-ckan-api-only-contain-metadata-about-datasets--this-metadata-includes-urls-and-descriptions-of-datasets-but-it-does-not-include-the-actual-data-within-each-dataset-
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
---