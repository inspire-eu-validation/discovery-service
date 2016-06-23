# A.2.10 Supported languages

**Purpose**: Verification whether the Extended Capabilities of the INSPIRE Get Discovery Service Metadata response (i.e. the GetCapabilities document) contain the list of supported languages.

**Prerequisites**

**Test method**

Examine whether the Extended Capabilities of the INSPIRE Get Discovery Service Metadata response contain the list of supported languages. More specifically examine whether:
1. the INSPIRE Get Discovery Service Metadata response (i.e. the GetCapabilities document) consists of exactly one element [DefaultLanguage](#DefaultLanguage) indicating the service default language, and
2. zero or more [SupportedLanguage](#SupportedLanguage) to indicate all additional supported languages.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 23
* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 28
* [IR NS](README.md#ref_IR_NS), Annex II, Part B, section 2.2.3

**Test type**: Automated

**Notes**


## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="DefaultLanguage"></a> DefaultLanguage | ./inspire_common:SupportedLanguages/inspire_common:DefaultLanguage
<a name="SupportedLanguage"></a> SupportedLanguage | ./inspire_common:SupportedLanguages/inspire_common:SupportedLanguage
