# Ferromagnetic Iron DFT Database for Fracture
# lei.zhang@rug.nl
# Fri 24 Jun, 2022

This folder contains the extended DFT database developed for fracture prediction of ferromagnetic iron. 
It is developed based on the DFT database of Dragoni D. (Phys. Rev. Mater. 2, 013808).

The extended DFT database includes:
- DB9 (1743 structures): Highly strained BCC primitive cells containing one atom each. Distortions of cell vectors are obtained using a SOBOL-sampling algorithm. Energy is reported in eV; the virial tensor (stress*volume) is also reported in eV. Note the sign convention where contracted/expanded cells have negative/positive pressure. 
- DB10 (198 structures): Highly strained HCP primitive cell containing two atoms each. Distortions of cell vectors are obtained using a SOBOL-sampling algorithm. Energy and forces are reported in eV and eV/Å, respectively.
- DB11 (351 structures): Surface separation process of {100}, {110}, {111} and {112} crystallographic orientations. Both thin and thick slabs are included. Thick supercells have a thickness of >30Å along the separation direction to avoid replica interactions. The separation is performed from 0Å to 4Å with a step of 0.4Å. The rigid separation includes two sets of structures, i.e., ideal crystal structures and "rattled" structures. The rattled structures areobtained by adding a Gaussian noise N~[0;0:05*a0] to the three Cartesian coordinates (a0 lattice constant). Energy and forces are reported in eV and eV/Å, respectively.
- DB12 (14 structures): Small crack tip configurations developed via active learning method. Energy and forces are reported in eV and eV/Å, respectively.