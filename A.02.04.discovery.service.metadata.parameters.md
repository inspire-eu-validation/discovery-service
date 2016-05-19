# A.2.4 Discovery Service metadata parameters

**Purpose**: Verification whether the discovery service metadata parameters are included in the GetCapabilities response.

**Prerequisites**

**Test method**

Examine whether the Get Discovery Service Metadata response of the Discovery service contains:
1. the tag ```MetadataURL``` which points to an INSPIRE compliant ISO metadata document;
AND/OR
2. the tag ```ExtendedCapabilities``` containing INSPIRE compliant metadata.

If the ```ExtendedCapabilities``` tag is present, the test case should return that 'scenario 2' is being used. If only a ```MetadataURL``` URL is provided, the test case should return 'scenario 1'.

**Reference(s)**

 * [TG DISC](README.md#ref_TG_DISC), Implementation Requirement 7
 * [IR NS](README.md#ref_IR_NS), Annex II, Part B, section 3.2.1

**Test type**: Automated

**Notes**

The Technical Guidance offers two implementation possibilities for the requirement originating from the Commission Regulation No 976/2009

## Contextual XPath references

The namespace prefixes used as described in [README.md](README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
<a name="#MetadataURL"></a> MetadataURL |  /xs:complexType/xs:choice/xs:sequence/xs:element[@name="MetadataUrl"]
