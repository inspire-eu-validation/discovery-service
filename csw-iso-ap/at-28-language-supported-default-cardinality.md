# Language Supported Default Cardinality

**Purpose**: Test that the cardinality of supported languages is correct.

**Prerequisites**

**Test method**

* Send a GetCapabilities request.

* Check that exactly one [Default Language](#defaultLanguage) element exists.

* Check that zero or more [Supported Language](#supportedLanguage) elements exists.

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 28

**Test type**: Automated

**Notes**


**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression (relative to /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities)
---------------------------------------------------------- | -------------------------------------------------------------------------
Default Language <a name="defaultLanguage"></a> | inspire_common:SupportedLanguages/inspire_common:DefaultLanguage/inspire_common:Language
Supported Language <a name="supportedLanguage"></a> | inspire_common:ResponseLanguage/inspire_common:Language
