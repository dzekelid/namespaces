swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/namespaces:
    get:
      summary: Get Namespaces
      description: Get a namespaces list
      operationId: getV3Namespaces
      x-api-path-slug: v3namespaces-get
      parameters:
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: search
        description: Search query for namespaces
      responses:
        200:
          description: OK
      tags:
      - Namespaces