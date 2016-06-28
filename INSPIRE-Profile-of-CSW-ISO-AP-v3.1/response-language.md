# Response language

**Purpose**: Verification whether the Get Discovery Service Metadata response (i.e. the GetCapabilities document) contains an appropriate response language.

**Prerequisites**

* [XML schema](xml-schema.md)

**Test method**

Examine whether:

1. The language requested by a client is contained in the list of supported languages: in such cases the requested language shall correspond to the language used in the Get Discovery Service Metadata response (i.e. the GetCapabilities document) as defined in [ResponseLanguage](#ResponseLanguage);
2. The language requested by a client is NOT contained in the list of supported languages: in such cases the Get Discovery Service Metadata response (i.e. the getcapabilities document) is provided in the service default language as defined in [defaultlanguage](#defaultlanguage). this test can be performed by the test case for [unsupported languages](unsupported-languages.md)

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Chapter 4.5.1, Implementation Requirement 27


**Test type**: Automated

**Notes**


## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="ResponseLanguage"></a>ResponseLanguage | /inspire_common:ResponseLanguage/inspire_common:Language
<a name="DefaultLanguage"></a>Defaultlanguage | /inspire_common:SupportedLanguages/inspire_common:DefaultLanguage
