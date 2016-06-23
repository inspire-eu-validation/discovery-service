# A.2.9 Response language

**Purpose**: Verification whether the Get Discovery Service Metadata response (i.e. the GetCapabilities document) contains an appropriate response language.

**Prerequisites**

* [XML schema](https://github.com/inspire-eu-validation/ats-discovery-service/blob/master/A.02.11.xml.schema.md)

**Test method**

Examine whether:

1. The language requested by a client is contained in the list of supported languages: in such cases the requested language shall correspond to the language used in the Get Discovery Service Metadata response (i.e. the GetCapabilities document) as defined in [ResponseLanguage](#ResponseLanguage);
2. The language requested by a client is NOT contained in the list of supported languages: in such cases the Get Discovery Service Metadata response (i.e. the GetCapabilities document) is provided in the service default language as defined in [DefaultLanguage](#DefaultLanguage). This test can be performed by the test case for [Unsupported Languages](https://github.com/inspire-eu-validation/ats-discovery-service/blob/master/A.01.06.unsupported.languages.md)

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 27
* [IR NS](README.md#ref_IR_NS), Annex II, Part B, section 2.2.3

**Test type**: Automated

**Notes**


## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="ResponseLanguage"></a>ResponseLanguage | /inspire_common:ResponseLanguage/inspire_common:Language
<a name="DefaultLanguage"></a>Defaultlanguage | /inspire_common:SupportedLanguages/inspire_common:DefaultLanguage
