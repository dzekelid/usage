swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/usage_rights:
    delete:
      summary: Remove usage rights
      description: Remove usage rights.
      operationId: remove-usage-rights
      x-api-path-slug: coursescourse-idusage-rights-delete
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to remove associated usage rights from
      - in: query
        name: folder_ids[]
        description: List of ids of folders
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Usage
      - Rights
    put:
      summary: Set usage rights
      description: Set usage rights.
      operationId: set-usage-rights
      x-api-path-slug: coursescourse-idusage-rights-put
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to set usage rights for
      - in: query
        name: folder_ids[]
        description: List of ids of folders to search for files to set usage rights
          for
      - in: query
        name: publish
        description: Whether the file(s) or folder(s) should be published on save,
          provided thatnusage rights have been specified (set to `true` to publish
          on save)
      - in: query
        name: usage_rights[legal_copyright]
        description: The legal copyright line for the files
      - in: query
        name: usage_rights[license]
        description: The license that applies to the files
      - in: query
        name: usage_rights[use_justification]
        description: 'The intellectual property justification for using the files
          in Canvasnn        n        n          Allowed values: own_copyright, used_by_permission,
          fair_use, public_domain, creative_commons'
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Usage
      - Rights
  /groups/{group_id}/usage_rights:
    delete:
      summary: Remove usage rights
      description: Remove usage rights.
      operationId: remove-usage-rights
      x-api-path-slug: groupsgroup-idusage-rights-delete
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to remove associated usage rights from
      - in: query
        name: folder_ids[]
        description: List of ids of folders
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Usage
      - Rights
    put:
      summary: Set usage rights
      description: Set usage rights.
      operationId: set-usage-rights
      x-api-path-slug: groupsgroup-idusage-rights-put
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to set usage rights for
      - in: query
        name: folder_ids[]
        description: List of ids of folders to search for files to set usage rights
          for
      - in: query
        name: publish
        description: Whether the file(s) or folder(s) should be published on save,
          provided thatnusage rights have been specified (set to `true` to publish
          on save)
      - in: query
        name: usage_rights[legal_copyright]
        description: The legal copyright line for the files
      - in: query
        name: usage_rights[license]
        description: The license that applies to the files
      - in: query
        name: usage_rights[use_justification]
        description: 'The intellectual property justification for using the files
          in Canvasnn        n        n          Allowed values: own_copyright, used_by_permission,
          fair_use, public_domain, creative_commons'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Usage
      - Rights
  /users/{user_id}/usage_rights:
    delete:
      summary: Remove usage rights
      description: Remove usage rights.
      operationId: remove-usage-rights
      x-api-path-slug: usersuser-idusage-rights-delete
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to remove associated usage rights from
      - in: query
        name: folder_ids[]
        description: List of ids of folders
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Usage
      - Rights
    put:
      summary: Set usage rights
      description: Set usage rights.
      operationId: set-usage-rights
      x-api-path-slug: usersuser-idusage-rights-put
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to set usage rights for
      - in: query
        name: folder_ids[]
        description: List of ids of folders to search for files to set usage rights
          for
      - in: query
        name: publish
        description: Whether the file(s) or folder(s) should be published on save,
          provided thatnusage rights have been specified (set to `true` to publish
          on save)
      - in: query
        name: usage_rights[legal_copyright]
        description: The legal copyright line for the files
      - in: query
        name: usage_rights[license]
        description: The license that applies to the files
      - in: query
        name: usage_rights[use_justification]
        description: 'The intellectual property justification for using the files
          in Canvasnn        n        n          Allowed values: own_copyright, used_by_permission,
          fair_use, public_domain, creative_commons'
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Usage
      - Rights