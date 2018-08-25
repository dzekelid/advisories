{
  "info": {
    "name": "Charity Navigator Get Organizations Ein Advisories",
    "_postman_id": "c237bea5-860d-427e-89bc-bbc3fab3d7f6",
    "description": "Retrieve the full set of Charity Navigator advisories for a specified\norganization. An advisory is a cautionary communication from Charity Navigator,\nadvising of unusual events or behavior related to a known organization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "c9848f0f-a67c-443f-9bd0-59e0e7e2fc28",
          "name": "searchOrganizations",
          "request": {
            "url": "http://api.data.charitynavigator.org/v2/Organizations?app_id=%7B%7D&app_key=%7B%7D&categoryID=%7B%7D&causeID=%7B%7D&cfcCharities=%7B%7D&city=%7B%7D&donorPrivacy=%7B%7D&fundraisingOrgs=%7B%7D&maxRating=%7B%7D&minRating=%7B%7D&noGovSupport=%7B%7D&pageNum=%7B%7D&pageSize=%7B%7D&rated=%7B%7D&scopeOfWork=%7B%7D&search=%7B%7D&searchType=%7B%7D&sizeRange=%7B%7D&sort=%7B%7D&state=%7B%7D&zip=%7B%7D",
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
            "description": "Retrieve a list of the organizations available in the Charity Navigator Data\nStore. Allows paged retrieval, simple and advanced searching."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a972911-2e63-4d72-b6f7-5f43b7ca1768"
            }
          ]
        },
        {
          "id": "7f2c502d-8a5e-4a0b-a2b3-c34c4cfca03a",
          "name": "getOrganization",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.charitynavigator.org",
              "path": [
                "v2",
                "Organizations/:ein"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "app_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ein",
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
            "description": "Retrieve full detail of a single Organization. This is a composite set of\ninformation describing an organization that may engage in charitable work.\nNormally the Organization data structure includes a single legal entity, though\nlegal entity information may be excluded in exceptional cases."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86834bb2-fb82-4d60-a917-9a38122b8dbe"
            }
          ]
        },
        {
          "id": "1095ab9d-c425-460d-b763-2e7b5845f12c",
          "name": "getRatings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.charitynavigator.org",
              "path": [
                "v2",
                "Organizations/:ein/Ratings"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "app_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageNum",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ein",
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
            "description": "Retrieve all Charity Navigator ratings for a single organization. <br/>\n![Content\nSubscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png\n\"Included with the paid Content Subscription.\")"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66ad2658-0939-4937-85f0-4dbebac97d4e"
            }
          ]
        },
        {
          "id": "9e39a9ff-4e67-4039-bb74-1f1ed0135c5b",
          "name": "getRating",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.charitynavigator.org",
              "path": [
                "v2",
                "Organizations/:ein/Ratings/:RatingID"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "app_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ein",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "RatingID",
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
            "description": "Retrieve a single Rating object for an Organization. Each rating is listed\nonce, under its primary `referenceOrganization`. Note that the rating may apply\nto other organizations, and this is represented by `includedOrganizations`,\nwhich is a collection of hyperlinks to all of the organizations to which the\nrating applies.\nThe rating is a point-in-time assessment provided by Charity Navigator, along\nwith related metrics and ratios taken from financial statements for a fiscal\nyear, on which the rating is based. <br/> ![Content\nSubscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png\n\"Included with the paid Content Subscription.\")"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96dee140-68b9-4ba4-a4a5-9f6c0d329a74"
            }
          ]
        },
        {
          "id": "a12f1646-f053-4ea4-a667-9b0d3b0f9930",
          "name": "getAdvisories",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.charitynavigator.org",
              "path": [
                "v2",
                "Organizations/:ein/Advisories"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "app_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageNum",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "status",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ein",
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
            "description": "Retrieve the full set of Charity Navigator advisories for a specified\norganization. An advisory is a cautionary communication from Charity Navigator,\nadvising of unusual events or behavior related to a known organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49a40e3f-e320-4f85-9690-64501f009c61"
            }
          ]
        }
      ]
    }
  ]
}