---
swagger: "2.0"
x-collection-name: AWS EC2 Container Registry Service
x-complete: 0
info:
  title: AWS EC2 Container Registry API Get Download Url For Layer
  version: 1.0.0
  description: .Retrieves the pre-signed Amazon S3 download URL corresponding to an
    image layer. You can only get URLs for image layers that are referenced in an
    image.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetDownloadUrlForLayer:
    get:
      summary: Get Download Url For Layer
      description: .Retrieves the pre-signed Amazon S3 download URL corresponding
        to an image layer. You can only get URLs for image layers that are referenced
        in an image.
      operationId: getDownloadUrlForLayer
      x-api-path-slug: actiongetdownloadurlforlayer-get
      responses:
        200:
          description: OK
      tags:
      - Layers
  /?Action=BatchCheckLayerAvailability:
    get:
      summary: Batch Check Layer Availability
      description: Check the availability of multiple image layers in a specified
        registry and repository.
      operationId: batchCheckLayerAvailability
      x-api-path-slug: actionbatchchecklayeravailability-get
      parameters:
      - in: query
        name: layerDigests
        description: The digests of the image layers to check
        type: string
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the image layers to check
        type: string
      - in: query
        name: repositoryName
        description: The name of the repository that is associated with the image
          layers to check
        type: string
      responses:
        200:
          description: OK
      tags:
      - Layer Availability
  /?Action=CompleteLayerUpload:
    get:
      summary: Complete Layer Upload
      description: Inform Amazon ECR that the image layer upload for a specified registry,
        repository name, and upload ID, has completed.
      operationId: completeLayerUpload
      x-api-path-slug: actioncompletelayerupload-get
      responses:
        200:
          description: OK
      tags:
      - Layer Upload
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