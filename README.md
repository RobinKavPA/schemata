![generate-markdown](https://github.com/HDRUK/schemata/workflows/generate-markdown/badge.svg)

# HDR UK Schemata - Dataset V2.0.0

### 1. [HDR UK Dataset Schema](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset.md)

 - Latest json schema and yml can be found here:  https://github.com/HDRUK/schemata/blob/develop/schema/dataset/latest
 - Example json files can be found here including a current mapped dataset, a minimium json example and a ful example: https://github.com/HDRUK/schemata/blob/develop/examples 
 - Latest word documentation, change log and mapping file can be found here: https://github.com/HDRUK/schemata/tree/develop/docs/dataset/2.0.0/distribution
 - Impact assessment and indicative mapping files can be found here: https://github.com/HDRUK/schemata/tree/develop/docs/dataset/2.0.0/impact-assessment
      - aggregated_errors.xlsx: aggregated validation errors with an overview on the most common errors per attribute that will need to be resolved during migration
      - generated_mapping.py: the mapping algorithm that generates v2 data-models, (basically a mapping function for all fields in the new v2 specs).
      - v1_to_v2.json: for each data-model (key is the UUID) v1: old schema, v2: new schema, which is the mapping result (generated_mapping.py) of all data-models in the gateway.
      - dm_validation.json: for each data-model (key again is UUID) the data-set in form of the v2 attributes and the JSON schema validation.
      - aggregated_errors.json: an aggregation of the validation of all data-models by attribute with a list of unique error messages, a count of unique error messages, and a total count of the errors across all data-models; note that JSON schema validator generates an entry for all hierarchy levels, which means some error messages are repeated along the hierarchy.

### 2. Dataset Properties Breakdown

[ADD DESCRIPTION]

<!--ts-->

   * [summary](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#summary-schema)
      * [title](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#title)
      * [abstract](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#abstract)
      * [publisher](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#publisher)
      * [contactPoint](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#contactpoint)
      * [keywords](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#keywords)
      * [alternateIdentifiers](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#alternateidentifiers)
      * [doiName](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#doiname)
   * [documentation](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-documentation.md#documentation-schema)
      * [description](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-documentation.md#description)
      * [associatedMedia](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-documentation.md#associatedmedia)
      * [isPartOf](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-documentation.md#ispartof)
   * [coverage](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-coverage.md#coverage-schema)
      * [spatial](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-coverage.md#spatial)
      * [typicalAgeRange](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-coverage.md#typicalagerange)
      * [physicalSampleAvailability](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-coverage.md#physicalsampleavailability)
      * [followup](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-coverage.md#followup)
      * [pathway](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-coverage.md#pathway)
   * [provenance](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-provenance.md#provenance-schema)
      * [origin](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-provenance.md#origin)
      * [temporal](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-provenance.md#temporal)
   * [accessibility](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-accessibility.md#accessibility-schema)
      * [usage](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-accessibility.md#usage)
      * [access](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-accessibility.md#access)
      * [formatAndStandards](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-accessibility.md#formatandstandards)
   * [enrichmentAndLinkage](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-enrichment-and-linkage.md#enrichment-and-linkage-schema)
      * [qualifiedRelation](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-enrichment-and-linkage.md#qualifiedrelation)
      * [derivation](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-enrichment-and-linkage.md#derivation)
      * [tools](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-enrichment-and-linkage.md#tools)
   * [observations](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-observations.md#observations-schema)

<!--te-->



   * [identifier](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-dataset-identifier.md#dataset-identifier-schema)
   * [version](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-dataset-version.md#dataset-version-schema)
 * [revisions](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-dataset-revisions.md#dataset-revisions-schema)
 * [issued](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-creation-date.md#creation-date-schema)
 * [modified](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-modification-date.md#modification-date-schema)
