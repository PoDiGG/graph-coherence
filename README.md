# Graph Coherence

Calculates the coherence of RDF datasets based on the algorithm provided by [Duan et al](http://dl.acm.org/citation.cfm?id=1989340).
In essence, this calculates the structuredness of a dataset.
This can be used to check the _realism_ of synthetic datasets, which should have a similar coherence as its counterpart.

Any dataset that is supported by the [N3 module](https://www.npmjs.com/package/n3#parsing) can be loaded,
which currently consists of Turtle, TriG, N-Triples or N-Quads.

## Install

```bash
npm install graph-coherence
```

## Usage

```bash
graph-coherence [path to my RDF dataset]
```

This will return a number from 0 to 1 on stdout, with 1 being the maximum coherence.
