---
swagger: "2.0"
x-collection-name: Azure Traffic Manager
x-complete: 1
info:
  title: TrafficManagerManagementClient
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /providers/Microsoft.Network/checkTrafficManagerNameAvailability:
    post:
      summary: Profiles Check Traffic Manager Relative Dns Name Availability
      description: Checks the availability of a Traffic Manager Relative DNS name.
      operationId: Profiles_CheckTrafficManagerRelativeDnsNameAvailability
      x-api-path-slug: providersmicrosoft-networkchecktrafficmanagernameavailability-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The Traffic Manager name parameters supplied to the CheckTrafficManagerNameAvailability
          operation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Profiles Traffic Manager Relative Dns Name Availability
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/trafficmanagerprofiles:
    get:
      summary: Profiles List By In Resource Group
      description: Lists all Traffic Manager profiles within a resource group.
      operationId: Profiles_ListByInResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networktrafficmanagerprofiles-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the Traffic Manager
          profiles to be listed
      responses:
        200:
          description: OK
      tags:
      - Profiles
  /subscriptions/{subscriptionId}/providers/Microsoft.Network/trafficmanagerprofiles:
    get:
      summary: Profiles List All
      description: Lists all Traffic Manager profiles within a subscription.
      operationId: Profiles_ListAll
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-networktrafficmanagerprofiles-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Profiles
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/trafficmanagerprofiles/{profileName}
  : get:
      summary: Profiles Get
      description: Gets a Traffic Manager profile.
      operationId: Profiles_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networktrafficmanagerprofilesprofilename-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: profileName
        description: The name of the Traffic Manager profile
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the Traffic Manager
          profile
      responses:
        200:
          description: OK
      tags:
      - Profiles
    put:
      summary: Profiles Create Or Update
      description: Create or update a Traffic Manager profile.
      operationId: Profiles_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networktrafficmanagerprofilesprofilename-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The Traffic Manager profile parameters supplied to the CreateOrUpdate
          operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileName
        description: The name of the Traffic Manager profile
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the Traffic Manager
          profile
      responses:
        200:
          description: OK
      tags:
      - Profiles
    delete:
      summary: Profiles Delete
      description: Deletes a Traffic Manager profile.
      operationId: Profiles_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networktrafficmanagerprofilesprofilename-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: profileName
        description: The name of the Traffic Manager profile to be deleted
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the Traffic Manager
          profile to be deleted
      responses:
        200:
          description: OK
      tags:
      - Profiles
    patch:
      summary: Profiles Update
      description: Update a Traffic Manager profile.
      operationId: Profiles_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networktrafficmanagerprofilesprofilename-patch
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The Traffic Manager profile parameters supplied to the Update
          operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileName
        description: The name of the Traffic Manager profile
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the Traffic Manager
          profile
      responses:
        200:
          description: OK
      tags:
      - Profiles
---