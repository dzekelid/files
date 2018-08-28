---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Create Filter
  description: "Creates a new filter given a list of includes, excludes, a base filter,
    and whether or not this filter should be \"unsafe\".\n \nFilter \"safety\" is
    defined as follows. Any string returned as a result of an API call with a safe
    filter will be inline-able into HTML without script-injection concerns. That is
    to say, no additional sanitizing (encoding, HTML tag stripping, etc.) will be
    necessary on returned strings. Applications that wish to handle sanitizing themselves
    should create an unsafe filter. All filters are safe by default, under the assumption
    that double-encoding bugs are more desirable than script injections.\n \nIf no
    base filter is specified, the default filter is assumed. When building a filter
    from scratch, the none built-in filter is useful.\n \nWhen the size of the parameters
    being sent to this method grows to large, problems can occur. This method will
    accept POST requests to mitigate this.\n \nIt is not expected that many applications
    will call this method at runtime, filters should be pre-calculated and \"baked
    in\" in the common cases. Furthermore, there are a number of built-in filters
    which cover common use cases.\n \nThis method returns a single filter."
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /filters/create:
    get:
      summary: Create Filter
      description: "Creates a new filter given a list of includes, excludes, a base
        filter, and whether or not this filter should be \"unsafe\".\n \nFilter \"safety\"
        is defined as follows. Any string returned as a result of an API call with
        a safe filter will be inline-able into HTML without script-injection concerns.
        That is to say, no additional sanitizing (encoding, HTML tag stripping, etc.)
        will be necessary on returned strings. Applications that wish to handle sanitizing
        themselves should create an unsafe filter. All filters are safe by default,
        under the assumption that double-encoding bugs are more desirable than script
        injections.\n \nIf no base filter is specified, the default filter is assumed.
        When building a filter from scratch, the none built-in filter is useful.\n
        \nWhen the size of the parameters being sent to this method grows to large,
        problems can occur. This method will accept POST requests to mitigate this.\n
        \nIt is not expected that many applications will call this method at runtime,
        filters should be pre-calculated and \"baked in\" in the common cases. Furthermore,
        there are a number of built-in filters which cover common use cases.\n \nThis
        method returns a single filter."
      operationId: creates-a-new-filter-given-a-list-of-includes-excludes-a-base-filter-and-whether-or-not-this-filter-
      x-api-path-slug: filterscreate-get
      parameters:
      - in: query
        name: base
      - in: query
        name: exclude
        description: String list (semicolon delimited)
      - in: query
        name: include
        description: String list (semicolon delimited)
      - in: query
        name: unsafe
      responses:
        200:
          description: OK
      tags:
      - Files
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