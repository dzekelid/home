---
swagger: "2.0"
x-collection-name: Kentico Cloud
x-complete: 0
info:
  title: Kentico Cloud Getting items by localized URL slug
  description: "Get a *Home* content item whose URL slug in Spanish is *inicio* by
    using the following parameters:\n\n* `language=es-ES` \u2013 specifies the codename
    of the requested language.\n* `system.type=home` \u2013 filters content items
    by their content type.\n* `elements.url_pattern=inicio` \u2013 filters content
    items by a value of a specific content element.\n\nSee [Getting items by localized
    URL slug](https://developer.kenticocloud.com/docs/localization#section-getting-items-by-localized-url-slug)
    for more details."
  version: 1.0.0
host: deliver.kenticocloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    get:
      summary: Getting items by localized URL slug
      description: "Get a *Home* content item whose URL slug in Spanish is *inicio*
        by using the following parameters:\n\n* `language=es-ES` \u2013 specifies
        the codename of the requested language.\n* `system.type=home` \u2013 filters
        content items by their content type.\n* `elements.url_pattern=inicio` \u2013
        filters content items by a value of a specific content element.\n\nSee [Getting
        items by localized URL slug](https://developer.kenticocloud.com/docs/localization#section-getting-items-by-localized-url-slug)
        for more details."
      operationId: UnnammedEndpointGet
      x-api-path-slug: get
      responses:
        200:
          description: OK
      tags:
      - Ting
      - Items
      - By
      - Localized
      - URL
      - Slug
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