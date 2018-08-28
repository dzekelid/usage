swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{projectid}/diskusage:
    get:
      summary: Gets project disk usage in bytes
      description: Gets project disk usage in bytes.
      operationId: getProjectDiskUsage
      x-api-path-slug: projectsprojectiddiskusage-get
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Disk
      - Usage
      - In
      - Bytes