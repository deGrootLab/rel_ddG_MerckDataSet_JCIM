
## Summary ##
This is a collection of the input files for 8 protein-ligand systems (552 ligand perturbations):
cdk8, cmet, eg5, hif2a, pfkfb3, shp2, syk, tnks2.

## Citation: ##
  submitted

## Folder structure: ##
   ### For every protein-ligand dataset ###
	- ligands_gaff2: for every ligand two topology files are present. 
	ffMOL.itp contains the atomtypes, the rest of topology parameters are in MOL.itp. 
	Structure is in the mol_gmx.pdb file. Force field: Gaff v2.11
	
	- ligands_cgenff: topology and structure for cgenff. 
	CGenFF v3.0.1 with the atom typing based on MATCH was used.
	
	- ligands_openff: topology and structure for OpenFF. 
	OpenFF 1.2.0 Parsley

	- protein_amber: structure and topology for protein and, 
	if available, co-crystallized waters and ions. Force field: amber99sb*ILDN
	
	- protein_charmm: structure and topology for Charmm36m force field
	
	- transformations_gaff2: edge information and hybrid structures/topologies for gaff2.
	
	- transformations_cgenff: edge information for cgenff. 

	- transformations_openff: edge information for OpenFF. 
	
  ddg_data: the folder contains calculated ddG values for all the protein-ligand datasets

  mdp: simulation parameter files
  ```
	- em_l0.mdp and em_l1.mdp: energy minimization for the states A and B
	- eq_nvt_l0.mdp and eq_nvt_l1.mdp: 100 ps NVT equilibration for the states A and B
	- eq_l0.mdp and eq_l1.mdp: 6 ns equilibrium run for the states A and B
	- ti_l0.mdp and ti_l1.mdp: 50 ps transition A->B and B->A. 
```
