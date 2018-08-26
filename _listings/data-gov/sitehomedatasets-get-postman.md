{
  "info": {
    "name": "Data.gov API Get Site Home Datasets",
    "_postman_id": "2d797fbd-f256-4ce1-9895-cce494429a45",
    "description": "List homepage datasets",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "site",
      "item": [
        {
          "id": "cd89b145-7cb9-4140-87ca-5efe53cf90ea",
          "name": "getSiteHomeDatasets",
          "request": {
            "url": "http://catalog.data.gov/api/3/site/home/datasets/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List homepage datasets"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b60cf8a8-aab5-4ba1-bc70-70486f55d6e7"
            }
          ]
        }
      ]
    }
  ]
}