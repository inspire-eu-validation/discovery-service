# A.3.10 Missing language filter

**Purpose**: Verification whether the response to a Discover Metadata request without a language specific filter contains metadata records independent from any language.

**Prerequisites**

**Test method**

Examine whether the response to a Discover Metadata request without a language specific filter contains metadata records independent from any language. In other words, the response (i.e. the GetRecords response XML) contains all the metadata records matching the query regardless of their metadata language.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 30

**Test type**: Automated

**Notes**


## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
