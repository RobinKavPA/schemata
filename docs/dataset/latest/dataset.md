# HDR UK Dataset Schema

```txt
https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json
```

HDR UK Dataset Schema


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                       |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------------------------------ |
| Can be instantiated | Yes        | Unknown status | No           | Forbidden         | Forbidden             | none                | [dataset.schema.json](../../../schema/dataset/latest/dataset.schema.json "open original schema") |

## HDR UK Dataset Type

`object` ([HDR UK Dataset](dataset.md))

# HDR UK Dataset Properties

| Property                                      | Type          | Required | Nullable       | Defined by                                                                                                                            |
| :-------------------------------------------- | ------------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------ |
| [identifier](#identifier)                     | Merged        | Required | cannot be null | [HDR UK Dataset](dataset-properties-dataset-identifier.md "\#/properties/identifier#/properties/identifier")                          |
| [version](#version)                           | `string`      | Required | cannot be null | [HDR UK Dataset](dataset-properties-dataset-version.md "\#/properties/version#/properties/version")                                   |
| [revisions](#revisions)                       | `array`       | Required | cannot be null | [HDR UK Dataset](dataset-properties-dataset-revisions.md "\#/properties/revisions#/properties/revisions")                             |
| [issued](#issued)                             | `string`      | Required | cannot be null | [HDR UK Dataset](dataset-properties-creation-date.md "\#/properties/issued#/properties/issued")                                       |
| [modified](#modified)                         | `string`      | Required | cannot be null | [HDR UK Dataset](dataset-properties-modification-date.md "\#/properties/modified#/properties/modified")                               |
| [summary](#summary)                           | Not specified | Required | cannot be null | [HDR UK Dataset](dataset-properties-summary.md "\#/definitions/summary#/properties/summary")                                          |
| [documentation](#documentation)               | Not specified | Optional | cannot be null | [HDR UK Dataset](dataset-properties-documentation.md "\#/definitions/member#/properties/documentation")                               |
| [coverage](#coverage)                         | Not specified | Optional | cannot be null | [HDR UK Dataset](dataset-properties-coverage.md "\#/definitions/coverage#/properties/coverage")                                       |
| [provenance](#provenance)                     | Not specified | Optional | cannot be null | [HDR UK Dataset](dataset-properties-provenance.md "\#/definitions/provenance#/properties/provenance")                                 |
| [accessibility](#accessibility)               | Not specified | Required | cannot be null | [HDR UK Dataset](dataset-properties-accessibility.md "\#/definitions/accessibility#/properties/accessibility")                        |
| [enrichmentAndLinkage](#enrichmentAndLinkage) | Not specified | Optional | cannot be null | [HDR UK Dataset](dataset-properties-enrichment-and-linkage.md "\#/definitions/enrichmentAndLinkage#/properties/enrichmentAndLinkage") |
| [observations](#observations)                 | `array`       | Optional | cannot be null | [HDR UK Dataset](dataset-properties-observations.md "\#/properties/observations#/properties/observations")                            |

## identifier

System dataset identifier


> <http://purl.org/dc/terms/identifier>
>

`identifier`

-   is required
-   Type: merged type ([Dataset identifier](dataset-properties-dataset-identifier.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-dataset-identifier.md "\#/properties/identifier#/properties/identifier")

### identifier Type

merged type ([Dataset identifier](dataset-properties-dataset-identifier.md))

any of

-   [Untitled undefined type in HDR UK Dataset](dataset-properties-dataset-identifier-anyof-0.md "check type definition")
-   [Untitled string in HDR UK Dataset](dataset-properties-dataset-identifier-anyof-1.md "check type definition")

### identifier Examples

```json
[
  "226fb3f1-4471-400a-8c39-2b66d46a39b6"
]
```

## version

Dataset metadata version


`version`

-   is required
-   Type: `string` ([Dataset Version](dataset-properties-dataset-version.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-dataset-version.md "\#/properties/version#/properties/version")

### version Type

`string` ([Dataset Version](dataset-properties-dataset-version.md))

### version Constraints

**pattern**: the string must match the following regular expression: 

```regexp
^([0-9]+)\.([0-9]+)\.([0-9]+)$
```

[try pattern](https://regexr.com/?expression=%5E(%5B0-9%5D%2B)%5C.(%5B0-9%5D%2B)%5C.(%5B0-9%5D%2B)%24 "try regular expression with regexr.com")

### version Examples

```json
"1.1.0"
```

## revisions

Revisions of Dataset metadata


`revisions`

-   is required
-   Type: an array where each item follows the corresponding schema in the following list:

    1.  [Untitled undefined type in HDR UK Dataset](dataset-properties-dataset-revisions-items-0.md "check type definition")
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-dataset-revisions.md "\#/properties/revisions#/properties/revisions")

### revisions Type

an array where each item follows the corresponding schema in the following list:

1.  [Untitled undefined type in HDR UK Dataset](dataset-properties-dataset-revisions-items-0.md "check type definition")

## issued

Dataset Metadata Creation Date


> dcat:issued
>

`issued`

-   is required
-   Type: `string` ([Creation Date](dataset-properties-creation-date.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-creation-date.md "\#/properties/issued#/properties/issued")

### issued Type

`string` ([Creation Date](dataset-properties-creation-date.md))

### issued Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## modified

Dataset Metadata Creation Date


> dcat:modified
>

`modified`

-   is required
-   Type: `string` ([Modification Date](dataset-properties-modification-date.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-modification-date.md "\#/properties/modified#/properties/modified")

### modified Type

`string` ([Modification Date](dataset-properties-modification-date.md))

### modified Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## summary

Summary metadata must be completed by Data Custodians onboarding metadata into the Innovation Gateway MVP.


`summary`

-   is required
-   Type: unknown ([Summary](dataset-properties-summary.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-summary.md "\#/definitions/summary#/properties/summary")

### summary Type

unknown ([Summary](dataset-properties-summary.md))

## documentation

Documentation can include a rich text description of the dataset or links to media such as documents, images, presentations, videos or links to data dictionaries, profiles or dashboards. Organisations are required to confirm that they have permission to distribute any additional media.


`documentation`

-   is optional
-   Type: unknown ([Documentation](dataset-properties-documentation.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-documentation.md "\#/definitions/member#/properties/documentation")

### documentation Type

unknown ([Documentation](dataset-properties-documentation.md))

## coverage

This information includes attributes for geographical and temporal coverage, cohort details etc. to enable a deeper understanding of the dataset content so that researchers can make decisions about the relevance of the underlying data.


`coverage`

-   is optional
-   Type: unknown ([Coverage](dataset-properties-coverage.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-coverage.md "\#/definitions/coverage#/properties/coverage")

### coverage Type

unknown ([Coverage](dataset-properties-coverage.md))

## provenance

Provenance information allows researchers to understand data within the context of its origins and can be an indicator of quality, authenticity and timeliness.


`provenance`

-   is optional
-   Type: unknown ([Provenance](dataset-properties-provenance.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-provenance.md "\#/definitions/provenance#/properties/provenance")

### provenance Type

unknown ([Provenance](dataset-properties-provenance.md))

## accessibility

Accessibility information allows researchers to understand access, usage, limitations, formats, standards and linkage or interoperability with toolsets.


`accessibility`

-   is required
-   Type: unknown ([Accessibility](dataset-properties-accessibility.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-accessibility.md "\#/definitions/accessibility#/properties/accessibility")

### accessibility Type

unknown ([Accessibility](dataset-properties-accessibility.md))

## enrichmentAndLinkage

This section includes information about related datasets that may have previously been linked, as well as indicating if there is the opportunity to link to other datasets in the future. If a dataset has been enriched and/or derivations, scores and existing tools are available this section allows providers to indicate this to researchers.


`enrichmentAndLinkage`

-   is optional
-   Type: unknown ([Enrichment and Linkage](dataset-properties-enrichment-and-linkage.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-enrichment-and-linkage.md "\#/definitions/enrichmentAndLinkage#/properties/enrichmentAndLinkage")

### enrichmentAndLinkage Type

unknown ([Enrichment and Linkage](dataset-properties-enrichment-and-linkage.md))

## observations

Multiple observations about the dataset may be provided and users are expected to provide at least one observation (1..\*). We will be supporting the schema.org observation model (<https://schema.org/Observation>) with default values. Users will be encouraged to provide their own statistical populations as the project progresses. Example: &lt;b> Statistical Population 1 &lt;/b> type: StatisticalPopulation populationType: Persons numConstraints: 0 &lt;b> Statistical Population 2 &lt;/b> type: StatisticalPopulation populationType: Events numConstraints: 0 &lt;b> Statistical Population 3 &lt;/b> type: StatisticalPopulation populationType: Findings numConstraints: 0 typeOf: Observation observedNode: &lt;b> Statistical Population 1 &lt;/b> measuredProperty: count measuredValue: 32937 observationDate: “2017”


> <https://schema.org/observation>
>

`observations`

-   is optional
-   Type: an array of merged types ([Details](dataset-properties-observations-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-observations.md "\#/properties/observations#/properties/observations")

### observations Type

an array of merged types ([Details](dataset-properties-observations-items.md))

# HDR UK Dataset Definitions

## Definitions group revision

Reference this group by using

```json
{"$ref":"#/definitions/revision#/definitions/revision"}
```




`revision`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-revision.md "\#/definitions/revision#/definitions/revision")

### revision Type

unknown

## Definitions group summary

Reference this group by using

```json
{"$ref":"#/definitions/summary#/definitions/summary"}
```




`summary`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-summary.md "\#/definitions/summary#/definitions/summary")

### summary Type

unknown

## Definitions group organisation

Reference this group by using

```json
{"$ref":"#/definitions/organisation#/definitions/organisation"}
```

Describes an organisation for purposes of discovery and identification.


`organisation`

-   is optional
-   Type: `object` ([Organisation Metadata](dataset-definitions-organisation-metadata.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-organisation-metadata.md "\#/definitions/organisation#/definitions/organisation")

### organisation Type

`object` ([Organisation Metadata](dataset-definitions-organisation-metadata.md))

## Definitions group documentation

Reference this group by using

```json
{"$ref":"#/definitions/member#/definitions/documentation"}
```




`documentation`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-documentation.md "\#/definitions/member#/definitions/documentation")

### documentation Type

unknown

## Definitions group coverage

Reference this group by using

```json
{"$ref":"#/definitions/coverage#/definitions/coverage"}
```




`coverage`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-coverage.md "\#/definitions/coverage#/definitions/coverage")

### coverage Type

unknown

## Definitions group provenance

Reference this group by using

```json
{"$ref":"#/definitions/provenance#/definitions/provenance"}
```




`provenance`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-provenance.md "\#/definitions/provenance#/definitions/provenance")

### provenance Type

unknown

## Definitions group origin

Reference this group by using

```json
{"$ref":"#/definitions/origin#/definitions/origin"}
```




`origin`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-origin.md "\#/definitions/origin#/definitions/origin")

### origin Type

unknown

## Definitions group temporal

Reference this group by using

```json
{"$ref":"#/definitions/temporal#/definitions/temporal"}
```




`temporal`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-temporal.md "\#/definitions/temporal#/definitions/temporal")

### temporal Type

unknown

## Definitions group accessibility

Reference this group by using

```json
{"$ref":"#/definitions/accessibility#/definitions/accessibility"}
```




`accessibility`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-accessibility.md "\#/definitions/accessibility#/definitions/accessibility")

### accessibility Type

unknown

## Definitions group usage

Reference this group by using

```json
{"$ref":"#/definitions/usage#/definitions/usage"}
```




`usage`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-usage.md "\#/definitions/usage#/definitions/usage")

### usage Type

unknown

## Definitions group access

Reference this group by using

```json
{"$ref":"#/definitions/access#/definitions/access"}
```




`access`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-access.md "\#/definitions/access#/definitions/access")

### access Type

unknown

## Definitions group formatAndStandards

Reference this group by using

```json
{"$ref":"#/definitions/formatAndStandards#/definitions/formatAndStandards"}
```




`formatAndStandards`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-formatandstandards.md "\#/definitions/formatAndStandards#/definitions/formatAndStandards")

### formatAndStandards Type

unknown

## Definitions group enrichmentAndLinkage

Reference this group by using

```json
{"$ref":"#/definitions/enrichmentAndLinkage#/definitions/enrichmentAndLinkage"}
```




`enrichmentAndLinkage`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-enrichmentandlinkage.md "\#/definitions/enrichmentAndLinkage#/definitions/enrichmentAndLinkage")

### enrichmentAndLinkage Type

unknown

## Definitions group observation

Reference this group by using

```json
{"$ref":"#/definitions/observation#/definitions/observation"}
```




`observation`

-   is optional
-   Type: unknown
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-observation.md "\#/definitions/observation#/definitions/observation")

### observation Type

unknown

## Definitions group uuidv4

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/uuidv4"}
```




`uuidv4`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-uuidv4.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/uuidv4")

### uuidv4 Type

`string`

### uuidv4 Constraints

**maximum length**: the maximum number of characters for this string is: `36`

**minimum length**: the minimum number of characters for this string is: `36`

**pattern**: the string must match the following regular expression: 

```regexp
^[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}$
```

[try pattern](https://regexr.com/?expression=%5E%5Ba-fA-F0-9%5D%7B8%7D-%5Ba-fA-F0-9%5D%7B4%7D-%5Ba-fA-F0-9%5D%7B4%7D-%5Ba-fA-F0-9%5D%7B4%7D-%5Ba-fA-F0-9%5D%7B12%7D%24 "try regular expression with regexr.com")

## Definitions group semver

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/semver"}
```




`semver`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-semver.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/semver")

### semver Type

`string`

### semver Constraints

**pattern**: the string must match the following regular expression: 

```regexp
^([0-9]+)\.([0-9]+)\.([0-9]+)$
```

[try pattern](https://regexr.com/?expression=%5E(%5B0-9%5D%2B)%5C.(%5B0-9%5D%2B)%5C.(%5B0-9%5D%2B)%24 "try regular expression with regexr.com")

## Definitions group url

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/url"}
```




`url`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-url.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/url")

### url Type

`string`

### url Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

## Definitions group eightyCharacters

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/eightyCharacters"}
```




`eightyCharacters`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-eightycharacters.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/eightyCharacters")

### eightyCharacters Type

`string`

### eightyCharacters Constraints

**maximum length**: the maximum number of characters for this string is: `80`

**minimum length**: the minimum number of characters for this string is: `2`

## Definitions group abstractText

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/abstractText"}
```




`abstractText`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-abstracttext.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/abstractText")

### abstractText Type

`string`

### abstractText Constraints

**maximum length**: the maximum number of characters for this string is: `255`

**minimum length**: the minimum number of characters for this string is: `5`

## Definitions group emailAddress

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/emailAddress"}
```




`emailAddress`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-emailaddress.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/emailAddress")

### emailAddress Type

`string`

### emailAddress Constraints

**email**: the string must be an email address, according to [RFC 5322, section 3.4.1](https://tools.ietf.org/html/rfc5322 "check the specification")

## Definitions group shortDescription

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/shortDescription"}
```




`shortDescription`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-shortdescription.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/shortDescription")

### shortDescription Type

`string`

### shortDescription Constraints

**maximum length**: the maximum number of characters for this string is: `1000`

**minimum length**: the minimum number of characters for this string is: `2`

## Definitions group description

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/description"}
```




`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-description.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/description")

### description Type

`string`

### description Constraints

**maximum length**: the maximum number of characters for this string is: `3000`

**minimum length**: the minimum number of characters for this string is: `2`

## Definitions group longDescription

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/longDescription"}
```




`longDescription`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-longdescription.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/longDescription")

### longDescription Type

`string`

### longDescription Constraints

**maximum length**: the maximum number of characters for this string is: `5000`

**minimum length**: the minimum number of characters for this string is: `2`

## Definitions group commaSeparatedValues

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/commaSeparatedValues"}
```




`commaSeparatedValues`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-commaseparatedvalues.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/commaSeparatedValues")

### commaSeparatedValues Type

`string`

### commaSeparatedValues Constraints

**pattern**: the string must match the following regular expression: 

```regexp
([^,]+)
```

[try pattern](https://regexr.com/?expression=(%5B%5E%2C%5D%2B) "try regular expression with regexr.com")

## Definitions group doi

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/doi"}
```




`doi`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-doi.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/doi")

### doi Type

`string`

### doi Constraints

**pattern**: the string must match the following regular expression: 

```regexp
^10.\d{4,9}/[-._;()/:a-zA-Z0-9]+$
```

[try pattern](https://regexr.com/?expression=%5E10.%5Cd%7B4%2C9%7D%2F%5B-._%3B()%2F%3Aa-zA-Z0-9%5D%2B%24 "try regular expression with regexr.com")

## Definitions group ageRange

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/ageRange"}
```




`ageRange`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-agerange.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/ageRange")

### ageRange Type

`string`

### ageRange Constraints

**pattern**: the string must match the following regular expression: 

```regexp
(150|1[0-4][0-9]|[0-9]|[1-8][0-9]|9[0-9])-(150|1[0-4][0-9]|[0-9]|[1-8][0-9]|9[0-9])
```

[try pattern](https://regexr.com/?expression=(150%7C1%5B0-4%5D%5B0-9%5D%7C%5B0-9%5D%7C%5B1-8%5D%5B0-9%5D%7C9%5B0-9%5D)-(150%7C1%5B0-4%5D%5B0-9%5D%7C%5B0-9%5D%7C%5B1-8%5D%5B0-9%5D%7C9%5B0-9%5D) "try regular expression with regexr.com")

## Definitions group format

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/format"}
```




> FIXME: Conforms to spec, but may be a list of strings given cardinality 1:\*. Validate against external list of formats, e.g. <https://www.iana.org/assignments/media-types/media-types.xhtml>
>

`format`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-format.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/format")

### format Type

`string`

### format Constraints

**minimum length**: the minimum number of characters for this string is: `1`

## Definitions group isocountrycode

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/isocountrycode"}
```




> FIXME: Add ISO 3166-2 Subdivision code pattern
>

`isocountrycode`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-isocountrycode.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/isocountrycode")

### isocountrycode Type

`string`

### isocountrycode Constraints

**pattern**: the string must match the following regular expression: 

```regexp
^[A-Z]{2}(-[A-Z]{2,3})?$
```

[try pattern](https://regexr.com/?expression=%5E%5BA-Z%5D%7B2%7D(-%5BA-Z%5D%7B2%2C3%7D)%3F%24 "try regular expression with regexr.com")

## Definitions group memberOf

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/memberOf"}
```




`memberOf`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-memberof.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/memberOf")

### memberOf Type

`string`

### memberOf Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value        | Explanation |
| :----------- | ----------- |
| `"HUB"`      |             |
| `"ALLIANCE"` |             |
| `"OTHER"`    |             |

## Definitions group physicalSampleAvailability

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/physicalSampleAvailability"}
```




`physicalSampleAvailability`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-physicalsampleavailability.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/physicalSampleAvailability")

### physicalSampleAvailability Type

`string`

### physicalSampleAvailability Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                            | Explanation |
| :------------------------------- | ----------- |
| `"NOT AVAILABLE"`                |             |
| `"BONE MARROW"`                  |             |
| `"CANCER CELL LINES"`            |             |
| `"CORE BIOPSY"`                  |             |
| `"CDNA OR MRNA"`                 |             |
| `"DNA"`                          |             |
| `"FAECES"`                       |             |
| `"IMMORTALIZED CELL LINES"`      |             |
| `"MICRORNA"`                     |             |
| `"PERIPHERAL BLOOD CELLS"`       |             |
| `"PLASMA"`                       |             |
| `"PM TISSUE"`                    |             |
| `"PRIMARY CELLS"`                |             |
| `"RNA"`                          |             |
| `"SALIVA"`                       |             |
| `"SERUM"`                        |             |
| `"SWABS"`                        |             |
| `"TISSUE"`                       |             |
| `"URINE"`                        |             |
| `"WHOLE BLOOD"`                  |             |
| `"AVAILABILITY TO BE CONFIRMED"` |             |
| `"OTHER"`                        |             |

## Definitions group followup

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/followup"}
```




`followup`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-followup.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/followup")

### followup Type

`string`

### followup Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value             | Explanation |
| :---------------- | ----------- |
| `"0-6 MONTHS"`    |             |
| `"6-12 MONTHS"`   |             |
| `"1-10 YEARS"`    |             |
| `"MORE 10 YEARS"` |             |
| `"UNKNOWN"`       |             |
| `"OTHER"`         |             |

## Definitions group periodicity

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/periodicity"}
```




`periodicity`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-periodicity.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/periodicity")

### periodicity Type

`string`

### periodicity Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | ----------- |
| `"STATIC"`     |             |
| `"IRREGULAR"`  |             |
| `"CONTINUOUS"` |             |
| `"BIENNIAL"`   |             |
| `"ANNUAL"`     |             |
| `"BIANNUAL"`   |             |
| `"QUARTERLY"`  |             |
| `"BIMONTHLY"`  |             |
| `"MONTHLY"`    |             |
| `"BIWEEKLY"`   |             |
| `"WEEKLY"`     |             |
| `"SEMIWEEKLY"` |             |
| `"DAILY"`      |             |
| `"OTHER"`      |             |

## Definitions group purpose

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/purpose"}
```




`purpose`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-purpose.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/purpose")

### purpose Type

`string`

### purpose Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                | Explanation |
| :------------------- | ----------- |
| `"STUDY"`            |             |
| `"DISEASE REGISTRY"` |             |
| `"TRIAL"`            |             |
| `"CARE"`             |             |
| `"AUDIT"`            |             |
| `"ADMINISTRATIVE"`   |             |
| `"FINANCIAL"`        |             |
| `"OTHER"`            |             |

## Definitions group source

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/source"}
```




`source`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-source.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/source")

### source Type

`string`

### source Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                 | Explanation |
| :-------------------- | ----------- |
| `"EPR"`               |             |
| `"ELECTRONIC SURVEY"` |             |
| `"LIMS"`              |             |
| `"PAPER BASED"`       |             |
| `"FREETEXT NLP"`      |             |
| `"MACHINE GENERATED"` |             |
| `"OTHER"`             |             |

## Definitions group setting

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/setting"}
```




`setting`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-setting.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/setting")

### setting Type

`string`

### setting Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                     | Explanation |
| :------------------------ | ----------- |
| `"CLINIC"`                |             |
| `"PRIMARY CARE"`          |             |
| `"ACCIDENT AN EMERGENCY"` |             |
| `"OUTPATIENTS"`           |             |
| `"IN-PATIENTS"`           |             |
| `"SERVICES"`              |             |
| `"COMMUNITY"`             |             |
| `"HOME"`                  |             |
| `"PRIVATE"`               |             |
| `"PHARMACY"`              |             |
| `"OTHER"`                 |             |

## Definitions group timeLag

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/timeLag"}
```




`timeLag`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-timelag.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/timeLag")

### timeLag Type

`string`

### timeLag Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value              | Explanation |
| :----------------- | ----------- |
| `"LESS 1 WEEK"`    |             |
| `"1-2 WEEKS"`      |             |
| `"2-4 WEEKS"`      |             |
| `"1-2 MONTHS"`     |             |
| `"2-6 MONTHS"`     |             |
| `"MORE 6 MONTHS"`  |             |
| `"VARIABLE"`       |             |
| `"NOT APPLICABLE"` |             |
| `"OTHER"`          |             |

## Definitions group dataUseLimitation

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/dataUseLimitation"}
```




`dataUseLimitation`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-datauselimitation.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/dataUseLimitation")

### dataUseLimitation Type

`string`

### dataUseLimitation Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                              | Explanation |
| :--------------------------------- | ----------- |
| `"GENERAL RESEARCH USE"`           |             |
| `"GENETIC STUDIES ONLY"`           |             |
| `"NO GENERAL METHODS RESEARCH"`    |             |
| `"NO RESTRICTION"`                 |             |
| `"RESEARCH SPECIFIC RESTRICTIONS"` |             |
| `"RESEARCH USE ONLY"`              |             |
| `"NO LINKAGE"`                     |             |

## Definitions group dataUseRequirements

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/dataUseRequirements"}
```




`dataUseRequirements`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-datauserequirements.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/dataUseRequirements")

### dataUseRequirements Type

`string`

### dataUseRequirements Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                                 | Explanation |
| :------------------------------------ | ----------- |
| `"COLLABORATION REQUIRED"`            |             |
| `"ETHICS APPROVAL REQUIRED"`          |             |
| `"GEOGRAPHICAL RESTRICTIONS"`         |             |
| `"INSTITUTION SPECIFIC RESTRICTIONS"` |             |
| `"NOT FOR PROFIT USE"`                |             |
| `"PROJECT SPECIFIC RESTRICTIONS"`     |             |
| `"PUBLICATION MORATORIUM"`            |             |
| `"PUBLICATION REQUIRED"`              |             |
| `"RETURN TO DATABASE OR RESOURCE"`    |             |
| `"TIME LIMIT ON USE"`                 |             |
| `"USER SPECIFIC RESTRICTION"`         |             |

## Definitions group deliveryLeadTime

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/deliveryLeadTime"}
```




`deliveryLeadTime`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-deliveryleadtime.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/deliveryLeadTime")

### deliveryLeadTime Type

`string`

### deliveryLeadTime Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value              | Explanation |
| :----------------- | ----------- |
| `"LESS 1 WEEK"`    |             |
| `"1-2 WEEKS"`      |             |
| `"2-4 WEEKS"`      |             |
| `"1-2 MONTHS"`     |             |
| `"2-6 MONTHS"`     |             |
| `"MORE 6 MONTHS"`  |             |
| `"VARIABLE"`       |             |
| `"NOT APPLICABLE"` |             |
| `"OTHER"`          |             |

## Definitions group standardisedDataModels

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/standardisedDataModels"}
```




`standardisedDataModels`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-standardiseddatamodels.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/standardisedDataModels")

### standardisedDataModels Type

`string`

### standardisedDataModels Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                            | Explanation |
| :------------------------------- | ----------- |
| `"HL7 FHIR"`                     |             |
| `"HL7 V2"`                       |             |
| `"HL7 CDA"`                      |             |
| `"HL7 CCOW"`                     |             |
| `"LOINC"`                        |             |
| `"DICOM"`                        |             |
| `"I2B2"`                         |             |
| `"IHE"`                          |             |
| `"OMOP"`                         |             |
| `"OPENEHR"`                      |             |
| `"SENTINEL"`                     |             |
| `"PCORNET"`                      |             |
| `"CDISC"`                        |             |
| `"NHS DATA DICTIONARY"`          |             |
| `"NHS SCOTLAND DATA DICTIONARY"` |             |
| `"NHS WALES DATA DICTIONARY"`    |             |
| `"LOCAL"`                        |             |
| `"OTHER"`                        |             |

## Definitions group controlledVocabulary

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/controlledVocabulary"}
```




`controlledVocabulary`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-controlledvocabulary.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/controlledVocabulary")

### controlledVocabulary Type

`string`

### controlledVocabulary Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                           | Explanation |
| :------------------------------ | ----------- |
| `"LOCAL"`                       |             |
| `"OPCS4"`                       |             |
| `"READ"`                        |             |
| `"SNOMED CT"`                   |             |
| `"SNOMED RT"`                   |             |
| `"DM PLUS D"`                   |             |
| `"NHS NATIONAL CODES"`          |             |
| `"NHS SCOTLAND NATIONAL CODES"` |             |
| `"NHS WALES NATIONAL CODES"`    |             |
| `"ODS"`                         |             |
| `"LOINC"`                       |             |
| `"ICD10"`                       |             |
| `"ICD10CM"`                     |             |
| `"ICD10PCS"`                    |             |
| `"ICD9CM"`                      |             |
| `"ICD9"`                        |             |
| `"ICDO3"`                       |             |
| `"AMT"`                         |             |
| `"APC"`                         |             |
| `"ATC"`                         |             |
| `"CIEL"`                        |             |
| `"HPO"`                         |             |
| `"CPT4"`                        |             |
| `"DPD"`                         |             |
| `"DRG"`                         |             |
| `"HEMONC"`                      |             |
| `"JMDC"`                        |             |
| `"KCD7"`                        |             |
| `"MULTUM"`                      |             |
| `"NAACCR"`                      |             |
| `"NDC"`                         |             |
| `"NDFRT"`                       |             |
| `"OXMIS"`                       |             |
| `"RXNORM"`                      |             |
| `"RXNORM EXTENSION"`            |             |
| `"SPL"`                         |             |
| `"OTHER"`                       |             |

## Definitions group language

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/language"}
```




`language`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-language.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/language")

### language Type

`string`

### language Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value  | Explanation |
| :----- | ----------- |
| `"aa"` |             |
| `"ab"` |             |
| `"ae"` |             |
| `"af"` |             |
| `"ak"` |             |
| `"am"` |             |
| `"an"` |             |
| `"ar"` |             |
| `"as"` |             |
| `"av"` |             |
| `"ay"` |             |
| `"az"` |             |
| `"ba"` |             |
| `"be"` |             |
| `"bg"` |             |
| `"bh"` |             |
| `"bi"` |             |
| `"bm"` |             |
| `"bn"` |             |
| `"bo"` |             |
| `"br"` |             |
| `"bs"` |             |
| `"ca"` |             |
| `"ce"` |             |
| `"ch"` |             |
| `"co"` |             |
| `"cr"` |             |
| `"cs"` |             |
| `"cu"` |             |
| `"cv"` |             |
| `"cy"` |             |
| `"da"` |             |
| `"de"` |             |
| `"dv"` |             |
| `"dz"` |             |
| `"ee"` |             |
| `"el"` |             |
| `"en"` |             |
| `"eo"` |             |
| `"es"` |             |
| `"et"` |             |
| `"eu"` |             |
| `"fa"` |             |
| `"ff"` |             |
| `"fi"` |             |
| `"fj"` |             |
| `"fo"` |             |
| `"fr"` |             |
| `"fy"` |             |
| `"ga"` |             |
| `"gd"` |             |
| `"gl"` |             |
| `"gn"` |             |
| `"gu"` |             |
| `"gv"` |             |
| `"ha"` |             |
| `"he"` |             |
| `"hi"` |             |
| `"ho"` |             |
| `"hr"` |             |
| `"ht"` |             |
| `"hu"` |             |
| `"hy"` |             |
| `"hz"` |             |
| `"ia"` |             |
| `"id"` |             |
| `"ie"` |             |
| `"ig"` |             |
| `"ii"` |             |
| `"ik"` |             |
| `"io"` |             |
| `"is"` |             |
| `"it"` |             |
| `"iu"` |             |
| `"ja"` |             |
| `"jv"` |             |
| `"ka"` |             |
| `"kg"` |             |
| `"ki"` |             |
| `"kj"` |             |
| `"kk"` |             |
| `"kl"` |             |
| `"km"` |             |
| `"kn"` |             |
| `"ko"` |             |
| `"kr"` |             |
| `"ks"` |             |
| `"ku"` |             |
| `"kv"` |             |
| `"kw"` |             |
| `"ky"` |             |
| `"la"` |             |
| `"lb"` |             |
| `"lg"` |             |
| `"li"` |             |
| `"ln"` |             |
| `"lo"` |             |
| `"lt"` |             |
| `"lu"` |             |
| `"lv"` |             |
| `"mg"` |             |
| `"mh"` |             |
| `"mi"` |             |
| `"mk"` |             |
| `"ml"` |             |
| `"mn"` |             |
| `"mr"` |             |
| `"ms"` |             |
| `"mt"` |             |
| `"my"` |             |
| `"na"` |             |
| `"nb"` |             |
| `"nd"` |             |
| `"ne"` |             |
| `"ng"` |             |
| `"nl"` |             |
| `"nn"` |             |
| `"no"` |             |
| `"nr"` |             |
| `"nv"` |             |
| `"ny"` |             |
| `"oc"` |             |
| `"oj"` |             |
| `"om"` |             |
| `"or"` |             |
| `"os"` |             |
| `"pa"` |             |
| `"pi"` |             |
| `"pl"` |             |
| `"ps"` |             |
| `"pt"` |             |
| `"qu"` |             |
| `"rm"` |             |
| `"rn"` |             |
| `"ro"` |             |
| `"ru"` |             |
| `"rw"` |             |
| `"sa"` |             |
| `"sc"` |             |
| `"sd"` |             |
| `"se"` |             |
| `"sg"` |             |
| `"si"` |             |
| `"sk"` |             |
| `"sl"` |             |
| `"sm"` |             |
| `"sn"` |             |
| `"so"` |             |
| `"sq"` |             |
| `"sr"` |             |
| `"ss"` |             |
| `"st"` |             |
| `"su"` |             |
| `"sv"` |             |
| `"sw"` |             |
| `"ta"` |             |
| `"te"` |             |
| `"tg"` |             |
| `"th"` |             |
| `"ti"` |             |
| `"tk"` |             |
| `"tl"` |             |
| `"tn"` |             |
| `"to"` |             |
| `"tr"` |             |
| `"ts"` |             |
| `"tt"` |             |
| `"tw"` |             |
| `"ty"` |             |
| `"ug"` |             |
| `"uk"` |             |
| `"ur"` |             |
| `"uz"` |             |
| `"ve"` |             |
| `"vi"` |             |
| `"vo"` |             |
| `"wa"` |             |
| `"wo"` |             |
| `"xh"` |             |
| `"yi"` |             |
| `"yo"` |             |
| `"za"` |             |
| `"zh"` |             |
| `"zu"` |             |

## Definitions group statisticalPopulationConstrained

Reference this group by using

```json
{"$ref":"https://raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/statisticalPopulationConstrained"}
```




`statisticalPopulationConstrained`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-statisticalpopulationconstrained.md "https&#x3A;//raw.githubusercontent.com/HDRUK/schemata/master/schema/dataset/dataset.schema.json#/definitions/statisticalPopulationConstrained")

### statisticalPopulationConstrained Type

`string`

### statisticalPopulationConstrained Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value        | Explanation |
| :----------- | ----------- |
| `"PERSONS"`  |             |
| `"EVENTS"`   |             |
| `"FINDINGS"` |             |
