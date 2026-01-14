# Origin-1
This repository contains data generated as part of the study [Origin-1: a generative AI platform for _de novo_ antibody design](https://www.absci.com/). _In silico_ and _in vitro_ data are included in this repository. Additional binding, developability, functionality, and structure confirmation results can be found in the paper.

-----------------------------------------------------------------------------------------------------
Data in `de_novo_spr_data.csv` are organized with the following columns:
* `Design`: Design identifier indicating target and rank (lower = higher rank)
* `Heavy Chain`: Heavy chain variable domain sequence
* `Light Chain`: Light chain variable domain sequence
* `Target`: Target antigen
* `Framework`: Therapeutic antibody used for framework scaffold
* `Epitope`: Epitope identifier
* `Binder`: Boolean indicating whether or not the design is a binder
-----------------------------------------------------------------------------------------------------
Data in `lead_optimization_spr_data.csv` are organized with the following columns:
* `Heavy Chain`: Heavy chain variable domain sequence
* `Light Chain`: Light chain variable domain sequence
* `Target`: Target antigen. We use AZGP1-A and AZGP1-B to both indicate screening against AZGP1 but that different parents were used for optimization.
* `Mutation`: Mutation made from parent sequence (e.g. H-S31A is an S to A mutation at 1-indexed position 31 of the heavy chain)
* `Binder`: Boolean indicating whether or not the design is a binder. Note that a NaN may be present which indicates the respective antibody could not be measured for binding.
* `KD (nM)`: Dissociation constant in nM units
* `pKD`: Negative logarithm of dissociation constant
-----------------------------------------------------------------------------------------------------
The `abscibind` and `abscigen` folders contain the computational models generated for the reported designs by AbsciBind and AbsciGen, respectively.

# Citations
If you find these data or results useful, we ask that you cite our work: TBA
