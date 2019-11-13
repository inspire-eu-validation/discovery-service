# Language Response Value

**Purpose**: Test that the response language is correct based on the requested language.

**Prerequisites**

**Test method**

* Send a GetCapabilities request with LANGUAGE parameter and its value equals to [Default Language](#defaultLanguage).

    * Check that [Response Language](#responseLanguage) value is equal to [Default Language](#defaultLanguage).

* For every [Supported Language](#supportedLanguage),

    * Send a GetCapabilities request with LANGUAGE parameter and corresponding value.

        * Check that [Response Language](#responseLanguage) value is equal to requested language.

* Send a GetCapabilities request with LANGUAGE parameter and invalid value.

    * Check that [Response Language](#responseLanguage) value is equal to [Default Language](#defaultLanguage).

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 27

**Test type**: Automated

**Notes**


**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression (relative to /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities)
---------------------------------------------------------- | -------------------------------------------------------------------------
Default Language <a name="defaultLanguage"></a> | inspire_common:SupportedLanguages/inspire_common:DefaultLanguage/inspire_common:Language
Response Language <a name="responseLanguage"></a> | inspire_common:SupportedLanguages/inspire_common:SupportedLanguage/inspire_common:Language
Supported Language <a name="supportedLanguage"></a> | inspire_common:ResponseLanguage/inspire_common:Language
