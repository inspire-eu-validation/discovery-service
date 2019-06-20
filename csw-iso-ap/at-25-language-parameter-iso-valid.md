# Language Parameter ISO valid

**Purpose**: Test that the service support the parameter LANGUAGE.

**Prerequisites**

**Test method**

* Send a GetCapabilities request with mandatory parameters only.

    * Check that [Default Language](#defaultLanguage), [Supported Language](#supportedLanguage) and [Response Language](#responseLanguage) are ISO 639-2/B alpha 3 valid.

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 25

**Test type**: Automated

**Notes**


**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression (relative to /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities)
---------------------------------------------------------- | -------------------------------------------------------------------------
Default Language <a name="defaultLanguage"></a> | inspire_common:SupportedLanguages/inspire_common:DefaultLanguage/inspire_common:Language
Supported Language <a name="supportedLanguage"></a> | inspire_common:SupportedLanguages/inspire_common:SupportedLanguage/inspire_common:Language
Response Language <a name="responseLanguage"></a> | inspire_common:ResponseLanguage/inspire_common:Language
