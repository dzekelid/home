---
swagger: "2.0"
x-collection-name: Kentico Cloud
x-complete: 1
info:
  title: Kentico Cloud
  description: this-is-a-collection-of-resources-you-can-find-within-the-kentico-cloud-developer-hubhttpsdeveloper-kenticocloud-com--kentico-cloudhttpskenticocloud-com-is-a-cloudfirst-headless-cms-that-allows-you-to-distribute-content-to-any-channel-and-device-websites-mobile-devices-mixed-reality-devices-presentation-kiosks-etc--through-an-api-certain-apis-require-that-you-include-the-authorization-header--find-more-in-httpsdeveloper-kenticocloud-comreferenceauthentication-
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
---