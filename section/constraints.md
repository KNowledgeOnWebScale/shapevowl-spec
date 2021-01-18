# Constraints

First, we provide a mapping from semantic constructs of RDF constraint languages
to visual elements of ShapeVOWL (see figures).
Next, we explain splitting rules with respect to the visualization of property shapes.
Finally, we provide a complete visual example.

## Semantic constructs

The SHACL specification [[SHACL]] contains core constraints and other concepts relevant for data validation.
We provide a mapping of semantic constructs to visual representations with ShapeVOWL,
i.e. in the first figure we provide the mapping from SHACL core constraints
and in the second figure we provide the mapping from other relevant SHACL concepts.

<figure id="semantic-constructs"> 
  <img src="./resources/images/2020-journal-mapping-shapevowl-core-constraints-summary.svg" style="height:100%;width:100%" />
  <figcaption>
    Semantic constructs of SHACL core constraints
    and their visual representation in ShapeVOWL.
  </figcaption>
</figure>

<figure id="semantic-constructs"> 
  <img src="./resources/images/2020-journal-mapping-shapevowl-other-concepts-summary.svg" style="height:100%;width:100%" />
  <figcaption>
    Semantic constructs of validation-related SHACL concepts
    and their visual representation in ShapeVOWL.
  </figcaption>
</figure>
 
 
## Splitting rules


Node shapes can be reused by a directed dashed connection, however we recommend splitting rules for the visualization of reused property shapes as trade-off for the graph rendering.
Different splittings for property shapes are possible; in the following we describe three possible splitting rules for property shapes.
Depending on the level of detail, applications may choose one of the splitting rules.

Property shapes consist of two parts: a solid directed edge with the property path as label in a rectangle and a value the directed edge points too which is either a node or a literal.

### Duplicate property shape

A reused property shape is visualized for each reuse, i.e. a property shape which is used <code>n</code> times will be visualized <code>n</code> times.

### Duplicate property path

The value of a reused property shape is visualized only once but the directed edge and label are visualized for each reuse.

### No duplication

A reused property shape is visualized only once, i.e. a property shape which is used <code>n</code> times will be visualized exactly one time
and will have <code>n</code> ingoing solid edges to the rectangle containing the property path.

## Example

Below you can find an example for constraints expressed with ShapeVOWL.

<figure id="example-shapeuml"> 
  <img src="./resources/images/example-shapevowl.svg" style="height:100%;width:100%" />
  <figcaption>
    Constraints visualized using ShapeVOWL: A subject valid to the Person data shape should have an IRI (1),
    at least one but maximum two <code>ex:address</code> properties (2) of class <code>schema:PostalAddress</code> (3)
    and the object of at least one <code>ex:address</code> property should comply with the existing data shape <code>ex:validAddress</code> (4).
    Additionally, the subject valid to person should either have exactly one <code>ex:fullName</code> or at least one <code>schema:givenName</code> (5)
    and at least one <code>schema:familyName</code> all of datatype <code>xsd:string</code>.
	The value of <code>ex:fullName</code> must not comply with the data shape <code>ex:organizationShape</code> (6).
	Addresses must only have values for the property <code>postalAddress</code> with an exception for <code>rdf:type</code> (7).
	Constraints of the <code>ex:organizationShape</code> are not considered for validation (8). 
  ShapeVOWL also visualizes optional accompanying logos for constraint types (9).
  </figcaption>
</figure>

