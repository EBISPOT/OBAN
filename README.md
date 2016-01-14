OBAN
====

### What is OBAN
OBAN stands for **O**pen **B**iomedical **AN**notations. It is an ontology model used to describe associations between biomedical entities in triple format based on W3C specification. OBAN is a generic association representation model that loosely couples a subject and object (e.g. disease and its associated phenotypes supported by the source of evidence for that association) via a construction of class *OBAN:association*. The association is supported by an evidence of class *OBAN:provenance* where a tracable record for that association assertion is described. OBAN was introduced as a mediator to resolve the limitation of representing a probability-bound event at a class level (where an assertion of subject-object relation must be true at all time, or P=1). OBAN overcomes this issue by representing the subject-object association with an individual (i.e., at ontology instance level) of class *OBAN:association* that are specific to an evidence of that association of class *OBAN:provenance* as shown in this diagram.

# 

![](https://github.com/EBISPOT/OBAN/blob/master/oban%20db%20source%20model.png)

### Implementation guideline


### Projects utilising OBAN
* [Disease-phenotype associations](https://sourceforge.net/p/efo/code/HEAD/tree/trunk/src/efoassociations/) at the Centre for Therapeutic Target Validation [CTTV](http://www.targetvalidation.org)
* 


### Contact us
