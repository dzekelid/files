swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 1
info:
  title: Entertainment Express
  description: your-gateway-to-building-incredible-movie-tv-and-game-content-discovery-experiences-
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Images/{FilePath}/Redirect:
    get:
      summary: Redirect to an image based on filepath.
      description: "Images should be downloaded and stored on the client server. Use
        /Common/ImageTypes to see a list of available image types.  \n\n\n`Note: The
        swagger U/I does not support redirects.`"
      operationId: GetImage
      x-api-path-slug: imagesfilepathredirect-get
      parameters:
      - in: path
        name: FilePath
        description: Filepath of Image
      - in: query
        name: Redirect
        description: Redirect to the image
      responses:
        200:
          description: OK
      tags:
      - Images
      - FilePath
      - Redirect