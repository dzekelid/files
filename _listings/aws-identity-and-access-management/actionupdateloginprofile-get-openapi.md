---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Update Login Profile
  version: 1.0.0
  description: Changes the password for the specified IAM user.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateInstanceProfile:
    get:
      summary: Create Instance Profile
      description: Creates a new instance profile.
      operationId: createInstanceProfile
      x-api-path-slug: actioncreateinstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to create
        type: string
      - in: query
        name: Path
        description: The path to the instance profile
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles
  /?Action=CreateLoginProfile:
    get:
      summary: Create Login Profile
      description: |-
        Creates a password for the specified user, giving the user the ability to access AWS
              services through the AWS Management Console.
      operationId: createLoginProfile
      x-api-path-slug: actioncreateloginprofile-get
      parameters:
      - in: query
        name: Password
        description: The new password for the user
        type: string
      - in: query
        name: PasswordResetRequired
        description: Specifies whether the user is required to set a new password
          on next sign-in
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user to create a password for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Login Profiles
  /?Action=DeleteInstanceProfile:
    get:
      summary: Delete Instance Profile
      description: Deletes the specified instance profile.
      operationId: deleteInstanceProfile
      x-api-path-slug: actiondeleteinstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles
  /?Action=DeleteLoginProfile:
    get:
      summary: Delete Login Profile
      description: |-
        Deletes the password for the specified IAM user, which terminates the user's ability
              to access AWS services through the AWS Management Console.
      operationId: deleteLoginProfile
      x-api-path-slug: actiondeleteloginprofile-get
      parameters:
      - in: query
        name: UserName
        description: The name of the user whose password you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Login Profiles
  /?Action=GetInstanceProfile:
    get:
      summary: Get Instance Profile
      description: |-
        Retrieves information about the specified instance profile, including the instance
              profile's path, GUID, ARN, and role.
      operationId: getInstanceProfile
      x-api-path-slug: actiongetinstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to get information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles
  /?Action=GetLoginProfile:
    get:
      summary: Get Login Profile
      description: Retrieves the user name and password-creation date for the specified
        IAM user.
      operationId: getLoginProfile
      x-api-path-slug: actiongetloginprofile-get
      parameters:
      - in: query
        name: UserName
        description: The name of the user whose login profile you want to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Login Profiles
  /?Action=ListInstanceProfiles:
    get:
      summary: List Instance Profiles
      description: Lists the instance profiles that have the specified path prefix.
      operationId: listInstanceProfiles
      x-api-path-slug: actionlistinstanceprofiles-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles
  /?Action=ListInstanceProfilesForRole:
    get:
      summary: List Instance Profiles For Role
      description: Lists the instance profiles that have the specified associated
        IAM role.
      operationId: listInstanceProfilesForRole
      x-api-path-slug: actionlistinstanceprofilesforrole-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: RoleName
        description: The name of the role to list instance profiles for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles For Role
  /?Action=RemoveRoleFromInstanceProfile:
    get:
      summary: Remove Role From Instance Profile
      description: Removes the specified IAM role from the specified EC2 instance
        profile.
      operationId: removeRoleFromInstanceProfile
      x-api-path-slug: actionremoverolefrominstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to update
        type: string
      - in: query
        name: RoleName
        description: The name of the role to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role From Instance Profiles
  /?Action=UpdateLoginProfile:
    get:
      summary: Update Login Profile
      description: Changes the password for the specified IAM user.
      operationId: updateLoginProfile
      x-api-path-slug: actionupdateloginprofile-get
      parameters:
      - in: query
        name: Password
        description: The new password for the specified IAM user
        type: string
      - in: query
        name: PasswordResetRequired
        description: Allows this new password to be used only once by requiring the
          specified IAM user to      set a new password on next sign-in
        type: string
      - in: query
        name: UserName
        description: The name of the user whose password you want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Login Profiles
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