---
name: Slack
x-slug: slack
description: Slack is a team communication application providing services such as
  real-time messaging, archiving, and to search for modern teams. It offers one-on-one
  messaging, private groups, persistent chat rooms, and direct messaging as well as
  group chats organized by topic. All content inside Slack is searchable from one
  search box and it integrates with a number of third-party services, including Google
  Docs, Dropbox, Heroku, Crashlytics, GitHub, and Zendesk.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Files
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/apis.md
specificationVersion: "0.14"
apis:
- name: Slack Edit File Comments
  x-api-slug: slack
  description: Edit an existing file comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//files.comments.edit
  tags: Messaging,Files,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-comments-edit-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-comments-edit-post-openapi.md
- name: Slack Upload File
  x-api-slug: slack
  description: Uploads or creates a file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//files.upload
  tags: Messaging,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-upload-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-upload-post-openapi.md
- name: Slack Delete File Comments
  x-api-slug: slack
  description: Deletes an existing comment on a file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//files.comments.delete
  tags: Messaging,Files,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-comments-delete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-comments-delete-post-openapi.md
- name: Slack Revoke Public URL
  x-api-slug: slack
  description: Revokes public/external sharing access for a file
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//files.revokePublicURL
  tags: Messaging,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-revokepublicurl-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-revokepublicurl-post-openapi.md
- name: Slack List Files
  x-api-slug: slack
  description: Lists & filters team files.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//files.list
  tags: Messaging,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-list-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-list-get-openapi.md
- name: Slack Delete File
  x-api-slug: slack
  description: Deletes a file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//files.delete
  tags: Messaging,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-delete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-delete-post-openapi.md
- name: Slack Get File
  x-api-slug: slack
  description: Gets information about a team file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//files.info
  tags: Messaging,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-info-get-openapi.md
- name: Slack Share Public URL
  x-api-slug: slack
  description: Enables a file for public/external sharing.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//files.sharedPublicURL
  tags: Messaging,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-sharedpublicurl-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-sharedpublicurl-post-openapi.md
- name: Slack Add File Comments
  x-api-slug: slack
  description: Add a comment to an existing file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//files.comments.add
  tags: Messaging,Files,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-comments-add-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/files-comments-add-post-openapi.md
- name: Slack
  x-api-slug: slack
  description: Slack is a team communication application providing services such as
    real-time messaging, archiving, and to search for modern teams. It offers one-on-one
    messaging, private groups, persistent chat rooms, and direct messaging as well
    as group chats organized by topic. All content inside Slack is searchable from
    one search box and it integrates with a number of third-party services, including
    Google Docs, Dropbox, Heroku, Crashlytics, GitHub, and Zendesk.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/files/master/_listings/slack/openapi.md
x-common:
- type: x-website
  url: https://api.slack.com
- type: x-application-gallery
  url: https://slack.com/apps
- type: x-blog
  url: http://slackhq.com/
- type: x-blog
  url: https://medium.com/slack-developer-blog
- type: x-blog-rss
  url: http://slackhq.com/rss
- type: x-blog-rss
  url: https://medium.com/feed/slack-developer-blog
- type: x-branding
  url: https://slack.com/brand-guidelines
- type: x-buttons
  url: https://api.slack.com/docs/slack-button
- type: x-c-sharp-sdk
  url: https://api.slack.com/web
- type: x-change-log
  url: https://api.slack.com/changelog
- type: x-developer
  url: https://api.slack.com/
- type: x-faq
  url: https://api.slack.com/faq
- type: x-getting-started
  url: https://slack.com/getting-started
- type: x-github
  url: https://github.com/slackhq
- type: x-incoming-webhooks
  url: https://api.slack.com/incoming-webhooks
- type: x-oauth-overview
  url: https://api.slack.com/docs/oauth
- type: x-oauth-scopes
  url: https://api.slack.com/docs/oauth-scopes
- type: x-outgoing-webhooks
  url: https://api.slack.com/outgoing-webhooks
- type: x-presence
  url: https://api.slack.com/docs/presence
- type: x-pricing
  url: https://slack.com/pricing
- type: x-privacy
  url: https://slack.com/privacy-policy
- type: x-rate-limits
  url: https://api.slack.com/docs/rate-limits
- type: x-real-time-messaging-api
  url: https://api.slack.com/rtm
- type: x-road-map
  url: https://api.slack.com/roadmap
- type: x-security
  url: https://slack.com/security
- type: x-status
  url: https://status.slack.com/
- type: x-support
  url: https://get.slack.help/hc/en-us
- type: x-terms-of-service
  url: https://slack.com/terms-of-service
- type: x-transparency-report
  url: https://slack.com/transparency-report
- type: x-twitter
  url: https://twitter.com/slackapi
- type: x-website
  url: http://slack.com
- type: x-website
  url: https://slack.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---