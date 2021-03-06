# Identifier




## identifierValue 1 
# identifierValue

#### Description
Value of identifier.

#### Derivation
Datacite

#### Mapping

#### Content
String

#### Example
10013/epic.10033

## IdentifierType 1 
# identifierType

#### Description
The type of identifier.

#### Derivation
Datacite v.4

#### Mapping

#### Content

Controlled Vocabulary

Term|Origin
----|------
ARK|Datacite
arXiv|Datacite
bibcode|Datacite
DOI|Datacite
EAN13|Datacite
EISSN|Datacite
Handle|Datacite
IGSN|Datacite
ISBN|Datacite
ISSN|Datacite
ISTC|Datacite
LISSN|Datacite
LSID|Datacite
PMID|Datacite
PUID|PREMIS
PURL|Datacite
UPC|Datacite
URL|Datacite
URN|Datacite

## relationType 0..1 
# relationType

#### Description
Description of the relationship between entities using these identifiers.

#### Derivation
Datacite / Crossref

#### Mapping

#### Obligation	
Recommended (where a relationship exists)

#### Occurence	
Non-repeatable

#### Content
Controlled vocabulary

Term|Origin
----|------
isCitedBy|Datacite
cites|Datacite
isSupplementTo|Datacite
isSupplementedBy|Datacite
isContinuedBy|Datacite
continues|Datacite
hasMetadata|Datacite
isMetadataFor|Datacite
isNewVersionOf|Datacite
isPreviousVersionOf|Datacite
isPartOf|Datacite
hasPart|Datacite
isReferencedBy|Datacite
references|Datacite
isDocumentedBy|Datacite
documents|Datacite
isCompiledBy|Datacite
compiles|Datacite
isVariantFormOf|Datacite
isOriginalFormOf|Datacite
isIdenticalTo|Datacite
isReviewedBy|Datacite
reviews|Datacite
isDerivedFrom|Datacite
isSourceOf|Datacite
isCommentOn|Crossref
hasComment|Crossref
isReplyTo|Crossref
hasReply|Crossref
basedOnData|Crossref
hasRelatedMaterial||Crossref
isBasedOn|Crossref
isBasisFor|Crossref
requires|Crossref
isRequiredBy|Crossref
hasParent|Preservica
isParentOf|Preservica
