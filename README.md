ats-discovery-service
===========================

Abstract Test Suite for INSPIRE profile of CSW ISO Application Profile.

*Note*: This ATS is in draft stage, none of the tests have an official INSPIRE MIG approval.

## External document references

| Abbreviation | Document name                       |
| ------------ | ----------------------------------- |
| INSPIRE <a name="ref_INSPIRE"></a> | [Directive 2007/2/EC of the European Parliament and of the Council of 14 March 2007 establishing an Infrastructure for Spatial Information in the European Community (INSPIRE)](http://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32007L0002&from=EN)
| IR NS <a name="ref_IR_NS"></a>   | [Commission Regulation (EC) No 976/2009 of 19 October 2009 implementing Directive 2007/2/EC of the European Parliament and of the Council as regards the Network Services](http://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32009R0976&from=EN)
| IR NS AMD <a name="ref_IR_NS_AMD"></a> | [Commission Regulation (EU) No 1311/2014 of 10 December 2014 amending Regulation (EC) No 976/2009 as regards the definition of an INSPIRE metadata element](http://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32014R1311&from=EN)
| TG DISC <a name="ref_TG_DISC"></a> | [Technical Guidance for INSPIRE Discovery Services, version 3.1](http://inspire.jrc.ec.europa.eu/documents/Network_Services/TechnicalGuidance_DiscoveryServices_v3.1.pdf)
| CSW <a name="ref_CSW"></a> | [OGC Catalogue Services Specification, version 2.0.2 (Corrigendum Release 2) (OGC 07-006r1)](http://portal.opengeospatial.org/files/?artifact_id=20555)
| CSW_ISO_AP <a name="ref_CSW_ISO_AP"></a> | [OGC Catalogue Services Specification 2.0.2 - ISO Metadata Application Profile for CSW 2.0, version 1.0.0 (OGC 07-045)](http://portal.opengeospatial.org/files/?artifact_id=21460)
| OWS_COMMON_10 <a name="ref_OWS_COMMON_10"></a> | [OGC Web Services Common Specification, version 1.0 (OGC 05-008c1](http://portal.opengeospatial.org/files/?artifact_id=8798)

## TG Requirement coverage

Based on requirement numbering in [TG DISC](#ref_TG_DISC).

| Req#   | Description                          | Covered by test(s)                 | IR reference(s)                  |
| ------ | ------------------------------------ | ---------------------------------- | -------------------------------- |
| 1      | Scope: CSW ISO AP + INSPIRE extensions| [A.1.1 ISO Metadata Application Profile](A.01.01.ISO_AP.md) | n/a |
| 2      | Overview: INSPIRE extensions | [A.1.2 Extended behaviour](A.01.02.extended.behaviour.md) | |
| 3      | Federated catalogs advertised | [A.2.6 Federated catalogues advertisement](A.02.06.federated.catalogues.advertisement.md) | |
| 4      | Additional search attributes mandatory | [A.3.1 INSPIRE search attributes](A.03.01.inspire.search.attributes.md) | |
| 5      | Additional search attributes advertised | [A.2.3 Additional search attributes](A.02.03.addiotional.search.attributes.md) | |
| 6      | Get Discovery Service Metadata request: language attribute | [A.2.2 Additional language parameter](A.02.02.additional.language.parameter.md) | |
| 7      | Either MetadataURL or embedded metadata | [A.2.4 Discovery Service metadata parameters](A.02.04.discovery.service.metadata.parameters.md) | |
| 8      | INSPIRE requirements to GetCapabilities response | [A.2.5 INSPIRE service metadata conformant](A.02.05.inspire.service.md.conformant.md) | |
| 9      | Discover Metadata request: Language & Query | [A.3.2 Language and query parameters](A.03.02.language.query.parameters.md) | |
| 10     | Discover Metadata request: Language| [A.3.3 Language search attribute](A.03.03.language.search.attribute.md) | |
| 11     | Discover Metadata request: Query | [A.3.4 Query](A.03.04.query.md) | |
| 12     | At least the INSPIRE MD elements in Discover Metadata response | [A.3.5 INSPIRE metadata elements](A.03.05.inspire.md.elements.md) | |
| 13     | Publish Metadata: resource type and format | [A.4.1 Harvesting readiness](A.04.01.harvesting.readiness.md) | |
| 14     | Link Discovery Service | [A.5.1 Third Party Discovery Services harvestable by MS Discovery Service](A.05.01.third.party.discovery.services.harvestable.md) | |
| 15     | Third Party Discovery Services published in MS Discovery Service | [A.4.2 Third Party Discovery Services published to MS Discovery Service](A.04.02.third.party.discovery.services.published.md) | |
| 16     | FederatedCatalogues declared | [A.2.7 Federated Discovery Service](A.02.07.federated.discovery.service.md) | |
| 17     | DistributedSearch fixed hop count = 2 | [A.3.6 Distributed search parameter](A.03.06.distributed.search.parameter.md) | |
| 18     | INSPIRE MD records requested through Discovery Service | [A.1.3 ISO 19115/19119 information model](A.01.03.iso_19115_19119.model.md) | |
| 19     | Mandatory INSPIRE queryables | [A.3.7 INSPIRE search criteria](A.03.07.inspire.search.criteria.md) | |
| 20     | Language queryable | [A.3.8 Language search criteria](A.03.08.language.search.criteria.md) | |
| 21     | Non ISO AP INSPIRE queryables | [A.3.9 Additional search criteria](A.03.09.additional.search.criteria.md) | |
| 22     | Declare INSPIRE queryables in Capabilities | [A.2.1 ISO searching parameters](A.02.01.iso.searching.parameters.md) | |
| 23     | List supported natural languages | [A.2.8 Natural languages](A.02.08.natural.languages.md) | |
| 24     | Client may select a natural language | [A.1.4 Language parameter](A.01.04.language.parameter.md) | |
| 25     | Name and value range of the language parameter| [A.1.5 ISO 639 codes](A.01.05.iso-639.codes.md) | |
| 26     | Default used for unsupported language requests | [A.1.6 Unsupported languages](A.01.06.unsupported.languages.md) | |
| 27     | ResponseLanguage declared | [A.2.9 Response language](A.02.09.response.language.md) | |
| 28     | Use SupportedLanguages element for supported languages | [A.2.10 Supported languages](A.02.10.supported.languages.md) | |
| 29     | Extended capabilities XML Schema | [A.2.11 XML schema](A.02.11.xml.schema.md) | |
| 30     | GetRecords with no language filter | [A.3.10 Missing language filter](A.03.10.missing.language.filter.md) | |
| 31     | GetRecords with a language filter | [A.3.11 Language filter](A.03.11.language.filter.md) | |
| 32     | Language for Exceptions | [A.3.12 Invalid request](A.03.12.invalid.request.md) | |

## Tests

The ATS for the INSPIRE profile of CSW ISO AP contains the following tests:

| Identifier                                                        | Status   |
| ----------------------------------------------------------------- | -------- |
| [A.1.1 ISO Metadata Application Profile](A.01.01.ISO_AP.md)       | missing  |
| [A.1.2 Extended behaviour](A.01.02.extended.behaviour.md)         | missing  |
| [A.1.3 ISO 19115/19119 information model](A.01.03.iso_19115_19119.model.md) | missing  |
| [A.1.4 Language parameter](A.01.04.language.parameter.md) | missing  |
| [A.1.5 ISO 639 codes](A.01.05.iso-639.codes.md) | missing  |
| [A.1.6 Unsupported languages](A.01.06.unsupported.languages.md) | missing  |
| [A.2.1 ISO searching parameters](A.02.01.iso.searching.parameters.md) | missing  |
| [A.2.2 Additional language parameter](A.02.02.additional.language.parameter.md) | missing  |
| [A.2.3 Additional search attributes](A.02.03.addiotional.search.attributes.md) | missing  |
| [A.2.4 Discovery Service metadata parameters](A.02.04.discovery.service.metadata.parameters.md) | missing  |
| [A.2.5 INSPIRE service metadata conformant](A.02.05.inspire.service.md.conformant.md) | missing  |
| [A.2.6 Federated catalogues advertisement](A.02.06.federated.catalogues.advertisement.md) | missing  |
| [A.2.7 Federated Discovery Service](A.02.07.federated.discovery.service.md) | missing  |
| [A.2.8 Natural languages](A.02.08.natural.languages.md) | missing  |
| [A.2.9 Response language](A.02.09.response.language.md) | missing  |
| [A.2.10 Supported languages](A.02.10.supported.languages.md) | missing  |
| [A.2.11 XML schema](A.02.11.xml.schema.md) | missing  |
| [A.3.1 INSPIRE search attributes](A.03.01.inspire.search.attributes.md) | missing  |
| [A.3.2 Language and query parameters](A.03.02.language.query.parameters.md) | missing  |
| [A.3.3 Language search attribute](A.03.03.language.search.attribute.md) | missing  |
| [A.3.4 Query](A.03.04.query.md) | missing  |
| [A.3.5 INSPIRE metadata elements](A.03.05.inspire.md.elements.md) | missing  |
| [A.3.6 Distributed search parameter](A.03.06.distributed.search.parameter.md) | missing  |
| [A.3.7 INSPIRE search criteria](A.03.07.inspire.search.criteria.md) | missing  |
| [A.3.8 Language search criteria](A.03.08.language.search.criteria.md) | missing  |
| [A.3.9 Additional search criteria](A.03.09.additional.search.criteria.md) | missing  |
| [A.3.10 Missing language filter](A.03.10.missing.language.filter.md) | missing  |
| [A.3.11 Language filter](A.03.11.language.filter.md) | missing  |
| [A.3.12 Invalid request](A.03.12.invalid.request.md) | missing  |
| [A.4.1 Harvesting readiness](A.04.01.harvesting.readiness.md) | missing  |
| [A.4.2 Third Party Discovery Services published to MS Discovery Service](A.04.02.third.party.discovery.services.published.md) | missing  |
| [A.5.1 Third Party Discovery Services harvestable by MS Discovery Service](A.05.01.third.party.discovery.services.harvestable.md) | missing  |
| [A.6.1 Performance](A.06.01.QoS.performance.md) | missing  |
| [A.6.2 Capacity](A.06.02.QoS.capacity.md) | missing  |
| [A.6.3 Availability](A.06.03.QoS.availability.md) | missing  |

## Open issues
* Tests [A.6.1 Performance](A.06.01.QoS.performance.md), [A.6.2 Capacity](A.06.02.QoS.capacity.md) and [A.6.3 Availability](A.06.03.QoS.availability.md) do not have corresponding explicit Implementation Requirements in the [TG DISC](#ref_TG_DISC).

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
