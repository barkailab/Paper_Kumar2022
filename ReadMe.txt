Dear Reader,
thanks for your interest in our research.
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
This file contains the median promoter signal values between repeats for all strains
4) MatFiles/medianMotifNew.mat
This file contains the median in vivo 7mer scores between repeats for all strains
5) MatFiles/otherMatFiles.mat
  CISBP7merDist- in vitro 7mer scores
  CISBP7seqLogo- in vitro PWM after selecting the most informative 7nt
  contOPNDPN- OPN-Score
  descTF- this the similar to supplemetary table 2, containing information about each TF used
  dirStdClean- gene expression plasticity
  HahnFeatures- promoter properties described by Donczew et al
  intCorrMotifNew: standard deviation between repeats on in vivo 7mer signals
  intCorrSumPromNewAll: standard deviation between repeats on all promoter signals
  intCorrSumPromNewWOSubtel : standard deviation between repeats on promoter signals except subtelomeric promoters
  intGeneDist: inergenic distance upstram the promoter
  nmerRed7- 7mer motif sequences 
  promoterIDXVec- this array identifies promoter regions
  promoterLengthsTS- promoter Lengths
  PughFeatures- promoter properties described by Rossi et al
  SC_genome - genome sequence
  whichProm- array containing promoter numbers on promoter positions
6) medianNucleosomeData- median nucleosome signal on genome
Due to space constrains some data (nucleotide-resolution coverage of each strain) had to be omitted from the repository. But are available as processed files on our GEO archive (GSE209631).

We hope you enjoy looking at our data and if some scripts do not run on your computer please do not hesitate to contact us and we will try help you getting started.
For the most updated version of the codes, we refer to our GitHub repository: https://github.com/barkailab/Paper_Kumar2022.

Felix Jonas (fxjonas@gmail.com) & Divya Kumar (kdivya5706@gmail.com)
