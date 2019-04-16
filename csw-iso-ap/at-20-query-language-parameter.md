# Query Language Parameter

**Purpose**: Test that the Discover Metadata service accepts the language parameter.

**Prerequisites**

**Test method**

* Send a GetCapabilities request.

* Check that the following 'Language' value exists in [SupportedISOQueryables](#supportedISOQueryables).

* Send a GetRecords request with a language restriction.

    * Check that the response is valid with the restriction.

* If any of the checks or validations fails, the test fails.

**Reference(s)**:
* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), Implementation Requirement 20

**Test type**: Automated / Manual

**Notes**


**Contextual XPath references**

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
| SupportedISOQueryables <a name="supportedISOQueryables"></a>   | /csw:Capabilities/ows:OperationsMetadata/ows:Operation[@name="GetRecords"]/ows:Constraint[@name="SupportedISOQueryables"]
