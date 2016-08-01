# QoS Performance

**Purpose**: Verification whether the response time for sending the initial response to a Discovery service request is maximum 3 seconds in normal situation.

**Prerequisites**

**Test method**

Examine whether the response time for sending the initial response to a Discovery service request is maximum 3 seconds in normal situation. Normal situation represents periods out of peak load. It is set at 90% of the time.

**Reference(s)**

* [TG DISC](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#ref_TG_DISC), section 5;

**Test type**: Automated

**Notes**

Technical Guidance recommends that performance shall be measured using the Discovery Metadata operation (with filter PropertyName=AnyText, Literal=dataset, and with varying BBOX requests), however it shall be applicable to all operations according to the Commission Regulation No 976/2009. Such simplification of the test originates from the fact that the Discovery Metadata operation is the most complex one, i.e. its processing is the most demanding from the computational point of view.


## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/discovery-service/3.1/csw-iso-ap/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
