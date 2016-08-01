# Discovery service metadata: scenario 1

**Purpose**: Verification whether the discovery service metadata is included in the GetCapabilities response. This test covers scenario 1 (metadata referenced from the Capabilities document).

**Prerequisites**

**Test method**

* If a [MetadataUrl](#MetadataUrl) element exists in the [ExtendedCapabilities](#ExtendedCapabilities) section, test whether the referenced resource is a conformant [ISO 19115/19119 profile](http://inspire.ec.europa.eu/id/ats/metadata/1.3/iso-19115-19119) metadata record.

**Reference(s)**

 * [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Chapter 4.3.1.2, Implementation Requirement 7

**Test type**: Automated

**Notes**

The Technical Guidance offers two implementation possibilities for the requirement originating from the Commission Regulation No 976/2009

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
ExtendedCapabilities <a name="ExtendedCapabilities"></a> | /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities
MetadataUrl <a name="MetadataUrl"></a>   | /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities/inspire_common:MetadataUrl
