# Query Additional Parameters

**Purpose**: Test that the Discover Metadata service supports additional queryables.

**Prerequisites**

**Test method**

* Send a GetCapabilities request.

* Check that the following values in [AdditionalQueryables](#additionalQueryables) exists:

    * Degree, SpecificationTitle, SpecificationDate, SpecificationDateType, AccessConstraints, OtherConstraints, Classification, ConditionApplyingToAccessAndUse, Lineage, ResponsiblePartyRole

* If any of the checks or validations fails, the test fails.

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 21

**Test type**: Automated

**Notes**

The queryables that shall be supported are shown in [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC) table 5, 6 and 7.

**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
| AdditionalQueryables <a name="additionalQueryables"></a>   | /csw:Capabilities/ows:OperationsMetadata/ows:Operation[@name="GetRecords"]/ows:Constraint[@name="AdditionalQueryables"]
