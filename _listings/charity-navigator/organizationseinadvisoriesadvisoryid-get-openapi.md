---
swagger: "2.0"
x-collection-name: Charity Navigator
x-complete: 0
info:
  title: Charity Navigator Get Organizations Ein Advisories Advisory
  description: |-
    Retrieve full details of a single Advisory, under a given organization. An
    advisory is a cautionary communication from Charity Navigator, advising of
    unusual events or behavior related to a known organization.
  version: 1.0.0
host: api.data.charitynavigator.org
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Organizations/{ein}/Advisories:
    get:
      summary: Get Organizations Ein Advisories
      description: |-
        Retrieve the full set of Charity Navigator advisories for a specified
        organization. An advisory is a cautionary communication from Charity Navigator,
        advising of unusual events or behavior related to a known organization.
      operationId: getAdvisories
      x-api-path-slug: organizationseinadvisories-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: path
        name: ein
      - in: query
        name: pageNum
        description: Page number to return, in case the number of available objects
          in the resultset is greater than the specified or default `pageSize`
      - in: query
        name: pageSize
        description: Number of objects to return in a single response message
      - in: query
        name: status
        description: An optional filter parameter to limit the Advisories returned,
          based onstatus:| Status Value | Advisories Included                                 ||
          ------------ | --------------------------------------------------- || ALL
          | All advisories included, regardless of status
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Ein
      - Advisories
  /Organizations/{ein}/Advisories/{AdvisoryID}:
    get:
      summary: Get Organizations Ein Advisories Advisory
      description: |-
        Retrieve full details of a single Advisory, under a given organization. An
        advisory is a cautionary communication from Charity Navigator, advising of
        unusual events or behavior related to a known organization.
      operationId: getAdvisory
      x-api-path-slug: organizationseinadvisoriesadvisoryid-get
      parameters:
      - in: path
        name: AdvisoryID
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: path
        name: ein
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Ein
      - Advisories
      - Advisory
  /Advisory:
    get:
      summary: Get Advisory
      description: |-
        Retrieve the full set of Charity Navigator advisories for a specified
        organization. An advisory is a cautionary communication from Charity Navigator,
        advising of unusual events or behavior related to a known organization.
      operationId: getAllActiveAdvisories
      x-api-path-slug: advisory-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: query
        name: pageNum
        description: Page number to return, in case the number of available objects
          in the resultset is greater than the specified or default `pageSize`
      - in: query
        name: pageSize
        description: Number of organizations to return in a single response message
      responses:
        200:
          description: OK
      tags:
      - Advisory
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