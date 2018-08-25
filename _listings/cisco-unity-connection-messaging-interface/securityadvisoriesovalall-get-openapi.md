---
swagger: "2.0"
x-collection-name: Cisco Unity Connection Messaging Interface
x-complete: 0
info:
  title: Cisco PSIRT open Vuln Get Security Advisories Oval All
  description: Used to obtain all Open Vulnerability and Assessment Language (OVAL)
    definitions available for Cisco security vulnerabilities. For more information
    about OVAL go to https://communities.cisco.com/docs/DOC-63158 . By default the
    output is in JSON. To obtain the output in XML use the .xml extension. For example,
    /advisories/oval/all.xml
  contact:
    name: Omar Santos
    email: os@cisco.com
  version: 0.0.3
host: api.cisco.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /security/advisories/cvrf/advisory/{advisory_id}:
    get:
      summary: Get Security Advisories Advisory Advisory
      description: Used to obtain an advisory in CVRF format for a given advisory
        ID `advisory_id` (i.e., cisco-sa-20150819-pcp)
      operationId: used-to-obtain-an-advisory-in-cvrf-format-for-a-given-advisory-id-advisory-id-i-e--ciscosa20150819pc
      x-api-path-slug: securityadvisoriescvrfadvisoryadvisory-id-get
      parameters:
      - in: path
        name: advisory_id
        description: advisory ID
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Advisory
      - Advisory
  /security/advisories/cvrf/all:
    get:
      summary: Get Security Advisories All
      description: Used to obtain all advisories in Common Vulnerability Reporting
        Format (CVRF). For more information about CVRF go to https://communities.cisco.com/docs/DOC-63156
        . By default the output is in JSON. To obtain the output in XML use the .xml
        extension. For example, /advisories/cvrf/all.xml
      operationId: used-to-obtain-all-advisories-in-common-vulnerability-reporting-format-cvrf--for-more-information-ab
      x-api-path-slug: securityadvisoriescvrfall-get
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
  /security/advisories/cvrf/cve/{cve_id}:
    get:
      summary: Get Security Advisories
      description: Used to obtain an advisory in CVRF format for a given Common Vulnerability
        Enumerator (CVE). The `cve_id` format is CVE-YYYY-NNNN. For more information
        about CVE visit http://cve.mitre.org/
      operationId: used-to-obtain-an-advisory-in-cvrf-format-for-a-given-common-vulnerability-enumerator-cve--the-cve-i
      x-api-path-slug: securityadvisoriescvrfcvecve-id-get
      parameters:
      - in: path
        name: cve_id
        description: CVE Identifier (i
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
  /security/advisories/cvrf/latest/{number}:
    get:
      summary: Get Security Advisories Latest Number
      description: Used to obtain all the latest security advisories in CVRF format
        given an absolute number. For instance, the latest 10 or latest 5.
      operationId: used-to-obtain-all-the-latest-security-advisories-in-cvrf-format-given-an-absolute-number--for-insta
      x-api-path-slug: securityadvisoriescvrflatestnumber-get
      parameters:
      - in: path
        name: number
        description: An absolute number to obtain the latest security advisories
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Latest
      - Number
  /security/advisories/cvrf/product:
    get:
      summary: Get Security Advisories Product
      description: Used to obtain all the advisories that affects the given product
        name.
      operationId: used-to-obtain-all-the-advisories-that-affects-the-given-product-name-
      x-api-path-slug: securityadvisoriescvrfproduct-get
      parameters:
      - in: query
        name: product
        description: An product name to obtain security advisories that matches given
          product name
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Product
  /security/advisories/cvrf/severity/{severity}:
    get:
      summary: Get Security Advisories Severity Severity
      description: Used to obtain all security advisories for a given security impact
        rating (critical, high, medium, or low) in CVRF format.
      operationId: used-to-obtain-all-security-advisories-for-a-given-security-impact-rating-critical-high-medium-or-lo
      x-api-path-slug: securityadvisoriescvrfseverityseverity-get
      parameters:
      - in: path
        name: severity
        description: Critical, High, Medium, Low
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Severity
      - Severity
  /security/advisories/cvrf/severity/{severity}/firstpublished:
    get:
      summary: Get Security Advisories Severity Severity Firstpublished
      description: Used to obtain all security advisories for a given security impact
        rating (critical, high, medium, or low) in CVRF format and additionally filter
        based of firstpublished start date and enddate
      operationId: used-to-obtain-all-security-advisories-for-a-given-security-impact-rating-critical-high-medium-or-lo
      x-api-path-slug: securityadvisoriescvrfseverityseverityfirstpublished-get
      parameters:
      - in: query
        name: endDate
      - in: path
        name: severity
        description: Used to obtain all advisories that have a security impact rating
          of critical
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Severity
      - Severity
      - Firstpublished
  /security/advisories/cvrf/severity/{severity}/lastpublished:
    get:
      summary: Get Security Advisories Severity Severity Lastpublished
      description: Used to obtain all security advisories for a given security impact
        rating (critical, high, medium, or low) in CVRF format.
      operationId: used-to-obtain-all-security-advisories-for-a-given-security-impact-rating-critical-high-medium-or-lo
      x-api-path-slug: securityadvisoriescvrfseverityseveritylastpublished-get
      parameters:
      - in: query
        name: endDate
      - in: path
        name: severity
        description: Used to obtain all advisories that have a security impact rating
          of critical
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Severity
      - Severity
      - Lastpublished
  /security/advisories/cvrf/year/{year}:
    get:
      summary: Get Security Advisories Year Year
      description: Used to obtain all security advisories that have were orginally
        published in a specific year `YYYY`.
      operationId: used-to-obtain-all-security-advisories-that-have-were-orginally-published-in-a-specific-year-yyyy-
      x-api-path-slug: securityadvisoriescvrfyearyear-get
      parameters:
      - in: path
        name: year
        description: The four digit year
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Year
      - Year
  /security/advisories/ios:
    get:
      summary: Get Security Advisories Ios
      description: Used to obtain all advisories that affects the given ios version
      operationId: used-to-obtain-all-advisories-that-affects-the-given-ios-version
      x-api-path-slug: securityadvisoriesios-get
      parameters:
      - in: query
        name: version
        description: IOS version to obtain security advisories
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Ios
  /security/advisories/iosxe:
    get:
      summary: Get Security Advisories Iosxe
      description: Used to obtain all advisories that affects the given ios version
      operationId: used-to-obtain-all-advisories-that-affects-the-given-ios-version
      x-api-path-slug: securityadvisoriesiosxe-get
      parameters:
      - in: query
        name: version
        description: IOS version to obtain security advisories
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Iosxe
  /security/advisories/oval/advisory/{advisory_id}:
    get:
      summary: Get Security Advisories Oval Advisory Advisory
      description: Used to obtain OVAL definitions for a given advisory ID `advisory_id`
        (i.e., cisco-sa-20150819-pcp)
      operationId: used-to-obtain-oval-definitions-for-a-given-advisory-id-advisory-id-i-e--ciscosa20150819pcp
      x-api-path-slug: securityadvisoriesovaladvisoryadvisory-id-get
      parameters:
      - in: path
        name: advisory_id
        description: advisory ID
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Oval
      - Advisory
      - Advisory
  /security/advisories/oval/all:
    get:
      summary: Get Security Advisories Oval All
      description: Used to obtain all Open Vulnerability and Assessment Language (OVAL)
        definitions available for Cisco security vulnerabilities. For more information
        about OVAL go to https://communities.cisco.com/docs/DOC-63158 . By default
        the output is in JSON. To obtain the output in XML use the .xml extension.
        For example, /advisories/oval/all.xml
      operationId: used-to-obtain-all-open-vulnerability-and-assessment-language-oval-definitions-available-for-cisco-s
      x-api-path-slug: securityadvisoriesovalall-get
      responses:
        200:
          description: OK
      tags:
      - Security
      - Advisories
      - Oval
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