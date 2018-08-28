---
swagger: "2.0"
x-collection-name: IBM Cloud
x-complete: 0
info:
  title: IBM Containers Retrieve the namespace of an organization.
  description: 'This endpoint retrieves the namespace that was set for the organization
    that owns the current space (corresponding IBM Containers command: `cf ic namespace
    get`).'
  version: 3.0.0
host: containers-api.ng.bluemix.net
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /registry/namespaces:
    get:
      summary: Retrieve the namespace of an organization.
      description: 'This endpoint retrieves the namespace that was set for the organization
        that owns the current space (corresponding IBM Containers command: `cf ic
        namespace get`).'
      operationId: this-endpoint-retrieves-the-namespace-that-was-set-for-the-organization-that-owns-the-current-space-
      x-api-path-slug: registrynamespaces-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Registry
      - Namespaces
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