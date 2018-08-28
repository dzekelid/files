---
name: BC Geographical Names
x-slug: bc-geographical-names
description: Geographical names are more than labels on maps and road signs. They
  can reveal patterns of settlement, exploration and migration, and mirror outside
  influences to our history - aspects of the heritage and promise of an area that
  might otherwise be overlooked or forgotten by visitors and later generations.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Files
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/apis.md
specificationVersion: "0.14"
apis:
- name: Geo Mark Web Service - Get information about a particular geomark
  x-api-slug: geomarksgeomarkid-fileformatextension-get
  description: The attribution can be downloaded as a info file format. The download
    files can then be processed by a client application to access the geomark info
    fields and to get the URLs to the geometry download resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkid-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkid-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Gets the bounding box of the geomark
  x-api-slug: geomarksgeomarkidboundingbox-fileformatextension-get
  description: The source geomarks can be specified by with the geomarkUrl parameter.  Repeat
    the parameter if sourcing from multiple geomarks
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidboundingbox-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidboundingbox-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Get the feature and attribution of the geomark
  x-api-slug: geomarksgeomarkidfeature-fileformatextension-get
  description: The geomark feature resource returns a single spatial feature with
    either a single (Point, LineString, Polygon) or multi-part geometry (MultiPoint,
    MultiLineString, MultiPolygon) and the geomark attribution.  The geometry and
    attribution can be downloaded as a spatial download file format in a supported
    coordinate system. The download files can then be used in a desktop GIS application
    (e.g. ArcMap), Google Earth or a web mapping application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidfeature-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidfeature-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Get the individual geometries within a multi-part geometry
  x-api-slug: geomarksgeomarkidparts-fileformatextension-get
  description: The geomark parts resource returns a one or more spatial features.
    One for each part of the Geomark's geomerty. Each part contains a single (Point,
    LineString, Polygon) geometry and the geomark attribution.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidparts-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidparts-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Gets a single spatial point representative of the geomark.
  x-api-slug: geomarksgeomarkidpoint-fileformatextension-get
  description: The geomark point resource returns a single spatial feature with a
    single Point and the geomark attribution.  The point geometry will be created
    from the first geometry part of the Geomark. Point geomarks will return the first
    Point part in the geomark.  LineString geomarks will return the first coordinate
    of the first LineString part in the geomark. Polygon geomarks will return the
    centroid or another point inside the first Polygon part in the geomark. The geometry
    and attribution can be downloaded as a spatial download file format in a supported
    coordinate system. The download files can then be used in a desktop GIS application
    (e.g. ArcMap), Google Earth or a web mapping application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidpoint-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidpoint-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Get information about a particular geomark
  x-api-slug: geomarksgeomarkid-fileformatextension-get
  description: The attribution can be downloaded as a info file format. The download
    files can then be processed by a client application to access the geomark info
    fields and to get the URLs to the geometry download resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkid-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkid-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Gets the bounding box of the geomark
  x-api-slug: geomarksgeomarkidboundingbox-fileformatextension-get
  description: The source geomarks can be specified by with the geomarkUrl parameter.  Repeat
    the parameter if sourcing from multiple geomarks
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidboundingbox-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidboundingbox-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Get the feature and attribution of the geomark
  x-api-slug: geomarksgeomarkidfeature-fileformatextension-get
  description: The geomark feature resource returns a single spatial feature with
    either a single (Point, LineString, Polygon) or multi-part geometry (MultiPoint,
    MultiLineString, MultiPolygon) and the geomark attribution.  The geometry and
    attribution can be downloaded as a spatial download file format in a supported
    coordinate system. The download files can then be used in a desktop GIS application
    (e.g. ArcMap), Google Earth or a web mapping application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidfeature-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidfeature-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Get the individual geometries within a multi-part geometry
  x-api-slug: geomarksgeomarkidparts-fileformatextension-get
  description: The geomark parts resource returns a one or more spatial features.
    One for each part of the Geomark's geomerty. Each part contains a single (Point,
    LineString, Polygon) geometry and the geomark attribution.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidparts-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidparts-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Gets a single spatial point representative of the geomark.
  x-api-slug: geomarksgeomarkidpoint-fileformatextension-get
  description: The geomark point resource returns a single spatial feature with a
    single Point and the geomark attribution.  The point geometry will be created
    from the first geometry part of the Geomark. Point geomarks will return the first
    Point part in the geomark.  LineString geomarks will return the first coordinate
    of the first LineString part in the geomark. Polygon geomarks will return the
    centroid or another point inside the first Polygon part in the geomark. The geometry
    and attribution can be downloaded as a spatial download file format in a supported
    coordinate system. The download files can then be used in a desktop GIS application
    (e.g. ArcMap), Google Earth or a web mapping application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidpoint-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidpoint-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Gets a single spatial point representative of the geomark.
  x-api-slug: geomarksgeomarkidpoint-fileformatextension-get
  description: The geomark point resource returns a single spatial feature with a
    single Point and the geomark attribution.  The point geometry will be created
    from the first geometry part of the Geomark. Point geomarks will return the first
    Point part in the geomark.  LineString geomarks will return the first coordinate
    of the first LineString part in the geomark. Polygon geomarks will return the
    centroid or another point inside the first Polygon part in the geomark. The geometry
    and attribution can be downloaded as a spatial download file format in a supported
    coordinate system. The download files can then be used in a desktop GIS application
    (e.g. ArcMap), Google Earth or a web mapping application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidpoint-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidpoint-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Get the individual geometries within a multi-part geometry
  x-api-slug: geomarksgeomarkidparts-fileformatextension-get
  description: The geomark parts resource returns a one or more spatial features.
    One for each part of the Geomark's geomerty. Each part contains a single (Point,
    LineString, Polygon) geometry and the geomark attribution.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidparts-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidparts-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Get the feature and attribution of the geomark
  x-api-slug: geomarksgeomarkidfeature-fileformatextension-get
  description: The geomark feature resource returns a single spatial feature with
    either a single (Point, LineString, Polygon) or multi-part geometry (MultiPoint,
    MultiLineString, MultiPolygon) and the geomark attribution.  The geometry and
    attribution can be downloaded as a spatial download file format in a supported
    coordinate system. The download files can then be used in a desktop GIS application
    (e.g. ArcMap), Google Earth or a web mapping application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidfeature-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidfeature-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Gets the bounding box of the geomark
  x-api-slug: geomarksgeomarkidboundingbox-fileformatextension-get
  description: The source geomarks can be specified by with the geomarkUrl parameter.  Repeat
    the parameter if sourcing from multiple geomarks
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidboundingbox-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkidboundingbox-fileformatextension-get-openapi.md
- name: Geo Mark Web Service - Get information about a particular geomark
  x-api-slug: geomarksgeomarkid-fileformatextension-get
  description: The attribution can be downloaded as a info file format. The download
    files can then be processed by a client application to access the geomark info
    fields and to get the URLs to the geometry download resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/british-columbia.png
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/geomark
  tags: Geo, Geography, Locations, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkid-fileformatextension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/bc-geographical-names/geomarksgeomarkid-fileformatextension-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://bbc.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bc.geographical.names.stack.network
- type: x-website
  url: https://apps.gov.bc.ca/pub/bcgnws/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---