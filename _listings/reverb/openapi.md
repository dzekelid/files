---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shops/{shop_id}/shipping_profiles:
    get:
      summary: Get Shops Shop Shipping Profiles
      description: List of shipping profiles for your shop
      operationId: getShopsShopShippingProfiles
      x-api-path-slug: shopsshop-idshipping-profiles-get
      parameters:
      - in: path
        name: shop_id
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Id
      - Shipping
      - Profiles
---