### Lexically Constrained Decoding with Grid Beam Search

This project is a reference implementation of Grid Beam Search for Lexically Constrained Decoding.

We provide two sample implementations of translation models -- one using our framework for
Neural Interactive Machine Translation, 
and another for models trained with [Nematus](https://github.com/rsennrich/nematus).

Any Nematus model should work out of the box. This project can also be used as a general-purpose 
ensembled decoder for Nematus models with or without constraints. 

### Citing
TODO(chris): citation/publications 


### Quick Start


### Project Structure


#### Core Abstractions


### Running Experiments

#### Pick-Revise 


### Performance

Right now, this implementation is pretty slow, and it gets slower the more constraints you add :disappointed:. 
The GBS algorithm can be easily parallelized, because each cell in a column is independent of the others (see paper). 
However, implementing this requires us to make some assumptions about the underlying model, and would thus
limit the generality of the code base. If you have ideas about how to make things faster, please create an issue. 

### Features

TODO: table
Ensemble and weighted decoding for Nematus models

Even models with different inputs can be used jointly.


#### Domain-Adaptation 


### Running Tests


If you use code or ideas from this project, please cite:

TODO(chrishokamp): add arxiv bibtex 