# adapter4srna

## Adapter in small RNA sequencing
This is an open access reporitory to collect all used adapter sequences in currently commercial available and discontinued kits.

### Any comments and contributions are welcomed.


3' adapter for small RNA sequencing on Illumina platform


| Vendor        | Kit           | Version | 3' Adapter sequence |
|:-----------:|:-----------:|-----------:|-----------|
| New England Biolabs        | NEBNext Multiplex Small RNA Library Prep Kit for Illumina           | V3 | 5'-AGATCGGAAGAGCACACGTCT-3' |
| Illumina        | TruSeq Small RNA           | Version | 5’-TGGAATTCTCGGGTGCCAAGG-3' |
| PerkinElmer        | NEXTflex Small RNA Sequencing Kit **           | V3 | 5’-TGGAATTCTCGGGTGCCAAGG-3' |
| Qiagen        | QIAseq miRNA Library Kit           | Version | 5’-AACTGTAGGCACCATCAAT-3' |
| Lexogen        | Small RNA-Seq Library Prep Kit           | Version | 5’-TGGAATTCTCGGGTGCCAAGGAACTCCAGTCAC-3'  |
| SeqMatic        | TailorMix miRNA Sample Preparation Kit           | V2 | 5’-TGGAATTCTCGGGTGCCAAGG-3' |
| Takara        | SMARTer smRNA-Seq Kit for Illumina           | Version | 5’-AAAAAAAAAA-3' |
| TriLink        | CleanTag Small RNA Library Prep Kit           | Version | 5'-TGGAATTCTCGGGTGCCAAGG-3' |
| Diagenode        | CATS small RNA-seq Kit           | Version | 5'-GATCGGAAGAGCACACGTCTG-3'  |
| GenXPro         | TrueQuant SmallRNA Seq Kit for Ultra Low Input           | Version | TODO |
| ~~Epicentre~~        | ~~ScriptMiner Small RNA-Seq Library Preparation Kit~~           | ~~Version~~ | ~~ ~~ | 
| ~~Life Technology~~        | ~~SREK, Small RNA Expression Kit~~           | ~~version C~~ | ~~ ~~ | 

**4 random bases

~~Kit~~ Discontinued kit


##### CATS Small RNA sequencing kit for Illumina

Version 2 | 01.17
```
cutadapt -u 3 input_file.fastq | cutadapt -a AAAAAAAA - | cutadapt -a AAAAAAAN$ -a AAAAAAN$ -a AAAAAN$ - | cutadapt -a AGAGCACACGTCTG - | cutadapt -O 8 -g GTTCAGAGTTCTACAGTCCGACGATCNNN - | cutadapt -m 18 -o output_file.fastq -
```

Version 2 | 03.17
```
cutadapt -u 3 input_file.fastq | cutadapt -a AAAAAAAA - | cutadapt -a AAAAAAAN$ -a AAAAAAN$ -a AAAAAN$ - | cutadapt -a AGAGCACACGTCTG - | cutadapt -O 8 -g GTTCAGAGTTCTACAGTCCGACGATCNNN - | cutadapt -m 18 -o output_file.fastq -
```


Version 2 | 09.17
```
cutadapt --trim-n -a GATCGGAAGAGCACACGTCTG -a AGAGCACACGTCTG <input.file> | cutadapt -u 3 -a A{100} --no-indels -e 0.16666666666666666 - | cutadapt -O 8 --match-read- wildcards -g GTTCAGAGTTCTACAGTCCGACGATCSSS -m 18 -o <output.file> -
```


## Contributing
Any comments and contributions are welcome.
Pull requests are welcome.


