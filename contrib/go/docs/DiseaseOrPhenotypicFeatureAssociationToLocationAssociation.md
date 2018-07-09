# Class: disease or phenotypic feature association to location association


An association between either a disease or a phenotypic feature and an anatomical entity, where the disease/feature manifests in that site.

URI: [http://bioentity.io/vocab/DiseaseOrPhenotypicFeatureAssociationToLocationAssociation](http://bioentity.io/vocab/DiseaseOrPhenotypicFeatureAssociationToLocationAssociation)

![img](http://yuml.me/diagram/nofunky;dir:TB/class/\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation|id(i):identifier_type%20%3F;name(i):label_type%20%3F;category(i):label_type%20%3F;node_property(i):string%20%3F;iri(i):iri_type%20%3F;full_name(i):label_type%20%3F;description(i):narrative_text%20%3F;systematic_synonym(i):label_type%20%3F;title(i):label_type%20%3F;subject_taxon_closure_label(i):string%20*;object_taxon_closure_label(i):string%20*;has_evidence(i):evidence_instance%20%3F;negated(i):boolean%20%3F;association_slot(i):string%20%3F]-%20subject(i)>\[DiseaseOrPhenotypicFeature],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20provided%20by(i)%20%3F>\[Provider],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20publications(i)%20*>\[Publication],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20qualifiers(i)%20*>\[OntologyClass],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20relation(i)>\[RelationshipType],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20association%20type(i)%20%3F>\[OntologyClass],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20has%20evidence%20type(i)%20%3F>\[EvidenceType],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20object%20extensions(i)%20*>\[PropertyValuePair],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20object%20taxon%20closure(i)%20*>\[OntologyClass],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20object%20taxon(i)%20%3F>\[OrganismTaxon],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20subject%20taxon%20closure(i)%20*>\[OntologyClass],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20subject%20taxon(i)%20%3F>\[OrganismTaxon],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20related%20to(i)%20%3F>\[NamedThing],%20\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation]-%20object>\[AnatomicalEntity],%20\[DiseaseOrPhenotypicFeatureAssociationToThingAssociation]^-\[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation])
## Mappings

 * [NCIT:R100](http://purl.obolibrary.org/obo/NCIT_R100)
## Inheritance

 *  is_a: [DiseaseOrPhenotypicFeatureAssociationToThingAssociation](DiseaseOrPhenotypicFeatureAssociationToThingAssociation.md)
## Children

## Used in

## Fields

 * _[disease or phenotypic feature association to location association.object](disease_or_phenotypic_feature_association_to_location_association_object.md)_
    * _anatomical entity in which the disease or feature is found_
    * range: [AnatomicalEntity](AnatomicalEntity.md) [required]
    * __Local__
 * _[association slot](association_slot.md)_
    * _any slot that relates an association to another entity_
    * range: **string**
    * inherited from: [Association](Association.md)
 * _[association type](association_type.md)_
    * _connects an association to the type of association (e.g. gene to phenotype)_
    * range: [OntologyClass](OntologyClass.md)
    * inherited from: [Association](Association.md)
 * _[category](category.md) *subsets*: (translator_minimal)_
    * _Name of the high level ontology class in which this entity is categorized. Corresponds to the label for the biolink entity type class. In a neo4j database this MAY correspond to the neo4j label tag_
    * range: [LabelType](LabelType.md)
    * inherited from: [NamedThing](NamedThing.md)
 * _[description](description.md) *subsets*: (translator_minimal)_
    * _a human-readable description of a thing_
    * range: [NarrativeText](NarrativeText.md)
    * inherited from: [NamedThing](NamedThing.md)
 * _[disease or phenotypic feature association to thing association.subject](disease_or_phenotypic_feature_association_to_thing_association_subject.md)_
    * _disease or phenotype_
    * range: [DiseaseOrPhenotypicFeature](DiseaseOrPhenotypicFeature.md) [required]
    * inherited from: [DiseaseOrPhenotypicFeatureAssociationToThingAssociation](DiseaseOrPhenotypicFeatureAssociationToThingAssociation.md)
 * _[full name](full_name.md)_
    * _a long-form human readable name for a thing_
    * range: [LabelType](LabelType.md)
    * inherited from: [NamedThing](NamedThing.md)
 * _[has evidence](has_evidence.md)_
    * _connects an association to an instance of supporting evidence_
    * range: [EvidenceInstance](EvidenceInstance.md)
    * inherited from: [ExtensionsAndEvidenceAssociationMixin](ExtensionsAndEvidenceAssociationMixin.md)
 * _[has evidence type](has_evidence_type.md)_
    * _connects an association to the class of evidence used_
    * range: [EvidenceType](EvidenceType.md)
    * inherited from: [ExtensionsAndEvidenceAssociationMixin](ExtensionsAndEvidenceAssociationMixin.md)
 * _[id](id.md) *subsets*: (translator_minimal)_
    * _A unique identifier for a thing. Must be either a CURIE shorthand for a URI or a complete URI_
    * range: [IdentifierType](IdentifierType.md)
    * inherited from: [NamedThing](NamedThing.md)
 * _[iri](iri.md) *subsets*: (translator_minimal)_
    * _An IRI for the node. This is determined by the id using expansion rules._
    * range: [IriType](IriType.md)
    * inherited from: [NamedThing](NamedThing.md)
 * _[name](name.md) *subsets*: (translator_minimal)_
    * _A human-readable name for a thing_
    * range: [LabelType](LabelType.md)
    * inherited from: [NamedThing](NamedThing.md)
 * _[negated](negated.md)_
    * _if set to true, then the association is negated i.e. is not true_
    * range: **boolean**
    * inherited from: [Association](Association.md)
 * _[node property](node_property.md)_
    * _A grouping for any property that holds between a node and a value_
    * range: **string**
    * inherited from: [NamedThing](NamedThing.md)
 * _[object extensions](object_extensions.md)_
    * _Additional relationships that are true of the object in the context of the association. For example, if the object is an anatomical term in an expression association, the object extensions may include part-of links_
    * range: [PropertyValuePair](PropertyValuePair.md)*
    * inherited from: [ExtensionsAndEvidenceAssociationMixin](ExtensionsAndEvidenceAssociationMixin.md)
 * _[object taxon](object_taxon.md)_
    * _the taxonomic class of the entity in the object slot_
    * range: [OrganismTaxon](OrganismTaxon.md)
    * inherited from: [TaxonClosureMixin](TaxonClosureMixin.md)
 * _[object taxon closure](object_taxon_closure.md)_
    * _The taxon class or ancestor class for the object_
    * range: [OntologyClass](OntologyClass.md)*
    * inherited from: [TaxonClosureMixin](TaxonClosureMixin.md)
 * _[object taxon closure label](object_taxon_closure_label.md)_
    * _The label for the taxon class or ancestor class for the object_
    * range: **string***
    * inherited from: [TaxonClosureMixin](TaxonClosureMixin.md)
 * _[object taxon label](object_taxon_label.md)_
    * range: label
    * inherited from: [TaxonClosureMixin](TaxonClosureMixin.md)
 * _[provided by](provided_by.md)_
    * _connects an association to the agent (person, organization or group) that provided it_
    * range: [Provider](Provider.md)
    * inherited from: [Association](Association.md)
 * _[publications](publications.md)_
    * _connects an association to publications supporting the association_
    * range: [Publication](Publication.md)*
    * inherited from: [Association](Association.md)
 * _[qualifiers](qualifiers.md)_
    * _connects an association to qualifiers that modify or qualify the meaning of that association_
    * range: [OntologyClass](OntologyClass.md)*
    * inherited from: [Association](Association.md)
 * _[related to](related_to.md)_
    * _A grouping for any relationship type that holds between any two things_
    * range: [NamedThing](NamedThing.md)
    * inherited from: [NamedThing](NamedThing.md)
 * _[relation](relation.md)_
    * _the relationship type by which a subject is connected to an object in an association_
    * range: [RelationshipType](RelationshipType.md) [required]
    * inherited from: [Association](Association.md)
 * _[subject taxon](subject_taxon.md)_
    * _the taxonomic class of the entity in the object slot_
    * range: [OrganismTaxon](OrganismTaxon.md)
    * inherited from: [TaxonClosureMixin](TaxonClosureMixin.md)
 * _[subject taxon closure](subject_taxon_closure.md)_
    * _The taxon class or ancestor class for the subject_
    * range: [OntologyClass](OntologyClass.md)*
    * inherited from: [TaxonClosureMixin](TaxonClosureMixin.md)
 * _[subject taxon closure label](subject_taxon_closure_label.md)_
    * _The label for the taxon class or ancestor class for the subject_
    * range: **string***
    * inherited from: [TaxonClosureMixin](TaxonClosureMixin.md)
 * _[subject taxon label](subject_taxon_label.md)_
    * range: label
    * inherited from: [TaxonClosureMixin](TaxonClosureMixin.md)
 * _[systematic synonym](systematic_synonym.md)_
    * _more commonly used for gene symbols in yeast_
    * range: [LabelType](LabelType.md)
    * inherited from: [NamedThing](NamedThing.md)
 * _[title](title.md)_
    * _Narrative text describing the entity_
    * range: [LabelType](LabelType.md)
    * inherited from: [InformationContentEntity](InformationContentEntity.md)