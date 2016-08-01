# Language selection capabilities

**Purpose**: The user must be able to select one of the supported languages.
This language selection must be reflected in the provided capabilities document.

**Prerequisites**

* [Schema validation](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/schema-validation)
* [Check supported and response languages node](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/supported-and-response-languages-node)

**Test method**

* Let the value of [GetCapabilities OnlineResource](#getcap-href) be ```getcapabilities-url```.
* For each [SupportedLanguage codes](#supported-languages) as ```lang-code```:
  * Create a GetCapabilities HTTP request by adding the parameters ```SERVICE=CSW```, ```REQUEST=GetCapabilities```, ```ACCEPTVERSIONS=2.0.2``` and ```LANGUAGE=``` + ```lang-code``` to the ```getcapabilities-url```
  * Execute the request. 
  * Check that the [INSPIRE Discovery Service 1.0 schema](http://inspire.ec.europa.eu/schemas/inspire_ds/1.0/inspire_ds.xsd) and the [CSW 2.0.2 schema](http://schemas.opengis.net/csw/2.0.2/csw.xsd) are referenced in the service capabilities. Then check that the GetCapabilities request result validates against these schemas.
  * Check that there is a [SupportedLanguages](#SupportedLanguages) node and a [ResponseLanguage](ResponseLanguage) node.
  * Check that the [ResponseLanguage code](#response-language) equals the ```lang-code```. If it does not, fail the test for this language.
  * Otherwise fail the test.
* Repeat the previous test step with an unsupported `LANGUAGE` parameter (e.g. "xxx" as this is not one of the valid language codes). In this case, check that the [ResponseLanguage code](#response-language) equals the [DefaultLanguage code](#default-language). If it does not, fail the test.
* Repeat the previous test step without the `LANGUAGE` parameter. In this case, check that the [ResponseLanguage code](#response-language) equals the [DefaultLanguage code](#default-language). If it does not, fail the test.
* If the test for any of the languages failed, fail the test. Otherwise pass the test.

**Reference(s)**:

* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Chapter 4.5.1, Implementation Requirements 26, 27, 28, 29

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
DefaultLanguage code <a name="default-language"></a>   | /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities[1]/inspire_common:SupportedLanguages/inspire_common:DefaultLanguage/inspire_common:Language
SupportedLanguage codes <a name="supported-languages"></a>   | /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities[1]/inspire_common:SupportedLanguages/*[self::inspire_common:SupportedLanguage or self::inspire_common:DefaultLanguage]/inspire_common:Language
ResponseLanguage code <a name="response-language"></a>   | /csw:Capabilities/ows:OperationsMetadatainspire_ds:ExtendedCapabilities[1]/inspire_common:ResponseLanguage/inspire_common:Language
GetCapabilities OnlineResource <a name="getcap-href"></a> | /csw:Capabilities/ows:OperationsMetadata/ows:Operation[@name="GetCapabilities"]/ows:DCP/ows:HTTP/ows:Get/@xlink:href
