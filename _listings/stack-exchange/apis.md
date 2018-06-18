---
name: Stack Exchange
x-slug: stack-exchange
description: After someone asks a question, members of the community propose answers.
  Others vote on those answers. Very quickly, the answers with the most votes rise
  to the top. You don???t have to read through a lot of discussion to find the best
  answer.    Like to...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
x-kinRank: "8"
x-alexaRank: "126"
tags: Files
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/stack-exchange/apis.md
specificationVersion: "0.14"
apis:
- name: Stack Exchange Create Filter
  x-api-slug: stack-exchange
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//filters/create
  tags: Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/stack-exchange/filterscreate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/stack-exchange/filterscreate-get-openapi.md
- name: Stack Exchange Get Filters
  x-api-slug: stack-exchange
  description: "Returns the fields included by the given filters, and the \"safeness\"
    of those filters.\n \nIt is not expected that this method will be consumed by
    many applications at runtime, it is provided to aid in debugging.\n \n{filters}
    can contain up to 20 semicolon delimited filters. Filters are obtained via calls
    to /filters/create, or by using a built-in filter.\n \nThis method returns a list
    of filters."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//filters/{filters}
  tags: Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/stack-exchange/filtersfilters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/stack-exchange/filtersfilters-get-openapi.md
- name: Stack Exchange
  x-api-slug: stack-exchange
  description: After someone asks a question, members of the community propose answers.
    Others vote on those answers. Very quickly, the answers with the most votes rise
    to the top. You don???t have to read through a lot of discussion to find the best
    answer.    Like to...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/stack-exchange/openapi.md
x-common:
- type: x-authentication
  url: https://api.stackexchange.com/docs/authentication
- type: x-base
  url: https://api.stackexchange.com/
- type: x-blog
  url: http://stackexchange.com/blogs
- type: x-blog-rss
  url: http://blog.stackoverflow.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stack-exchange
- type: x-crunchbase
  url: https://crunchbase.com/organization/stack-exchange
- type: x-developer
  url: http://api.stackexchange.com/
- type: x-email
  url: legal@stackexchange.com
- type: x-email
  url: team@stackexchange.com
- type: x-email
  url: team+api@stackexchange.com
- type: x-error-codes
  url: https://api.stackexchange.com/docs/error-handling
- type: x-github
  url: https://github.com/StackExchange
- type: x-javascript-sdk
  url: https://api.stackexchange.com/docs/js-lib
- type: x-privacy
  url: https://stackexchange.com/legal/privacy-policy
- type: x-rate-limits
  url: https://api.stackexchange.com/docs/throttle
- type: x-selfservice-registration
  url: https://stackapps.com/users/login?returnurl=/apps/oauth/register
- type: x-support
  url: https://stackexchange.com/about/contact
- type: x-terms-of-service
  url: http://stackexchange.com/legal/api-terms-of-use
- type: x-twitter
  url: https://twitter.com/StackExchange
- type: x-website
  url: http://stackexchange.com
- type: x-website
  url: https://stackexchange.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---