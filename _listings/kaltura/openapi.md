---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 1
info:
  title: Kaltura VPaaS
  description: building-video-experiences-consists-of-ingesting-media-files-playing-back-videos-and-reviewing-usage-and-engagement-analytics--in-between-there-is-a-world-of-nuances-required-for-your-unique-usecase-and-application--kaltura-vpaas-is-built-on-the-principles-of-atomic-services-sdks-and-tools-that-allow-you-full-control-and-flexibility-over-every-element-and-process-in-your-medias-life-cycle-
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/annotation_annotation/action/add:
    get:
      summary: Get Service Annotation Annotation Action Add
      description: Allows you to add an annotation object associated with an entry
      operationId: annotation.add
      x-api-path-slug: serviceannotation-annotationactionadd-get
      parameters:
      - in: query
        name: annotation[adType]
        description: 'Enum Type: `KalturaAdType`'
      - in: query
        name: annotation[answerKey]
      - in: query
        name: annotation[assetId]
      - in: query
        name: annotation[code]
      - in: query
        name: annotation[correctAnswerKeys]
      - in: query
        name: annotation[description]
      - in: query
        name: annotation[duration]
        description: Duration in milliseconds
      - in: query
        name: annotation[endTime]
        description: End time in milliseconds
      - in: query
        name: annotation[entryId]
        description: '`insertOnly`'
      - in: query
        name: annotation[eventType]
        description: 'Enum Type: `KalturaEventType`'
      - in: query
        name: annotation[explanation]
      - in: query
        name: annotation[forceStop]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: annotation[hint]
      - in: query
        name: annotation[isPublic]
        description: 'Enum Type: `KalturaNullableBoolean`Is the annotation public'
      - in: query
        name: annotation[objectType]
      - in: query
        name: annotation[optionalAnswers]
      - in: query
        name: annotation[parentId]
        description: '`insertOnly`'
      - in: query
        name: annotation[partnerData]
      - in: query
        name: annotation[partnerSortValue]
      - in: query
        name: annotation[protocolType]
        description: '`insertOnly`Enum Type: `KalturaAdProtocolType`'
      - in: query
        name: annotation[question]
      - in: query
        name: annotation[quizUserEntryId]
        description: '`insertOnly`'
      - in: query
        name: annotation[searchableOnEntry]
        description: 'Enum Type: `KalturaNullableBoolean`Should the cue point get
          indexed on the entry'
      - in: query
        name: annotation[sourceUrl]
      - in: query
        name: annotation[startTime]
        description: Start time in milliseconds
      - in: query
        name: annotation[subType]
        description: 'Enum Type: `KalturaThumbCuePointSubType`The sub type of the
          ThumbCuePoint'
      - in: query
        name: annotation[systemName]
      - in: query
        name: annotation[tags]
      - in: query
        name: annotation[text]
      - in: query
        name: annotation[thumbOffset]
      - in: query
        name: annotation[title]
      - in: query
        name: annotation[triggeredAt]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Add
  /service/annotation_annotation/action/addFromBulk:
    post:
      summary: Post Service Annotation Annotation Action Addfrombulk
      description: Allows you to add multiple cue points objects by uploading XML
        that contains multiple cue point definitions
      operationId: annotation.addFromBulk
      x-api-path-slug: serviceannotation-annotationactionaddfrombulk-post
      parameters:
      - in: formData
        name: fileData
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - AddFromBulk
  /service/annotation_annotation/action/clone:
    get:
      summary: Get Service Annotation Annotation Action Clone
      description: Clone cuePoint with id to given entry
      operationId: annotation.clone
      x-api-path-slug: serviceannotation-annotationactionclone-get
      parameters:
      - in: query
        name: entryId
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Clone
  /service/annotation_annotation/action/count:
    get:
      summary: Get Service Annotation Annotation Action Count
      description: count cue point objects by filter
      operationId: annotation.count
      x-api-path-slug: serviceannotation-annotationactioncount-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[codeEqual]
      - in: query
        name: filter[codeIn]
      - in: query
        name: filter[codeLike]
      - in: query
        name: filter[codeMultiLikeAnd]
      - in: query
        name: filter[codeMultiLikeOr]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[cuePointTypeEqual]
        description: 'Enum Type: `KalturaCuePointType`'
      - in: query
        name: filter[cuePointTypeIn]
      - in: query
        name: filter[descriptionLike]
      - in: query
        name: filter[descriptionMultiLikeAnd]
      - in: query
        name: filter[descriptionMultiLikeOr]
      - in: query
        name: filter[durationGreaterThanOrEqual]
      - in: query
        name: filter[durationLessThanOrEqual]
      - in: query
        name: filter[endTimeGreaterThanOrEqual]
      - in: query
        name: filter[endTimeLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[entryIdIn]
      - in: query
        name: filter[eventTypeEqual]
        description: 'Enum Type: `KalturaEventType`'
      - in: query
        name: filter[eventTypeIn]
      - in: query
        name: filter[forceStopEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[freeText]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[isPublicEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[parentIdEqual]
      - in: query
        name: filter[parentIdIn]
      - in: query
        name: filter[partnerSortValueEqual]
      - in: query
        name: filter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: filter[partnerSortValueIn]
      - in: query
        name: filter[partnerSortValueLessThanOrEqual]
      - in: query
        name: filter[protocolTypeEqual]
        description: 'Enum Type: `KalturaAdProtocolType`'
      - in: query
        name: filter[protocolTypeIn]
      - in: query
        name: filter[questionLike]
      - in: query
        name: filter[questionMultiLikeAnd]
      - in: query
        name: filter[questionMultiLikeOr]
      - in: query
        name: filter[quizUserEntryIdEqual]
      - in: query
        name: filter[quizUserEntryIdIn]
      - in: query
        name: filter[startTimeGreaterThanOrEqual]
      - in: query
        name: filter[startTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaCuePointStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[subTypeEqual]
        description: 'Enum Type: `KalturaThumbCuePointSubType`'
      - in: query
        name: filter[subTypeIn]
      - in: query
        name: filter[systemNameEqual]
      - in: query
        name: filter[systemNameIn]
      - in: query
        name: filter[tagsLike]
      - in: query
        name: filter[tagsMultiLikeAnd]
      - in: query
        name: filter[tagsMultiLikeOr]
      - in: query
        name: filter[textLike]
      - in: query
        name: filter[textMultiLikeAnd]
      - in: query
        name: filter[textMultiLikeOr]
      - in: query
        name: filter[titleLike]
      - in: query
        name: filter[titleMultiLikeAnd]
      - in: query
        name: filter[titleMultiLikeOr]
      - in: query
        name: filter[triggeredAtGreaterThanOrEqual]
      - in: query
        name: filter[triggeredAtLessThanOrEqual]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[userIdCurrent]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[userIdEqualCurrent]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[userIdEqual]
      - in: query
        name: filter[userIdIn]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Count
  /service/annotation_annotation/action/delete:
    get:
      summary: Get Service Annotation Annotation Action Delete
      description: delete cue point by id, and delete all children cue points
      operationId: annotation.delete
      x-api-path-slug: serviceannotation-annotationactiondelete-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Delete
  /service/annotation_annotation/action/get:
    get:
      summary: Get Service Annotation Annotation Action Get
      description: Retrieve an CuePoint object by id
      operationId: annotation.get
      x-api-path-slug: serviceannotation-annotationactionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Get
  /service/annotation_annotation/action/list:
    get:
      summary: Get Service Annotation Annotation Action List
      description: List annotation objects by filter and pager
      operationId: annotation.list
      x-api-path-slug: serviceannotation-annotationactionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[codeEqual]
      - in: query
        name: filter[codeIn]
      - in: query
        name: filter[codeLike]
      - in: query
        name: filter[codeMultiLikeAnd]
      - in: query
        name: filter[codeMultiLikeOr]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[cuePointTypeEqual]
        description: 'Enum Type: `KalturaCuePointType`'
      - in: query
        name: filter[cuePointTypeIn]
      - in: query
        name: filter[descriptionLike]
      - in: query
        name: filter[descriptionMultiLikeAnd]
      - in: query
        name: filter[descriptionMultiLikeOr]
      - in: query
        name: filter[durationGreaterThanOrEqual]
      - in: query
        name: filter[durationLessThanOrEqual]
      - in: query
        name: filter[endTimeGreaterThanOrEqual]
      - in: query
        name: filter[endTimeLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[entryIdIn]
      - in: query
        name: filter[eventTypeEqual]
        description: 'Enum Type: `KalturaEventType`'
      - in: query
        name: filter[eventTypeIn]
      - in: query
        name: filter[forceStopEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[freeText]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[isPublicEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[parentIdEqual]
      - in: query
        name: filter[parentIdIn]
      - in: query
        name: filter[partnerSortValueEqual]
      - in: query
        name: filter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: filter[partnerSortValueIn]
      - in: query
        name: filter[partnerSortValueLessThanOrEqual]
      - in: query
        name: filter[protocolTypeEqual]
        description: 'Enum Type: `KalturaAdProtocolType`'
      - in: query
        name: filter[protocolTypeIn]
      - in: query
        name: filter[questionLike]
      - in: query
        name: filter[questionMultiLikeAnd]
      - in: query
        name: filter[questionMultiLikeOr]
      - in: query
        name: filter[quizUserEntryIdEqual]
      - in: query
        name: filter[quizUserEntryIdIn]
      - in: query
        name: filter[startTimeGreaterThanOrEqual]
      - in: query
        name: filter[startTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaCuePointStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[subTypeEqual]
        description: 'Enum Type: `KalturaThumbCuePointSubType`'
      - in: query
        name: filter[subTypeIn]
      - in: query
        name: filter[systemNameEqual]
      - in: query
        name: filter[systemNameIn]
      - in: query
        name: filter[tagsLike]
      - in: query
        name: filter[tagsMultiLikeAnd]
      - in: query
        name: filter[tagsMultiLikeOr]
      - in: query
        name: filter[textLike]
      - in: query
        name: filter[textMultiLikeAnd]
      - in: query
        name: filter[textMultiLikeOr]
      - in: query
        name: filter[titleLike]
      - in: query
        name: filter[titleMultiLikeAnd]
      - in: query
        name: filter[titleMultiLikeOr]
      - in: query
        name: filter[triggeredAtGreaterThanOrEqual]
      - in: query
        name: filter[triggeredAtLessThanOrEqual]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[userIdCurrent]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[userIdEqualCurrent]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[userIdEqual]
      - in: query
        name: filter[userIdIn]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - List
  /service/annotation_annotation/action/serveBulk:
    get:
      summary: Get Service Annotation Annotation Action Servebulk
      description: Download multiple cue points objects as XML definitions
      operationId: annotation.serveBulk
      x-api-path-slug: serviceannotation-annotationactionservebulk-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[codeEqual]
      - in: query
        name: filter[codeIn]
      - in: query
        name: filter[codeLike]
      - in: query
        name: filter[codeMultiLikeAnd]
      - in: query
        name: filter[codeMultiLikeOr]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[cuePointTypeEqual]
        description: 'Enum Type: `KalturaCuePointType`'
      - in: query
        name: filter[cuePointTypeIn]
      - in: query
        name: filter[descriptionLike]
      - in: query
        name: filter[descriptionMultiLikeAnd]
      - in: query
        name: filter[descriptionMultiLikeOr]
      - in: query
        name: filter[durationGreaterThanOrEqual]
      - in: query
        name: filter[durationLessThanOrEqual]
      - in: query
        name: filter[endTimeGreaterThanOrEqual]
      - in: query
        name: filter[endTimeLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[entryIdIn]
      - in: query
        name: filter[eventTypeEqual]
        description: 'Enum Type: `KalturaEventType`'
      - in: query
        name: filter[eventTypeIn]
      - in: query
        name: filter[forceStopEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[freeText]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[isPublicEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[parentIdEqual]
      - in: query
        name: filter[parentIdIn]
      - in: query
        name: filter[partnerSortValueEqual]
      - in: query
        name: filter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: filter[partnerSortValueIn]
      - in: query
        name: filter[partnerSortValueLessThanOrEqual]
      - in: query
        name: filter[protocolTypeEqual]
        description: 'Enum Type: `KalturaAdProtocolType`'
      - in: query
        name: filter[protocolTypeIn]
      - in: query
        name: filter[questionLike]
      - in: query
        name: filter[questionMultiLikeAnd]
      - in: query
        name: filter[questionMultiLikeOr]
      - in: query
        name: filter[quizUserEntryIdEqual]
      - in: query
        name: filter[quizUserEntryIdIn]
      - in: query
        name: filter[startTimeGreaterThanOrEqual]
      - in: query
        name: filter[startTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaCuePointStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[subTypeEqual]
        description: 'Enum Type: `KalturaThumbCuePointSubType`'
      - in: query
        name: filter[subTypeIn]
      - in: query
        name: filter[systemNameEqual]
      - in: query
        name: filter[systemNameIn]
      - in: query
        name: filter[tagsLike]
      - in: query
        name: filter[tagsMultiLikeAnd]
      - in: query
        name: filter[tagsMultiLikeOr]
      - in: query
        name: filter[textLike]
      - in: query
        name: filter[textMultiLikeAnd]
      - in: query
        name: filter[textMultiLikeOr]
      - in: query
        name: filter[titleLike]
      - in: query
        name: filter[titleMultiLikeAnd]
      - in: query
        name: filter[titleMultiLikeOr]
      - in: query
        name: filter[triggeredAtGreaterThanOrEqual]
      - in: query
        name: filter[triggeredAtLessThanOrEqual]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[userIdCurrent]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[userIdEqualCurrent]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[userIdEqual]
      - in: query
        name: filter[userIdIn]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - ServeBulk
  /service/annotation_annotation/action/update:
    get:
      summary: Get Service Annotation Annotation Action Update
      description: Update annotation by id
      operationId: annotation.update
      x-api-path-slug: serviceannotation-annotationactionupdate-get
      parameters:
      - in: query
        name: annotation[adType]
        description: 'Enum Type: `KalturaAdType`'
      - in: query
        name: annotation[answerKey]
      - in: query
        name: annotation[assetId]
      - in: query
        name: annotation[code]
      - in: query
        name: annotation[correctAnswerKeys]
      - in: query
        name: annotation[description]
      - in: query
        name: annotation[duration]
        description: Duration in milliseconds
      - in: query
        name: annotation[endTime]
        description: End time in milliseconds
      - in: query
        name: annotation[entryId]
        description: '`insertOnly`'
      - in: query
        name: annotation[eventType]
        description: 'Enum Type: `KalturaEventType`'
      - in: query
        name: annotation[explanation]
      - in: query
        name: annotation[forceStop]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: annotation[hint]
      - in: query
        name: annotation[isPublic]
        description: 'Enum Type: `KalturaNullableBoolean`Is the annotation public'
      - in: query
        name: annotation[objectType]
      - in: query
        name: annotation[optionalAnswers]
      - in: query
        name: annotation[parentId]
        description: '`insertOnly`'
      - in: query
        name: annotation[partnerData]
      - in: query
        name: annotation[partnerSortValue]
      - in: query
        name: annotation[protocolType]
        description: '`insertOnly`Enum Type: `KalturaAdProtocolType`'
      - in: query
        name: annotation[question]
      - in: query
        name: annotation[quizUserEntryId]
        description: '`insertOnly`'
      - in: query
        name: annotation[searchableOnEntry]
        description: 'Enum Type: `KalturaNullableBoolean`Should the cue point get
          indexed on the entry'
      - in: query
        name: annotation[sourceUrl]
      - in: query
        name: annotation[startTime]
        description: Start time in milliseconds
      - in: query
        name: annotation[subType]
        description: 'Enum Type: `KalturaThumbCuePointSubType`The sub type of the
          ThumbCuePoint'
      - in: query
        name: annotation[systemName]
      - in: query
        name: annotation[tags]
      - in: query
        name: annotation[text]
      - in: query
        name: annotation[thumbOffset]
      - in: query
        name: annotation[title]
      - in: query
        name: annotation[triggeredAt]
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Update
  /service/annotation_annotation/action/updateStatus:
    get:
      summary: Get Service Annotation Annotation Action Updatestatus
      description: Update cuePoint status by id
      operationId: annotation.updateStatus
      x-api-path-slug: serviceannotation-annotationactionupdatestatus-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      - in: query
        name: status
        description: 'Enum Type: `KalturaCuePointStatus`'
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - UpdateStatus
---