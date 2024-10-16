# Wk09 Assignment Edgerton

In this assignment you will practice using your the pipeline to create BCF files from alignments.
Keep a long of your commands and results in `{repo_root}/excercises/{userid}/wk09`.

## Notes from Assignment Description In Class/Comments from Will

- **Overall Goal:** High Level goal: you are trying to find the snps that make this a snowflake: so snps that are actually important in this context. 


- **Will already:**
    - Aligned the genomes
    - Intersected them against the genes using the .gff
    - Useful tools: SnpEff is a tool that takes the vcf file and looks at which gene is it in and asks: 
        - will it change the codon of that amino acid
        - low impact: synonomous mutation or no change mutation 
        - severe impact: frameshift/stopcodon


## Pipeline

Adjust your pipeline so you can specify which chromosome you generate variant calls for at the command line.
Update the documentation and place it in your week 9 excercise folder and commit it.

## Exercise

For each of the three strains aligned in `/data/share/omics/wk06/alns`

1. Use the pipeline to create bcf files for the OG_strain, SF_aer, and SF_ann from any chromosome but `chrI`.
2. Use `bcftools isec` to find varaints that are unique to each of the three strains.
3. Use `bedtools` to find the unique variants that overlap with regions defined in `/share/refs/SGD/saccharomyces_cerevisiae.gff`.
4. Visualize a selection of them in IGV.

***


## Log of Commands Used



