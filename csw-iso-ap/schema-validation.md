# Schema validation

**Purpose**: The operation for implementing INSPIRE Get Discovery Service Metadata operation is the GetCapabilities operation. The response must be valid against the XML Schema specified by INSPIRE.

**Prerequisites**

**Test method**

* Access the service metadata using a GetCapabilities request without using the `LANGUAGE parameter. Check, if the [INSPIRE Discovery Service 1.0 schema](http://inspire.ec.europa.eu/schemas/inspire_ds/1.0/inspire_ds.xsd) and the [CSW 2.0.2 schema](http://schemas.opengis.net/csw/2.0.2/csw.`xsd) are referenced in the service capabilities. Then check that the GetCapabilities request result validates against these schemas.

**Reference (s)**: 

* [TG DS](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DS), Chapter 4.5.1, Implementation Requirement 29 and Annex A

**Test type**

Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                     |  XPath expression
------------------------------------------------ | ---------------------------------------------------------------
Capabilities <a name="Capabilities"></a>   | /csw:Capabilities/@xsi:schemaLocation
