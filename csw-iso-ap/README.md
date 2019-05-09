# Conformance class: INSPIRE Profile of CSW ISO AP (DRAFT)

This conformance class is part of the [Abstract Test Suite for the INSPIRE Discovery Services Technical Guidance](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1).

## Standardization target type

OGC web service (CSW ISO AP 1.0.0)

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the discovery service, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [CSW ISO AP 1.0.0](#ref_CSW_ISO_AP) | Read-only CSW, CSW Server (A.1.2) | n/a |

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [INSPIRE Metadata Implementing Rules: Technical Guidelines based on EN ISO 19115 and EN ISO 19119, version 1.3](#ref_TG_MD) | [ISO 19115/19119 profile](http://inspire.ec.europa.eu/id/ats/metadata/1.3/iso-19115-19119) | ISO 19115/19119 metadata record | `encoding` = `ISO AP 1.0` or `ISO/TS 19139` |

This indirect dependency applies to all resources referenced from `inspire_common:MetdataUrl` elements in the Capabilities document and for all metadata records returned as a response to `GetRecords` requests.
 
## External document references

| Abbreviation | Document name                       |
| ------------ | ----------------------------------- |
| INSPIRE <a name="ref_INSPIRE"></a> | [Directive 2007/2/EC of the European Parliament and of the Council of 14 March 2007 establishing an Infrastructure for Spatial Information in the European Community (INSPIRE)](http://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32007L0002&from=EN)
| IR NS <a name="ref_IR_NS"></a>   | [Commission Regulation (EC) No 976/2009 of 19 October 2009 implementing Directive 2007/2/EC of the European Parliament and of the Council as regards the Network Services](http://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32009R0976&from=EN)
| IR NS AMD <a name="ref_IR_NS_AMD"></a> | [Commission Regulation (EU) No 1311/2014 of 10 December 2014 amending Regulation (EC) No 976/2009 as regards the definition of an INSPIRE metadata element](http://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32014R1311&from=EN)
| IR MD <a name="ref_IR_MD"></a> | [Commission Regulation (EC) No 1205/2008 of December 2008 implementing Directive 2007/2/EC of the European Parliament and of the Council as regards metadata (Text with EEA relevance)](http://eur-lex.europa.eu/LexUriServ/LexUriServ.do?uri=OJ:L:2008:326:0012:0030:EN:PDF)
| TG DISC <a name="ref_TG_DISC"></a> | [Technical Guidance for INSPIRE Discovery Services, version 3.1](http://inspire.jrc.ec.europa.eu/documents/Network_Services/TechnicalGuidance_DiscoveryServices_v3.1.pdf)
| TG MD <a name="ref_TG_MD"></a> | [INSPIRE Metadata Implementing Rules: Technical Guidelines based on EN ISO 19115 and EN ISO 19119, version 1.3](http://inspire.jrc.ec.europa.eu/documents/Metadata/MD_IR_and_ISO_20131029.pdf)
| CSW <a name="ref_CSW"></a> | [OGC Catalogue Services Specification, version 2.0.2 (Corrigendum Release 2) (OGC 07-006r1)](http://portal.opengeospatial.org/files/?artifact_id=20555)
| CSW_ISO_AP <a name="ref_CSW_ISO_AP"></a> | [OGC Catalogue Services Specification 2.0.2 - ISO Metadata Application Profile for CSW 2.0, version 1.0.0 (OGC 07-045)](http://portal.opengeospatial.org/files/?artifact_id=21460)
| OWS_COMMON_10 <a name="ref_OWS_COMMON_10"></a> | [OGC Web Services Common Specification, version 1.0 (OGC 05-008c1](http://portal.opengeospatial.org/files/?artifact_id=8798)

## TG Requirement coverage

Based on requirement numbering in [TG DISC](#ref_TG_DISC).

| Req#   | Description                          | Covered by test(s)                 |
| ------ | ------------------------------------ | ---------------------------------- |
| 1      | Scope: CSW ISO AP + INSPIRE extensions| n/a, covered by dependency and the tests for the other requirements |
| 2      | Extended Behaviour | [at-02-extended-behaviour](./at-02-extended-behaviour.md) |
| 3      | Federated Catalogues | [at-03-federated-catalogues](./at-03-federated-catalogues.md) |
| 4      | Search Attributes Support | [at-04-search-attributes-support](./at-04-search-attributes-support.md) |
| 5      | Search Attributes Advertised | [at-05-search-attributes-advertised](./at-05-search-attributes-advertised.md) |
| 6      | Preferred Language | [at-06-preferred-language](./at-06-preferred-language.md) |
| 7      | Extended Capabilities | [at-07-extended-capabilities](./at-07-extended-capabilities.md) |
| 8      | Service Metadata Sections | [at-08-service-metadata-sections](./at-08-service-metadata-sections.md) |
| 9      | Discovery Language Query Parameters | [at-09-discover-language-query-parameters](./at-09-discover-language-query-parameters.md) |
| 10     | Discover Language Parameter | [at-10-discover-language-parameter](./at-10-discover-language-parameter.md) |
| 11     | Discover Query Paramater  | [at-11-discover-query-parameter](./at-11-discover-query-parameter.md) |
| 12     | Discover Resource Matching Query | [at-12-discover-resource-matching-query](./at-12-discover-resource-matching-query.md) |
| 13     | Publish Discovery Service | [at-13-publish-discovery-service](./at-13-publish-discovery-service.md) |
| 14     | Link Discovery Service Operation | [at-14-link-discovery-service-operation](./at-14-link-discovery-service-operation.md) |
| 15     | Link Publish Metadata Operation | [at-15-link-publish-metadata-operation](./at-15-link-publish-metadata-operation.md) |
| 16     | Link Federated Capabilities Document | [at-16-link-federated-capabilities-document](./at-16-link-federated-capabilities-document.md) |
| 17     | Link Federated Search Attribute | [at-17-link-federated-search-attribute](./at-17-link-federated-search-attribute.md) |
| 18     | Query Inspire Discovery Interface | [at-18-query-inspire-discovery-interface](./at-18-query-inspire-discovery-interface.md) |
| 19     | Query Search Criteria | [at-19-query-search-criteria](./at-19-query-search-criteria.md) |
| 20     | Query Language Parameter | [at-20-query-language-parameter](./at-20-query-language-parameter.md) |
| 21     | Query Additional Parameters | [at-21-query-additional-parameters](./at-21-query-additional-parameters.md) |
| 22     | Query Parameters Advertised | [at-22-query-parameters-advertised](./at-22-query-parameters-advertised.md) |
| 23     | Language Supported | [at-23-language-supported](./at-23-language-supported.md) |
| 24     | Language Natural Language Fields | [at-24-language-natural-lang-fields](./at-24-language-natural-lang-fields.md) |
| 25     | Language Parameter ISO valid | [at-25-language-parameter-iso-valid](./at-25-language-parameter-iso-valid.md) |
| 26     | Language Natural Fields Default | [at-26-language-natural-fields-default](./at-26-language-natural-fields-default.md) |
| 27     | Language Response Value | [at-27-language-response-value](./at-27-language-response-value.md) |
| 28     | Language Supported Default Cardinality | [at-28-language-supported-default-cardinality](./at-28-language-supported-default-cardinality.md) |
| 29     | Extended Capabilities Schema Valid | [at-29-extended-capabilities-schema-valid](./at-29-extended-capabilities-schema-valid.md) |
| 30     | Language GetRecords without Parameter | [at-30-language-getrecords-without-parameter](./at-30-language-getrecords-without-parameter.md) |
| 31     | Language GetRecords Language Filter | [at-31-language-getrecords-lang-filter](./at-31-language-getrecords-lang-filter.md) |
| 32     | Language GetRecords Exception | [at-32-language-getrecords-exception](./at-32-language-getrecords-exception.md) |

## Tests

The Conformance Class contains the following test cases:

| Identifier                                                        | Type  | Status   |
| ----------------------------------------------------------------- | ----- | -------- |
| [at-02-extended-behaviour](./at-02-extended-behaviour.md) | None | ready for review  |
| [at-03-federated-catalogues](./at-03-federated-catalogues.md) | None | ready for review  |
| [at-04-search-attributes-support](./at-04-search-attributes-support.md) | None | ready for review  |
| [at-05-search-attributes-advertised](./at-05-search-attributes-advertised.md) | None | ready for review  |
| [at-06-preferred-language](./at-06-preferred-language.md) | None | ready for review  |
| [at-07-extended-capabilities](./at-07-extended-capabilities.md) | Automated | ready for review  |
| [at-08-service-metadata-sections](./at-08-service-metadata-sections.md) | None | ready for review  |
| [at-09-discover-language-query-parameters](./at-09-discover-language-query-parameters.md) | None | ready for review  |
| [at-10-discover-language-parameter](./at-10-discover-language-parameter.md) | None | ready for review  |
| [at-11-discover-query-parameter](./at-11-discover-query-parameter.md) | None | ready for review  |
| [at-12-discover-resource-matching-query](./at-12-discover-resource-matching-query.md) | Automated | ready for review  |
| [at-13-publish-discovery-service](./at-13-publish-discovery-service.md) | None | ready for review  |
| [at-14-link-discovery-service-operation](./at-14-link-discovery-service-operation.md) | None | ready for review  |
| [at-15-link-publish-metadata-operation](./at-15-link-publish-metadata-operation.md) | Manual | ready for review  |
| [at-16-link-federated-capabilities-document](./at-16-link-federated-capabilities-document.md) | Manual | ready for review  |
| [at-17-link-federated-search-attribute](./at-17-link-federated-search-attribute.md) | None | ready for review  |
| [at-18-query-inspire-discovery-interface](./at-18-query-inspire-discovery-interface.md) | None | ready for review  |
| [at-19-query-search-criteria](./at-19-query-search-criteria.md) | Manual | ready for review  |
| [at-20-query-language-parameter](./at-20-query-language-parameter.md) | Automated | ready for review  |
| [at-21-query-additional-parameters](./at-21-query-additional-parameters.md) | Manual | ready for review  |
| [at-22-query-parameters-advertised](./at-22-query-parameters-advertised.md) | Automated | ready for review  |
| [at-23-language-supported](./at-23-language-supported.md) | None | ready for review  |
| [at-24-language-natural-lang-fields](./at-24-language-natural-lang-fields.md) | Manual | ready for review  |
| [at-25-language-parameter-iso-valid](./at-25-language-parameter-iso-valid.md) | Automated | ready for review  |
| [at-26-language-natural-fields-default](./at-26-language-natural-fields-default.md) | Automated | ready for review  |
| [at-27-language-response-value](./at-27-language-response-value.md) | Automated | ready for review  |
| [at-28-language-supported-default-cardinality](./at-28-language-supported-default-cardinality.md) | Automated | ready for review  |
| [at-29-extended-capabilities-schema-valid](./at-29-extended-capabilities-schema-valid.md) | Automated | ready for review  |
| [at-30-language-getrecords-without-parameter](./at-30-language-getrecords-without-parameter.md) | Manual | ready for review  |
| [at-31-language-getrecords-lang-filter](./at-31-language-getrecords-lang-filter.md) | Manual | ready for review  |
| [at-32-language-getrecords-exception](./at-32-language-getrecords-exception.md) | Manual | ready for review  |

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
gmd | http://www.isotc211.org/2005/gmd
gco | http://www.isotc211.org/2005/gco
gml | http://www.opengis.net/gml/3.2
srv | http://www.isotc211.org/2005/srv
xlink          | http://www.w3.org/1999/xlink
inspire_ds | http://inspire.ec.europa.eu/schemas/inspire_ds/1.0
inspire_common | http://inspire.ec.europa.eu/schemas/common/1.0
ows | http://www.opengis.net/ows
csw | http://www.opengis.net/cat/csw/2.0.2
ogc | http://www.opengis.net/ogc
