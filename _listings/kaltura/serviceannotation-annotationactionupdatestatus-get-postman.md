{
  "info": {
    "name": "Kaltura VPaaS Get Service Annotation Annotation Action Updatestatus",
    "_postman_id": "95d9d4a0-1078-4cf2-91b3-15e6e062d3cb",
    "description": "Update cuePoint status by id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "3464b051-cdce-415d-b8f9-ea35ed8f7014",
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
              "id": "d9d06878-704a-47c3-ba3e-79e5abd32c96"
            }
          ]
        },
        {
          "id": "c4fc3cd6-97a9-4c64-b2a0-f78be5323072",
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
              "id": "67067653-c8b7-4c1d-856f-262930c332b3"
            }
          ]
        },
        {
          "id": "b61219b0-d338-4c4d-a34f-b34b4fd1fa52",
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
              "id": "adc501e3-0c5e-4594-ad30-8737cbb78a58"
            }
          ]
        },
        {
          "id": "763412ef-b3b8-4d72-b792-b21d87fce166",
          "name": "annotation.count",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/annotation_annotation/action/count?filter[advancedSearch][attribute]=%7B%7D&filter[advancedSearch][categoriesMatchOr]=%7B%7D&filter[advancedSearch][categoryEntryStatusIn]=%7B%7D&filter[advancedSearch][categoryIdEqual]=%7B%7D&filter[advancedSearch][comparison]=%7B%7D&filter[advancedSearch][contentLike]=%7B%7D&filter[advancedSearch][contentMultiLikeAnd]=%7B%7D&filter[advancedSearch][contentMultiLikeOr]=%7B%7D&filter[advancedSearch][cuePointsFreeText]=%7B%7D&filter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&filter[advancedSearch][cuePointTypeIn]=%7B%7D&filter[advancedSearch][depthGreaterThanEqual]=%7B%7D&filter[advancedSearch][distributionProfileId]=%7B%7D&filter[advancedSearch][distributionSunStatus]=%7B%7D&filter[advancedSearch][entryDistributionFlag]=%7B%7D&filter[advancedSearch][entryDistributionStatus]=%7B%7D&filter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][extendedStatusEqual]=%7B%7D&filter[advancedSearch][extendedStatusIn]=%7B%7D&filter[advancedSearch][field]=%7B%7D&filter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][idEqual]=%7B%7D&filter[advancedSearch][idIn]=%7B%7D&filter[advancedSearch][indexIdGreaterThan]=%7B%7D&filter[advancedSearch][isQuiz]=%7B%7D&filter[advancedSearch][items]=%7B%7D&filter[advancedSearch][memberIdEq]=%7B%7D&filter[advancedSearch][memberIdIn]=%7B%7D&filter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&filter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&filter[advancedSearch][metadataProfileId]=%7B%7D&filter[advancedSearch][noDistributionProfiles]=%7B%7D&filter[advancedSearch][not]=%7B%7D&filter[advancedSearch][objectType]=%7B%7D&filter[advancedSearch][orderBy]=%7B%7D&filter[advancedSearch][type]=%7B%7D&filter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&filter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&filter[advancedSearch][userIdEqual]=%7B%7D&filter[advancedSearch][userIdIn]=%7B%7D&filter[advancedSearch][value]=%7B%7D&filter[advancedSearch][watermarkId]=%7B%7D&filter[codeEqual]=%7B%7D&filter[codeIn]=%7B%7D&filter[codeLike]=%7B%7D&filter[codeMultiLikeAnd]=%7B%7D&filter[codeMultiLikeOr]=%7B%7D&filter[createdAtGreaterThanOrEqual]=%7B%7D&filter[createdAtLessThanOrEqual]=%7B%7D&filter[cuePointTypeEqual]=%7B%7D&filter[cuePointTypeIn]=%7B%7D&filter[descriptionLike]=%7B%7D&filter[descriptionMultiLikeAnd]=%7B%7D&filter[descriptionMultiLikeOr]=%7B%7D&filter[durationGreaterThanOrEqual]=%7B%7D&filter[durationLessThanOrEqual]=%7B%7D&filter[endTimeGreaterThanOrEqual]=%7B%7D&filter[endTimeLessThanOrEqual]=%7B%7D&filter[entryIdEqual]=%7B%7D&filter[entryIdIn]=%7B%7D&filter[eventTypeEqual]=%7B%7D&filter[eventTypeIn]=%7B%7D&filter[forceStopEqual]=%7B%7D&filter[freeText]=%7B%7D&filter[idEqual]=%7B%7D&filter[idIn]=%7B%7D&filter[isPublicEqual]=%7B%7D&filter[objectType]=%7B%7D&filter[orderBy]=%7B%7D&filter[parentIdEqual]=%7B%7D&filter[parentIdIn]=%7B%7D&filter[partnerSortValueEqual]=%7B%7D&filter[partnerSortValueGreaterThanOrEqual]=%7B%7D&filter[partnerSortValueIn]=%7B%7D&filter[partnerSortValueLessThanOrEqual]=%7B%7D&filter[protocolTypeEqual]=%7B%7D&filter[protocolTypeIn]=%7B%7D&filter[questionLike]=%7B%7D&filter[questionMultiLikeAnd]=%7B%7D&filter[questionMultiLikeOr]=%7B%7D&filter[quizUserEntryIdEqual]=%7B%7D&filter[quizUserEntryIdIn]=%7B%7D&filter[startTimeGreaterThanOrEqual]=%7B%7D&filter[startTimeLessThanOrEqual]=%7B%7D&filter[statusEqual]=%7B%7D&filter[statusIn]=%7B%7D&filter[subTypeEqual]=%7B%7D&filter[subTypeIn]=%7B%7D&filter[systemNameEqual]=%7B%7D&filter[systemNameIn]=%7B%7D&filter[tagsLike]=%7B%7D&filter[tagsMultiLikeAnd]=%7B%7D&filter[tagsMultiLikeOr]=%7B%7D&filter[textLike]=%7B%7D&filter[textMultiLikeAnd]=%7B%7D&filter[textMultiLikeOr]=%7B%7D&filter[titleLike]=%7B%7D&filter[titleMultiLikeAnd]=%7B%7D&filter[titleMultiLikeOr]=%7B%7D&filter[triggeredAtGreaterThanOrEqual]=%7B%7D&filter[triggeredAtLessThanOrEqual]=%7B%7D&filter[updatedAtGreaterThanOrEqual]=%7B%7D&filter[updatedAtLessThanOrEqual]=%7B%7D&filter[userIdCurrent]=%7B%7D&filter[userIdEqualCurrent]=%7B%7D&filter[userIdEqual]=%7B%7D&filter[userIdIn]=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "count cue point objects by filter"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41cde87f-c3df-49f3-94ce-d88c6418dfe2"
            }
          ]
        },
        {
          "id": "26f59ba5-9c91-4ea3-827b-c379e7e17c74",
          "name": "annotation.delete",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/annotation_annotation/action/delete?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "delete cue point by id, and delete all children cue points"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73294758-40d3-4e32-9333-e22297321629"
            }
          ]
        },
        {
          "id": "977406aa-6470-4e7f-927c-f8be4a309e0e",
          "name": "annotation.get",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/annotation_annotation/action/get?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve an CuePoint object by id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c42d244-2f72-4d9e-881b-a5a1e9fad94d"
            }
          ]
        },
        {
          "id": "4c079209-c815-49a8-bb6c-5cb1e533eb40",
          "name": "annotation.list",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/annotation_annotation/action/list?filter[advancedSearch][attribute]=%7B%7D&filter[advancedSearch][categoriesMatchOr]=%7B%7D&filter[advancedSearch][categoryEntryStatusIn]=%7B%7D&filter[advancedSearch][categoryIdEqual]=%7B%7D&filter[advancedSearch][comparison]=%7B%7D&filter[advancedSearch][contentLike]=%7B%7D&filter[advancedSearch][contentMultiLikeAnd]=%7B%7D&filter[advancedSearch][contentMultiLikeOr]=%7B%7D&filter[advancedSearch][cuePointsFreeText]=%7B%7D&filter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&filter[advancedSearch][cuePointTypeIn]=%7B%7D&filter[advancedSearch][depthGreaterThanEqual]=%7B%7D&filter[advancedSearch][distributionProfileId]=%7B%7D&filter[advancedSearch][distributionSunStatus]=%7B%7D&filter[advancedSearch][entryDistributionFlag]=%7B%7D&filter[advancedSearch][entryDistributionStatus]=%7B%7D&filter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][extendedStatusEqual]=%7B%7D&filter[advancedSearch][extendedStatusIn]=%7B%7D&filter[advancedSearch][field]=%7B%7D&filter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][idEqual]=%7B%7D&filter[advancedSearch][idIn]=%7B%7D&filter[advancedSearch][indexIdGreaterThan]=%7B%7D&filter[advancedSearch][isQuiz]=%7B%7D&filter[advancedSearch][items]=%7B%7D&filter[advancedSearch][memberIdEq]=%7B%7D&filter[advancedSearch][memberIdIn]=%7B%7D&filter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&filter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&filter[advancedSearch][metadataProfileId]=%7B%7D&filter[advancedSearch][noDistributionProfiles]=%7B%7D&filter[advancedSearch][not]=%7B%7D&filter[advancedSearch][objectType]=%7B%7D&filter[advancedSearch][orderBy]=%7B%7D&filter[advancedSearch][type]=%7B%7D&filter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&filter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&filter[advancedSearch][userIdEqual]=%7B%7D&filter[advancedSearch][userIdIn]=%7B%7D&filter[advancedSearch][value]=%7B%7D&filter[advancedSearch][watermarkId]=%7B%7D&filter[codeEqual]=%7B%7D&filter[codeIn]=%7B%7D&filter[codeLike]=%7B%7D&filter[codeMultiLikeAnd]=%7B%7D&filter[codeMultiLikeOr]=%7B%7D&filter[createdAtGreaterThanOrEqual]=%7B%7D&filter[createdAtLessThanOrEqual]=%7B%7D&filter[cuePointTypeEqual]=%7B%7D&filter[cuePointTypeIn]=%7B%7D&filter[descriptionLike]=%7B%7D&filter[descriptionMultiLikeAnd]=%7B%7D&filter[descriptionMultiLikeOr]=%7B%7D&filter[durationGreaterThanOrEqual]=%7B%7D&filter[durationLessThanOrEqual]=%7B%7D&filter[endTimeGreaterThanOrEqual]=%7B%7D&filter[endTimeLessThanOrEqual]=%7B%7D&filter[entryIdEqual]=%7B%7D&filter[entryIdIn]=%7B%7D&filter[eventTypeEqual]=%7B%7D&filter[eventTypeIn]=%7B%7D&filter[forceStopEqual]=%7B%7D&filter[freeText]=%7B%7D&filter[idEqual]=%7B%7D&filter[idIn]=%7B%7D&filter[isPublicEqual]=%7B%7D&filter[objectType]=%7B%7D&filter[orderBy]=%7B%7D&filter[parentIdEqual]=%7B%7D&filter[parentIdIn]=%7B%7D&filter[partnerSortValueEqual]=%7B%7D&filter[partnerSortValueGreaterThanOrEqual]=%7B%7D&filter[partnerSortValueIn]=%7B%7D&filter[partnerSortValueLessThanOrEqual]=%7B%7D&filter[protocolTypeEqual]=%7B%7D&filter[protocolTypeIn]=%7B%7D&filter[questionLike]=%7B%7D&filter[questionMultiLikeAnd]=%7B%7D&filter[questionMultiLikeOr]=%7B%7D&filter[quizUserEntryIdEqual]=%7B%7D&filter[quizUserEntryIdIn]=%7B%7D&filter[startTimeGreaterThanOrEqual]=%7B%7D&filter[startTimeLessThanOrEqual]=%7B%7D&filter[statusEqual]=%7B%7D&filter[statusIn]=%7B%7D&filter[subTypeEqual]=%7B%7D&filter[subTypeIn]=%7B%7D&filter[systemNameEqual]=%7B%7D&filter[systemNameIn]=%7B%7D&filter[tagsLike]=%7B%7D&filter[tagsMultiLikeAnd]=%7B%7D&filter[tagsMultiLikeOr]=%7B%7D&filter[textLike]=%7B%7D&filter[textMultiLikeAnd]=%7B%7D&filter[textMultiLikeOr]=%7B%7D&filter[titleLike]=%7B%7D&filter[titleMultiLikeAnd]=%7B%7D&filter[titleMultiLikeOr]=%7B%7D&filter[triggeredAtGreaterThanOrEqual]=%7B%7D&filter[triggeredAtLessThanOrEqual]=%7B%7D&filter[updatedAtGreaterThanOrEqual]=%7B%7D&filter[updatedAtLessThanOrEqual]=%7B%7D&filter[userIdCurrent]=%7B%7D&filter[userIdEqualCurrent]=%7B%7D&filter[userIdEqual]=%7B%7D&filter[userIdIn]=%7B%7D&No Name=%7B%7D&pager[pageIndex]=%7B%7D&pager[pageSize]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List annotation objects by filter and pager"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7886ab3-2e94-432a-bc74-94e70a30a5de"
            }
          ]
        },
        {
          "id": "9f2785c1-86c1-4d75-9f37-96aa93623634",
          "name": "annotation.serveBulk",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/annotation_annotation/action/serveBulk?filter[advancedSearch][attribute]=%7B%7D&filter[advancedSearch][categoriesMatchOr]=%7B%7D&filter[advancedSearch][categoryEntryStatusIn]=%7B%7D&filter[advancedSearch][categoryIdEqual]=%7B%7D&filter[advancedSearch][comparison]=%7B%7D&filter[advancedSearch][contentLike]=%7B%7D&filter[advancedSearch][contentMultiLikeAnd]=%7B%7D&filter[advancedSearch][contentMultiLikeOr]=%7B%7D&filter[advancedSearch][cuePointsFreeText]=%7B%7D&filter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&filter[advancedSearch][cuePointTypeIn]=%7B%7D&filter[advancedSearch][depthGreaterThanEqual]=%7B%7D&filter[advancedSearch][distributionProfileId]=%7B%7D&filter[advancedSearch][distributionSunStatus]=%7B%7D&filter[advancedSearch][entryDistributionFlag]=%7B%7D&filter[advancedSearch][entryDistributionStatus]=%7B%7D&filter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][extendedStatusEqual]=%7B%7D&filter[advancedSearch][extendedStatusIn]=%7B%7D&filter[advancedSearch][field]=%7B%7D&filter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][idEqual]=%7B%7D&filter[advancedSearch][idIn]=%7B%7D&filter[advancedSearch][indexIdGreaterThan]=%7B%7D&filter[advancedSearch][isQuiz]=%7B%7D&filter[advancedSearch][items]=%7B%7D&filter[advancedSearch][memberIdEq]=%7B%7D&filter[advancedSearch][memberIdIn]=%7B%7D&filter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&filter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&filter[advancedSearch][metadataProfileId]=%7B%7D&filter[advancedSearch][noDistributionProfiles]=%7B%7D&filter[advancedSearch][not]=%7B%7D&filter[advancedSearch][objectType]=%7B%7D&filter[advancedSearch][orderBy]=%7B%7D&filter[advancedSearch][type]=%7B%7D&filter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&filter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&filter[advancedSearch][userIdEqual]=%7B%7D&filter[advancedSearch][userIdIn]=%7B%7D&filter[advancedSearch][value]=%7B%7D&filter[advancedSearch][watermarkId]=%7B%7D&filter[codeEqual]=%7B%7D&filter[codeIn]=%7B%7D&filter[codeLike]=%7B%7D&filter[codeMultiLikeAnd]=%7B%7D&filter[codeMultiLikeOr]=%7B%7D&filter[createdAtGreaterThanOrEqual]=%7B%7D&filter[createdAtLessThanOrEqual]=%7B%7D&filter[cuePointTypeEqual]=%7B%7D&filter[cuePointTypeIn]=%7B%7D&filter[descriptionLike]=%7B%7D&filter[descriptionMultiLikeAnd]=%7B%7D&filter[descriptionMultiLikeOr]=%7B%7D&filter[durationGreaterThanOrEqual]=%7B%7D&filter[durationLessThanOrEqual]=%7B%7D&filter[endTimeGreaterThanOrEqual]=%7B%7D&filter[endTimeLessThanOrEqual]=%7B%7D&filter[entryIdEqual]=%7B%7D&filter[entryIdIn]=%7B%7D&filter[eventTypeEqual]=%7B%7D&filter[eventTypeIn]=%7B%7D&filter[forceStopEqual]=%7B%7D&filter[freeText]=%7B%7D&filter[idEqual]=%7B%7D&filter[idIn]=%7B%7D&filter[isPublicEqual]=%7B%7D&filter[objectType]=%7B%7D&filter[orderBy]=%7B%7D&filter[parentIdEqual]=%7B%7D&filter[parentIdIn]=%7B%7D&filter[partnerSortValueEqual]=%7B%7D&filter[partnerSortValueGreaterThanOrEqual]=%7B%7D&filter[partnerSortValueIn]=%7B%7D&filter[partnerSortValueLessThanOrEqual]=%7B%7D&filter[protocolTypeEqual]=%7B%7D&filter[protocolTypeIn]=%7B%7D&filter[questionLike]=%7B%7D&filter[questionMultiLikeAnd]=%7B%7D&filter[questionMultiLikeOr]=%7B%7D&filter[quizUserEntryIdEqual]=%7B%7D&filter[quizUserEntryIdIn]=%7B%7D&filter[startTimeGreaterThanOrEqual]=%7B%7D&filter[startTimeLessThanOrEqual]=%7B%7D&filter[statusEqual]=%7B%7D&filter[statusIn]=%7B%7D&filter[subTypeEqual]=%7B%7D&filter[subTypeIn]=%7B%7D&filter[systemNameEqual]=%7B%7D&filter[systemNameIn]=%7B%7D&filter[tagsLike]=%7B%7D&filter[tagsMultiLikeAnd]=%7B%7D&filter[tagsMultiLikeOr]=%7B%7D&filter[textLike]=%7B%7D&filter[textMultiLikeAnd]=%7B%7D&filter[textMultiLikeOr]=%7B%7D&filter[titleLike]=%7B%7D&filter[titleMultiLikeAnd]=%7B%7D&filter[titleMultiLikeOr]=%7B%7D&filter[triggeredAtGreaterThanOrEqual]=%7B%7D&filter[triggeredAtLessThanOrEqual]=%7B%7D&filter[updatedAtGreaterThanOrEqual]=%7B%7D&filter[updatedAtLessThanOrEqual]=%7B%7D&filter[userIdCurrent]=%7B%7D&filter[userIdEqualCurrent]=%7B%7D&filter[userIdEqual]=%7B%7D&filter[userIdIn]=%7B%7D&No Name=%7B%7D&pager[pageIndex]=%7B%7D&pager[pageSize]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Download multiple cue points objects as XML definitions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c89170f3-d12e-4f2f-bacf-73177ea64d36"
            }
          ]
        },
        {
          "id": "e755d327-a59a-4582-bd93-209dfcfbb8dd",
          "name": "annotation.update",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/annotation_annotation/action/update?annotation[adType]=%7B%7D&annotation[answerKey]=%7B%7D&annotation[assetId]=%7B%7D&annotation[code]=%7B%7D&annotation[correctAnswerKeys]=%7B%7D&annotation[description]=%7B%7D&annotation[duration]=%7B%7D&annotation[endTime]=%7B%7D&annotation[entryId]=%7B%7D&annotation[eventType]=%7B%7D&annotation[explanation]=%7B%7D&annotation[forceStop]=%7B%7D&annotation[hint]=%7B%7D&annotation[isPublic]=%7B%7D&annotation[objectType]=%7B%7D&annotation[optionalAnswers]=%7B%7D&annotation[parentId]=%7B%7D&annotation[partnerData]=%7B%7D&annotation[partnerSortValue]=%7B%7D&annotation[protocolType]=%7B%7D&annotation[question]=%7B%7D&annotation[quizUserEntryId]=%7B%7D&annotation[searchableOnEntry]=%7B%7D&annotation[sourceUrl]=%7B%7D&annotation[startTime]=%7B%7D&annotation[subType]=%7B%7D&annotation[systemName]=%7B%7D&annotation[tags]=%7B%7D&annotation[text]=%7B%7D&annotation[thumbOffset]=%7B%7D&annotation[title]=%7B%7D&annotation[triggeredAt]=%7B%7D&id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Update annotation by id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd26a1ae-ff0c-4489-9c67-8ffe56cfad98"
            }
          ]
        },
        {
          "id": "80afe615-d618-470d-9b8f-b7c3b4ee2d49",
          "name": "annotation.updateStatus",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/annotation_annotation/action/updateStatus?id=%7B%7D&No Name=%7B%7D&status=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Update cuePoint status by id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce9dccb2-68a6-4c2a-9160-db776e971fbd"
            }
          ]
        }
      ]
    }
  ]
}