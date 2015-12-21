# A.3.10 Missing language filter

**Purpose**: Verification whether the response to a Discover Metadata request without a language specific filter contains metadata records independent from any language.

**Prerequisites**

**Test method**

Examine whether the response to a Discover Metadata request without a language specific filter contains metadata records independent from any language. The response (i.e. the GetRecords response XML) may contain metadata records of several natural languages, if the  INSPIRE Discovery Service under test contains records in different languages.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 30

**Test type**: Automated

**Notes**


## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
