# Additional search attributes

**Purpose**: Verification whether the additional search attributes are advertised as the results of a Service metadata response to a discover metadata request.

**Prerequisites**

**Test method**

Examine whether the additional search attributes are advertised as a result of a Service metadata response (i.e. a capabilities document) to a Discover Metadata request; i.e. whether the ```OperationsMetadata``` contains the list of search attributes ([AdditionalQueryables](#AdditionalQueryables)).

**Reference(s)**

* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Chapter 4.2, Implementation Requirements 5, 22

**Test type**: Automated

**Notes**

The XML excerpt of a capabilities document may be found in section 4.4.3.

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="AdditionalQueryables"></a>AdditionalQueryables | /csw:Capabilities/ows:OperationsMetadata/ows:Operation[@name="GetRecords"]/ows:Constraint[@name="AdditionalQueryables"]
