# graph-percolation

Short study about several models of aleatory graphs and their properties using percolation and experimenting with Monte Carlo methods.

## Introduction

Percolation consists in a method that, from a probability `q`, decides if a vertex or a edge fails or,
what is the same, that with probability `1-q` not fails.

This process is applied on certain graphs to unveil from which probability the percolation is given (or not).
This value is called **phase transition**.

In this study, we have generated several graphs based in models from
[Erdős-Rényi](https://www.geeksforgeeks.org/erdos-renyl-model-generating-random-graphs/) and
[Watts-Strogatz](https://en.wikipedia.org/wiki/Watts%E2%80%93Strogatz_model).

The properties studied are:
- Top and bottom
- Connectivity
- Eulerian
- Cyclic

In addition, we have created a Union-Find class implementing a Weighted Quick Union using path compression.
This class is very useful to find the properties listed.

## Models

The models are grouped into [graphgen.h](./src/graphgen.h), except for the grid graph,
which is generated at the same time that tests are performed to improve the efficiency.

Aleatory graphs are implemented with an adjacency matrix.
Each model has an associated method that returns their aleatory graph.

The models studied are:
- Grid
- Erdős-Rényi
- Watts-Strogatz
- Uniform
- Cyclic

## Documentation

Check the full report of the models and experiments in [report.pdf](./docs/report.pdf). (Spanish)

## Credits

This study was done with the help of Alex Iniesta and Adrián Navarro.
