# Language Natural Language Fields

**Purpose**: Test that natural language fields vary depending on the requested language.

**Prerequisites**

**Test method**

* Send a GetCapabilities request for each supported language.

    * Check manually that [Title](#title) and [Abstract](#abstract) fields are in the requested language.

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 24

**Test type**: Manual

**Notes**


**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
Title <a name="title"></a> | /csw:Capabilities/ows:ServiceIdentification/ows:Title
Abstract <a name="abstract"></a> | /csw:Capabilities/ows:ServiceIdentification/ows:Abstract
