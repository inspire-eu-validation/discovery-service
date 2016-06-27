INSPIRE Profile of CSW ISO AP v3.1
==================================

Conformance Class for INSPIRE Profile of CSW ISO AP v3.1

*Note*: This CC is in ready for review stage, none of the tests have an official INSPIRE MIG approval.

## External document references

| Abbreviation | Document name                       |
| ------------ | ----------------------------------- |
| INSPIRE <a name="ref_INSPIRE"></a> | [Directive 2007/2/EC of the European Parliament and of the Council of 14 March 2007 establishing an Infrastructure for Spatial Information in the European Community (INSPIRE)](http://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32007L0002&from=EN)
| IR NS <a name="ref_IR_NS"></a>   | [Commission Regulation (EC) No 976/2009 of 19 October 2009 implementing Directive 2007/2/EC of the European Parliament and of the Council as regards the Network Services](http://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32009R0976&from=EN)
| IR NS AMD <a name="ref_IR_NS_AMD"></a> | [Commission Regulation (EU) No 1311/2014 of 10 December 2014 amending Regulation (EC) No 976/2009 as regards the definition of an INSPIRE metadata element](http://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32014R1311&from=EN)
| IR MD <a name="ref_IR_MD"></a> | [Commission Regulation (EC) No 1205/2008 of December 2008 implementing Directive 2007/2/EC of the European Parliament and of the Council as regards metadata (Text with EEA relevance)](http://eur-lex.europa.eu/LexUriServ/LexUriServ.do?uri=OJ:L:2008:326:0012:0030:EN:PDF)
| TG DISC <a name="ref_TG_DISC"></a> | [Technical Guidance for INSPIRE Discovery Services, version 3.1](http://inspire.jrc.ec.europa.eu/documents/Network_Services/TechnicalGuidance_DiscoveryServices_v3.1.pdf)
| CSW <a name="ref_CSW"></a> | [OGC Catalogue Services Specification, version 2.0.2 (Corrigendum Release 2) (OGC 07-006r1)](http://portal.opengeospatial.org/files/?artifact_id=20555)
| CSW_ISO_AP <a name="ref_CSW_ISO_AP"></a> | [OGC Catalogue Services Specification 2.0.2 - ISO Metadata Application Profile for CSW 2.0, version 1.0.0 (OGC 07-045)](http://portal.opengeospatial.org/files/?artifact_id=21460)
| OWS_COMMON_10 <a name="ref_OWS_COMMON_10"></a> | [OGC Web Services Common Specification, version 1.0 (OGC 05-008c1](http://portal.opengeospatial.org/files/?artifact_id=8798)

## TG Requirement coverage

Based on requirement numbering in [TG DISC](#ref_TG_DISC).

| Req#   | Description                          | Covered by test(s)                 | IR reference(s)                  |
| ------ | ------------------------------------ | ---------------------------------- | -------------------------------- |
| 1      | Scope: CSW ISO AP + INSPIRE extensions| [ISO Metadata Application Profile](ISO_AP.md) | n/a |
| 2      | Overview: INSPIRE extensions | [Extended behaviour](extended.behaviour.md) | [INSPIRE](#ref_INSPIRE), [IR NS](#ref_IR_NS) |
| 3      | Federated catalogs advertised | [Federated catalogues advertisement](federated.catalogues.advertisement.md) | n/a |
| 4      | Additional search attributes mandatory | [INSPIRE search attributes](inspire.search.attributes.md) | [IR NS](#ref_IR_NS), Annex II – Part A|
| 5      | Additional search attributes advertised | [Additional search attributes](addiotional.search.attributes.md) | [IR NS](#ref_IR_NS), Annex A |
| 6      | Get Discovery Service Metadata request: language attribute | [Additional language parameter](additional.language.parameter.md) | [IR NS](#ref_IR_NS), Annex II, Part B, section 2.1.1 |
| 7      | Either MetadataURL or embedded metadata | [Discovery Service metadata parameters](discovery.service.metadata.parameters.md) |[IR NS](#ref_IR_NS), Annex II, Part B, section 3.2.1 |
| 8      | INSPIRE requirements to GetCapabilities response | [INSPIRE service metadata conformant](inspire.service.md.conformant.md) | [IR NS](#ref_IR_NS), Article 2; [IR MD](#ref_IR_MD) |
| 9      | Discover Metadata request: Language & Query | [Language and query parameters](language.query.parameters.md) |[IR NS](#ref_IR_NS), Annex II, Part B, section 3.1 |
| 10     | Discover Metadata request: Language| [Language search attribute](language.search.attribute.md) | [IR NS](#ref_IR_NS), Annex II, Part B, section 3.1|
| 11     | Discover Metadata request: Query | [Query](query.md) | [IR NS](#ref_IR_NS), Annex II, Part B, section 3.1 |
| 12     | At least the INSPIRE MD elements in Discover Metadata response | [INSPIRE metadata elements](inspire.md.elements.md) | [IR NS](#ref_IR_NS), Annex II, Part B, section 3.2.1|
| 13     | Publish Metadata: resource type and format | [Harvesting readiness](harvesting.readiness.md) | n/a |
| 14     | Link Discovery Service | [Third Party Discovery Services harvestable by MS Discovery Service](third.party.discovery.services.harvestable.md) | [IR NS](#ref_IR_NS), Annex II, Part B, section 5|
| 15     | Third Party Discovery Services published in MS Discovery Service | Not testable | [IR NS](#ref_IR_NS), Annex II, Part B, section 4.2.2.1|
| 16     | FederatedCatalogues declared | [Federated Discovery Service](federated.discovery.service.md) | n/a |
| 17     | DistributedSearch fixed hop count = 2 | [Distributed search parameter](distributed.search.parameter.md) | n/a |
| 18     | INSPIRE MD records requested through Discovery Service | [ISO 19115/19119 information model](iso_19115_19119.model.md) | n/a |
| 19     | Mandatory INSPIRE queryables | [INSPIRE search criteria](inspire.search.criteria.md) | [IR NS](#ref_IR_NS), Annex II, Part A |
| 20     | Language queryable | [Language search criteria](language.search.criteria.md) |  [IR NS](#ref_IR_NS), Annex II, Part B, section 3.1; [ID MD](#ref_IR_MD), Annex, Part B, section 10.3|
| 21     | Non ISO AP INSPIRE queryables | [Additional search criteria](additional.search.criteria.md) | [IR NS](#ref_IR_NS), Annex II, Part A|
| 22     | Declare INSPIRE queryables in Capabilities | [ISO searching parameters](iso.searching.parameters.md) | [IR NS](#ref_IR_NS), Annex II, Part A|
| 23     | List supported natural languages | [Natural languages](natural.languages.md) | [IR NS](#ref_IR_NS), Annex II, Part B, section 2.2|
| 24     | Client may select a natural language | [Language parameter](language.parameter.md) | [IR NS](#ref_IR_NS), Annex II, Part B, sections 2.1.1, 2.2, 2.2.3, 3.1, 3.1.1 |
| 25     | Name and value range of the language parameter| [ISO 639 codes](iso-639.codes.md) | n/a |
| 26     | Default used for unsupported language requests | [Unsupported languages](unsupported.languages.md) | n/a |
| 27     | ResponseLanguage declared | [Response language](response.language.md) | [IR NS](#ref_IR_NS), Annex II, Part B, section 2.2.3|
| 28     | Use SupportedLanguages element for supported languages | [Supported languages](supported.languages.md) |[IR NS](#ref_IR_NS), Annex II, Part B, section 2.2.3 |
| 29     | Extended capabilities XML Schema | [XML schema](xml.schema.md) | n/a |
| 30     | GetRecords with no language filter | [Missing language filter](missing.language.filter.md) | n/a |
| 31     | GetRecords with a language filter | [Language filter](language.filter.md) | n/a |
| 32     | Language for Exceptions | [Invalid request](invalid.request.md) | n/a |

## Tests

The CC for the INSPIRE Profile of CSW ISO AP v3.1 contains the following test cases:

| Identifier                                                        | Status   |
| ----------------------------------------------------------------- | -------- |
| [ISO Metadata Application Profile](ISO_AP.md)       | ready for review  |
| [Extended behaviour](extended.behaviour.md)         | ready for review  |
| [ISO 19115/19119 information model](iso_19115_19119.model.md) | ready for review  |
| [Language parameter](language.parameter.md) | ready for review  |
| [ISO 639 codes](iso-639.codes.md) | ready for review  |
| [Unsupported languages](unsupported.languages.md) | ready for review  |
| [ISO searching parameters](iso.searching.parameters.md) | ready for review  |
| [Additional language parameter](additional.language.parameter.md) | ready for review  |
| [Additional search attributes](addiotional.search.attributes.md) | ready for review  |
| [Discovery Service metadata parameters](discovery.service.metadata.parameters.md) | ready for review  |
| [INSPIRE service metadata conformant](inspire.service.md.conformant.md) | ready for review  |
| [Federated catalogues advertisement](federated.catalogues.advertisement.md) | ready for review  |
| [Federated Discovery Service](federated.discovery.service.md) | ready for review  |
| [Natural languages](natural.languages.md) | ready for review  |
| [Response language](response.language.md) | ready for review  |
| [Supported languages](supported.languages.md) | ready for review  |
| [XML schema](xml.schema.md) | ready for review  |
| [INSPIRE search attributes](inspire.search.attributes.md) | ready for review  |
| [Language and query parameters](language.query.parameters.md) | ready for review  |
| [Language search attribute](language.search.attribute.md) | ready for review  |
| [Query](query.md) | ready for review  |
| [INSPIRE metadata elements](inspire.md.elements.md) | ready for review  |
| [Distributed search parameter](distributed.search.parameter.md) | ready for review  |
| [INSPIRE search criteria](inspire.search.criteria.md) | ready for review  |
| [Language search criteria](language.search.criteria.md) | ready for review  |
| [Additional search criteria](additional.search.criteria.md) | ready for review  |
| [Missing language filter](missing.language.filter.md) | ready for review  |
| [Language filter](language.filter.md) | ready for review  |
| [Invalid request](invalid.request.md) | ready for review  |
| [Harvesting readiness](harvesting.readiness.md) | ready for review  |
| [Third Party Discovery Services harvestable by MS Discovery Service](third.party.discovery.services.harvestable.md) | ready for review  |


## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
gmd | http://www.isotc211.org/2005/gmd
gml | http://www.opengis.net/gml/3.2
srv | http://www.isotc211.org/2005/srv
xlink          | http://www.w3.org/1999/xlink
inspire_ds | http://inspire.ec.europa.eu/schemas/inspire_ds/1.0
inspire_common | http://inspire.ec.europa.eu/schemas/common/1.0
ows_common | http://www.opengis.net/ows
