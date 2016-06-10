# A.1.5 ISO 639 codes

**Purpose**: Verification whether the INSPIRE Discovery Service whether the Discover Metadata request parameter “language” accepts values that are based on ISO 639-2/B alpha 3 codes.

**Prerequisites**

**Test method**

Examine whether the Discovery Service Metadata (GetCapabilities) request supports the parameter 'LANGUAGE'.

Then, examine whether the values in the list of [SupportedLanguages](#SupportedLanguages) of the INSPIRE Discovery Service are based on ISO 639-2/B alpha 3 codes. In other words, whether the INSPIRE Discovery Service supports at least one of those language codes: eng, bul, cze, dan, est, fin, fre, hrv, dut, gle, ice, ita, lit, lav, hun, mlt, nor, ger, pol, por, rum, roh, gre, slo, slv, spa, swe.

**Reference(s)**

* [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 25

See note 1

**Test type**: Automated or Manual

**Notes**
This test may be applied at least for the Get Discovery Service Metadata and Discover Metadata operations since “language” parameter is defined in the Commission Regulation No 976/2009 only for those two operations. The list of codes in the Technical Guidelines for INSPIRE metadata and Technical Guidance for INSPIRE Discovery Services does not comply with each. The Technical Guidance for INSPIRE Discovery Services also provides codes for the EFTA countries while Technical Guidelines for INSPIRE metadata provides codes only for the EU Member States.

Note 1: The ISO 639-2 values are required by the Commission Regulation No 1205/2008, which is not directly related to the “language” parameter in the INSPIRE Discovery Service.


## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="SupportedLanguages"></a> SupportedLanguages  | ./inspire_common:SupportedLanguages
