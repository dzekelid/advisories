{
  "info": {
    "name": "Cisco PSIRT open Vuln Get Security Advisories All",
    "_postman_id": "fc02a268-1618-4c36-aee8-233fdad22ae0",
    "description": "Used to obtain all advisories in Common Vulnerability Reporting Format (CVRF). For more information about CVRF go to https://communities.cisco.com/docs/DOC-63156 . By default the output is in JSON. To obtain the output in XML use the .xml extension. For example, /advisories/cvrf/all.xml",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Security",
      "item": [
        {
          "id": "b40e2587-2ba7-4307-9234-f587b6a80abb",
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
              "id": "c38739d4-a31f-4e30-9793-03e9e3a53905"
            }
          ]
        },
        {
          "id": "d26cb53a-4a0b-4fe3-96f4-ddff3665b8d7",
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
              "id": "42aacd2b-48a7-4a9a-b284-22b57e7f4982"
            }
          ]
        }
      ]
    }
  ]
}