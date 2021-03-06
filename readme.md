# PyMC 3

[![Build Status](https://travis-ci.org/pymc-devs/pymc.png?branch=master)](https://travis-ci.org/pymc-devs/pymc)

PyMC is a python module for Bayesian statistical modeling and model fitting which focuses on advanced Markov chain Monte Carlo fitting algorithms. Its flexibility and extensibility make it applicable to a large suite of problems.

Check out the [Tutorial](http://nbviewer.ipython.org/urls/raw.github.com/pymc-devs/pymc/master/pymc/examples/tutorial.ipynb)!

## Features

 * Intuitive model specification syntax, for example, `x ~ N(0,1)` translates to `x = Normal(0,1)`
 * Powerful sampling algorithms such as [Hamiltonian Monte Carlo](http://en.wikipedia.org/wiki/Hybrid_Monte_Carlo)
 * Easy optimization for finding the *maximum a posteriori* point
 * [Theano](http://deeplearning.net/software/theano/) features
  * Numpy broadcasting and advanced indexing
  * Linear algebra operators
  * Computation optimization and dynamic C compilation
 * Simple extensibility

## Getting started
 * [PyMC 3 Tutorial](http://nbviewer.ipython.org/urls/raw.github.com/pymc-devs/pymc/master/pymc/examples/tutorial.ipynb)
 * Coal Mining Disasters model in [PyMC 2](https://github.com/pymc-devs/pymc/blob/2.3/pymc/examples/disaster_model.py) and [PyMC 3](https://github.com/pymc-devs/pymc/blob/master/pymc/examples/disaster_model.py)
 * [Global Health Metrics & Evaluation model](http://nbviewer.ipython.org/urls/raw.github.com/pymc-devs/pymc/master/pymc/examples/GHME%202013.ipynb) case study for GHME 2013
 * [Stochastic Volatility model](http://nbviewer.ipython.org/urls/raw.github.com/pymc-devs/pymc/master/pymc/examples/stochastic_volatility.ipynb)

## Installation

```
pip install git+https://github.com/pymc-devs/pymc
```

### Optional

[`scikits.sparse`](https://github.com/njsmith/scikits-sparse) enables sparse scaling matrices which are useful for large problems. Installation on Ubuntu is easy:

```
sudo apt-get install libsuitesparse-dev
pip install git+https://github.com/njsmith/scikits-sparse.git
```

On Mac OS X you can install libsuitesparse 4.2.1 via homebrew (see http://brew.sh/ to install homebrew), manually add a link so the include files are where scikits-sparse expects them, and then install scikits-sparse:

```
brew install suite-sparse
ln -s /usr/local/Cellar/suite-sparse/4.2.1/include/ /usr/local/include/suitesparse
pip install git+https://github.com/njsmith/scikits-sparse.git
```


## License
[Apache License, Version 2.0](https://github.com/pymc-devs/pymc/blob/master/LICENSE)
