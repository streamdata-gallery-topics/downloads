swagger: "2.0"
x-collection-name: Swagger
x-complete: 1
info:
  title: Swagger Generator
  description: this-is-an-online-swagger-codegen-server---you-can-find-out-more-at-httpsgithub-comswaggerapiswaggercodegen-or-on-irc-freenode-net-swaggerhttpswagger-ioirc-
  termsOfService: http://swagger.io/terms/
  contact:
    name: apiteam@swagger.io
  version: 2.2.3
host: generator.swagger.io
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gen/download/{fileId}:
    get:
      summary: Downloads a pre-generated file
      description: A valid `fileId` is generated by the `/clients/{language}` or `/servers/{language}`
        POST operations.  The fileId code can be used just once, after which a new
        `fileId` will need to be requested.
      operationId: downloadFile
      x-api-path-slug: gendownloadfileid-get
      parameters:
      - in: path
        name: fileId
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Download
      - FileId