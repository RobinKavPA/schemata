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

Below is the breakdown of the HDR UK V2 Dataset Schema by it's properties and sub properties as defined in the [JSON Schema](https://github.com/HDRUK/schemata/blob/develop/schema/dataset/latest/dataset.schema.json). Each property has its own Schema with a description of its corresponding sub properties, including their data type and whether it is a required field.

<!--ts-->

#### 0. [Metadata] (properties generated when dataset is entered into the system)

   * [identifier](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-dataset-identifier.md#dataset-identifier-schema)
   * [version](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-dataset-version.md#dataset-version-schema)
 * [revisions](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-dataset-revisions.md#dataset-revisions-schema)
 * [issued](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-creation-date.md#creation-date-schema)
 * [modified](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-modification-date.md#modification-date-schema)

#### 1. [summary](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#summary-schema): Summary metadata must be completed by Data Custodians onboarding metadata into the Innovation Gateway MVP.

 * [title](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#title)
 * [abstract](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#abstract)
 * [publisher](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#publisher)
 * [contactPoint](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#contactpoint)
 * [keywords](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#keywords)
 * [alternateIdentifiers](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#alternateidentifiers)
 * [doiName](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-summary.md#doiname)

#### 2. [documentation](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-documentation.md#documentation-schema): Documentation can include a rich text description of the dataset or links to media such as documents, images, presentations, videos or links to data dictionaries, profiles or dashboards. Organisations are required to confirm that they have permission to distribute any additional media.

 * [description](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-documentation.md#description)
 * [associatedMedia](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-documentation.md#associatedmedia)
 * [isPartOf](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-documentation.md#ispartof)

#### 3. [coverage](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-coverage.md#coverage-schema): This information includes attributes for geographical and temporal coverage, cohort details etc. to enable a deeper understanding of the dataset content so that researchers can make decisions about the relevance of the underlying data.

 * [spatial](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-coverage.md#spatial)
 * [typicalAgeRange](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-coverage.md#typicalagerange)
 * [physicalSampleAvailability](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-coverage.md#physicalsampleavailability)
 * [followup](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-coverage.md#followup)
 * [pathway](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-coverage.md#pathway)

#### 4. [provenance](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-provenance.md#provenance-schema): Provenance information allows researchers to understand data within the context of its origins and can be an indicator of quality, authenticity and timeliness.

 * [origin](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-provenance.md#origin)
 * [temporal](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-provenance.md#temporal)

#### 5. [accessibility](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-accessibility.md#accessibility-schema): Accessibility information allows researchers to understand access, usage, limitations, formats, standards and linkage or interoperability with toolsets.

 * [usage](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-accessibility.md#usage)
 * [access](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-accessibility.md#access)
 * [formatAndStandards](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-accessibility.md#formatandstandards)

#### 6. [enrichmentAndLinkage](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-enrichment-and-linkage.md#enrichment-and-linkage-schema): This section includes information about related datasets that may have previously been linked, as well as indicating if there is the opportunity to link to other datasets in the future. If a dataset has been enriched and/or derivations, scores and existing tools are available this section allows providers to indicate this to researchers.

 * [qualifiedRelation](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-enrichment-and-linkage.md#qualifiedrelation)
 * [derivation](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-enrichment-and-linkage.md#derivation)
 * [tools](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-enrichment-and-linkage.md#tools)

#### 7. [observations](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset-properties-observations.md#observations-schema): Multiple observations about the dataset may be provided and users are expected to provide at least one observation (1..*). We will be supporting the schema.org observation model (https://schema.org/Observation) with default values. Users will be encouraged to provide their own statistical populations as the project progresses.

<!--te-->
