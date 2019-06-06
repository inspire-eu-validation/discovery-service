# Extended Capabilities

**Purpose**: Test that the service provides the INSPIRE extended metadata.

**Prerequisites**

**Test method**

* Send a GetCapabilities request.

* Check that the [ExtendedCapabilities](#extendedCapabilities) exists. If it does,

  * If [Metadata Url](#metadataUrl) child node exists,

    * Check that [Metadata Url](#metadataUrl) is a valid URL.
  
  * Else

    * Check that the [ExtendedCapabilities](#extendedCapabilities) section contains all the mandatory INSPIRE metadata for the Discovery Service according with table 2 and table 3 of [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC).

* If any of the checks or validations fails, the test fails.

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 7

**Test type**: Automated

**Notes**

The multiplicity of [ExtendedCapabilities](#extendedCapabilities) is 1.

The multiplicity of [Metadata Url](#metadataUrl) is 0 or 1.

**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
| ExtendedCapabilities <a name="extendedCapabilities"></a>   | /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities |
| Metadata Url <a name="metadataUrl"></a> | /csw:Capabilities/ows:OperationsMetadata/inspire_ds:ExtendedCapabilities/inspire_common:MetadataUrl/inspire_common:URL |
