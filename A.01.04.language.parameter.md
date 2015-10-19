# A.1.4 Language parameter

**Purpose**: Verification whether the INSPIRE Discovery Service properly supports natural languages.

**Prerequisites**

**Test method**

Examine whether the Get Discovery Service Metadata and Discover Metadata operations support the parameter “language”, which is an INSPIRE extension of the OGC Catalogue Service Specification in version 2.0.2. Both options below shall be tested:
1. the language requested by a client is contained in the list of supported languages, i.e. the natural language fields of the service response shall be in the requested language;
2. the language requested by a client is not supported by the INSPIRE Discovery Service, i.e. the “language” parameter shall be ignored.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 24
* [IR NS](README.md#ref_IR_NS), Annex II, Part B, sections 2.1.1, 2.2, 2.2.3, 3.1, 3.1.1

**Test type**: Automated

**Notes**


## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
