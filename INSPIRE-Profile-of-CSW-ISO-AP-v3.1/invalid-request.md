# Invalid request

**Purpose**: Verification whether the response in a form of an exception to an invalid Discover Metadata request containing a language specific parameter is provided in the default or in a requested and supported language.

**Prerequisites**

* [Supported languages](supported-languages.md)

**Test method**

Examine whether an invalid Discover Metadata request (from an ISO Metadata Application Profile of the OGC Catalogue Service Specification in version 2.0.2 point of view) containing a language specific parameter results in an exception that is responded in the default or in a requested and supported language. More specifically, the following tests will be performed:

1. Issue an invalid request using a valid but unsupported language: the response should be in the [DefaultLanguage](#DefaultLanguage).
2. Issue an invalid request asking explicitly for the [DefaultLanguage](#DefaultLanguage): the response should be in the default language
3. Conditional on the system supporting more than one language, issue an invalid request using a supported language other than the default: the response should be in that language.

The use of a valid language specific filter itself shall not raise an exception, even if the requested language is not supported.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Chapter 4.5.2, Implementation Requirement 32

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="DefaultLanguage"></a>Defaultlanguage | /inspire_common:SupportedLanguages/inspire_common:DefaultLanguage
