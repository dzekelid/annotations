---
swagger: "2.0"
x-collection-name: Google Books
x-complete: 1
info:
  title: Books
  description: searches-for-books-and-manages-your-google-books-library-
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
  /mylibrary/annotations:
    get:
      summary: Get Annotations
      description: Retrieves a list of annotations, possibly filtered.
      operationId: books.mylibrary.annotations.list
      x-api-path-slug: mylibraryannotations-get
      parameters:
      - in: query
        name: contentVersion
        description: The content version for the requested volume
      - in: query
        name: layerId
        description: The layer ID to limit annotation by
      - in: query
        name: layerIds
        description: The layer ID(s) to limit annotation by
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous page
      - in: query
        name: showDeleted
        description: Set to true to return deleted annotations
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: updatedMax
        description: RFC 3339 timestamp to restrict to items updated prior to this
          timestamp (exclusive)
      - in: query
        name: updatedMin
        description: RFC 3339 timestamp to restrict to items updated since this timestamp
          (inclusive)
      - in: query
        name: volumeId
        description: The volume to restrict annotations to
      responses:
        200:
          description: OK
      tags:
      - Annotation
    post:
      summary: insert Annotation
      description: Inserts a new annotation.
      operationId: books.mylibrary.annotations.insert
      x-api-path-slug: mylibraryannotations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: country
        description: ISO-3166-1 code to override the IP-based location
      - in: query
        name: showOnlySummaryInResponse
        description: Requests that only the summary of the specified layer be provided
          in the response
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /mylibrary/annotations/summary:
    post:
      summary: Get Annotation
      description: Gets the summary of specified layers.
      operationId: books.mylibrary.annotations.summary
      x-api-path-slug: mylibraryannotationssummary-post
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
      - Annotation
  /mylibrary/annotations/{annotationId}:
    delete:
      summary: Delete Annotation
      description: Deletes an annotation.
      operationId: books.mylibrary.annotations.delete
      x-api-path-slug: mylibraryannotationsannotationid-delete
      parameters:
      - in: path
        name: annotationId
        description: The ID for the annotation to delete
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Annotation
    put:
      summary: Update Annotation
      description: Updates an existing annotation.
      operationId: books.mylibrary.annotations.update
      x-api-path-slug: mylibraryannotationsannotationid-put
      parameters:
      - in: path
        name: annotationId
        description: The ID for the annotation to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /volumes/{volumeId}/layers/{layerId}:
    get:
      summary: Get Volume Annotations
      description: Gets the volume annotations for a volume and layer.
      operationId: books.layers.volumeAnnotations.list
      x-api-path-slug: volumesvolumeidlayerslayerid-get
      parameters:
      - in: query
        name: contentVersion
        description: The content version for the requested volume
      - in: query
        name: endOffset
        description: The end offset to end retrieving data from
      - in: query
        name: endPosition
        description: The end position to end retrieving data from
      - in: path
        name: layerId
        description: The ID for the layer to get the annotations
      - in: query
        name: locale
        description: The locale information for the data
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous page
      - in: query
        name: showDeleted
        description: Set to true to return deleted annotations
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: startOffset
        description: The start offset to start retrieving data from
      - in: query
        name: startPosition
        description: The start position to start retrieving data from
      - in: query
        name: updatedMax
        description: RFC 3339 timestamp to restrict to items updated prior to this
          timestamp (exclusive)
      - in: query
        name: updatedMin
        description: RFC 3339 timestamp to restrict to items updated since this timestamp
          (inclusive)
      - in: query
        name: volumeAnnotationsVersion
        description: The version of the volume annotations that you are requesting
      - in: path
        name: volumeId
        description: The volume to retrieve annotations for
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /volumes/{volumeId}/layers/{layerId}/annotations/{annotationId}:
    get:
      summary: Get Volume Annotion
      description: Gets the volume annotation.
      operationId: books.layers.volumeAnnotations.get
      x-api-path-slug: volumesvolumeidlayerslayeridannotationsannotationid-get
      parameters:
      - in: path
        name: annotationId
        description: The ID of the volume annotation to retrieve
      - in: path
        name: layerId
        description: The ID for the layer to get the annotations
      - in: query
        name: locale
        description: The locale information for the data
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: volumeId
        description: The volume to retrieve annotations for
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /volumes/{volumeId}/layers/{layerId}/data:
    get:
      summary: Get Annotations
      description: Gets the annotation data for a volume and layer.
      operationId: books.layers.annotationData.list
      x-api-path-slug: volumesvolumeidlayerslayeriddata-get
      parameters:
      - in: query
        name: annotationDataId
        description: The list of Annotation Data Ids to retrieve
      - in: query
        name: contentVersion
        description: The content version for the requested volume
      - in: query
        name: h
        description: The requested pixel height for any images
      - in: path
        name: layerId
        description: The ID for the layer to get the annotation data
      - in: query
        name: locale
        description: The locale information for the data
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous page
      - in: query
        name: scale
        description: The requested scale for the image
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: updatedMax
        description: RFC 3339 timestamp to restrict to items updated prior to this
          timestamp (exclusive)
      - in: query
        name: updatedMin
        description: RFC 3339 timestamp to restrict to items updated since this timestamp
          (inclusive)
      - in: path
        name: volumeId
        description: The volume to retrieve annotation data for
      - in: query
        name: w
        description: The requested pixel width for any images
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /volumes/{volumeId}/layers/{layerId}/data/{annotationDataId}:
    get:
      summary: Get Annotation
      description: Gets the annotation data.
      operationId: books.layers.annotationData.get
      x-api-path-slug: volumesvolumeidlayerslayeriddataannotationdataid-get
      parameters:
      - in: query
        name: allowWebDefinitions
        description: For the dictionary layer
      - in: path
        name: annotationDataId
        description: The ID of the annotation data to retrieve
      - in: query
        name: contentVersion
        description: The content version for the volume you are trying to retrieve
      - in: query
        name: h
        description: The requested pixel height for any images
      - in: path
        name: layerId
        description: The ID for the layer to get the annotations
      - in: query
        name: locale
        description: The locale information for the data
      - in: query
        name: scale
        description: The requested scale for the image
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: volumeId
        description: The volume to retrieve annotations for
      - in: query
        name: w
        description: The requested pixel width for any images
      responses:
        200:
          description: OK
      tags:
      - Annotation
---