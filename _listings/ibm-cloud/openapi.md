---
swagger: "2.0"
x-collection-name: IBM Cloud
x-complete: 1
info:
  title: IBM Containers
  description: containers-are-virtual-software-objects-that-include-all-the-elements-that-an-app-needs-to-run--a-container-has-the-benefits-of-resource-isolation-and-allocation-but-is-more-portable-and-efficient-than-for-example-a-virtual-machine--this-documentation-describes-the-ibm-containers-api-which-is-based-on-the-docker-remote-api--the-api-provides-endpoints-that-you-can-use-to-create-and-manage-your-single-containers-and-container-groups-in-bluemix--endpoints-are-summarized-under-the-following-tags--authentication-retrieve-and-refresh-your-tls-certificates---private-docker-images-registry-create-your-own-private-docker-images-registry-in-bluemix-by-setting-a-namespace-for-your-organization---images-view-build-and-push-your-images-to-your-private-bluemix-registry-so-you-can-use-them-with-ibm-containers--you-can-also-scan-your-container-images-with-the-vulnerability-advisor-against-standard-policies-set-by-the-organization-manager-and-a-database-of-known-ubuntu-issues---single-containers-create-and-manage-single-containers-in-bluemix--use-a-single-container-to-implement-shortlived-processes-or-to-run-simple-tests-as-you-develop-an-app-or-service--to-make-your-single-container-available-from-the-internet-review-the-public-ip-addresses-endpoints---container-groups-create-and-manage-your-container-groups-in-bluemix--a-container-group-consists-of-multiple-single-containers-that-are-all-created-from-the-same-container-image-and-as-a-consequence-are-configured-in-the-same-way--container-groups-offer-further-options-at-no-cost-to-make-your-app-highly-available--these-options-include-inbuilt-load-balancing-autorecovery-of-unhealthy-container-instances-and-autoscaling-of-container-instances-based-on-cpu-and-memory-usage--map-a-public-route-to-your-container-group-to-make-your-app-accessible-from-the-internet----public-ip-addresses-use-these-endpoints-to-request-public-ip-addresses-for-your-space--you-can-bind-this-ip-address-to-your-container-to-make-your-container-accessible-from-the-internet---file-shares-create-list-and-delete-file-shares-in-a-space--a-file-share-is-a-nfs-storage-system-that-hosts-docker-volumes----volumes-create-and-manage-container-volumes-in-your-space-to-persist-the-data-of-your-containers----each-api-request-requires-an-http-header-that-includes-the-xauthtoken-and-xauthprojectid-parameter---xauthtoken-the-json-web-token-jwt-that-you-receive-when-logging-into-the-bluemix-platform--it-allows-you-to-use-the-ibm-containers-rest-api-access-services-and-resources--run-cf-oauthtoken-to-retrieve-your-access-token-information--xauthprojectid-the-unique-id-of-your-organization-space-where-you-want-to-create-or-work-with-your-containers--run-cf-space-space-name-guid-where-space-name-is-the-name-of-your-space-to-retrieve-your-space-id--for-further-information-about-how-containers-work-in-the-ibm-containers-service-review-the-documentation-under-httpsnewconsole-ng-bluemix-netdocscontainerscontainer-index-html--
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
    put:
      summary: Set a namespace for your private Bluemix registry.
      description: "Set up your own Docker images registry in Bluemix by defining
        a namespace for your organization (corresponding IBM Containers command: `cf
        ic namespace set <namespace>`). The namespace is used to generate a unique
        URL to your private Bluemix registry. In your private registry you store all
        Docker images that you want to share across your organization. To create a
        container from an image, you must first push the image to your registry. \n\n
        The namespace cannot be changed after is has been set. Consider the following
        rules to choose a namespace for your organization: \n\n- Every organization
        can have one namespace at a time only \n- The namespace must be unique in
        Bluemix. \n- The namespace can be 4-30 characters long. \n- The namespace
        must start with at least one letter or number. \n- The namespace can only
        contain lowercase letters, numbers or underscores (_)."
      operationId: set-up-your-own-docker-images-registry-in-bluemix-by-defining-a-namespace-for-your-organization-corr
      x-api-path-slug: registrynamespacesnamespace-put
      parameters:
      - in: path
        name: namespace
        description: The name for your namespace to create your private Docker images
          registry in Bluemix
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
---