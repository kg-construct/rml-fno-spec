## Definitions

- <dfn>FnO</dfn>: the Function Ontology. Describes implementation-independent functions' inputs and outputs, and execution descriptions.
- <dfn>RML</dfn>: RDF Mapping Language. Describes schema transformations from heterogeneous data sources to RDF.
- An <dfn>RML mapping</dfn> is a set of mapping rules, described in <a>RML</a>.
- An <dfn>RML processor</dfn> is a tool that interprets the <a>RML mapping</a> and executes its rules to generate a knowledge graph.
- <dfn>FNML</dfn>: describes how to integrate data transformations in schema transformations using <a>FnO</a> in <a>RML</a>.
- A <dfn>function description</dfn> describes the function, i.e., talks about the inputs and outputs of the function.
  For example, a function can have the following description: `function int sum(int a, int b)`, namely,
  the function `sum` has two input parameters, `int a` and `int b`, and returns an integer.
- An <dfn>execution</dfn> is the assignment of the values of the parameters of a function.
  An <a>execution</a> has as result the value of the output of the function.
  For example, `sum(2, 4)` is an execution.
  The value of the output is known after the function is executed, and should in this case be the integer `6`.
- A <dfn>function map</dfn> is a specific type of [term map](https://rml.io/specs/rml/#term-map): it generates an [RDF term](https://rml.io/specs/rml/#rdf-term) from a [triples map](https://rml.io/specs/rml/#triples-map) that describes an <a>execution</a>.

<p class="note" data-format="markdown">
It is currently assumed that a <a>function map</a> always returns an RDF term [[rdf-concepts]] **or list thereof**.
How a list of RDF terms is handled, is out of scope of this spec, but currently discussed at https://github.com/kg-construct/mapping-challenges/pull/26 and https://github.com/kg-construct/mapping-challenges/pull/27
</p>
