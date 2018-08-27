{
  "info": {
    "name": "Cisco PSIRT open Vuln Get Security Advisories Oval Latest Number",
    "_postman_id": "0da56830-7561-4cf8-9f26-dbaeefd1bf08",
    "description": "Used to obtain all the latest OVAL definitions given an absolute number. For instance, the latest 10 or latest 5.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Security",
      "item": [
        {
          "id": "a380a785-a255-4f3e-a1e9-dbdea4dd586c",
          "name": "used-to-obtain-an-advisory-in-cvrf-format-for-a-given-advisory-id-advisory-id-i-e--ciscosa20150819pc",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/advisory/:advisory_id"
              ],
              "variable": [
                {
                  "id": "advisory_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain an advisory in CVRF format for a given advisory ID `advisory_id` (i.e., cisco-sa-20150819-pcp)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0eb48d0-6649-4341-aa9b-619b21560f6d"
            }
          ]
        },
        {
          "id": "f38f40cc-5f3f-42c3-9136-a94862039b2c",
          "name": "used-to-obtain-all-advisories-in-common-vulnerability-reporting-format-cvrf--for-more-information-ab",
          "request": {
            "url": "http://api.cisco.com/security/advisories/cvrf/all",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all advisories in Common Vulnerability Reporting Format (CVRF). For more information about CVRF go to https://communities.cisco.com/docs/DOC-63156 . By default the output is in JSON. To obtain the output in XML use the .xml extension. For example, /advisories/cvrf/all.xml"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7fa6bf28-be8b-4953-89ff-f7b83179be71"
            }
          ]
        },
        {
          "id": "73993420-44a7-426f-8908-172196f33736",
          "name": "used-to-obtain-an-advisory-in-cvrf-format-for-a-given-common-vulnerability-enumerator-cve--the-cve-i",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/cve/:cve_id"
              ],
              "variable": [
                {
                  "id": "cve_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain an advisory in CVRF format for a given Common Vulnerability Enumerator (CVE). The `cve_id` format is CVE-YYYY-NNNN. For more information about CVE visit http://cve.mitre.org/"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95fb1865-6ec8-43a2-b829-2cb09039f54c"
            }
          ]
        },
        {
          "id": "b5691ca1-41d7-470f-8e52-80d0712674c4",
          "name": "used-to-obtain-all-the-latest-security-advisories-in-cvrf-format-given-an-absolute-number--for-insta",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/latest/:number"
              ],
              "variable": [
                {
                  "id": "number",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all the latest security advisories in CVRF format given an absolute number. For instance, the latest 10 or latest 5."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97e90da6-870a-459b-9d2d-e4a969855a98"
            }
          ]
        },
        {
          "id": "0600fe98-cd5d-4e07-a484-2bcdc3e7fd06",
          "name": "used-to-obtain-all-the-advisories-that-affects-the-given-product-name-",
          "request": {
            "url": "http://api.cisco.com/security/advisories/cvrf/product?product=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all the advisories that affects the given product name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "513eec4e-1805-481f-9745-33d92c11760b"
            }
          ]
        },
        {
          "id": "02d8a041-07c8-44f8-9df1-6bdec93c1b15",
          "name": "used-to-obtain-all-security-advisories-for-a-given-security-impact-rating-critical-high-medium-or-lo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/severity/:severity"
              ],
              "variable": [
                {
                  "id": "severity",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in CVRF format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9aa5c8f7-64b7-4b8f-a177-7e4056e474be"
            }
          ]
        },
        {
          "id": "e3d0c55d-6c17-49d1-8e52-6eb9f016e510",
          "name": "used-to-obtain-all-security-advisories-for-a-given-security-impact-rating-critical-high-medium-or-lo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/severity/:severity/firstpublished"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "severity",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in CVRF format and additionally filter based of firstpublished start date and enddate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c83794c9-d5c1-4e97-bc92-51a7f4bb95bc"
            }
          ]
        },
        {
          "id": "82ed46f4-cb70-4645-9d0b-710812df8a84",
          "name": "used-to-obtain-all-security-advisories-for-a-given-security-impact-rating-critical-high-medium-or-lo1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/severity/:severity/lastpublished"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "severity",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in CVRF format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e8bf3b7-9cd9-4bdc-8c03-721524689604"
            }
          ]
        },
        {
          "id": "93b85567-7574-42f9-a7cb-edfc3c5e05f8",
          "name": "used-to-obtain-all-security-advisories-that-have-were-orginally-published-in-a-specific-year-yyyy-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/year/:year"
              ],
              "variable": [
                {
                  "id": "year",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all security advisories that have were orginally published in a specific year `YYYY`."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75aa5b31-69a4-4047-907e-21f7f1dd7e83"
            }
          ]
        },
        {
          "id": "4332666b-3f0f-40b5-886c-93e225fce5ae",
          "name": "used-to-obtain-all-advisories-that-affects-the-given-ios-version",
          "request": {
            "url": "http://api.cisco.com/security/advisories/ios?version=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all advisories that affects the given ios version"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e0bb63d-fd1f-4edd-9ca1-378ab6472d11"
            }
          ]
        },
        {
          "id": "7bddb3ed-1b6f-479e-bdb2-a605def5282b",
          "name": "used-to-obtain-all-advisories-that-affects-the-given-ios-version1",
          "request": {
            "url": "http://api.cisco.com/security/advisories/iosxe?version=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all advisories that affects the given ios version"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8883ce1-fcf8-453b-8f47-9b27566bc647"
            }
          ]
        },
        {
          "id": "603bf8bd-5644-4f9a-96bf-568cc9b0607e",
          "name": "used-to-obtain-oval-definitions-for-a-given-advisory-id-advisory-id-i-e--ciscosa20150819pcp",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/oval/advisory/:advisory_id"
              ],
              "variable": [
                {
                  "id": "advisory_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain OVAL definitions for a given advisory ID `advisory_id` (i.e., cisco-sa-20150819-pcp)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c4d6709-a148-4e41-8ee3-6fcc9744c194"
            }
          ]
        },
        {
          "id": "e8212536-4af3-4b52-87b7-bc573bce3727",
          "name": "used-to-obtain-all-open-vulnerability-and-assessment-language-oval-definitions-available-for-cisco-s",
          "request": {
            "url": "http://api.cisco.com/security/advisories/oval/all",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all Open Vulnerability and Assessment Language (OVAL) definitions available for Cisco security vulnerabilities. For more information about OVAL go to https://communities.cisco.com/docs/DOC-63158 . By default the output is in JSON. To obtain the output in XML use the .xml extension. For example, /advisories/oval/all.xml"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aab415da-9bfb-4cc1-b7ad-05e3d16f916f"
            }
          ]
        },
        {
          "id": "857b31c0-6bf6-465a-91f5-d7c46ec3e251",
          "name": "used-to-obtain-oval-definitions-for-a-given-cve-identifier--the-cve-id-format-is-cveyyyynnnn-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/oval/cve/:cve_id"
              ],
              "variable": [
                {
                  "id": "cve_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain OVAL definitions for a given CVE Identifier. The `cve_id` format is CVE-YYYY-NNNN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a39d315-ac80-4e99-a534-0741b0f91640"
            }
          ]
        },
        {
          "id": "db3218e0-bb9b-4844-8f1a-42c2188ad1f0",
          "name": "used-to-obtain-all-the-latest-oval-definitions-given-an-absolute-number--for-instance-the-latest-10-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/oval/latest/:number"
              ],
              "variable": [
                {
                  "id": "number",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all the latest OVAL definitions given an absolute number. For instance, the latest 10 or latest 5."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0544595-3834-48bc-b2b0-e8de0c5e2a81"
            }
          ]
        }
      ]
    }
  ]
}