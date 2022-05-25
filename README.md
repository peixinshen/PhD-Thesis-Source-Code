[![Mathematica](https://img.shields.io/badge/Wolfram-Mathematica-DD1100?logo=wolfram-mathematica&logoColor=DD1100)](https://www.wolfram.com/mathematica/)
[![View notebooks](https://wolfr.am/HAAhzkRq)](https://wolfr.am/13p40iO9O)
[![Julia](https://img.shields.io/badge/Julia-1.7.2-9558B2?logo=julia)](https://julialang.org/)
[![Python](https://img.shields.io/badge/Python-3.8.2-3776AB?logo=python)](https://www.python.org/)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6580092.svg)](https://doi.org/10.5281/zenodo.6580092)

# Quantum Machine Learning and Information Processing

This repository provides the source code for some analytical and numerical implementations of the PhD dissertation *Quantum Machine Learning and Information Processing*.

Most of the code is written by the Wolfram Language in the form of Mathematica notebook ([view online](https://wolfr.am/13p40iO9O)).

Some of the code is implemented by Julia and Python in the form of Jupyter Notebook.

This is the very initial version, detailed comments of the code will be updated in the near future.

# Contents

- `PhD-Thesis-Mathematica.nb` contains the code for symbolic calculation, numerical simulation, and image processing. Similar to the dissertation, this notebook contains the following chapters:
  - In *Chapter 1 Preliminaries*, we provide the source code for drawing the Bloch sphere, quantum circuits, artificial neural networks, and handwritten digits. Also, we can find the full symbolic calculation for both the Bethe ansatz and the transfer matrix method. A simple demonstration of GridWorld in reinforcement learning is also supplemented.
  - In *Chapter 2 Quantum Machine Learning in the NISQ Era*, we explicitly show the quantum circuits for both the Grover search algorithm and the quantum phase estimation algorithm.
  - In *Chapter 3 Quantum Architecture Search*, we attach the training results for both the neuroevolution of augmenting topologies algorithm, and our proposed Markovian neuroevolution algorithm [[1](#refer-anchor-1)].
  - In *Chapter 4 Information Processing in Quantum Spin Chains*, we give the explicit form of wave functions, and show how to analytically obtain the scattering matrix using the low-energy theory. The source code and numerical data of figures used in our Ising-XY-Ising model are also attached [[2](#refer-anchor-2)].
  - In *Appendix The Honeycomb Ising Model*, we specifically demonstrate how to solve the anisotropic honeycomb Ising model via the transfer matrix method.
- `GateBlockLibraryScaling.ipynb` investigates the scaling of gate-block library subjected to different restrictions of quantum circuit blocks. The data is saved in the directory `/GateBlockLibraryData`.
- `SymbolicTransformation.ipynb` provides a systematical way to transform Hamiltonians among different operators: qubits, fermions, and Majoranas.

# Packages

- Wolfram Language 13.0 with [QuantumFramework](https://resources.wolframcloud.com/PacletRepository/resources/Wolfram/QuantumFramework/) v1.0.2
- Python 3.8.2 with [OpenFermion](https://quantumai.google/openfermion) v1.4.0 and [SymPy](https://www.sympy.org/en/index.html) v1.9
- Julia 1.7.2, with [JLD2](https://github.com/JuliaIO/JLD2.jl) v0.4.22, [CairoMakie](https://makie.juliaplots.org/stable/documentation/backends/cairomakie/) v0.7.5, and [Combinatorics](https://github.com/JuliaMath/Combinatorics.jl) v1.0.2

# References

<div id="refer-anchor-1"></div> 

[1] Z. Lu*, P.-X. Shen*, and D.-L. Deng, [Markovian Quantum Neuroevolution for Machine Learning](https://link.aps.org/doi/10.1103/PhysRevApplied.16.044039), Phys. Rev. Applied 16, 044039 (2021).

<div id="refer-anchor-2"></div>

[2] P.-X. Shen, S. Hoffman, and M. Trif, [Theory of Topological Spin Josephson Junctions](https://link.aps.org/doi/10.1103/PhysRevResearch.3.013003), Phys. Rev. Research 3, 013003 (2021).