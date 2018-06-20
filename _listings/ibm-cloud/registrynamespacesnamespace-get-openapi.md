---
swagger: "2.0"
x-collection-name: IBM Cloud
x-complete: 0
info:
  title: IBM Containers Check the availability of a namespace
  description: "This endpoint checks whether a namespace is available in Bluemix and
    can be used to set up the private Docker images registry for an organization.
    When a HTTP code `201 Ok` is returned, the namespace is already assigned to another
    organization in Bluemix and cannot be used. When a HTTP code `404 Not found` is
    returned, the namespace can be used for your organization. \n\n Consider the following
    rules when choosing a namespace for your organization: \n\n- Every organization
    can have one namespace at a time only \n- The namespace must be unique in Bluemix.
    \n- The namespace can be 4-30 characters long. \n- The namespace must start with
    at least one letter or number. \n- The namespace can only contain lowercase letters,
    numbers or underscores (_)."
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
  /registry/namespaces/{namespace}:
    get:
      summary: Check the availability of a namespace
      description: "This endpoint checks whether a namespace is available in Bluemix
        and can be used to set up the private Docker images registry for an organization.
        When a HTTP code `201 Ok` is returned, the namespace is already assigned to
        another organization in Bluemix and cannot be used. When a HTTP code `404
        Not found` is returned, the namespace can be used for your organization. \n\n
        Consider the following rules when choosing a namespace for your organization:
        \n\n- Every organization can have one namespace at a time only \n- The namespace
        must be unique in Bluemix. \n- The namespace can be 4-30 characters long.
        \n- The namespace must start with at least one letter or number. \n- The namespace
        can only contain lowercase letters, numbers or underscores (_)."
      operationId: this-endpoint-checks-whether-a-namespace-is-available-in-bluemix-and-can-be-used-to-set-up-the-priva
      x-api-path-slug: registrynamespacesnamespace-get
      parameters:
      - in: path
        name: namespace
        description: The name of the namespace that you would like to use for your
          organization and for which you would like to check availability in Bluemix
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
      - Namespace
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