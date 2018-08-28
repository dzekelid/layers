swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 1
info:
  title: ClimaCell API
  description: the-climacell-rest-api-provides-access-to-high-resolution-weather-data-for-locations-across-the-u-s--with-global-data-coming-soon--it-uses-https-and-requires-an-access-token-key--the-api-requests-carry-query-parameters-and-the-responses-return-results-in-json-format-
  version: 1.0.0
host: api2.climacell.co
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /weather_map_layer/{ts}/{z}/{x}/{y}.png:
    get:
      summary: Get Weather Map Layer Ts Z X Y .png
      description: |-
        ## Weather Map Layer (Visual Tiles)
        The ```weather_map``` is a tiled image call compatible with most modern mapping UI libraries:
          * OpenLayers (see ???https://openlayers.org/en/latest/apidoc/ol.source.XYZ.html???)
          * Leaflets
          * MapBox
          * Google Maps

        The call displays a precipitation heatmap on your existing geography user interface. You can overlay an actual precipitation layer. In the future, Climacell will support other weather parameter overlays.

        The tile grid is composed of 256x256 pixel tiles with (x,y) coordinates, where (0,0) is at thenorthwest corner of the map. x increase as the map goes east, and y increases as it goes south.

        ![tiile layer|150x150](/api-docs/custom/tile_layer.png)

        Note: For more information about Tiling, please visit
        https://wiki.openstreetmap.org/wiki/Slippy_map_tilenames
      operationId: -weather-map-layer-visual-tilesthe-weather-map-is-a-tiled-image-call-compatible-with-most-modern-map
      x-api-path-slug: weather-map-layertszxy-png-get
      parameters:
      - in: path
        name: ts
        description: Requested timestamp for the map
      - in: path
        name: x
        description: The x coordinate for the map
      - in: path
        name: "y"
        description: The y coordinate for the map
      - in: path
        name: z
        description: The zoom level for the map
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Weather
      - Map
      - Layer
      - Ts
      - Z
      - X
      - "Y"
      - Png