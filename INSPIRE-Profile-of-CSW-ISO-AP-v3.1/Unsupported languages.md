# Unsupported languages

**Purpose**:Verification whether the response of the INSPIRE Discovery Service provides its response in the default language in the cases where a client requested an unsupported language, or the language parameter is absent in the request.

**Prerequisites**


**Test method**

When the language requested by a client is either not provided or not in the list of [SupportedLanguages](#SupportedLanguages), test whether the [ResponseLanguage](#ResponseLanguage) is equal to the [DefaultLanguage](#DefaultLanguage).

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 26

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="SupportedLanguages"></a> SupportedLanguages  | ./inspire_common:SupportedLanguages
<a name="ResponseLanguage"></a> ResponseLanguage  | ./inspire_common:ResponseLanguage
<a name="DefaultLanguage"></a> DefaultLanguage  | ./inspire_common:SupportedLanguages/inspire_common:DefaultLanguage
