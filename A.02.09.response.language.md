# A.2.9 Response language

**Purpose**: Verification whether the Get Discovery Service Metadata response (i.e. the GetCapabilities document) contains an appropriate response language.

**Prerequisites**

**Test method**

Examine whether:
1. the language requested by a client is contained in the list of supported languages: in such cases the requested language shall correspond to the language used in the Get Discovery Service Metadata response (i.e. the GetCapabilities document) as defined in ```inspire-common:ResponseLanguage``` / ```/inspire_common:Language```;
2. the language requested by a client is NOT contained in the list of supported languages: in such cases the Get Discovery Service Metadata response (i.e. the GetCapabilities document) is provided in the service default language as defined in ```inspire-common:ResponseLanguage``` / ```/inspire_common:Language```.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 27
* [IR NS](README.md#ref_IR_NS), Annex II, Part B, section 2.2.3

**Test type**: Automated

**Notes**


## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
