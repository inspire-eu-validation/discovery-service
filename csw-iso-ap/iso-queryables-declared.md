# ISO queryables advertised

**Purpose**: Verification whether the Get Discovery Service Metadata operation supports the advertisement of all supported ISO queryables.

**Prerequisites**

**Test method**

Examine whether the Get Discovery Service Metadata operation supports the advertisement of all [SupportedISOQueryables](#SupportedISOQueryables) as defined by Table 4 of [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC)

**Reference(s)**

* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Chapter 4.4.3, Implementation Requirement 22

**Test type**: Automated

**Notes**

The test ensures that the searching parameters defined in the A.3.1 INSPIRE search attributes test are properly advertised in the Get Discovery Service Metadata response. The list of SupportedISOQueryables and AdditionalQueryables may be extended by the service provider which still means passing this test.

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="SupportedISOQueryables"></a>SupportedISOQueryables | /csw:Capabilities/ows:OperationsMetadata/ows:Operation[@name="GetRecords"]/ows:Constraint[@name="SupportedISOQueryables"]/ows:Value
