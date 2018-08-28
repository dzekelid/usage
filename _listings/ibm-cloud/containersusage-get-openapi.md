---
swagger: "2.0"
x-collection-name: IBM Cloud
x-complete: 0
info:
  title: IBM Containers List container sizes and quota limits
  description: "This endpoint returns a list of available container sizes and the
    quota limit and usage for the space. \n\n- Container sizes: A list of available
    container sizes indicating the amount of container memory, disk space and virtual
    CPUs that can be assigned to the container.\n- Quota limit: Lists the number of
    containers, public IP addresses, available container memory, and virtual CPUS
    that are allocated to a space. \n- Quota usage: Lists the current number of containers,
    images, and public IP addresses in a space that is counted towards your quota
    limit."
  version: 3.0.0
host: containers-api.ng.bluemix.net
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /containers/usage:
    get:
      summary: List container sizes and quota limits
      description: "This endpoint returns a list of available container sizes and
        the quota limit and usage for the space. \n\n- Container sizes: A list of
        available container sizes indicating the amount of container memory, disk
        space and virtual CPUs that can be assigned to the container.\n- Quota limit:
        Lists the number of containers, public IP addresses, available container memory,
        and virtual CPUS that are allocated to a space. \n- Quota usage: Lists the
        current number of containers, images, and public IP addresses in a space that
        is counted towards your quota limit."
      operationId: this-endpoint-returns-a-list-of-available-container-sizes-and-the-quota-limit-and-usage-for-the-spac
      x-api-path-slug: containersusage-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Usage
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