---
name: Google Genomics
x-slug: google-genomics
description: Google Genomics helps the life science community organize the world&rsquo;s
  genomic information and make it accessible and useful. Big genomic data is here
  today, with petabytes rapidly growing toward exabytes. Through our extensions to
  Google Cloud Platform, you can apply the same technologies that power Google Search
  and Maps to securely store, process, explore, and share large, complex datasets.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Annotations
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/apis.md
specificationVersion: "0.14"
apis:
- name: Genomics - Create Annotation
  x-api-slug: v1annotations-post
  description: |-
    Creates a new annotation. Caller must have WRITE permission
    for the associated annotation set.

    The following fields are required:

    * annotationSetId
    * referenceName or
      referenceId

    ### Transcripts

    For annotations of type TRANSCRIPT, the following fields of
    transcript must be provided:

    * exons.start
    * exons.end

    All other fields may be optionally specified, unless documented as being
    server-generated (for example, the `id` field). The annotated
    range must be no longer than 100Mbp (mega base pairs). See the
    Annotation resource
    for additional restrictions on each field.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotations-post-openapi.md
- name: Genomics - Search Annotations
  x-api-slug: v1annotationssearch-post
  description: |-
    Searches for annotations that match the given criteria. Results are
    ordered by genomic coordinate (by reference sequence, then position).
    Annotations with equivalent genomic coordinates are returned in an
    unspecified order. This order is consistent, such that two queries for the
    same content (regardless of page size) yield annotations in the same order
    across their respective streams of paginated responses. Caller must have
    READ permission for the queried annotation sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationssearch-post-openapi.md
- name: Genomics - Delete Annotation
  x-api-slug: v1annotationsannotationid-delete
  description: |-
    Deletes an annotation. Caller must have WRITE permission for
    the associated annotation set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsannotationid-delete-openapi.md
- name: Genomics - Get Annotation
  x-api-slug: v1annotationsannotationid-get
  description: |-
    Gets an annotation. Caller must have READ permission
    for the associated annotation set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsannotationid-get-openapi.md
- name: Genomics - Update Annotation
  x-api-slug: v1annotationsannotationid-put
  description: |-
    Updates an annotation. Caller must have
    WRITE permission for the associated dataset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsannotationid-put-openapi.md
- name: Genomics - Create Batch Annotation
  x-api-slug: v1annotationsbatchcreate-post
  description: |-
    Creates one or more new annotations atomically. All annotations must
    belong to the same annotation set. Caller must have WRITE
    permission for this annotation set. For optimal performance, batch
    positionally adjacent annotations together.

    If the request has a systemic issue, such as an attempt to write to
    an inaccessible annotation set, the entire RPC will fail accordingly. For
    lesser data issues, when possible an error will be isolated to the
    corresponding batch entry in the response; the remaining well formed
    annotations will be created normally.

    For details on the requirements for each individual annotation resource,
    see
    CreateAnnotation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsbatchcreate-post-openapi.md
- name: Genomics - Create Annotation Set
  x-api-slug: v1annotationsets-post
  description: |-
    Creates a new annotation set. Caller must have WRITE permission for the
    associated dataset.

    The following fields are required:

      * datasetId
      * referenceSetId

    All other fields may be optionally specified, unless documented as being
    server-generated (for example, the `id` field).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsets-post-openapi.md
- name: Genomics - Search Annotation Sets
  x-api-slug: v1annotationsetssearch-post
  description: |-
    Searches for annotation sets that match the given criteria. Annotation sets
    are returned in an unspecified order. This order is consistent, such that
    two queries for the same content (regardless of page size) yield annotation
    sets in the same order across their respective streams of paginated
    responses. Caller must have READ permission for the queried datasets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsetssearch-post-openapi.md
- name: Genomics - Delete Annotation Set
  x-api-slug: v1annotationsetsannotationsetid-delete
  description: |-
    Deletes an annotation set. Caller must have WRITE permission
    for the associated annotation set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsetsannotationsetid-delete-openapi.md
- name: Genomics - Get Annotation Set
  x-api-slug: v1annotationsetsannotationsetid-get
  description: |-
    Gets an annotation set. Caller must have READ permission for
    the associated dataset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsetsannotationsetid-get-openapi.md
- name: Genomics - Update Annotation Set
  x-api-slug: v1annotationsetsannotationsetid-put
  description: |-
    Updates an annotation set. The update must respect all mutability
    restrictions and other invariants described on the annotation set resource.
    Caller must have WRITE permission for the associated dataset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsetsannotationsetid-put-openapi.md
- name: Genomics - Create Annotation
  x-api-slug: v1annotations-post
  description: |-
    Creates a new annotation. Caller must have WRITE permission
    for the associated annotation set.

    The following fields are required:

    * annotationSetId
    * referenceName or
      referenceId

    ### Transcripts

    For annotations of type TRANSCRIPT, the following fields of
    transcript must be provided:

    * exons.start
    * exons.end

    All other fields may be optionally specified, unless documented as being
    server-generated (for example, the `id` field). The annotated
    range must be no longer than 100Mbp (mega base pairs). See the
    Annotation resource
    for additional restrictions on each field.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotations-post-openapi.md
- name: Genomics - Search Annotations
  x-api-slug: v1annotationssearch-post
  description: |-
    Searches for annotations that match the given criteria. Results are
    ordered by genomic coordinate (by reference sequence, then position).
    Annotations with equivalent genomic coordinates are returned in an
    unspecified order. This order is consistent, such that two queries for the
    same content (regardless of page size) yield annotations in the same order
    across their respective streams of paginated responses. Caller must have
    READ permission for the queried annotation sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationssearch-post-openapi.md
- name: Genomics - Delete Annotation
  x-api-slug: v1annotationsannotationid-delete
  description: |-
    Deletes an annotation. Caller must have WRITE permission for
    the associated annotation set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsannotationid-delete-openapi.md
- name: Genomics - Get Annotation
  x-api-slug: v1annotationsannotationid-get
  description: |-
    Gets an annotation. Caller must have READ permission
    for the associated annotation set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsannotationid-get-openapi.md
- name: Genomics - Update Annotation
  x-api-slug: v1annotationsannotationid-put
  description: |-
    Updates an annotation. Caller must have
    WRITE permission for the associated dataset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsannotationid-put-openapi.md
- name: Genomics - Create Batch Annotation
  x-api-slug: v1annotationsbatchcreate-post
  description: |-
    Creates one or more new annotations atomically. All annotations must
    belong to the same annotation set. Caller must have WRITE
    permission for this annotation set. For optimal performance, batch
    positionally adjacent annotations together.

    If the request has a systemic issue, such as an attempt to write to
    an inaccessible annotation set, the entire RPC will fail accordingly. For
    lesser data issues, when possible an error will be isolated to the
    corresponding batch entry in the response; the remaining well formed
    annotations will be created normally.

    For details on the requirements for each individual annotation resource,
    see
    CreateAnnotation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsbatchcreate-post-openapi.md
- name: Genomics - Create Annotation Set
  x-api-slug: v1annotationsets-post
  description: |-
    Creates a new annotation set. Caller must have WRITE permission for the
    associated dataset.

    The following fields are required:

      * datasetId
      * referenceSetId

    All other fields may be optionally specified, unless documented as being
    server-generated (for example, the `id` field).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsets-post-openapi.md
- name: Genomics - Search Annotation Sets
  x-api-slug: v1annotationsetssearch-post
  description: |-
    Searches for annotation sets that match the given criteria. Annotation sets
    are returned in an unspecified order. This order is consistent, such that
    two queries for the same content (regardless of page size) yield annotation
    sets in the same order across their respective streams of paginated
    responses. Caller must have READ permission for the queried datasets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsetssearch-post-openapi.md
- name: Genomics - Delete Annotation Set
  x-api-slug: v1annotationsetsannotationsetid-delete
  description: |-
    Deletes an annotation set. Caller must have WRITE permission
    for the associated annotation set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsetsannotationsetid-delete-openapi.md
- name: Genomics - Get Annotation Set
  x-api-slug: v1annotationsetsannotationsetid-get
  description: |-
    Gets an annotation set. Caller must have READ permission for
    the associated dataset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsetsannotationsetid-get-openapi.md
- name: Genomics - Update Annotation Set
  x-api-slug: v1annotationsetsannotationsetid-put
  description: |-
    Updates an annotation set. The update must respect all mutability
    restrictions and other invariants described on the annotation set resource.
    Caller must have WRITE permission for the associated dataset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsetsannotationsetid-put-openapi.md
- name: Genomics - Create Annotation
  x-api-slug: v1annotations-post
  description: |-
    Creates a new annotation. Caller must have WRITE permission
    for the associated annotation set.

    The following fields are required:

    * annotationSetId
    * referenceName or
      referenceId

    ### Transcripts

    For annotations of type TRANSCRIPT, the following fields of
    transcript must be provided:

    * exons.start
    * exons.end

    All other fields may be optionally specified, unless documented as being
    server-generated (for example, the `id` field). The annotated
    range must be no longer than 100Mbp (mega base pairs). See the
    Annotation resource
    for additional restrictions on each field.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotations-post-openapi.md
- name: Genomics - Search Annotations
  x-api-slug: v1annotationssearch-post
  description: |-
    Searches for annotations that match the given criteria. Results are
    ordered by genomic coordinate (by reference sequence, then position).
    Annotations with equivalent genomic coordinates are returned in an
    unspecified order. This order is consistent, such that two queries for the
    same content (regardless of page size) yield annotations in the same order
    across their respective streams of paginated responses. Caller must have
    READ permission for the queried annotation sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationssearch-post-openapi.md
- name: Genomics - Delete Annotation
  x-api-slug: v1annotationsannotationid-delete
  description: |-
    Deletes an annotation. Caller must have WRITE permission for
    the associated annotation set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsannotationid-delete-openapi.md
- name: Genomics - Get Annotation
  x-api-slug: v1annotationsannotationid-get
  description: |-
    Gets an annotation. Caller must have READ permission
    for the associated annotation set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsannotationid-get-openapi.md
- name: Genomics - Update Annotation
  x-api-slug: v1annotationsannotationid-put
  description: |-
    Updates an annotation. Caller must have
    WRITE permission for the associated dataset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsannotationid-put-openapi.md
- name: Genomics - Create Batch Annotation
  x-api-slug: v1annotationsbatchcreate-post
  description: |-
    Creates one or more new annotations atomically. All annotations must
    belong to the same annotation set. Caller must have WRITE
    permission for this annotation set. For optimal performance, batch
    positionally adjacent annotations together.

    If the request has a systemic issue, such as an attempt to write to
    an inaccessible annotation set, the entire RPC will fail accordingly. For
    lesser data issues, when possible an error will be isolated to the
    corresponding batch entry in the response; the remaining well formed
    annotations will be created normally.

    For details on the requirements for each individual annotation resource,
    see
    CreateAnnotation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsbatchcreate-post-openapi.md
- name: Genomics - Create Annotation Set
  x-api-slug: v1annotationsets-post
  description: |-
    Creates a new annotation set. Caller must have WRITE permission for the
    associated dataset.

    The following fields are required:

      * datasetId
      * referenceSetId

    All other fields may be optionally specified, unless documented as being
    server-generated (for example, the `id` field).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsets-post-openapi.md
- name: Genomics - Search Annotation Sets
  x-api-slug: v1annotationsetssearch-post
  description: |-
    Searches for annotation sets that match the given criteria. Annotation sets
    are returned in an unspecified order. This order is consistent, such that
    two queries for the same content (regardless of page size) yield annotation
    sets in the same order across their respective streams of paginated
    responses. Caller must have READ permission for the queried datasets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsetssearch-post-openapi.md
- name: Genomics - Delete Annotation Set
  x-api-slug: v1annotationsetsannotationsetid-delete
  description: |-
    Deletes an annotation set. Caller must have WRITE permission
    for the associated annotation set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsetsannotationsetid-delete-openapi.md
- name: Genomics - Get Annotation Set
  x-api-slug: v1annotationsetsannotationsetid-get
  description: |-
    Gets an annotation set. Caller must have READ permission for
    the associated dataset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsetsannotationsetid-get-openapi.md
- name: Genomics - Update Annotation Set
  x-api-slug: v1annotationsetsannotationsetid-put
  description: |-
    Updates an annotation set. The update must respect all mutability
    restrictions and other invariants described on the annotation set resource.
    Caller must have WRITE permission for the associated dataset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/annotations/master/_listings/google-genomics/v1annotationsetsannotationsetid-put-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.fusion.tables.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.genomics.stack.network
- type: x-documentation
  url: https://cloud.google.com/genomics/overview
- type: x-forum
  url: https://groups.google.com/forum/#!forum/google-genomics-discuss/join
- type: x-pricing
  url: https://cloud.google.com/genomics/pricing
- type: x-rate-limits
  url: https://cloud.google.com/genomics/quotas
- type: x-support
  url: https://cloud.google.com/genomics/support
- type: x-website
  url: https://cloud.google.com/genomics/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---