# equations
A collection of modular equations that are used throughout the SimPEG ecosystem.

## Why

Equations are an example of a modular piece of text that can be reused.
Currently this is hard, and is often not done - especially not between
multiple researchers. This repository our first take at that problem
in the geophysics community where notation is often dissonant between
various research groups.

## Goals

The goals of `equations` is to provide a small repository of equations
used in geophysics.

* a collection of equations with consistent notation
* a place to flag issues and have discussions
* increase ease of reuse of equations through writing, presentations and documentation
* meta data about the equation can be provided
* attribution can be given (through citations, git commits etc.)

## Scope

We will focus on the equations used throughout the SimPEG ecosystem specifically:

* inverse problems
* optimization
* electromagnetics
* potential fields
* vadose zone fluid flow

## Alternatives

Copy paste equations. Booooo

## Connections

* Listen to Lindsey Heagy talk about [equation banks](https://youtu.be/IW2LDsevvDk?t=15m8s) in [GeoSci](http://geosci.xyz) at SciPy2016
* Creating [modular documents](https://en.wikibooks.org/wiki/LaTeX/Modular_Documents) in latex using `input` and `include`
* SimPEG project at [http://simpeg.xyz](http://simpeg.xyz)
* [GitProject](https://github.com/3ptscience/git-project) for inclusion of this repository in other writing projects

# Example

## latex

In a latex document, clone the github repository into your working path (use git project or alternative).
In the header of your document input the header material:

```
\input{equations/index}
```

When you want to include a specific figure, just call that up:

```
\input{equations/richards/richards-objective-deriv}
```

This keeps your latex code clean. In our experience, we often work on google docs for collaborative document
this allows us to just write minimal latex and copy paste it when ready for a publication view.
