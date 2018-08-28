---
name: Azure Notification Hubs
x-slug: azure-notification-hubs
description: Azure Notification Hubs provide an easy-to-use, multi-platform, scaled-out
  push engine. With a single cross-platform API call, you can easily send targeted
  and personalized push notifications to any mobile platform from any cloud or on-premises
  backend.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-notification-hubs.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Namespaces
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-notification-hubs/apis.md
specificationVersion: "0.14"
apis:
- name: NotificationHubsManagementClient - Namespaces Create Or Update
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacename-put
  description: Creates/Updates a service namespace. Once created, this namespace's
    resource manifest is immutable. This operation is idempotent.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-notification-hubs.png
  humanURL: https://docs.microsoft.com/en-us/azure/notification-hubs/
  baseURL: ://management.azure.com//
  tags: Notifications, Microsoft, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacename-put-openapi.md
- name: NotificationHubsManagementClient - Namespaces Patch
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacename-patch
  description: Patches the existing namespace
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-notification-hubs.png
  humanURL: https://docs.microsoft.com/en-us/azure/notification-hubs/
  baseURL: ://management.azure.com//
  tags: Notifications, Microsoft, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacename-patch-openapi.md
- name: NotificationHubsManagementClient - Namespaces Delete
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacename-delete
  description: Deletes an existing namespace. This operation also removes all associated
    notificationHubs under the namespace.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-notification-hubs.png
  humanURL: https://docs.microsoft.com/en-us/azure/notification-hubs/
  baseURL: ://management.azure.com//
  tags: Notifications, Microsoft, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacename-delete-openapi.md
- name: NotificationHubsManagementClient - Namespaces Get
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacename-get
  description: Returns the description for the specified namespace.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-notification-hubs.png
  humanURL: https://docs.microsoft.com/en-us/azure/notification-hubs/
  baseURL: ://management.azure.com//
  tags: Notifications, Microsoft, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacename-get-openapi.md
- name: NotificationHubsManagementClient - Namespaces List
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespaces-get
  description: Lists the available namespaces within a resourceGroup.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-notification-hubs.png
  humanURL: https://docs.microsoft.com/en-us/azure/notification-hubs/
  baseURL: ://management.azure.com//
  tags: Notifications, Microsoft, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespaces-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/namespaces/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespaces-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://azure.monitor.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.notification.hubs.stack.network
- type: x-documentation
  url: https://docs.microsoft.com/en-us/rest/api/notificationhubs
- type: x-website
  url: https://docs.microsoft.com/en-us/azure/notification-hubs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---