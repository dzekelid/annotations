swagger: "2.0"
x-collection-name: Google Cloud Natural Language
x-complete: 1
info:
  title: Google Cloud Natural Language
  description: google-cloud-natural-language-api-provides-natural-language-understanding-technologies-to-developers--examples-include-sentiment-analysis-entity-recognition-and-text-annotations-
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
        analyzeEntities, and analyzeSyntax provide in one call.
      operationId: language.documents.annotateText
      x-api-path-slug: v1documentsannotatetext-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Annotation