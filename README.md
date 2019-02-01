# Martinize2 and vermouth: The ultimate resolution transformation tools

[![Build Status](https://travis-ci.org/marrink-lab/vermouth-martinize.svg?branch=master)](https://travis-ci.org/marrink-lab/vermouth-martinize)
[![codecov](https://codecov.io/gh/marrink-lab/vermouth-martinize/branch/master/graph/badge.svg)](https://codecov.io/gh/marrink-lab/vermouth-martinize)
[![Documentation Status](https://readthedocs.org/projects/vermouth-martinize/badge/?version=latest)](https://vermouth-martinize.readthedocs.io/en/latest/?badge=latest)


Martinize2 is a rewrite of [Martinize]. It is aimed at producing
coarse-grained structures and topologies from an atomistic structure. Martinize
is primarily developed for the [Martini] coarse-grained force field and the
[Gromacs] simulation engine. However the architecture of the program will
allow us to support a broader range of force fields and simulation engines in
the future.

Vermouth (for VERsatile, MOdular,  and Universal Tranformation Helper) is the
python library that powers Martinize2. It allows to describe and apply
transformation on molecular structures and topologies using graph algorithms.

## Disclaimer

**Both Martinize2 and vermouth are at a prototype stage. DO NOT USE IN
PRODUCTION.**

## Installation

Martinize2 and vermouth require python 3.5 or greater. They can be installed
using the `pip` command:

    pip install git+https://github.com/marrink-lab/vermouth-martinize.git#vermouth

The behavior of the `pip` command can vary depending of the specificity of your
python installation. See the [documentation on installing a python
package][pipdoc] to learn more.

## Basic usage

Installing Martinize2 and vermouth with `pip` adds the `martinize2` program to
the research PATH. You can see the available option of the program by running:

    martinize2 -h

At the moment, martinize2 tries to reproduce the interface of the original
Martinize. You can find explanations on how to use Martinize on the [Martini
tutorials]; in most cases, replacing calls to `martinize.py` by calls to
`martinize2` should produce similar results.

The documentation of the vermouth python library will come soon.

## License

Martinize2 and vermouth are distributed under the Apache 2.0 license.

    Copyright 2018 University of Groningen

	Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at

		http://www.apache.org/licenses/LICENSE-2.0

	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.

The [full text of the license][license] is available in the source repository.

## Contributions

The development of Martinize2 and vermouth is done on [github]. Contributions
are welcome as [bug reports] and [pull requests]. Note however that the
decision of whether or not contributions can give authorship on the resulting
academic paper is left to our sole discretion.

[Martinize]: https://github.com/Tsjerk/Martinize
[Martini]: http://cgmartini.nl
[Martini tutorials]: http://cgmartini.nl/index.php/tutorials-general-introduction-gmx5
[Gromacs]: http://www.gromacs.org
[pipdoc]: https://packaging.python.org/tutorials/installing-packages/#installing-packages
[license]: https://github.com/marrink-lab/vermouth-martinize/blob/master/LICENSE
[github]: https://github.com/marrink-lab/vermouth-martinize
[bug reports]: https://github.com/marrink-lab/vermouth-martinize/issues
[pull requests]: https://github.com/marrink-lab/vermouth-martinize/pulls
