# Language GetRecords Exception

**Purpose**: Test that GetRecords exceptions are provided in the correct language.

**Prerequisites**

**Test method**

* Send a valid GetRecords request with a language filter where the language is not supported by the service.

    * Check that the service does not raise an exception.

* Send an invalid GetRecords request that raise an exception with a language filter.

    * Check manually that the exception is in the default or the requested language.

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 32

**Test type**: Manual

**Notes**


**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------

