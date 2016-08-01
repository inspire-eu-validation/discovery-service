# Conformance class: CSW ISO AP Quality-of-service (DRAFT)

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

none

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

There are no requirements with identifiers for QoS in the current version of the TG.

## Tests

The Conformance Class contains the following test cases:

| Conformance Class | Identifier                                                        | Status   |
| ------------------| ----------------------------------------------------------------- | -------- |
| INSPIRE Quality of Services v3.1 | [QoS Performance](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap-qos/performance) | ready for review  |
| INSPIRE Quality of Services v3.1 | [QoS Capacity](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap-qos/capacity) | ready for review  |
| INSPIRE Quality of Services v3.1 | [QoS Availability](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap-qos/availability) | ready for review  |

## Open issues

* Tests [QoS Performance](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap-qos/performance.md), [qos capacity](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap-qos/capacity.md) and [qos availability](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap-qos/availability.md) do not have corresponding explicit Implementation Requirements in the [TG DISC](#ref_TG_DISC).

* Tests are declared to be of type "automated", but this is not correct, as the test methods include statements like: "Periods of planned downtime e.g. because of system maintenance, are not included in the measure. Downtime is considered planned when notified to the community well in advance (minimum 1 week), e.g. via notifications to registered users or on portals."

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
ows | http://www.opengis.net/ows
