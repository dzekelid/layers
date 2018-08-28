swagger: "2.0"
x-collection-name: WebTRIS
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: webtris.highwaysengland.co.uk
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v{version}/sitetypes/{siteType_Id}/sites:
    get:
      summary: Returns the layer metadata for the LayerId specified.
      description: Returns the layer metadata for the layerid specified..
      operationId: SiteTypes_GetSitesForPublicFacingAPI
      x-api-path-slug: vversionsitetypessitetype-idsites-get
      parameters:
      - in: path
        name: siteType_Id
        description: 1 = MIDAS, 2 = TAME, 3 = TMU, 4 = TRADS Legacy
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Layer
      - Metadatathe
      - LayerId
      - Specified