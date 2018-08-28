---
name: Azure Event Hubs
x-slug: azure-event-hubs
description: Azure Event Hubs is a hyper-scale telemetry ingestion service that collects,
  transforms, and stores millions of events. As a distributed streaming platform,
  it gives you low latency and configurable time retention, which enables you to ingress
  massive amounts of telemetry into the cloud and read the data from multiple applications
  using publish-subscribe semantics.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-event-hubs-stream.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Namespaces
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-event-hubs/apis.md
specificationVersion: "0.14"
apis:
- name: EventHubManagementClient - Namespaces Create Or Update
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacename-put
  description: Creates or updates a namespace. Once created, this namespace's resource
    manifest is immutable. This operation is idempotent.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-event-hubs-stream.png
  humanURL: https://azure.microsoft.com/en-us/services/event-hubs/
  baseURL: ://management.azure.com//
  tags: Microsoft, Jobs, Orchestration, Stack Network, API Service Provider, API Provider,
    SDIO Competition, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-event-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacename-put-openapi.md
- name: EventHubManagementClient - Namespaces Delete
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacename-delete
  description: Deletes an existing namespace. This operation also removes all associated
    resources under the namespace.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-event-hubs-stream.png
  humanURL: https://azure.microsoft.com/en-us/services/event-hubs/
  baseURL: ://management.azure.com//
  tags: Microsoft, Jobs, Orchestration, Stack Network, API Service Provider, API Provider,
    SDIO Competition, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-event-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-event-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacename-delete-openapi.md
- name: EventHubManagementClient - Namespaces Get
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacename-get
  description: Gets the description of the specified namespace.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-event-hubs-stream.png
  humanURL: https://azure.microsoft.com/en-us/services/event-hubs/
  baseURL: ://management.azure.com//
  tags: Microsoft, Jobs, Orchestration, Stack Network, API Service Provider, API Provider,
    SDIO Competition, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-event-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-event-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacename-get-openapi.md
- name: EventHubManagementClient - Namespaces Update
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacename-patch
  description: Creates or updates a namespace. Once created, this namespace's resource
    manifest is immutable. This operation is idempotent.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-event-hubs-stream.png
  humanURL: https://azure.microsoft.com/en-us/services/event-hubs/
  baseURL: ://management.azure.com//
  tags: Microsoft, Jobs, Orchestration, Stack Network, API Service Provider, API Provider,
    SDIO Competition, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-event-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacename-patch-openapi.md
x-common:
- type: x-hacker-news-search
  url: Azure Event Hubs
- type: x-api-gallery
  url: http://azure.documentdb.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.event.hubs.stack.network
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/event-hubs/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/event-hubs/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/event-hubs/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/event-hubs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---