{
  "info": {
    "name": "Cisco PSIRT open Vuln Get Security Advisories Oval Advisory Advisory",
    "_postman_id": "d9b8487b-db0e-47f2-b1ac-7ebdb53ddf5d",
    "description": "Used to obtain OVAL definitions for a given advisory ID `advisory_id` (i.e., cisco-sa-20150819-pcp)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Security",
      "item": [
        {
          "id": "a9bc869d-42a5-47e4-8c98-7f11505ebdcb",
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
              "id": "c3dfe6da-3fb3-4288-be82-d043a80749da"
            }
          ]
        },
        {
          "id": "4b672c93-16f4-4bf5-a94e-c6b26dda7884",
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
              "id": "471bbecb-f098-4d13-9bef-6630b5370fe4"
            }
          ]
        },
        {
          "id": "50119e9a-097f-4522-bc67-f48e470c88ae",
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
              "id": "aae5d27f-d2a9-49a4-ac44-b4c7acf31067"
            }
          ]
        },
        {
          "id": "3657508f-5761-452d-9a6c-cb7da98fe562",
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
              "id": "8f1b23a2-0edc-472a-890f-539d75e46013"
            }
          ]
        },
        {
          "id": "549af21b-cfc3-4910-bc3d-cac2b33cad83",
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
              "id": "0f0e1fed-eefe-4b03-abcb-ec08dbd4bd7d"
            }
          ]
        },
        {
          "id": "567445ea-0f98-41cb-8da7-43b7d19ebd3a",
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
              "id": "372ed81d-7fa6-431d-a2b8-6433d713b303"
            }
          ]
        },
        {
          "id": "0c706bb7-d5c7-40b0-b3ba-d34948daf6ce",
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
              "id": "4e8b2cb6-87de-4c71-8e67-0acffdc27c95"
            }
          ]
        },
        {
          "id": "eb81f52f-cd94-4a0c-a359-518e72ebeef7",
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
              "id": "ad693195-f3ef-424b-bad1-4fb66a8b712f"
            }
          ]
        },
        {
          "id": "f3b4a6ca-3437-4c21-9063-74af89cad7b9",
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
              "id": "01fdb63c-c42c-44ee-81bc-4cf449d4b1c7"
            }
          ]
        },
        {
          "id": "748ea5b4-2f18-4fac-afaa-c1908120f8a6",
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
              "id": "8dbc48f2-6e99-4551-a12b-b373ca9520c5"
            }
          ]
        },
        {
          "id": "5180e6cc-1134-423e-beb2-5de6a025dfe9",
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
              "id": "f960a506-4b6b-4d3f-a45c-ef6fcdcefe34"
            }
          ]
        },
        {
          "id": "f7e29ffa-d7d5-4846-96c9-c2623beb82cd",
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
              "id": "1480a5f6-e794-48aa-9bd6-33f6e3417a0c"
            }
          ]
        }
      ]
    }
  ]
}