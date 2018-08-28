---
name: NxtPort
x-slug: nxtport
description: NxtPort opens the gates to the Port of the future. This project is a
  milestone in the digitalization of logistics and cargo.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
x-kinRank: "7"
x-alexaRank: "3933231"
tags: Layers
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/layers/master/_listings/nxtport/apis.md
specificationVersion: "0.14"
apis:
- name: Bel Air API (staging) - Retrieve available layers
  x-api-slug: layers-get
  description: "This operation lists the currently available city layers. \nThe returned
    strings can then be used as a layerId path parameter in the /layers operations
    included in this API."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api-stg.nxtport.eu//belair/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/layers/master/_listings/nxtport/layers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/layers/master/_listings/nxtport/layers-get-openapi.md
- name: Bel Air API (staging) - Retrieve the city layer data for the specified layer,
    metric and date.
  x-api-slug: layerslayeridmetriciddate-get
  description: 'This operation retrieves city layer data for the specified layer,
    metric and date combination. The date is passed in the following format: YYYYMMDD.
    The values for the layerId and metricId can be fetched from the /layers and /metrics
    operations.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api-stg.nxtport.eu//belair/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/layers/master/_listings/nxtport/layerslayeridmetriciddate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/layers/master/_listings/nxtport/layerslayeridmetriciddate-get-openapi.md
- name: Bel Air API (staging) - Retrieve the city layer data for the specified layer,
    metric and date.
  x-api-slug: layerslayeridmetriciddatehour-get
  description: 'This operation retrieves city layer data for the specified layer,
    metric and date combination. The date is passed in the following format: YYYYMMDD.
    The values for the layerId and metricId can be fetched from the /layers and /metrics
    operations.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api-stg.nxtport.eu//belair/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/layers/master/_listings/nxtport/layerslayeridmetriciddatehour-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/layers/master/_listings/nxtport/layerslayeridmetriciddatehour-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://npr.api.gallery.streamdata.io
- type: x-api-stack
  url: http://nxtport.stack.network
- type: x-email
  url: mail@nxtport.eu
- type: x-email
  url: development@nxtport.eu
- type: x-email
  url: privacy@nxtport.eu
- type: x-github
  url: https://github.com/NxtPort
- type: x-openapi
  url: https://github.com/NxtPort/nxtport.github.io/tree/master/api
- type: x-twitter
  url: https://twitter.com/NxtPortNews
- type: x-website
  url: https://www.nxtport.eu
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---