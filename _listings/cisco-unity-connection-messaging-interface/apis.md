---
name: Cisco Unity Connection Messaging Interface
x-slug: cisco-unity-connection-messaging-interface
description: The Cisco Unity Connection Messaging Interface (CUMI) is a messaging
  API for Cisco Unity Connection that has been designed to be stable and simple to
  use. It is based on leading industry standards for web-based API development, and
  provides access to a wide set of Connection messaging functionality.
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Advisories
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/apis.md
specificationVersion: "0.14"
apis:
- name: Cisco PSIRT open Vuln - Get Security Advisories Advisory Advisory
  x-api-slug: securityadvisoriescvrfadvisoryadvisory-id-get
  description: Used to obtain an advisory in CVRF format for a given advisory ID `advisory_id`
    (i.e., cisco-sa-20150819-pcp)
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfadvisoryadvisory-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfadvisoryadvisory-id-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories All
  x-api-slug: securityadvisoriescvrfall-get
  description: Used to obtain all advisories in Common Vulnerability Reporting Format
    (CVRF). For more information about CVRF go to https://communities.cisco.com/docs/DOC-63156
    . By default the output is in JSON. To obtain the output in XML use the .xml extension.
    For example, /advisories/cvrf/all.xml
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfall-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfall-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories
  x-api-slug: securityadvisoriescvrfcvecve-id-get
  description: Used to obtain an advisory in CVRF format for a given Common Vulnerability
    Enumerator (CVE). The `cve_id` format is CVE-YYYY-NNNN. For more information about
    CVE visit http://cve.mitre.org/
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfcvecve-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfcvecve-id-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Latest Number
  x-api-slug: securityadvisoriescvrflatestnumber-get
  description: Used to obtain all the latest security advisories in CVRF format given
    an absolute number. For instance, the latest 10 or latest 5.
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrflatestnumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrflatestnumber-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Product
  x-api-slug: securityadvisoriescvrfproduct-get
  description: Used to obtain all the advisories that affects the given product name.
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfproduct-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfproduct-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Severity Severity
  x-api-slug: securityadvisoriescvrfseverityseverity-get
  description: Used to obtain all security advisories for a given security impact
    rating (critical, high, medium, or low) in CVRF format.
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfseverityseverity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfseverityseverity-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Severity Severity Firstpublished
  x-api-slug: securityadvisoriescvrfseverityseverityfirstpublished-get
  description: Used to obtain all security advisories for a given security impact
    rating (critical, high, medium, or low) in CVRF format and additionally filter
    based of firstpublished start date and enddate
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfseverityseverityfirstpublished-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfseverityseverityfirstpublished-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Severity Severity Lastpublished
  x-api-slug: securityadvisoriescvrfseverityseveritylastpublished-get
  description: Used to obtain all security advisories for a given security impact
    rating (critical, high, medium, or low) in CVRF format.
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfseverityseveritylastpublished-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfseverityseveritylastpublished-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Year Year
  x-api-slug: securityadvisoriescvrfyearyear-get
  description: Used to obtain all security advisories that have were orginally published
    in a specific year `YYYY`.
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfyearyear-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfyearyear-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Ios
  x-api-slug: securityadvisoriesios-get
  description: Used to obtain all advisories that affects the given ios version
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesios-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesios-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Iosxe
  x-api-slug: securityadvisoriesiosxe-get
  description: Used to obtain all advisories that affects the given ios version
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesiosxe-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesiosxe-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Oval Advisory Advisory
  x-api-slug: securityadvisoriesovaladvisoryadvisory-id-get
  description: Used to obtain OVAL definitions for a given advisory ID `advisory_id`
    (i.e., cisco-sa-20150819-pcp)
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovaladvisoryadvisory-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovaladvisoryadvisory-id-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Oval All
  x-api-slug: securityadvisoriesovalall-get
  description: Used to obtain all Open Vulnerability and Assessment Language (OVAL)
    definitions available for Cisco security vulnerabilities. For more information
    about OVAL go to https://communities.cisco.com/docs/DOC-63158 . By default the
    output is in JSON. To obtain the output in XML use the .xml extension. For example,
    /advisories/oval/all.xml
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovalall-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovalall-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Oval
  x-api-slug: securityadvisoriesovalcvecve-id-get
  description: Used to obtain OVAL definitions for a given CVE Identifier. The `cve_id`
    format is CVE-YYYY-NNNN.
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovalcvecve-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovalcvecve-id-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Oval Latest Number
  x-api-slug: securityadvisoriesovallatestnumber-get
  description: Used to obtain all the latest OVAL definitions given an absolute number.
    For instance, the latest 10 or latest 5.
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovallatestnumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovallatestnumber-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Oval Product
  x-api-slug: securityadvisoriesovalproduct-get
  description: Used to obtain all the oval advisories that affects the given product
    name.
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovalproduct-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovalproduct-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Oval Severity Severity
  x-api-slug: securityadvisoriesovalseverityseverity-get
  description: Used to obtain all OVAL definitions for a given security impact rating
    (critical, high, medium, or low).
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovalseverityseverity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovalseverityseverity-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Oval Severity Severity Firstpublished
  x-api-slug: securityadvisoriesovalseverityseverityfirstpublished-get
  description: Used to obtain all security advisories for a given security impact
    rating (critical, high, medium, or low) in OVAL format.
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovalseverityseverityfirstpublished-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovalseverityseverityfirstpublished-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Oval Severity Severity Lastpublished
  x-api-slug: securityadvisoriesovalseverityseveritylastpublished-get
  description: Used to obtain all security advisories for a given security impact
    rating (critical, high, medium, or low) in OVAL format.
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovalseverityseveritylastpublished-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovalseverityseveritylastpublished-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Advisory Advisory
  x-api-slug: securityadvisoriescvrfadvisoryadvisory-id-get
  description: Used to obtain an advisory in CVRF format for a given advisory ID `advisory_id`
    (i.e., cisco-sa-20150819-pcp)
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfadvisoryadvisory-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfadvisoryadvisory-id-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Oval Advisory Advisory
  x-api-slug: securityadvisoriesovaladvisoryadvisory-id-get
  description: Used to obtain OVAL definitions for a given advisory ID `advisory_id`
    (i.e., cisco-sa-20150819-pcp)
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovaladvisoryadvisory-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovaladvisoryadvisory-id-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Advisory Advisory
  x-api-slug: securityadvisoriescvrfadvisoryadvisory-id-get
  description: Used to obtain an advisory in CVRF format for a given advisory ID `advisory_id`
    (i.e., cisco-sa-20150819-pcp)
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfadvisoryadvisory-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriescvrfadvisoryadvisory-id-get-openapi.md
- name: Cisco PSIRT open Vuln - Get Security Advisories Oval Advisory Advisory
  x-api-slug: securityadvisoriesovaladvisoryadvisory-id-get
  description: Used to obtain OVAL definitions for a given advisory ID `advisory_id`
    (i.e., cisco-sa-20150819-pcp)
  image: ""
  humanURL: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
  baseURL: https://api.cisco.com//
  tags: Collaboration, Messages, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovaladvisoryadvisory-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/advisories/master/_listings/cisco-unity-connection-messaging-interface/securityadvisoriesovaladvisoryadvisory-id-get-openapi.md
x-common:
- type: x-website
  url: http://docwiki.cisco.com/wiki/Cisco_Unity_Connection_Messaging_Interface_%28CUMI%29_API
- type: x-api-gallery
  url: http://circleci.api.gallery.streamdata.io
- type: x-api-stack
  url: http://cisco.unity.connection.messaging.interface.stack.network
- type: x-developer
  url: https://developer.cisco.com/
- type: x-support
  url: https://developer.cisco.com/site/devnet/support/
- type: x-website
  url: http://cisco.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---