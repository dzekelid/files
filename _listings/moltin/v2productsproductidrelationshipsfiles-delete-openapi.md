---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Delete Products <=> Files Relationship
  description: Here you can delete a relationship between a `Product` and `File`'s.
    Only relationships to `File`'s specified in the payload will be removed.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/products/{productID}/relationships/files:
    put:
      summary: Update Products <=> Files Relationships
      description: '`File`''s specified in the payload willbe related to the product
        any relatiosnhips to `File`''s **NOT** specified in payload will be removed.'
      operationId: V2ProductsRelationshipsFilesByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipsfiles-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Files
      - Relationships
    post:
      summary: Create Products <=> Files Relationships
      description: Here you can add `File`'s to a product. `File`'s specified in the
        payload willbe related to the product.
      operationId: V2ProductsRelationshipsFilesByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipsfiles-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Files
      - Relationships
    delete:
      summary: Delete Products <=> Files Relationship
      description: Here you can delete a relationship between a `Product` and `File`'s.
        Only relationships to `File`'s specified in the payload will be removed.
      operationId: V2ProductsRelationshipsFilesByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipsfiles-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Files
      - Relationship
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