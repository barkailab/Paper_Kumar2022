Dear Reader,
thansk for your interest in our research.
This repository contains the scripts and data necessary to generate most of the Figures used in the Paper: "Complementary strategies for directing transcription factor binding in-vivo through DNA-binding domains and intrinsically disordered regions" by Kumar et al. 2023.
Scripts and data for Figure 1,2 and 4AandE can be found in the respective folders (matFiles for data). For Figure 3 and the rest of Figure 4 the scripts can be found in the two .m files and the data is combined in redData.mat.xx, which need to be combined to generate redData.mat.
The scripts should only require a small knwoledge of Matlab syntax and were tested on Matlab 2021b. 
The mat files contain the variables processed sequencing data as well as additional annotation of the yeast genome.
In Detail:
1)redData.mat:
   - sTable:  meta data for each analysed strain column names should be self explanatory
   - sumProm: promoter (n=6701) binding data for all strains (mean across at least 2 repeats) ordered according to sTable
   - descs:   metadata for 60 analysed yeast transcription factors
   - tfs:     metadata for 72 analysed yeast transcription factors (ordered accoridng to tfid in sTable)
   - promType:Classification of all yeast promoters according to their genomic locations (Class 1,2 are in unique regions of the genome)
    -GP:      General annotation of the yeast genome. GP.gene_infoR64.nameNew contains the genenames in the 6701 order
   - seTf:    N/A
   - WTs:     N/A
   
2) MatFiles/GP.mat
   GP:   see above
3) MatFiles/medianSumPromNewAll.mat

4) MatFiles/otherMatFiles.mat
   
Due to space constrains some data (nucleotide-resolution coverage of each strain) had to be omitted from the repository. But are available as processed files on our GEO archive (GSE209631).

We hope you enjoy looking at our data and if some scripts do not run on your computer please do not hesitate to contact us and we will try to get it working.

Felix Jonas (fxjonas@gmail.com) & Divya Kumar ()
