---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Intelligent Mapping Create a new layer
  description: Creates a new layer and associates it with the specified map.
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/maps/{mapId}/orderlayers:
    post:
      summary: Update order of layers
      description: Updates the order of layers for a given map.
      operationId: updates-the-order-of-layers-for-a-given-map
      x-api-path-slug: v1mapsmapidorderlayers-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Order
      - Of
      - Layers
  /v1/maps/{mapId}/layers:
    post:
      summary: Create a new layer
      description: Creates a new layer and associates it with the specified map.
      operationId: creates-a-new-layer-and-associates-it-with-the-specified-map
      x-api-path-slug: v1mapsmapidlayers-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - New
      - Layer
  /v1/maps/{mapId}/layers/{layerId}:
    get:
      summary: Return layer details
      description: |-
        For the layer identified by the map and layer identifiers, returns the
        layer details (identifier, name, Uniform Resource Identifier (URI), and
        visibility).
      operationId: for-the-layer-identified-by-the-map-and-layer-identifiers-returns-thelayer-details-identifier-name-u
      x-api-path-slug: v1mapsmapidlayerslayerid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Return
      - Layer
      - Details
    put:
      summary: Update the layer properties
      description: |-
        For the layer identified by the specified map and layer identifiers,
        updates the layer properties.
      operationId: for-the-layer-identified-by-the-specified-map-and-layer-identifiersupdates-the-layer-properties
      x-api-path-slug: v1mapsmapidlayerslayerid-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Layer
      - Properties
    delete:
      summary: Delete a layer
      description: Deletes the layer identified by the specified map and layer identifiers.
      operationId: deletes-the-layer-identified-by-the-specified-map-and-layer-identifiers
      x-api-path-slug: v1mapsmapidlayerslayerid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Layer
  /v1/maps/{mapId}/layers/{layerId}/style:
    get:
      summary: Retrieves style data for a layer
      description: |-
        Retrieve style data for the layer identified by the specified map and
        layer identifiers.
      operationId: retrieve-style-data-for-the-layer-identified-by-the-specified-map-andlayer-identifiers
      x-api-path-slug: v1mapsmapidlayerslayeridstyle-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieves
      - Style
      - Dataa
      - Layer
    put:
      summary: Update the style data for a layer
      description: |-
        Update the style data for the layer identified by the specified map and
        layer identifiers.
      operationId: update-the-style-data-for-the-layer-identified-by-the-specified-map-andlayer-identifiers
      x-api-path-slug: v1mapsmapidlayerslayeridstyle-put
      parameters:
      - in: body
        name: body
        description: Style data
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Style
      - Dataa
      - Layer
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