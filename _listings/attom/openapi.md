swagger: "2.0"
x-collection-name: ATTOM
x-complete: 1
info:
  title: Attom Data Solutions API
  description: attom-empowers-customers-with-better-property-data--we-warehouse-property-data-nationwide-with-myriad-data-points-on-each-parcel-including-ownership-information-latlong-square-footage-loan-types-sales-history-sales-comps-crime-schools-and-more-
  version: 1.0.0
host: search.onboard-apis.com
basePath: /communityapi/v2.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sale/snapshot:
    get:
      summary: Returns home sale information for properties within a geography.
      description: Get a list of home sale snapshots within a Onboard GeoID that sold
        within a date range and specified sale amount.
      operationId: getHomeSaleSnapshotsGeoId
      x-api-path-slug: salesnapshot-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: endsalesearchdate
        description: The standardized date for search purposes
      - in: query
        name: geoid
        description: A list of geographies that this property belongs to
      - in: query
        name: maxsaleamt
        description: The recorded amount of the sale transaction
      - in: query
        name: minsaleamt
        description: The recorded amount of the sale transaction
      - in: query
        name: propertytype
        description: A specific property classification such as Detached Single Family
      - in: query
        name: radius
      - in: query
        name: startsalesearchdate
        description: The standardized date for search purposes
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Home
      - Sale
      - Informationproperties
      - Within
      - Geography