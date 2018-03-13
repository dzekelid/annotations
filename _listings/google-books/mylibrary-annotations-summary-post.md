---
swagger: "2.0"
info:
  title: Books
  description: Searches for books and manages your Google Books library.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /books/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mylibrary/annotations/summary:
    post:
      summary: Get Annotation
      description: Gets the summary of specified layers
      operationId: books.mylibrary.annotations.summary
      parameters:
      - in: query
        name: layerIds
        description: Array of layer IDs to get the summary for
      - in: query
        name: volumeId
        description: Volume id to get the summary for
      responses:
        200:
          description: OK
      tags:
      - annotation
definitions:
  Annotation:
    properties:
      afterSelectedText:
        description: This is a default description.
        type: parameters
      beforeSelectedText:
        description: This is a default description.
        type: parameters
      clientVersionRanges:
        description: This is a default description.
        type: parameters
      created:
        description: This is a default description.
        type: parameters
      currentVersionRanges:
        description: This is a default description.
        type: parameters
      data:
        description: This is a default description.
        type: parameters
      deleted:
        description: This is a default description.
        type: parameters
      highlightStyle:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Annotationdata:
    properties:
      annotationType:
        description: This is a default description.
        type: parameters
      encoded_data:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      layerId:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      updated:
        description: This is a default description.
        type: parameters
      volumeId:
        description: This is a default description.
        type: parameters
  Annotations:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      totalItems:
        description: This is a default description.
        type: parameters
  AnnotationsSummary:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      layers:
        description: This is a default description.
        type: parameters
  Annotationsdata:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      totalItems:
        description: This is a default description.
        type: parameters
  BooksAnnotationsRange:
    properties:
      endOffset:
        description: This is a default description.
        type: parameters
      endPosition:
        description: This is a default description.
        type: parameters
      startOffset:
        description: This is a default description.
        type: parameters
      startPosition:
        description: This is a default description.
        type: parameters
  BooksCloudloadingResource:
    properties:
      author:
        description: This is a default description.
        type: parameters
      processingState:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
      volumeId:
        description: This is a default description.
        type: parameters
  BooksVolumesRecommendedRateResponse:
    properties:
      consistency_token:
        description: This is a default description.
        type: parameters
  Bookshelf:
    properties:
      access:
        description: This is a default description.
        type: parameters
      created:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
      updated:
        description: This is a default description.
        type: parameters
      volumeCount:
        description: This is a default description.
        type: parameters
      volumesLastUpdated:
        description: This is a default description.
        type: parameters
  Bookshelves:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Category:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  ConcurrentAccessRestriction:
    properties:
      deviceAllowed:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      maxConcurrentDevices:
        description: This is a default description.
        type: parameters
      message:
        description: This is a default description.
        type: parameters
      nonce:
        description: This is a default description.
        type: parameters
      reasonCode:
        description: This is a default description.
        type: parameters
      restricted:
        description: This is a default description.
        type: parameters
      signature:
        description: This is a default description.
        type: parameters
      source:
        description: This is a default description.
        type: parameters
      timeWindowSeconds:
        description: This is a default description.
        type: parameters
  Dictlayerdata:
    properties:
      common:
        description: This is a default description.
        type: parameters
      dict:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Discoveryclusters:
    properties:
      clusters:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      totalClusters:
        description: This is a default description.
        type: parameters
  DownloadAccessRestriction:
    properties:
      deviceAllowed:
        description: This is a default description.
        type: parameters
      downloadsAcquired:
        description: This is a default description.
        type: parameters
      justAcquired:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      maxDownloadDevices:
        description: This is a default description.
        type: parameters
      message:
        description: This is a default description.
        type: parameters
      nonce:
        description: This is a default description.
        type: parameters
      reasonCode:
        description: This is a default description.
        type: parameters
      restricted:
        description: This is a default description.
        type: parameters
      signature:
        description: This is a default description.
        type: parameters
  DownloadAccesses:
    properties:
      downloadAccessList:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Geolayerdata:
    properties:
      common:
        description: This is a default description.
        type: parameters
      geo:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Layersummaries:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      totalItems:
        description: This is a default description.
        type: parameters
  Layersummary:
    properties:
      annotationCount:
        description: This is a default description.
        type: parameters
      annotationTypes:
        description: This is a default description.
        type: parameters
      annotationsDataLink:
        description: This is a default description.
        type: parameters
      annotationsLink:
        description: This is a default description.
        type: parameters
      contentVersion:
        description: This is a default description.
        type: parameters
      dataCount:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      layerId:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  Metadata:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Notification:
    properties:
      body:
        description: This is a default description.
        type: parameters
      crmExperimentIds:
        description: This is a default description.
        type: parameters
      doc_id:
        description: This is a default description.
        type: parameters
      doc_type:
        description: This is a default description.
        type: parameters
      dont_show_notification:
        description: This is a default description.
        type: parameters
      iconUrl:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      notificationGroup:
        description: This is a default description.
        type: parameters
      notification_type:
        description: This is a default description.
        type: parameters
      pcampaign_id:
        description: This is a default description.
        type: parameters
  Offers:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  ReadingPosition:
    properties:
      epubCfiPosition:
        description: This is a default description.
        type: parameters
      gbImagePosition:
        description: This is a default description.
        type: parameters
      gbTextPosition:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      pdfPosition:
        description: This is a default description.
        type: parameters
      updated:
        description: This is a default description.
        type: parameters
      volumeId:
        description: This is a default description.
        type: parameters
  RequestAccess:
    properties:
      kind:
        description: This is a default description.
        type: parameters
  Review:
    properties:
      author:
        description: This is a default description.
        type: parameters
      content:
        description: This is a default description.
        type: parameters
      date:
        description: This is a default description.
        type: parameters
      fullTextUrl:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      rating:
        description: This is a default description.
        type: parameters
      source:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
      volumeId:
        description: This is a default description.
        type: parameters
  Series:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      series:
        description: This is a default description.
        type: parameters
  Seriesmembership:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      member:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  Usersettings:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      notesExport:
        description: This is a default description.
        type: parameters
      notification:
        description: This is a default description.
        type: parameters
  Volume:
    properties:
      accessInfo:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      layerInfo:
        description: This is a default description.
        type: parameters
      recommendedInfo:
        description: This is a default description.
        type: parameters
      saleInfo:
        description: This is a default description.
        type: parameters
      searchInfo:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      userInfo:
        description: This is a default description.
        type: parameters
  Volume2:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  Volumeannotation:
    properties:
      annotationDataId:
        description: This is a default description.
        type: parameters
      annotationDataLink:
        description: This is a default description.
        type: parameters
      annotationType:
        description: This is a default description.
        type: parameters
      contentRanges:
        description: This is a default description.
        type: parameters
      data:
        description: This is a default description.
        type: parameters
      deleted:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      layerId:
        description: This is a default description.
        type: parameters
      pageIds:
        description: This is a default description.
        type: parameters
  Volumeannotations:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      totalItems:
        description: This is a default description.
        type: parameters
      version:
        description: This is a default description.
        type: parameters
  Volumes:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      totalItems:
        description: This is a default description.
        type: parameters
  Volumeseriesinfo:
    properties:
      bookDisplayNumber:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      shortSeriesBookTitle:
        description: This is a default description.
        type: parameters
      volumeSeries:
        description: This is a default description.
        type: parameters
x-collection-name: Google Books
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---