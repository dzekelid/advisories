{
  "info": {
    "name": "Cisco PSIRT open Vuln Get Security Advisories Oval Severity Severity",
    "_postman_id": "3e9c40a8-c4ef-4e87-a6da-7e3205f6061d",
    "description": "Used to obtain all OVAL definitions for a given security impact rating (critical, high, medium, or low).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Security",
      "item": [
        {
          "id": "e3883d76-f62a-4033-b232-3cb36c800afe",
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
              "id": "8f483e39-5a62-4e87-b129-0caa6002399f"
            }
          ]
        },
        {
          "id": "0a095f6d-6eb1-44bd-8961-85d45e2bf1c0",
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
              "id": "00e6e918-1dd3-4c9f-8075-72d25b9d70a5"
            }
          ]
        },
        {
          "id": "b64a3804-b0bf-402b-8892-bbff8b8bed55",
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
              "id": "d9534c45-dbe2-4db6-b228-b38136f1ab73"
            }
          ]
        },
        {
          "id": "521a1307-80c0-4627-bc30-3c0691ab9672",
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
              "id": "fa071c26-2823-48e0-85f5-fcd9ea435d9c"
            }
          ]
        },
        {
          "id": "e22e39bf-8438-4749-a7e8-d023ad6f8fdb",
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
              "id": "8c6d0012-e224-4ef3-9a20-b166d79b2ffe"
            }
          ]
        },
        {
          "id": "72084c8a-18af-4db5-a2b7-00480b92b67c",
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
              "id": "a2b88292-3194-48cd-9e74-11cfe085604b"
            }
          ]
        },
        {
          "id": "d4b72a15-6eaa-407e-8067-3b8b36d302d6",
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
              "id": "f43a5eb7-25c6-47b3-a833-b4b94463b1cf"
            }
          ]
        },
        {
          "id": "abda3971-b575-40a1-b7b0-42ee3334d048",
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
              "id": "76070cba-c030-460e-9a46-404fd63aa31a"
            }
          ]
        },
        {
          "id": "2eb97f0b-8872-4379-b60a-2fb3e037c4bf",
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
              "id": "d2ca1979-8f16-4b20-8abb-f68a86b7cc48"
            }
          ]
        },
        {
          "id": "03bb0ccc-9a21-4467-bf9d-b30a4a7fd031",
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
              "id": "9b485b38-016c-481a-9477-a465c67ea546"
            }
          ]
        },
        {
          "id": "aa8366ad-0818-4748-98d5-cd89a4bafef2",
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
              "id": "22316786-2211-4f29-83f2-b120416416ac"
            }
          ]
        },
        {
          "id": "cb12542b-46d6-4cb1-b0c5-35f4335650e3",
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
              "id": "ebb7f242-887b-486c-9da0-e5f3c6566ccc"
            }
          ]
        },
        {
          "id": "51223b47-300e-41e8-9361-69a14a83880c",
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
              "id": "3d9292a0-383c-428a-bad4-8b0fb0cccdd7"
            }
          ]
        },
        {
          "id": "26e4064c-644c-4680-9c00-95f7dcc3ce68",
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
              "id": "de11f314-578a-49fa-bac7-76e43187d54e"
            }
          ]
        },
        {
          "id": "d9e81e9a-714c-433f-9cee-b4b06de5a431",
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
              "id": "1a691a24-a6b0-40a6-9296-6066893eef61"
            }
          ]
        },
        {
          "id": "06110866-bcb7-4b9b-869d-857c75370401",
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
              "id": "395c434f-bd98-4953-b847-61a0515d9ae1"
            }
          ]
        },
        {
          "id": "80260516-4cac-433e-aa2f-350f97ab64a5",
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
              "id": "bd6adc2e-1211-4f53-9c0c-51a0f7330b00"
            }
          ]
        }
      ]
    }
  ]
}