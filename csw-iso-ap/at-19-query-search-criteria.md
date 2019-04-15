# Query Search Criteria

**Purpose**: Test that the Discover Metadata service supports queryables.

**Prerequisites**

**Test method**

* Send a GetCapabilities request.

* Check that the following values in [SupportedISOQueryables](#supportedISOQueryables) exists:

    * Keyword, Topic category, Spatial data service type, Lineage, Spatial resolution, Specification (composed of SpecificationTitle, SpecificationDate, SpecificationDateType), Degree, Geographic bounding box, Conditions applying to access and use, Limitations on public access (composed of AccessConstraints, OtherConstraints, Classification), Responsible party, Responsible party role, Resource Title, Resource Abstract, Resource Type, Unique resource identifier, Temporal Reference

* If any of the checks or validations fails, the test fails.

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 19

**Test type**: Automated

**Notes**

The queryables that shall be supported are shown in [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC) table 4.

**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
| SupportedISOQueryables <a name="supportedISOQueryables"></a>   | /csw:Capabilities/ows:OperationsMetadata/ows:Operation[@name="GetRecords"]/ows:Constraint[@name="SupportedISOQueryables"]
