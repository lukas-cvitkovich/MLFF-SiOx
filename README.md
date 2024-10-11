# MLFF_SiOx:
This repository contains the interatomic machine learning force field (MLFF) suitable for the dynamic oxidation of silicon. You are free to use the MLFF for scientific/non-commercial use. If you do, please cite [1] and [2] or the according publication in the Journal of Chemical Physics (to be published)

## Usage:
Download both GAP*.zip files. They are only separated to stay within the file size limit of GitHub.
Uncompress the files and store the resulting .xml files in the same folder (typically the folder where you run your simulation).

### For use in LAMMPS:
Please make sure to install QUIP and link it to LAMMPS.

In the LAMMPS input file define the interatomic potential as: <br>
pair_style	quip <br>
pair_coeff	* * GAP_SiOx_v1.0.xml "Potential xml_label=GAP_2023_9_18_120_4_5_0_872" 1 8 14


# References:
\[1\]: https://doi.org/10.1063/5.0220091 <br>
\[2\]: https://doi.org/10.1016/j.apsusc.2022.155378
