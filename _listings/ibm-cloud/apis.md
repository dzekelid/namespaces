---
name: IBM Cloud
x-slug: ibm-cloud
description: The IBM Cloud has been built to help you solve problems and advance opportunities
  in a world flush with data. Whether it&rsquo;s data you possess, data outside your
  firewall, or data that&rsquo;s coming, the IBM Cloud helps you protect it, move
  it, integrate it and unlock intelligence from it &mdash; giving you what it takes
  to prevail in a competitive market.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28560-ibm-containers.jpg
x-kinRank: "8"
x-alexaRank: "11207"
tags: Namespaces
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/ibm-cloud/apis.md
specificationVersion: "0.14"
apis:
- name: IBM Containers - Retrieve the namespace of an organization.
  x-api-slug: registrynamespaces-get
  description: 'This endpoint retrieves the namespace that was set for the organization
    that owns the current space (corresponding IBM Containers command: `cf ic namespace
    get`).'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28560-ibm-containers.jpg
  humanURL: https://www.ibm.com/cloud/
  baseURL: https://containers-api.ng.bluemix.net//v3
  tags: SaaS, Technology, Enterprise, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/ibm-cloud/registrynamespaces-get-openapi.md
- name: IBM Containers - Check the availability of a namespace
  x-api-slug: registrynamespacesnamespace-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28560-ibm-containers.jpg
  humanURL: https://www.ibm.com/cloud/
  baseURL: https://containers-api.ng.bluemix.net//v3
  tags: SaaS, Technology, Enterprise, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/ibm-cloud/registrynamespacesnamespace-get-openapi.md
- name: IBM Containers - Set a namespace for your private Bluemix registry.
  x-api-slug: registrynamespacesnamespace-put
  description: "Set up your own Docker images registry in Bluemix by defining a namespace
    for your organization (corresponding IBM Containers command: `cf ic namespace
    set <namespace>`). The namespace is used to generate a unique URL to your private
    Bluemix registry. In your private registry you store all Docker images that you
    want to share across your organization. To create a container from an image, you
    must first push the image to your registry. \n\n The namespace cannot be changed
    after is has been set. Consider the following rules to choose a namespace for
    your organization: \n\n- Every organization can have one namespace at a time only
    \n- The namespace must be unique in Bluemix. \n- The namespace can be 4-30 characters
    long. \n- The namespace must start with at least one letter or number. \n- The
    namespace can only contain lowercase letters, numbers or underscores (_)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28560-ibm-containers.jpg
  humanURL: https://www.ibm.com/cloud/
  baseURL: https://containers-api.ng.bluemix.net//v3
  tags: SaaS, Technology, Enterprise, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/ibm-cloud/registrynamespacesnamespace-put-openapi.md
x-common:
- type: x-api-gallery
  url: http://hsbc.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ibm.cloud.stack.network
- type: x-blog
  url: https://www.ibm.com/blogs/bluemix/
- type: x-crunchbase
  url: https://crunchbase.com/organization/product/ibm-bluemix
- type: x-github
  url: https://github.com/IBM-Cloud
- type: x-twitter
  url: https://twitter.com/IBMcloud
- type: x-website
  url: https://www.ibm.com/cloud/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---