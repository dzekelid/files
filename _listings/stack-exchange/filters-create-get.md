---
swagger: "2.0"
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
      description: Creates a new filter given a list of includes, excludes, a base
        filter, and whether or not this filter should be "unsafe"
      operationId: creates-a-new-filter-given-a-list-of-includes-excludes-a-base-filter-and-whether-or-not-this-filter-
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
      - files
definitions:
  created_comment:
    properties:
      body:
        description: This is a default description.
        type: get
      body_markdown:
        description: This is a default description.
        type: get
      can_flag:
        description: This is a default description.
        type: get
      comment_id:
        description: This is a default description.
        type: get
      creation_date:
        description: This is a default description.
        type: get
      edited:
        description: This is a default description.
        type: get
      link:
        description: This is a default description.
        type: get
      owner:
        description: This is a default description.
        type: get
      post_id:
        description: This is a default description.
        type: get
      post_type:
        description: This is a default description.
        type: get
  error:
    properties:
      error_id:
        description: This is a default description.
        type: get
      error_message:
        description: This is a default description.
        type: get
      error_name:
        description: This is a default description.
        type: get
  info_object:
    properties:
      answers_per_minute:
        description: This is a default description.
        type: get
      api_revision:
        description: This is a default description.
        type: get
      badges_per_minute:
        description: This is a default description.
        type: get
      new_active_users:
        description: This is a default description.
        type: get
      questions_per_minute:
        description: This is a default description.
        type: get
      site:
        description: This is a default description.
        type: get
      total_accepted:
        description: This is a default description.
        type: get
      total_answers:
        description: This is a default description.
        type: get
      total_badges:
        description: This is a default description.
        type: get
      total_comments:
        description: This is a default description.
        type: get
  single_filter:
    properties:
      filter:
        description: This is a default description.
        type: get
      filter_type:
        description: This is a default description.
        type: get
      included_fields:
        description: This is a default description.
        type: get
  user:
    properties:
      about_me:
        description: This is a default description.
        type: get
      accept_rate:
        description: This is a default description.
        type: get
      account_id:
        description: This is a default description.
        type: get
      age:
        description: This is a default description.
        type: get
      answer_count:
        description: This is a default description.
        type: get
      badge_counts:
        description: This is a default description.
        type: get
      creation_date:
        description: This is a default description.
        type: get
      display_name:
        description: This is a default description.
        type: get
      down_vote_count:
        description: This is a default description.
        type: get
      is_employee:
        description: This is a default description.
        type: get
x-collection-name: Stack Exchange
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