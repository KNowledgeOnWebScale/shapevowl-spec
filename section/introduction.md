## Introduction

Knowledge Graphs defined with the Resource Description Framework [[RDF]] consist of vocabulary terms and instance data both described using the graph model of RDF.
Several constraint languages exist to define conditions on such RDF graphs, one such language is the W3C recommended Shapes Constraint Language [[SHACL]]
which itself is represented using RDF.
Users rely on different types of constraints offered by constraint languages to define conditions on RDF graphs.


RDF follows a graph model which intuitively can be represented using nodes and edges.
The Visual Notation for OWL Ontologies [[VOWL]] leverages this graph model to visualize ontologies, the vocabulary of terms of Knowledge Graphs.
Besides this, VOWL-based visual notations were also used for the RDF Query Language SPARQL [[QueryVOWL]], used to query RDF data, and
for the RDF Mapping Language (RML) [[MapVOWL]], used to transform structured data to RDF.
ShapeVOWL is an attempt to leverage the broadly used visual notation VOWL for RDF constraints.
