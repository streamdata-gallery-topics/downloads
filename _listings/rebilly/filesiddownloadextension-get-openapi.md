---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Download image in specific format
  description: Download image in specific format. Images are converted server-side
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{id}/download:
    get:
      summary: Download a file
      description: Download a file
      operationId: files.id.download.get
      x-api-path-slug: filesiddownload-get
      responses:
        200:
          description: OK
      tags:
      - Download
      - File
  /files/{id}/download{extension}:
    get:
      summary: Download image in specific format
      description: Download image in specific format. Images are converted server-side
      operationId: files.id.downloadextension.get
      x-api-path-slug: filesiddownloadextension-get
      responses:
        200:
          description: OK
      tags:
      - Download
      - Image
      - In
      - Specific
      - Format
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