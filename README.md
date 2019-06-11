# ![LOGO](logo.png) Microsoft.ResourceHealth **flow**ground Connector

## Description

A generated **flow**ground connector for the Microsoft.ResourceHealth API (version 2017-07-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/resourcehealth/2017-07-01/swagger.json<br/>
Generated at: 2019-06-11T18:14:12+03:00

## API Description

The Resource Health Client.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists available operations for the resourcehealth resource provider

*Tags:* `Operations`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.

### Lists the current availability status for all the resources in the subscription. Use the nextLink property in the response to get the next page of availability statuses.

*Tags:* `AvailabilityStatuses`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `$filter` - _optional_ - The filter to apply on the operation. For more information please see https://docs.microsoft.com/en-us/rest/api/apimanagement/apis?redirectedfrom=MSDN
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `$expand` - _optional_ - Setting $expand=recommendedactions in url query expands the recommendedactions in the response.

### Lists the current availability status for all the resources in the resource group. Use the nextLink property in the response to get the next page of availability statuses.

*Tags:* `AvailabilityStatuses`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group.
* `api-version` - _required_ - Client Api Version.
* `$filter` - _optional_ - The filter to apply on the operation. For more information please see https://docs.microsoft.com/en-us/rest/api/apimanagement/apis?redirectedfrom=MSDN
* `$expand` - _optional_ - Setting $expand=recommendedactions in url query expands the recommendedactions in the response.

### Lists all historical availability transitions and impacting events for a single resource. Use the nextLink property in the response to get the next page of availability status

*Tags:* `AvailabilityStatuses`

#### Input Parameters
* `resourceUri` - _required_ - The fully qualified ID of the resource, including the resource name and resource type. Currently the API support not nested and one nesting level resource types : /subscriptions/{subscriptionId}/resourceGroups/{resource-group-name}/providers/{resource-provider-name}/{resource-type}/{resource-name} and /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resource-provider-name}/{parentResourceType}/{parentResourceName}/{resourceType}/{resourceName}
* `api-version` - _required_ - Client Api Version.
* `$filter` - _optional_ - The filter to apply on the operation. For more information please see https://docs.microsoft.com/en-us/rest/api/apimanagement/apis?redirectedfrom=MSDN
* `$expand` - _optional_ - Setting $expand=recommendedactions in url query expands the recommendedactions in the response.

### Gets current availability status for a single resource

*Tags:* `AvailabilityStatuses`

#### Input Parameters
* `resourceUri` - _required_ - The fully qualified ID of the resource, including the resource name and resource type. Currently the API support not nested and one nesting level resource types : /subscriptions/{subscriptionId}/resourceGroups/{resource-group-name}/providers/{resource-provider-name}/{resource-type}/{resource-name} and /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resource-provider-name}/{parentResourceType}/{parentResourceName}/{resourceType}/{resourceName}
* `api-version` - _required_ - Client Api Version.
* `$filter` - _optional_ - The filter to apply on the operation. For more information please see https://docs.microsoft.com/en-us/rest/api/apimanagement/apis?redirectedfrom=MSDN
* `$expand` - _optional_ - Setting $expand=recommendedactions in url query expands the recommendedactions in the response.

### Lists the historical availability statuses for a single child resource. Use the nextLink property in the response to get the next page of availability status

*Tags:* `ChildAvailabilityStatuses`

#### Input Parameters
* `resourceUri` - _required_ - The fully qualified ID of the resource, including the resource name and resource type. Currently the API only support one nesting level resource types : /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resource-provider-name}/{parentResourceType}/{parentResourceName}/{resourceType}/{resourceName}
* `api-version` - _required_ - Client Api Version.
* `$filter` - _optional_ - The filter to apply on the operation. For more information please see https://docs.microsoft.com/en-us/rest/api/apimanagement/apis?redirectedfrom=MSDN
* `$expand` - _optional_ - Setting $expand=recommendedactions in url query expands the recommendedactions in the response.

### Gets current availability status for a single resource

*Tags:* `ChildAvailabilityStatuses`

#### Input Parameters
* `resourceUri` - _required_ - The fully qualified ID of the resource, including the resource name and resource type. Currently the API only support one nesting level resource types : /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resource-provider-name}/{parentResourceType}/{parentResourceName}/{resourceType}/{resourceName}
* `api-version` - _required_ - Client Api Version.
* `$filter` - _optional_ - The filter to apply on the operation. For more information please see https://docs.microsoft.com/en-us/rest/api/apimanagement/apis?redirectedfrom=MSDN
* `$expand` - _optional_ - Setting $expand=recommendedactions in url query expands the recommendedactions in the response.

### Lists the all the children and its current health status for a parent resource. Use the nextLink property in the response to get the next page of children current health

*Tags:* `ChildResources`

#### Input Parameters
* `resourceUri` - _required_ - The fully qualified ID of the resource, including the resource name and resource type. Currently the API only support not nested parent resource type: /subscriptions/{subscriptionId}/resourceGroups/{resource-group-name}/providers/{resource-provider-name}/{resource-type}/{resource-name}
* `api-version` - _required_ - Client Api Version.
* `$filter` - _optional_ - The filter to apply on the operation. For more information please see https://docs.microsoft.com/en-us/rest/api/apimanagement/apis?redirectedfrom=MSDN
* `$expand` - _optional_ - Setting $expand=recommendedactions in url query expands the recommendedactions in the response.

## License

**flow**ground :- Telekom iPaaS / azure-com-resourcehealth-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
