
# HDR UK Dataset Properties

| Property                                      | Type          | Required | Nullable       | Defined by   | Weight |
| :-------------------------------------------- | ------------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------ | ------------- |
| [identifier](#identifier)                     | Merged        | Required | cannot be null | [HDR UK Dataset](dataset-properties-dataset-identifier.md "\#/properties/identifier#/properties/identifier")                          | INSERT |
| [version](#version)                           | `string`      | Required | cannot be null | [HDR UK Dataset](dataset-properties-dataset-version.md "\#/properties/version#/properties/version")                                   | INSERT |
| [revisions](#revisions)                       | `array`       | Required | cannot be null | [HDR UK Dataset](dataset-properties-dataset-revisions.md "\#/properties/revisions#/properties/revisions")                             | INSERT |
| [issued](#issued)                             | `string`      | Required | cannot be null | [HDR UK Dataset](dataset-properties-creation-date.md "\#/properties/issued#/properties/issued")                                       | INSERT |
| [modified](#modified)                         | `string`      | Required | cannot be null | [HDR UK Dataset](dataset-properties-modification-date.md "\#/properties/modified#/properties/modified")                               | INSERT |
| [summary](#summary)                           | Not specified | Required | cannot be null | [HDR UK Dataset](dataset-properties-summary.md "\#/definitions/summary#/properties/summary")                                          | INSERT |
| [documentation](#documentation)               | Not specified | Optional | cannot be null | [HDR UK Dataset](dataset-properties-documentation.md "\#/definitions/member#/properties/documentation")                               | INSERT |
| [coverage](#coverage)                         | Not specified | Optional | cannot be null | [HDR UK Dataset](dataset-properties-coverage.md "\#/definitions/coverage#/properties/coverage")                                       | INSERT |
| [provenance](#provenance)                     | Not specified | Optional | cannot be null | [HDR UK Dataset](dataset-properties-provenance.md "\#/definitions/provenance#/properties/provenance")                                 | INSERT |
| [accessibility](#accessibility)               | Not specified | Required | cannot be null | [HDR UK Dataset](dataset-properties-accessibility.md "\#/definitions/accessibility#/properties/accessibility")                        | INSERT |
| [enrichmentAndLinkage](#enrichmentandlinkage) | Not specified | Optional | cannot be null | [HDR UK Dataset](dataset-properties-enrichment-and-linkage.md "\#/definitions/enrichmentAndLinkage#/properties/enrichmentAndLinkage") | INSERT |
| [observations](#observations)                 | `array`       | Optional | cannot be null | [HDR UK Dataset](dataset-properties-observations.md "\#/properties/observations#/properties/observations")                            | INSERT |

