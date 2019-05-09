# Query Parameters Advertised

**Purpose**: Test that all ISO and additional queryables are advertised in the capabilities document.

**Prerequisites**

**Test method**

* Send a GetCapabilities request.

* Check that the following [SupportedISOQueryablesValue](#supportedISOQueryablesValue) exists:

    * 'Subject', 'TopicCategory', 'ServiceType', 'SpatialResolution', 'BoundingBox', 'OrganisationName', 'Title', 'Abstract', 'Type', 'ResourceIdentifier', 'TemporalExtent', 'PublicationDate', 'RevisionDate' and 'CreationDate'.

* Check that the following [AdditionalQueryablesValue](#additionalQueryablesValue) exists:

    * 'Degree', 'Specification', 'LimitationsOnPublicAccess', 'ConditionApplyingToAccessAndUse', 'Lineage', 'ResponsiblePartyRole',	'SpecificationTitle', 'SpecificationDate', 'SpecificationDateType', 'AccessConstraints', 'OtherConstraints' and 'Classification'.

* If any of the checks or validations fails, the test fails.

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 22

**Test type**: Automated

**Notes**

The ISO queryables that shall be supported are shown in [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC) table 4.

The Additional queryables that shall be supported are shown in [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC) table 5, 6 and 7.

**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
| SupportedISOQueryablesValue <a name="supportedISOQueryablesValue"></a>   | /csw:Capabilities/ows:OperationsMetadata/ows:Operation[@name="GetRecords"]/ows:Constraint[@name="SupportedISOQueryables"]/ows:Value
| AdditionalQueryablesValue <a name="additionalQueryablesValue"></a>   | /csw:Capabilities/ows:OperationsMetadata/ows:Operation[@name="GetRecords"]/ows:Constraint[@name="AdditionalQueryables"]/ows:Value
