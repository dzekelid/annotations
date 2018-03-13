---
swagger: "2.0"
info:
  title: Google Cloud Natural Language
  description: Google Cloud Natural Language API provides natural language understanding
    technologies to developers. Examples include sentiment analysis, entity recognition,
    and text annotations.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: language.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/documents:annotateText:
    post:
      summary: Annotate Text
      description: |-
        A convenience method that provides all the features that analyzeSentiment,
        analyzeEntities, and analyzeSyntax provide in one call
      operationId: language.documents.annotateText
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - annotation
definitions:
  AnalyzeEntitiesRequest:
    properties:
      encodingType:
        description: This is a default description.
        type: post
  AnalyzeEntitiesResponse:
    properties:
      entities:
        description: This is a default description.
        type: post
      language:
        description: This is a default description.
        type: post
  AnalyzeSentimentRequest:
    properties:
      encodingType:
        description: This is a default description.
        type: post
  AnalyzeSentimentResponse:
    properties:
      language:
        description: This is a default description.
        type: post
      sentences:
        description: This is a default description.
        type: post
  AnalyzeSyntaxRequest:
    properties:
      encodingType:
        description: This is a default description.
        type: post
  AnalyzeSyntaxResponse:
    properties:
      language:
        description: This is a default description.
        type: post
      sentences:
        description: This is a default description.
        type: post
      tokens:
        description: This is a default description.
        type: post
  AnnotateTextRequest:
    properties:
      encodingType:
        description: This is a default description.
        type: post
  AnnotateTextResponse:
    properties:
      entities:
        description: This is a default description.
        type: post
      language:
        description: This is a default description.
        type: post
      sentences:
        description: This is a default description.
        type: post
      tokens:
        description: This is a default description.
        type: post
  DependencyEdge:
    properties:
      headTokenIndex:
        description: This is a default description.
        type: post
      label:
        description: This is a default description.
        type: post
  Document:
    properties:
      content:
        description: This is a default description.
        type: post
      gcsContentUri:
        description: This is a default description.
        type: post
      language:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  Entity:
    properties:
      mentions:
        description: This is a default description.
        type: post
      metadata:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      salience:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  EntityMention:
    properties:
      type:
        description: This is a default description.
        type: post
  Features:
    properties:
      extractDocumentSentiment:
        description: This is a default description.
        type: post
      extractEntities:
        description: This is a default description.
        type: post
      extractSyntax:
        description: This is a default description.
        type: post
  PartOfSpeech:
    properties:
      aspect:
        description: This is a default description.
        type: post
      case:
        description: This is a default description.
        type: post
      form:
        description: This is a default description.
        type: post
      gender:
        description: This is a default description.
        type: post
      mood:
        description: This is a default description.
        type: post
      number:
        description: This is a default description.
        type: post
      person:
        description: This is a default description.
        type: post
      proper:
        description: This is a default description.
        type: post
      reciprocity:
        description: This is a default description.
        type: post
      tag:
        description: This is a default description.
        type: post
  Sentence:
    properties: []
  Sentiment:
    properties:
      magnitude:
        description: This is a default description.
        type: post
      score:
        description: This is a default description.
        type: post
  Status:
    properties:
      code:
        description: This is a default description.
        type: post
      details:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  TextSpan:
    properties:
      beginOffset:
        description: This is a default description.
        type: post
      content:
        description: This is a default description.
        type: post
  Token:
    properties:
      lemma:
        description: This is a default description.
        type: post
x-collection-name: Google Cloud Natural Language
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