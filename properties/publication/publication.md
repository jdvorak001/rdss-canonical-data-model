# Publication

* [`publicationUUID`](#publicationuuid)
* [`publicationFreeToRead`](#publicationfreetoread)
* [`publicationLicenseRef`](#publicationlicenseref)	
* [`publicationIdentifier`](#publicationidentifier)
* [`publicationCoverage`](https://github.com/JiscRDSS/Metadata/blob/master/properties/Dataset/Coverage/coverage.md)
* [`publicationDescription`](https://github.com/JiscRDSS/rdss-canonical-data-model/blob/master/properties/Dataset/Description/description.md)
* [`publicationFile`](https://github.com/JiscRDSS/Metadata/blob/master/properties/File/file.md)
* [`publicationLanguage`](https://github.com/JiscRDSS/rdss-canonical-data-model/blob/master/properties/Dataset/Language.md)
* [`publicationResourceType`](https://github.com/JiscRDSS/rdss-canonical-data-model/blob/master/properties/publication/publication%20resource%20type.md)
* [`publicationTitle`](https://github.com/JiscRDSS/rdss-canonical-data-model/blob/master/properties/Dataset/Title/title.md)
* [`publicationSubject`](https://github.com/JiscRDSS/rdss-canonical-data-model/blob/master/properties/Dataset/Subject/subject.md)
* [`publicationDate`](https://github.com/JiscRDSS/rdss-canonical-data-model/blob/master/properties/Dataset/Date.md)
* [`publicationAPC`](#publicationapc-1)
* [`publicationRelatedIdentifier`](https://github.com/JiscRDSS/rdss-canonical-data-model/blob/master/properties/identifier.md)
* [`publicationVersion`](https://github.com/JiscRDSS/Metadata/blob/master/properties/publication/publication%20version.md)
* [`publicationRights`](https://github.com/JiscRDSS/rdss-canonical-data-model/blob/master/properties/Rights/rights.md)
* [`publicationPerson`](https://github.com/JiscRDSS/rdss-canonical-data-model/blob/master/properties/Agent/Person/Person.md)
* [`publicationOrganisation`](https://github.com/JiscRDSS/rdss-canonical-data-model/blob/master/properties/Agent/Organisation/organisation.md)
* [`publicationProject`](https://github.com/JiscRDSS/rdss-canonical-data-model/blob/master/properties/Project/project.md)
* [`publicationAdditionalMetadata`](#publicationadditionalmetadata-1)

-------------------------------

## `publicationUUID`
#### Description
Unique identifier for the publication within the data model
#### Derivation
system
#### Mapping
None
#### Obligation	
Mandatory
#### Occurence	
Once
#### Content 
String
#### Example
0e7e9878-aae1-4dad-8ef6-9c74542cd7e1
--------------------------------

## `publicationFreeToRead`  

#### Description
This is defined in the NISO Open Access Metadata and Indicators. This element does not take a value - the semantics of ali:free_to_read are conveyed by its presence or absence. This element may be modified by two optional attributes:
start_date
end_date
Each of these attributes, if present, takes a date value which MUST be encoded using [ISO 8601](http://www.iso.org/iso/home/standards/iso8601.htm  (post–2004 versions) which follows the following format: YYYY-MM-DD. 

#### Derivation
RIOXX ([http://www.rioxx.net/profiles/v2-0-final/](http://www.rioxx.net/profiles/v2-0-final/)

#### Mapping
ali:free_to_read

#### Obligation	
Optional

#### Occurence	
Non-repeatable

#### Content 
string

#### Example
ali:free_to_read start_date="2013-03-28" end_date="2014-04-30"
ali:free_to_read start_date="2013-03-28"
ali:free_to_read
The absence of a start_date attribute implies that the meaning conveyed by the ali:free_to_read element is current and immediate, unless an end_date attribute which is a date in the subjective past, is present in the element.
--------------------------------

## `license ref`	

#### Description
This is defined in the NISO Open Access Metadata and Indicators. This element MUST take an HTTP URI for its value. This HTTP URI MUST point to a resource which expresses the license terms specifying how the resource may be used.

This element MUST include the attribute:

start_date
This attribute takes a date value which MUST be encoded using ISO 8601 (post–2004 versions) which follows the following format: YYYY-MM-DD.

#### Derivation
RIOXX

#### Mapping
ali:license_ref	

#### Obligation	
Mandatory

#### Occurence	
Repeatable

#### Content 
http:URI

#### Example

ali:license_ref start_date="2015-02-17">http://creativecommons.org/licenses/by/4.0</ali:license_ref
This approach allows the expression of 'embargoes', where a particular license takes effect at a date in the subjective future.

In the absence of any other license, the copyright holder reserves all rights automatically. As a convenience, RIOXX provides two URLs which may be used to explicitly convey this state:

http://www.rioxx.net/licenses/all-rights-reserved
http://www.rioxx.net/licenses/under-embargo-all-rights-reserved
--------------------------------

## `publicationAPC`

#### Description
This property expresses whether or not the resource has an associated Article Processing Charge

##### Derivation
rioxxterms:apc

#### Mapping

#### Obligation	
Mandatory

#### Occurence	
Non-repeatable

#### Content 

Controlled Vocabulary

Term | Source
-----|-------
paid | RIOXX
partiallyWaived | RIOXX
fullyWaived | RIOXX
notCharged | RIOXX
notRequired | RIOXX
unknown | RIOXX

--------------------------------

## `publicationAdditionalMetadata`

#### Description
Additional metadata about the object that is not recorded elsewhere. Can include technical metadata about description and standards.
#### Derivation
Preservica 
#### Mapping
None
#### Obligation	
Recommended
#### Occurence	
Non-repeatable
#### Content 
String
#### Example
