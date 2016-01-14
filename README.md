OBAN
====

### What is OBAN

OBAN stands for **O**pen **B**iomedical **AN**notations. It is an ontology model used to describe associations between biomedical entities in triple format based on W3C specification. OBAN is a generic association representation model that loosely couples a subject and object (e.g. disease and its associated phenotypes supported by the source of evidence for that association) via a construction of class *OBAN:association*. The association is supported by an evidence of class *OBAN:provenance* where a tracable record for that association assertion is described. OBAN was introduced as a mediator to resolve the limitation of representing a probability-bound event at a class level (where an assertion of subject-object relation must be true at all time, or P=1). OBAN overcomes this issue by representing the subject-object association with an individual (i.e., at ontology instance level) of class *OBAN:association* that are specific to an evidence of that association of class *OBAN:provenance* as shown in this diagram.

# 

![](https://github.com/EBISPOT/OBAN/blob/master/diagrams/oban%20db%20source%20model.png)


OBAN represents a triple-form entity of subject-related-to object through the object properties *association_has_subject* and *association_has_object*. This association is supported by an *OBAN:provenance* class that instantiates a provenance entity that supports the association. In OBAN, provenance is a class that validates the association statement in the corresponding *OBAN:association* class instance. One provenance individual can also be about several associations as the same provenance may provide evidence for multiple subject-object associations, and each association instance can have several items of provenance attached to it.


### Implementation guideline

OBAN is a small ontology with a core skeleton consisting of three main classes; *OBAN:association*, *OBAN:provenance*, and *ECO:evidence*. OBAN exploits the evidence codes in [Evidence Ontology (ECO)](http://www.evidenceontology.org/)'s in representing an evidence attached to the provenance. We have provided OBAN ontology is both OWL and TTL format in our file repository [here](https://github.com/EBISPOT/OBAN/tree/master/ontology). A new subject-object association is to be created as an instance. You can use an ontology editor software (such as [Protege](http://protege.stanford.edu/) - [how to add individuals](https://www.youtube.com/watch?v=_7MfDdsFePk)), or [OWL API](http://owlapi.sourceforge.net/) to programmatically do this.


### Projects utilising OBAN
* [Disease-phenotype associations](https://sourceforge.net/p/efo/code/HEAD/tree/trunk/src/efoassociations/) at the Centre for Therapeutic Target Validation [CTTV](http://www.targetvalidation.org)



### Publications
* Sirarat Sarntivijai, Drashtti Vasant, Gary Saunders, Patricia Bento, Daniel Gonzalez, Joanna Betts, Samiul Hasan, Gautier Koscielny, Ian Dunham, Helen Parkinson, and James Malone ["Linking rare and common disease: mapping clinical disease-phenotypes to ontologies in therapeutic target validation](https://github.com/EBISPOT/OBAN/blob/master/publications/Rare2Common_PhenoMap_Proceedings-SIG-2015.pdf)



### Contact us
Submit your questions via [OBAN issue tracker](https://github.com/EBISPOT/OBAN/issues)
