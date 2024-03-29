<img src="Ulogo.png" alt="drawing" width="100" align = "right"/>

# Surge: A Fast Open-Source Chemical Graph Generator
Brendan D. McKay, Mehmet Aziz Yirik and Christoph Steinbeck

## About
`Surge` is a chemical structure generator based on the canonical generation path method. `Surge` uses the Nauty package to compute automorphism groups of graphs and generates all non-isomorphic constitutional isomers of a given molecular formula. `Surge` is available under a liberal open source license.

# Documentation
A complete [**user manual**](https://github.com/StructureGenerator/surge/blob/main/doc/surge1_0.pdf) is included in the package.

# How to get surge
[Releases](https://github.com/StructureGenerator/surge/releases), source code and an issue tracker can be found at the [`surge` github repository](https://github.com/StructureGenerator/surge).

# Citing surge
If you use `surge`, please cite:

McKay, B.D., Yirik, M.A. & Steinbeck, C. Surge: a fast open-source chemical graph generator. J Cheminform 14, 24 (2022). https://doi.org/10.1186/s13321-022-00604-9

## Usage
`Surge` is a command line tool. Running `surge -u C10H16O` will generate the 452458 isomers of C<sub>10</sub>H<sub>16</sub>O in 0.1s on some vanilla flavor year-2021 PC. Running `surge -S C10H16O` outputs those structures in SMILES format. You can either use `surge -S C10H16O > myresults.smi` to redirect the output into a result file, or use the `-o`switch to provide a filename. Further formats supported are SD Files (SDF) and a concise Surge-specific format.  
For large sets of structures, the -z option for compressing the output in gzip format will come in handy.

`surge -help` will show all options. For complete instructions, please see the [**user manual**](https://github.com/StructureGenerator/surge/blob/main/doc/surge1_0.pdf).


## Authors
`Surge` was developed by

[Brendan McKay](http://users.cecs.anu.edu.au/~bdm), School of Computing, Australian National University, Canberra, ACT, Australia

[Mehmet Aziz Yirik](https://github.com/mehmetazizyirik), [Christoph Steinbeck](https://github.com/steinbeck), Institute for Inorganic and Analytical Chemistry, Friedrich-Schiller-University, Jena, Germany
