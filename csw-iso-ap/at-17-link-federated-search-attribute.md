# Link Federated Search Attribute

**Purpose**: Test the use of parameter indicating a distributed search.

**Prerequisites**

**Test method**


**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 17

**Test type**: None

**Notes**

Limitations: The requirement 17 of [TG DISC]() stands that to indicate that the query should be distributed the “DistributedSearch” parameter of a GetRecords
request shall be used with the “hopCount” attribute set always equal to “2” to avoid circular searches. Therefore, this requirement is intended for clients and it cannot be tested on the service itself.

**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------

