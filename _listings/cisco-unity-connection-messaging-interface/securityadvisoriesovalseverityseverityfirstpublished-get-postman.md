{
  "info": {
    "name": "Cisco PSIRT open Vuln Get Security Advisories Oval Severity Severity Firstpublished",
    "_postman_id": "2897eb6c-c18d-407d-b445-84a712754b62",
    "description": "Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in OVAL format.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Security",
      "item": [
        {
          "id": "909bfd57-6605-48aa-b7b1-5709257fe9a2",
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
              "id": "a47e3cc1-ce5f-4880-b489-af5749853ef9"
            }
          ]
        },
        {
          "id": "7cf391c9-bc40-4080-ade9-7b977c260b3c",
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
              "id": "02c7aaa4-9c3b-4f29-8369-dd7347796e95"
            }
          ]
        },
        {
          "id": "93826c2f-96a7-4fdc-9bbf-dde06d9c8d11",
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
              "id": "3cc17e98-4752-4da0-b349-6c2403c4e9ba"
            }
          ]
        },
        {
          "id": "5342813e-7bb8-40a4-b9af-bbbb441bd1e5",
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
              "id": "c3342f03-eb8f-4562-9a87-b3305efa632f"
            }
          ]
        },
        {
          "id": "ce6951c8-d4d0-4d88-b254-b3806da57448",
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
              "id": "a13fecde-4bbe-4b59-a4a3-59a7aec2f5cd"
            }
          ]
        },
        {
          "id": "2e5b8266-0ef5-4285-8ff2-23877738cb80",
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
              "id": "317df40b-08b1-444b-97f0-fe5e96aa0baa"
            }
          ]
        },
        {
          "id": "1b1c1ea7-2d26-46ee-9d23-9aa8878f02c2",
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
              "id": "4bfd2a5e-f37d-4481-ba16-832ffe873b5a"
            }
          ]
        },
        {
          "id": "8cbe392f-4795-4c8f-9ff8-4f20de7fe686",
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
              "id": "2d984b2d-996d-4335-ab7a-80d8642801ec"
            }
          ]
        },
        {
          "id": "7674ce92-0e4d-47ca-9031-2a507ed14c90",
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
              "id": "77149e93-6e65-49c0-ae87-f8400b3c0312"
            }
          ]
        },
        {
          "id": "79db4b18-61ab-40ad-88f2-ef7b84a2289f",
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
              "id": "1d7c7584-f0e8-4aac-8890-522051ec47ab"
            }
          ]
        },
        {
          "id": "c29114f7-f712-4e4c-96f6-4d53b1f8a355",
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
              "id": "99fbdc66-e106-462b-b3a3-3eb24ea08b44"
            }
          ]
        },
        {
          "id": "6b2eb826-02f0-48c6-a362-07b8ada22612",
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
              "id": "488c80c5-8695-4238-860a-ff6d950692c5"
            }
          ]
        },
        {
          "id": "6f97740b-c645-4498-b1c9-f405fe2d4934",
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
              "id": "c901383e-59f6-4d8e-a096-d6ae1f8424ee"
            }
          ]
        },
        {
          "id": "105df437-de0c-4e2e-95e7-db540f3b3854",
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
              "id": "2019c696-3d77-4ee1-bba4-fa6b12781cee"
            }
          ]
        },
        {
          "id": "7f777e88-ca57-4bf7-b80f-c0f70972f5d0",
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
              "id": "f20b6e87-4c05-4488-9e99-a8d9077ef69b"
            }
          ]
        },
        {
          "id": "4a373b3c-5797-4278-8429-d61b6190ebbb",
          "name": "used-to-obtain-all-the-oval-advisories-that-affects-the-given-product-name-",
          "request": {
            "url": "http://api.cisco.com/security/advisories/oval/product?product=%7B%7D",
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
            "description": "Used to obtain all the oval advisories that affects the given product name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1dec1825-3486-44a7-9ec5-227a73eb07a5"
            }
          ]
        },
        {
          "id": "6bcf9ce4-b1a3-4941-8b4f-5496c3722c22",
          "name": "used-to-obtain-all-oval-definitions-for-a-given-security-impact-rating-critical-high-medium-or-low-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/oval/severity/:severity"
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
            "description": "Used to obtain all OVAL definitions for a given security impact rating (critical, high, medium, or low)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "caf7280c-9d2d-4b08-985b-31fac6d22e1f"
            }
          ]
        },
        {
          "id": "5f6cbf50-6a61-40d4-a634-0815c56037b7",
          "name": "used-to-obtain-all-security-advisories-for-a-given-security-impact-rating-critical-high-medium-or-lo2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/oval/severity/:severity/firstpublished"
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
            "description": "Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in OVAL format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f405401b-7796-46df-baa4-fcf44f14c93e"
            }
          ]
        }
      ]
    }
  ]
}