# A.3.12 Invalid request

**Purpose**: Verification whether the response in a form of an exception to an invalid Discover Metadata request containing a language specific parameter is provided in the default or in a requested and supported language.

**Prerequisites**

* [Supported languages](https://github.com/inspire-eu-validation/ats-discovery-service/blob/master/A.02.10.supported.languages.md)

**Test method**

Examine whether an invalid Discover Metadata request (from an ISO Metadata Application Profile of the OGC Catalogue Service Specification in version 2.0.2 point of view) containing a language specific parameter results in an exception that is responded in the default or in a requested and supported language. The use of a valid language specific filter itself shall not raise an exception, even if the requested language is not supported.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 32

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
