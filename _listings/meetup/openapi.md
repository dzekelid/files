---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
  description: the-meetup-api-provides-simple-restful-http-and-streaming-interfaces-for-exploring-and-interacting-meetup-platform-from-your-own-apps--the-api-is-a-set-of-core-methods-and-a-common-request-format--these-are-combined-to-form-a-url-that-returns-the-information-you-want--
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /members/:member_id:
    patch:
      summary: Member Profile Edit
      description: Edits Member Profiles.For Group Profiles, see [this endpoint](/meetup_api/docs/:urlname/members/:member_id)
      operationId: profiles
      x-api-path-slug: membersmember-id-patch
      parameters:
      - in: query
        name: add_topics
        description: Comma-delimited list of topic ids to add to members interest
          list
        type: string
      - in: query
        name: bio
        description: Member bio of up to 250 characters
        type: string
      - in: query
        name: bio_privacy
        description: Preference for hiding or showing member bio to others
        type: string
      - in: query
        name: birthday
        description: Members date or year of birth
        type: string
      - in: query
        name: city_id
        description: Valid Meetup city identifier that indicates the city in which
          the member resides
        type: string
      - in: query
        name: facebook_privacy
        description: Preference for hiding showing information members facebook connection
        type: string
      - in: query
        name: gender
        description: Members gender
        type: string
      - in: query
        name: groups_privacy
        description: Preference for hiding or showing group memberships to others
        type: string
      - in: query
        name: lang
        description: Members language preference
        type: string
      - in: query
        name: lat
        description: A valid latitude to resolve the closest location to associate
          with the member
        type: string
      - in: query
        name: lon
        description: A valid longitude to resolve the closest location to associate
          with the memberThis parameter must be accompanied by lat and zip
        type: string
      - in: query
        name: messaging_pref
        description: Preference for which members may contact you via the Meetup platform
        type: string
      - in: query
        name: name
        description: Member name
        type: string
      - in: query
        name: photo_id
        description: A valid photo id to this member has previously updated to use
          as profile photo
        type: string
      - in: query
        name: remove_topics
        description: Comma-delimited list of topic ids to remove from members interest
          list
        type: string
      - in: query
        name: sync_photo
        description: When set to true, this parameter will sync all the groupprofile
          photos for the member with the provided photo_id
        type: string
      - in: query
        name: topics_privacy
        description: Preference for hiding or showing member interests to others
        type: string
      - in: query
        name: zip
        description: A valid zip code to associate with the member
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Profiles
---