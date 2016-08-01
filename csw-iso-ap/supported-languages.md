# Supported languages

**Purpose**: Verification whether the Extended Capabilities of the INSPIRE Get Discovery Service Metadata response (i.e. the Capabilities document) contain the list of supported languages.

**Prerequisites**

**Test method**

Examine whether the Extended Capabilities of the INSPIRE Get Discovery Service Metadata response contain the list of supported languages. More specifically examine whether:
1. the INSPIRE Get Discovery Service Metadata response (i.e. the Capabilities document) consists of exactly one element [DefaultLanguage](#DefaultLanguage) indicating the service default language, and
2. zero or more [SupportedLanguage](#SupportedLanguage) to indicate all additional supported languages.

Examine whether the values in the list [DefaultLanguage](#DefaultLanguage) and [SupportedLanguage](#SupportedLanguage) includes at least one of those language codes: eng, bul, cze, dan, est, fin, fre, hrv, dut, gle, ice, ita, lit, lav, hun, mlt, nor, ger, pol, por, rum, roh, gre, slo, slv, spa, swe.

**Reference(s)**

* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Chapter 4.5, Implementation Requirements 6, 23, 25, 28

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="DefaultLanguage"></a> DefaultLanguage | /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities/inspire_common:SupportedLanguages/inspire_common:DefaultLanguage
<a name="SupportedLanguage"></a> SupportedLanguage | /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities/inspire_common:SupportedLanguages/inspire_common:SupportedLanguage
