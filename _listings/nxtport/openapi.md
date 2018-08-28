swagger: "2.0"
x-collection-name: NxtPort
x-complete: 1
info:
  title: Portcall+ API (sandbox)
  description: portplus-api
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /nxtportdocument/{bookingnumber}/{containernumber}:
    get:
      summary: Get VERMAS Files
      description: Returns the VERMAS files with the according booking number and
        container number
      operationId: NxtportdocumentByBookingnumberByContainernumberGet
      x-api-path-slug: nxtportdocumentbookingnumbercontainernumber-get
      parameters:
      - in: path
        name: bookingnumber
        description: bookingnumber
      - in: path
        name: containernumber
        description: containernumber
      - in: header
        name: Ocp-Apim-Subscription-Key
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - VERMAS
      - Files