# TBC1D24_analysis
Data for the article "TBC1D24 emerges as important contributor to progressive postlingual dominant hearing loss"

Files description:

/alignments/TBC/TBC_alignment_full.fasta- the alignment of the TBC domains from TBCD124 protein. Note that the original alignment obtained according to the procedure described in the methods section contained additional 3 sequences gi|678194481, gi|765111257, gi|961865181, . These sequences represented either clusters with one member (for gi|678194481, and gi|765111257) or three members (remaining sequence). All these sequences have length shorter than 160 residues and were excluded from the analysis. 

/alignments/TBC/TBC_for_figure.fasta – the alignment used to generate Figure 5C. It’s identical to the TBC_alignment_full.fasta, however 5 sadditional equences were added Homo sapiens (id tbcd124), Rattus norvegicus (gi|157786588), Mus musculus (gi|25552817), Gallus gallus (gi|381140054) and Danio rerio gi(1040681450). For one sequence (gi|573895534) missing N-terminal residues were added, as the automatic procedure to determine domain boundaries failed to identify these residues as such.

/alignments/TLDc/TLDc_alignment_full.fasta – the the alignment of the TLDc domains from TBCD124 protein Note that the original alignment obtained according to the procedure described in the methods section contained additional 5 sequences (gi|736240310,  gi|642129481, gi|974121214, gi|731503468, gi|1012090943, all being a sole member of their respective clusters). All these sequences have length shorter than 141 residues and were excluded from the analysis.

Alignments/TLDc/TLDc_to_consurf.fasta – the alignment used to generate residues conservation of TLDc domain depicted in Figure 6A. The alignment is identical to TLDc_alignment_full.fasta with following changes. 1. Sequences which did not contain H487 were re-analyzed. If such a sequence originated from an organism which indeed contained other copy of TBCD124 homologue with H487, such a sequence was removed. If no other homologue with H487 could be found a sequence without H487 was kept. The sequence from pdb|6r82 was added. For the sequence gi|719795183 ‘X’ residues were replaced with ‘-‘. 

Alignments/TLDc/TLDc_alignment_for_figure.fasta- the alignment used to generate  Fig 6C its identical to TLDc_to_consurf.fasta with additional 5 sequences added Homo sapiens (id tbcd124), Rattus norvegicus (gi|157786588), Mus musculus (gi|25552817), Gallus gallus (gi|381140054) and Danio rerio gi(1040681450).

Alignments/TLDc/sequences_withot_H487_id.txt – ids of sequences without H487, species from which a given sequence originated and a short description whether a homologous sequence can be found in proteome of this organisms together with this sequence id.

Alignments/TLDc/representatives_withoutH487/* –Files contain the multiple sequence alignment of TBCD124 sequences identified in a given organism. Only species from Alignments/ TLDc /sequences_withot_H487_id.txt were analyzed. The full human sequence is added to all MSA for reference.

Consurf/6r82_With_Conservation_Scores.pdb – the pdb file for 6r82 (TLDc domain from Drosophila melanogaster).  B-factor for chain A were replaced by residue conservation score calculated using ConSurf server using alignment from Alignments/ TLDc /TLDc_to_consurf.fasta. The file was used to generate Figure 6A and 6B.

Consurf/Consurf_Outputs_1612811221.zip – the raw output of ConSurf server.

Hdock/* - this directory contain top 10 conformations obtained from docking TLDc domain from from Drosophila melanogaster (pdb|6r82) to TBC domain from Drosophila melanogaster (pdb|5hjn). The model1.pdb was used to generate figure 6B.

Models/TBC/alignment.fasta – the sequence-to-structure alignment used to propose the structure of the human TBC domain from TBC1D24. Input to MODELLER.

Models/TBC/tbc1d24.B9999000* - five best structures proposed by MODELLER.

Models/TBC/tbc_final_model.pdb – the final structure of the human TBC domain from TBCD124, obtained after a short MD simulation. Used to generate figures 5A and 5B.

Models/TLDc/S579428_results.tar – the archive containing the results of modelling the human TLDc domain from TBC1D24 uing I-TASSER server. The results were used to identify the putative position of the loop harboring H487 used in Figure 6B.

