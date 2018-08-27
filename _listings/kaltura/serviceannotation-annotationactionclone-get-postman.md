{
  "info": {
    "name": "Kaltura VPaaS Get Service Annotation Annotation Action Clone",
    "_postman_id": "22651723-caa3-4b95-b9ed-94d2a1ecacdb",
    "description": "Clone cuePoint with id to given entry",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "f605da31-a250-4422-bd60-4d73857450ba",
          "name": "annotation.add",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/annotation_annotation/action/add?annotation[adType]=%7B%7D&annotation[answerKey]=%7B%7D&annotation[assetId]=%7B%7D&annotation[code]=%7B%7D&annotation[correctAnswerKeys]=%7B%7D&annotation[description]=%7B%7D&annotation[duration]=%7B%7D&annotation[endTime]=%7B%7D&annotation[entryId]=%7B%7D&annotation[eventType]=%7B%7D&annotation[explanation]=%7B%7D&annotation[forceStop]=%7B%7D&annotation[hint]=%7B%7D&annotation[isPublic]=%7B%7D&annotation[objectType]=%7B%7D&annotation[optionalAnswers]=%7B%7D&annotation[parentId]=%7B%7D&annotation[partnerData]=%7B%7D&annotation[partnerSortValue]=%7B%7D&annotation[protocolType]=%7B%7D&annotation[question]=%7B%7D&annotation[quizUserEntryId]=%7B%7D&annotation[searchableOnEntry]=%7B%7D&annotation[sourceUrl]=%7B%7D&annotation[startTime]=%7B%7D&annotation[subType]=%7B%7D&annotation[systemName]=%7B%7D&annotation[tags]=%7B%7D&annotation[text]=%7B%7D&annotation[thumbOffset]=%7B%7D&annotation[title]=%7B%7D&annotation[triggeredAt]=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows you to add an annotation object associated with an entry"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ead6c50-ab68-4dcc-a5d2-1f5a24ca1073"
            }
          ]
        },
        {
          "id": "55dbfe60-32f7-40c4-bfe0-196658a6d02d",
          "name": "annotation.addFromBulk",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/annotation_annotation/action/addFromBulk?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "fileData",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Allows you to add multiple cue points objects by uploading XML that contains multiple cue point definitions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "608c7187-da1f-4c2a-895a-0ecc751b3d10"
            }
          ]
        },
        {
          "id": "2364750e-fd4e-415a-bd90-e7c54bcffd1c",
          "name": "annotation.clone",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/annotation_annotation/action/clone?entryId=%7B%7D&id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Clone cuePoint with id to given entry"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0473880f-dfba-4140-a688-09cf30e253e1"
            }
          ]
        }
      ]
    }
  ]
}