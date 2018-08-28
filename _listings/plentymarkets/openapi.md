swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/{contactId}/documents:
    delete:
      summary: Delete files from contact documents
      description: Delete files from contact documents.
      operationId: deleteRestAccountsContactsContactDocuments
      x-api-path-slug: restaccountscontactscontactiddocuments-delete
      parameters:
      - in: path
        name: contactId
      - in: query
        name: keyList
        description: List of storage keys to delete
      responses:
        200:
          description: OK
      tags:
      - Files
      - From
      - Contact
      - Documents
  /rest/storage/frontend/files:
    delete:
      summary: Delete files from frontend storage.
      description: Deletes a list of files from frontend storage. A list of storage
        keys must be specified.
      operationId: deleteRestStorageFrontendFiles
      x-api-path-slug: reststoragefrontendfiles-delete
      parameters:
      - in: query
        name: keyList
        description: List of storage keys for the files to be deleted
      responses:
        200:
          description: OK
      tags:
      - Files
      - From
      - Frontend
      - Storage
    get:
      summary: List files from frontend storage. Append public cloudfront url to each
        retrieved object.
      description: List files from frontend storage. append public cloudfront url
        to each retrieved object..
      operationId: getRestStorageFrontendFiles
      x-api-path-slug: reststoragefrontendfiles-get
      parameters:
      - in: query
        name: continuationToken
        description: The continuationToken of a previous request to continue listing
          objects with
      responses:
        200:
          description: OK
      tags:
      - List
      - Files
      - From
      - Frontend
      - Storage
      - ""
      - Append
      - Public
      - Cloudfront
      - Url
      - To
      - Each
      - Retrieved
      - Object
  /rest/storage/plugins/inbox:
    delete:
      summary: Delete files from the inbox
      description: Deletes a list of files from the inbox. A list of storage keys
        must be specified.
      operationId: deleteRestStoragePluginsInbox
      x-api-path-slug: reststoragepluginsinbox-delete
      parameters:
      - in: query
        name: keyList
        description: List of storage keys for the files to be deleted
      responses:
        200:
          description: OK
      tags:
      - Files
      - From
      - Inbox
  /rest/storage/plugins/inbox/list:
    get:
      summary: List files from the inbox
      description: |-
        Lists all files of all plugins stored in the inbox. A prefix can be specified to list all files of a specific
        plugin folder only.
      operationId: getRestStoragePluginsInboxList
      x-api-path-slug: reststoragepluginsinboxlist-get
      parameters:
      - in: query
        name: prefix
        description: Prefix to list all files of a specific plugin folder only
      responses:
        200:
          description: OK
      tags:
      - List
      - Files
      - From
      - Inbox
  /rest/accounts/contacts/{contactId}/vcard:
    get:
      summary: get a filestream of vcard from customer
      description: Get a filestream of vcard from customer.
      operationId: getRestAccountsContactsContactVcard
      x-api-path-slug: restaccountscontactscontactidvcard-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Get
      - Filestream
      - Of
      - Vcard
      - From
      - Customer