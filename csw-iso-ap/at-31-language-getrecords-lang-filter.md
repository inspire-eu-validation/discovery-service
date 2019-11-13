# Language GetRecords Language Filter

**Purpose**: Test that the service supports filtering by language.

**Prerequisites**

**Test method**

* Send a GetRecords request with a language filter using an unsupported language, which produces an empty set of metadata records.

    * Check that the service does not raise an exception.

* Send a GetRecords request with a language filter using a supported language.

    * Check manually that the records obtained are properly filtered.

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 31

**Test type**: Manual

**Notes**


**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------

