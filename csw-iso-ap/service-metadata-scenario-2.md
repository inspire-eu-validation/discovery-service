# Discovery service metadata: scenario 2

**Purpose**: Verification whether the Get Discovery Service Metadata response provides a document that is in conformance with the requirements for INSPIRE service metadata. This test covers scenario 2 (metadata in the Capabilities document).

**Prerequisites**

**Test method**

* If no [MetadataUrl](#MetadataUrl) element exists in the [ExtendedCapabilities](#ExtendedCapabilities) section:
  * Test whether all 13 mandatory elements given in Table 3 of [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC) are non-empty strings
  * If the type of the element is "URL", retrieve the resource using the URL and check that the HTTP status code is 200. 
  * If the element is "Date", check that are formatted correctly as YYYY-MM-DD.

**Reference(s)**

* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Chapter 4.3.1.3, Implementation Requirements 7, 8

**Test type**: Automated

**Notes**



## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
ExtendedCapabilities <a name="ExtendedCapabilities"></a> | /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities
MetadataUrl <a name="MetadataUrl"></a>   | /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities/inspire_common:MetadataUrl
