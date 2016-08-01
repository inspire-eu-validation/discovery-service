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

| Req#   | Description                          | Covered by test(s)                 | IR reference(s)                  |
| ------ | ------------------------------------ | ---------------------------------- | -------------------------------- |
| 1      | Scope: CSW ISO AP + INSPIRE extensions| n/a, covered by dependency and the tests for the other requirements | n/a |
| 2      | Overview: INSPIRE extensions | n/a, covered by the tests for the specific requirements | n/a |
| 3      | Federated catalogs advertised | [Federated catalogues](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/federated-catalogues) | n/a |
| 4      | Additional search attributes mandatory | n/a, covered by the tests for the specific requirements | [IR NS](#ref_IR_NS), Annex II – Part A|
| 5      | Additional search attributes advertised | [Additional queryables declared](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/additional-queryables-declared) | [IR NS](#ref_IR_NS), Annex A |
| 6      | Get Discovery Service Metadata request: language attribute | n/a, covered by the tests for the specific requirements | [IR NS](#ref_IR_NS), Annex II, Part B, section 2.1.1 |
| 7      | Either MetadataURL or embedded metadata | [Discovery service metadata: scenario 1](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/service-metadata-scenario-1), [Discovery service metadata: scenario 2](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/service-metadata-scenario-2) |[IR NS](#ref_IR_NS), Annex II, Part B, section 3.2.1 |
| 8      | INSPIRE requirements to GetCapabilities response | [Discovery service metadata: scenario 2](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/service-metadata-scenario-2) | [IR NS](#ref_IR_NS), Article 2; [IR MD](#ref_IR_MD) |
| 9      | Discover Metadata request: Language & Query | n/a, covered by the tests for the specific requirements |[IR NS](#ref_IR_NS), Annex II, Part B, section 3.1 |
| 10     | Discover Metadata request: Language | [Language queryable](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/language-queryable) | [IR NS](#ref_IR_NS), Annex II, Part B, section 3.1|
| 11     | Discover Metadata request: Query | n/a, covered by dependency to CSW ISO AP 1.0.0 | [IR NS](#ref_IR_NS), Annex II, Part B, section 3.1 |
| 12     | INSPIRE metadata elements according to ISO 19115/19119 | [INSPIRE metadata elements using ISO 19115/19119 information model](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/inspire-metadata-elements) | [IR NS](#ref_IR_NS), Annex II, Part B, section 3.2.1|
| 13     | Publish Metadata: resource type and format | not testable | n/a |
| 14     | Link Discovery Service | n/a, Three implementation scenarios: Centralised (req. implicitly fulfilled), Discovery Client: see req. 15, Discovery Service: see req. 16/17 | [IR NS](#ref_IR_NS), Annex II, Part B, section 5|
| 15     | Third Party Discovery Services published in MS Discovery Service | not testable | [IR NS](#ref_IR_NS), Annex II, Part B, section 4.2.2.1|
| 16     | Federated catalogues referenced | [Federated catalogues](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/federated-catalogues) | n/a |
| 17     | DistributedSearch fixed hop count = 2 | not a requirement | n/a |
| 18     | INSPIRE MD records requested through Discovery Service | [INSPIRE metadata elements using ISO 19115/19119 information model](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/inspire-metadata-elements) | n/a |
| 19     | Mandatory INSPIRE queryables | [INSPIRE queryables](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/inspire-queryables) | [IR NS](#ref_IR_NS), Annex II, Part A |
| 20     | Language queryable | [Language queryable](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/language-queryable) |  [IR NS](#ref_IR_NS), Annex II, Part B, section 3.1; [ID MD](#ref_IR_MD), Annex, Part B, section 10.3|
| 21     | Non ISO AP INSPIRE queryables | [INSPIRE queryables](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/inspire-queryables) | [IR NS](#ref_IR_NS), Annex II, Part A|
| 22     | Declare INSPIRE queryables in Capabilities | [ISO queryables declared](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/iso-queryables-declared), [Additional queryables declared](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/additional-queryables-declared) | [IR NS](#ref_IR_NS), Annex II, Part A |
| 23     | List supported natural languages | [Supported languages](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/supported-languages) | [IR NS](#ref_IR_NS), Annex II, Part B, section 2.2|
| 24     | Client may select a natural language | n/a, covered by the more specific tests | [IR NS](#ref_IR_NS), Annex II, Part B, sections 2.1.1, 2.2, 2.2.3, 3.1, 3.1.1 |
| 25     | Name and value range of the language parameter | [Supported languages](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/supported-languages) | n/a |
| 26     | Default used for unsupported language requests | [Language selection capabilities](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/language-selection-capabilities) | n/a |
| 27     | ResponseLanguage declared | [Language selection capabilities](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/language-selection-capabilities) | [IR NS](#ref_IR_NS), Annex II, Part B, section 2.2.3|
| 28     | Use SupportedLanguages element for supported languages | [Supported languages](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/supported-languages) |[IR NS](#ref_IR_NS), Annex II, Part B, section 2.2.3 |
| 29     | Extended capabilities XML Schema | [Schema validation](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/schema-validation) | n/a |
| 30     | GetRecords with no language filter | [Missing language filter](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/missing-language-filter) | n/a |
| 31     | GetRecords with a language filter | [Language queryable](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/language-queryable) | n/a |
| 32     | Language for Exceptions | [Invalid request](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/invalid-request) | n/a |

Note: Requirements marked as "not testable" should be reconsidered in a revision of the technical guidance. Requirements must be testable. 

## Tests

The Conformance Class contains the following test cases:

| Identifier                                                        | Status   |
| ----------------------------------------------------------------- | -------- |
| [Additional queryables declared](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/additional-queryables-declared) | ready for review  |
| [Federated catalogues](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/federated-catalogues) | ready for review  |
| [INSPIRE metadata elements using the ISO 19115/19119 information model](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/inspire-metadata-elements) | ready for review  |
| [INSPIRE queryables](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/inspire-queryables) | ready for review  |
| [Invalid request](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/invalid-request) | ready for review  |
| [ISO queryables declared](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/iso-queryables-declared) | ready for review  |
| [Language queryable](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/language-queryable) | ready for review  |
| [Language queryable declared](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/language-queryable-declared) | ready for review  |
| [Language selection capabilities](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/language-selection-capabilities) | ready for review  |
| [No language filter](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/no-language-filter) | ready for review  |
| [Schema validation](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/schema-validation) | ready for review  |
| Discovery service metadata: scenario 1](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/service-metadata-scenario-1) | ready for review |
| Discovery service metadata: scenario 2](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/service-metadata-scenario-2) | ready for review |
| [Supported languages](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/supported-languages) | ready for review  |

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
