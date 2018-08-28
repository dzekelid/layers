swagger: "2.0"
x-collection-name: Google Books
x-complete: 1
info:
  title: Books
  description: searches-for-books-and-manages-your-google-books-library-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /books/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /volumes/{volumeId}/layersummary:
    get:
      summary: Get Layers
      description: List the layer summaries for a volume.
      operationId: books.layers.list
      x-api-path-slug: volumesvolumeidlayersummary-get
      parameters:
      - in: query
        name: contentVersion
        description: The content version for the requested volume
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous page
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: volumeId
        description: The volume to retrieve layers for
      responses:
        200:
          description: OK
      tags:
      - Layer
  /volumes/{volumeId}/layersummary/{summaryId}:
    get:
      summary: Get Layer
      description: Gets the layer summary for a volume.
      operationId: books.layers.get
      x-api-path-slug: volumesvolumeidlayersummarysummaryid-get
      parameters:
      - in: query
        name: contentVersion
        description: The content version for the requested volume
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: summaryId
        description: The ID for the layer to get the summary for
      - in: path
        name: volumeId
        description: The volume to retrieve layers for
      responses:
        200:
          description: OK
      tags:
      - Layer