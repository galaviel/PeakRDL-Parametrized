[![Documentation Status](https://readthedocs.org/projects/peakrdl/badge/?version=latest)](http://peakrdl.readthedocs.io)
[![build](https://github.com/SystemRDL/PeakRDL/workflows/build/badge.svg)](https://github.com/SystemRDL/PeakRDL/actions?query=workflow%3Abuild+branch%3Amain)
[![Coverage Status](https://coveralls.io/repos/github/SystemRDL/PeakRDL/badge.svg?branch=main)](https://coveralls.io/github/SystemRDL/PeakRDL?branch=main)
[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peakrdl.svg)](https://pypi.org/project/peakrdl)

This is a fork of the original project, with the intent of adding experimental (very limited) parametrization support for regblock output. All parameters specified by the user (in the regblock sub-commnad) as --keep_params PARA1 PARAM2 ... will retain their symbolic, unresolved value (e.g. 'PARAM1`) instead of being resolved to actual (most commonly - integer) values. Support is provided for:

Parametrization of the dimensions of 1D array of registers (MDA - multi-dim - wip). The array dimension size must be an expression containing only the name of the parameter (without any further arithmetic or other operands).
Parametrization of the reset value of individual fields. Again - expression must be as 1. above.

# PeakRDL

PeakRDL is a free and open-source control & status register (CSR) toolchain.
This project provides a command-line tool that unifies many aspects of register
automation centered around the SystemRDL register description language.

# PeakRDL-Parametrized
Fork of PeakRDL that allows for generation of parametrized output files (keep the RTL symbolic, do not substitute the actual parameter values).

## Documentation
See the [PeakRDL Documentation](http://peakrdl.readthedocs.io) for more details.
