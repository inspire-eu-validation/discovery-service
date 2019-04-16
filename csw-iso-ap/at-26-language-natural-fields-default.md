# Language Natural Fields Default

**Purpose**: Test that natural language fields are provided in default language when requested language is unsupported or absent.

**Prerequisites**

**Test method**

* Send a GetCapabilities request.

* Send a GetCapabilities request with LANGUAGE parameter and its value equals to [Default Language](#defaultLanguage).

    * Check that [Title](#title) and [Abstract](#abstract) values are the same as first request.

* Send a GetCapabilities request with LANGUAGE parameter and unsupported value.

    * Check that [Title](#title) and [Abstract](#abstract) values are the same as first request.

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 26

**Test type**: Automated

**Notes**


**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression (relative to /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities)
---------------------------------------------------------- | -------------------------------------------------------------------------
Default Language <a name="defaultLanguage"></a> | inspire_common:SupportedLanguages/inspire_common:DefaultLanguage/inspire_common:Language
Title <a name="title"></a> | /csw:Capabilities/ows:ServiceIdentification/ows:Title
Abstract <a name="abstract"></a> | /csw:Capabilities/ows:ServiceIdentification/ows:Abstract

