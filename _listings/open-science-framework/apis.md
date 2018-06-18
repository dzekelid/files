---
name: Open Science Framework
x-slug: open-science-framework
description: OSF provides free and open source project management support for researchers
  across the entire research lifecycle. As a collaboration tool, OSF helps researchers
  work on projects privately with a limited number of collaborators and make parts
  of their projects public, or make all the project publicly accessible for broader
  dissemination. As a workflow system, OSF enables connections to the many services
  researchers already use to streamline their process and increase efficiency. As
  a flexible repository, it can store and archive research data, protocols, and materials.
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Files
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/apis.md
specificationVersion: "0.14"
apis:
- name: Open Science Framework Retrieve a file
  x-api-slug: open-science-framework
  description: |-
    Retrieves the details of a file (or folder)
    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested file, if the request was successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
    ###Waterbutler API actions

    Files can be modified through the Waterbutler API routes found in `links` (`new_folder`, `move`, `upload`, `download`, and `delete`).

    #### Download (files)

    To download a file, issue a GET request against the download link. The response will have the Content-Disposition header set, which will will trigger a download in a browser.

    #### Create Subfolder (folders)

    You can create a subfolder of an existing folder by issuing a PUT request against the new_folder link. The ?kind=folder portion of the query parameter is already included in the new_folder link. The name of the new subfolder should be provided in the name query parameter. The response will contain a WaterButler folder entity. If a folder with that name already exists in the parent directory, the server will return a 409 Conflict error response.

    #### Upload New File (folders)


      To upload a file to a folder, issue a PUT request to the folder's upload link with the raw file data in the request body, and the kind and name query parameters set to 'file' and the desired name of the file. The response will contain a WaterButler file entity that describes the new file. If a file with the same name already exists in the folder, the server will return a 409 Conflict error response.


    #### Update Existing File (file)

    To update an existing file, issue a PUT request to the file's upload link with the raw file data in the request body and the kind query parameter set to "file". The update action will create a new version of the file. The response will contain a WaterButler file entity that describes the updated file.

    #### Rename (files, folders)

    To rename a file or folder, issue a POST request to the move link with the action body parameter set to "rename" and the rename body parameter set to the desired name. The response will contain either a folder entity or file entity with the new name.

    #### Move & Copy (files, folders)

    Move and copy actions both use the same request structure, a POST to the move url, but with different values for the action body parameters. The path parameter is also required and should be the OSF path attribute of the folder being written to. The rename and conflict parameters are optional. If you wish to change the name of the file or folder at its destination, set the rename parameter to the new name. The conflict param governs how name clashes are resolved. Possible values are replace and keep. replace is the default and will overwrite the file that already exists in the target folder. keep will attempt to keep both by adding a suffix to the new file's name until it no longer conflicts. The suffix will be ' (x)' where x is a increasing integer starting from 1. This behavior is intended to mimic that of the OS X Finder. The response will contain either a folder entity or file entity with the new name.
    Files and folders can also be moved between nodes and providers. The resource parameter is the id of the node under which the file/folder should be moved. It must agree with the path parameter, that is the path must identify a valid folder under the node identified by resource. Likewise, the provider parameter may be used to move the file/folder to another storage provider, but both the resource and path parameters must belong to a node and folder already extant on that provider. Both resource and provider default to the current node and providers.
    If a moved/copied file is overwriting an existing file, a 200 OK response will be returned. Otherwise, a 201 Created will be returned.

    #### Delete (file, folders)

    To delete a file or folder send a DELETE request to the delete link. Nothing will be returned in the response body.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//files/{file_id}/
  tags: Files,File
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/filesfile-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/filesfile-id-get-openapi.md
- name: Open Science Framework Update a file
  x-api-slug: open-science-framework
  description: |-
    Updates the specified file by setting the values of the parameters passed. Any parameters not provided will be left unchanged.
    #### Returns
    Returns JSON with a `data` key containing the new representation of the updated file, if the request is successful.

    If the request is unsuccessful, JSON with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//files/{file_id}/
  tags: Files,File
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/filesfile-id-patch-openapi.md
- name: Open Science Framework List all file versions
  x-api-slug: open-science-framework
  description: |-
    A paginated list of all file versions.
    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of 10 file versions. Each resource in the array is a separate file version object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//files/{file_id}/versions/
  tags: Files,File,Versions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/filesfile-idversions-get-openapi.md
- name: Open Science Framework Retrieve a file version
  x-api-slug: open-science-framework
  description: |-
    Retrieves the details of a file version
    ####Returns

    Returns a JSON object with a `data` key containing the representation of the requested file, if the request was successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//files/{file_id}/versions/{version_id}/
  tags: Files,File,Versions,Version
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/filesfile-idversionsversion-id-get-openapi.md
- name: Open Science Framework List all storage providers
  x-api-slug: open-science-framework
  description: |-
    List of all storage providers that are configured for this node

    Users of the OSF may access their data on a [number of cloud-storage services](https://api.osf.io/v2/#storage-providers) that have integrations with the OSF. We call these **providers**. By default, every node has access to the OSF-provided storage but may use as many of the supported providers as desired.


    ####Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of files. Each resource in the array is a separate file object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    Note: In the OSF filesystem model, providers are treated as folders, but with special properties that distinguish them from regular folders. Every provider folder is considered a root folder, and may not be deleted through the regular file API.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//nodes/{node_id}/files/
  tags: Nodes,Node,Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/nodesnode-idfiles-get-openapi.md
- name: Open Science Framework Retrieve a storage provider
  x-api-slug: open-science-framework
  description: |-
    Retrieves the details of a storage provider enabled on this node.
    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested file object, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//nodes/{node_id}/files/providers/{provider}/
  tags: Nodes,Node,Files,Providers,Provider
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/nodesnode-idfilesprovidersprovider-get-openapi.md
- name: Open Science Framework List all node files
  x-api-slug: open-science-framework
  description: |-
    List of all the files/folders that are attached to your project for a given storage provider.
    ####Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of files. Each resource in the array is a separate file object and contains the full representation of the file.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    ####Filtering

    You can optionally request that the response only include files that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/ezcuj/files/osfstorage/?filter[kind]=file

    Node files may be filtered by `id`, `name`, `node`, `kind`, `path`, `provider`, `size`, and `last_touched`.

    ###Waterbutler API actions

    Files can be modified through the Waterbutler API routes found in `links` (`new_folder`, `move`, `upload`, `download`, and `delete`).

    #### Download (files)

    To download a file, issue a GET request against the download link. The response will have the Content-Disposition header set, which will will trigger a download in a browser.

    #### Create Subfolder (folders)

    You can create a subfolder of an existing folder by issuing a PUT request against the new_folder link. The ?kind=folder portion of the query parameter is already included in the new_folder link. The name of the new subfolder should be provided in the name query parameter. The response will contain a WaterButler folder entity. If a folder with that name already exists in the parent directory, the server will return a 409 Conflict error response.

    #### Upload New File (folders)

    To upload a file to a folder, issue a PUT request to the folder's upload link with the raw file data in the request body, and the kind and name query parameters set to 'file' and the desired name of the file. The response will contain a WaterButler file entity that describes the new file. If a file with the same name already exists in the folder, the server will return a 409 Conflict error response.

    #### Update Existing File (file)

    To update an existing file, issue a PUT request to the file's upload link with the raw file data in the request body and the kind query parameter set to "file". The update action will create a new version of the file. The response will contain a WaterButler file entity that describes the updated file.

    #### Rename (files, folders)

    To rename a file or folder, issue a POST request to the move link with the action body parameter set to "rename" and the rename body parameter set to the desired name. The response will contain either a folder entity or file entity with the new name.

    #### Move & Copy (files, folders)

    Move and copy actions both use the same request structure, a POST to the move url, but with different values for the action body parameters. The path parameter is also required and should be the OSF path attribute of the folder being written to. The rename and conflict parameters are optional. If you wish to change the name of the file or folder at its destination, set the rename parameter to the new name. The conflict param governs how name clashes are resolved. Possible values are replace and keep. replace is the default and will overwrite the file that already exists in the target folder. keep will attempt to keep both by adding a suffix to the new file's name until it no longer conflicts. The suffix will be ' (x)' where x is a increasing integer starting from 1. This behavior is intended to mimic that of the OS X Finder. The response will contain either a folder entity or file entity with the new name.
    Files and folders can also be moved between nodes and providers. The resource parameter is the id of the node under which the file/folder should be moved. It must agree with the path parameter, that is the path must identify a valid folder under the node identified by resource. Likewise, the provider parameter may be used to move the file/folder to another storage provider, but both the resource and path parameters must belong to a node and folder already extant on that provider. Both resource and provider default to the current node and providers.
    If a moved/copied file is overwriting an existing file, a 200 OK response will be returned. Otherwise, a 201 Created will be returned.

    #### Delete (file, folders)

    To delete a file or folder send a DELETE request to the delete link. Nothing will be returned in the response body.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//nodes/{node_id}/files/{provider}/
  tags: Nodes,Node,Files,Provider
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/nodesnode-idfilesprovider-get-openapi.md
- name: Open Science Framework Retrieve a file
  x-api-slug: open-science-framework
  description: |-
    Retrieves the details of a file attached to given node (project or component) for the given storage provider.
    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested file object, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//nodes/{node_id}/files/{provider}/{path}/
  tags: Nodes,Node,Files,Provider,Path
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/nodesnode-idfilesproviderpath-get-openapi.md
- name: Open Science Framework List all storage providers
  x-api-slug: open-science-framework
  description: |-
    A paginated list of storage providers enabled on the registration

    Users of the OSF may access their data on a [number of cloud-storage services](https://api.osf.io/v2/#storage-providers) that have integrations with the OSF. We call these **providers**. By default, every node has access to the OSF-provided storage but may use as many of the supported providers as desired.


    ####Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of up to 10 files. Each resource in the array is a separate file object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    Note: In the OSF filesystem model, providers are treated as folders, but with special properties that distinguish them from regular folders. Every provider folder is considered a root folder, and may not be deleted through the regular file API.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/files/
  tags: Registrations,Registration,Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/registrationsregistration-idfiles-get-openapi.md
- name: Open Science Framework List all files
  x-api-slug: open-science-framework
  description: |-
    List of all the registration's files/folders for a given storage provider.

    ####Returns

    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of files. Each resource in the array is a separate file object and contains the full representation of the file.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    ####Filtering

    You can optionally request that the response only include files that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/files/osfstorage/?filter[kind]=file

    Files may be filtered by `id`, `name`, `node`, `kind`, `path`, `provider`, `size`, and `last_touched`.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/files/{provider}/
  tags: Registrations,Registration,Files,Provider
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/registrationsregistration-idfilesprovider-get-openapi.md
- name: Open Science Framework Retrieve a file
  x-api-slug: open-science-framework
  description: |-
    Retrieves the details of a registration file for the given storage provider.
    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested registration file object, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/files/{provider}/{path}/
  tags: Registrations,Registration,Files,Provider,Path
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/registrationsregistration-idfilesproviderpath-get-openapi.md
- name: Open Science Framework
  x-api-slug: open-science-framework
  description: OSF provides free and open source project management support for researchers
    across the entire research lifecycle. As a collaboration tool, OSF helps researchers
    work on projects privately with a limited number of collaborators and make parts
    of their projects public, or make all the project publicly accessible for broader
    dissemination. As a workflow system, OSF enables connections to the many services
    researchers already use to streamline their process and increase efficiency. As
    a flexible repository, it can store and archive research data, protocols, and
    materials.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/open-science-framework/openapi.md
x-common:
- type: x-website
  url: https://cos.io
- type: x-github
  url: https://github.com/OSFramework
- type: x-twitter
  url: https://twitter.com/OSFramework
- type: x-website
  url: http://osf.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---