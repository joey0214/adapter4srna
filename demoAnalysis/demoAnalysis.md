
# DEMO analysis for importance of adapter sequence

#### Author: Xiangfu (Joey) Zhong
## Data Source 

Dard-Dascot, Cloelia, Delphine Naquin, Yves d’Aubenton-Carafa, Karine Alix, Claude Thermes, and Erwin van Dijk. "Systematic comparison of small RNA library preparation protocols for next-generation sequencing." BMC genomics 19, no. 1 (2018): 118. DOI: [https://doi.org/10.1186/s12864-018-4491-6](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-018-4491-6) 


## Data Description
Dard-Dascot *et.al.* compared libraries prepared by different small RNA library preparation kits: TruSeq, NEXTflex V2, NEBNext, SMARTer and CATS. 

The prepared libraries were sequenced on NextSeq 500 platform by miRNA-Seq approach.

## Selected datasets for demo analysis
| Accession number | Kit | sample name | 
| :----------- :|:-------------:| -------:| 
| SRR6464616   | NEBNext| NN_synth_equi_rep2 |
| SRR6464623  | NEBNext| NN_synth_equi_rep1 |
| SRR6464673  | CATS | C_synth_equi_rep2 |
| SRR6464674  | CATS | C_synth_equi_rep1 |

## Analysis steps

#### downloading
Download dataset using `fastq-dump`

#### 
