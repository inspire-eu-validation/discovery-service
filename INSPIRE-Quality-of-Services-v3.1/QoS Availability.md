# QoS Availability

**Purpose**: Verification whether the probability of a Discovery Service to be available is 99% of the time.

**Prerequisites**

**Test method**

Examine whether the Discovery Service has a maximum unplanned downtime less than 1% of time. Minimum 10 reference requests per hour shall be issued to the service continuously during its lifetime. Aggregation of such measurements shall be based on a time frame of one year. Periods of planned downtime e.g. because of system maintenance, are not included in the measure. Downtime is considered planned when notified to the community well in advance (minimum 1 week), e.g. via notifications to registered users or on portals.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), section 5;

**Test type**: Automated

**Notes**

 Note 1: The Technical Guidance for INSPIRE Discovery Service counts the 99% uptime differently from the way it is commonly applied for information systems. For example, for 99% availability, INSPIRE specifies maximum downtimes of 1.7 hours a week, 7.27 hours per month, and 3.63 days per year. On the other hand, 99% availability for information systems usually allows 1.68 hours a week, 7.20 hours per month, and 3.65 days per year.

Note 2: Maybe this kind of availability monitoring should not be done using the testing platform, where almost all the the tests are designed to be run on demand or possibly as batch jobs. Implementing this test requires a system with continuous monitoring availability ("Minimum of 10 reference requests per hour shall be issued to the service continuously during its lifetime").

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
