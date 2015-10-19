# A.3.11 Language filter

**Purpose**: Verification whether the response to a Discover Metadata request comply with a language defined in the request.

**Prerequisites**


**Test method**

Examine whether the response to a Discover Metadata request comply with a language defined in the request. In other words, the Discover Metadata response offers only the metadata records having the language identical to the language specific filter as defined by the Discover Metadata request. If no metadata records comply with the request, the service shall respond normally with an empty result set (without raising an exception).

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 31

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
