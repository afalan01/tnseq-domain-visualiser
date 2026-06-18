# Data Inventory

This document records the datasets and database sources required for the project.

## Project organism

Initial organism: *Mycobacterium tuberculosis* H37Rv

This organism has been selected as the starting point because it is well-studied, has published Tn-seq essentiality datasets, and has been used previously for domain-level essentiality visualisation.

## Required data sources

| Data type | Purpose | Proposed source | File type needed | Status | Notes |
|---|---|---|---|---|---|
| Reference genome sequence | Provides the DNA sequence for the organism | NCBI RefSeq | FASTA | Downloaded | Downloaded from NCBI Datasets for assembly GCF_000195955.2 |
| Gene annotation | Provides gene start/end positions and locus tags | NCBI RefSeq | GFF/GFF3 | Downloaded | Downloaded from NCBI Datasets for assembly GCF_000195955.2 |
| Tn-seq insertion data | Shows insertion positions/counts or essentiality states | Published Tn-seq datasets / MtbTnDB / DeJesus et al. | WIG, TSV, CSV, or processed table | Not downloaded | Main essentiality evidence |
| Protein-domain annotations | Shows domain positions within proteins | UniProtKB, InterPro, Pfam/CDD | TSV, GFF3, JSON, or downloaded table | Not downloaded | Needed to map domains to genes |
| Previous project reference | Provides methodological background only | Eliza Naismith 2024 dissertation | PDF/GitHub repository | Available as reference | Used for context, not copied |

## Downloaded reference genome files

Organism: *Mycobacterium tuberculosis* H37Rv  
Assembly accession: GCF_000195955.2  
Reference sequence accession: NC_000962.3  

Local file paths:

- `data/raw/ncbi_dataset/ncbi_dataset/data/GCF_000195955.2/GCF_000195955.2_ASM19595v2_genomic.fna`
- `data/raw/ncbi_dataset/ncbi_dataset/data/GCF_000195955.2/genomic.gff`

These files are stored locally in `data/raw/` and are not committed to GitHub.

## Minimum viable dataset

The first working version of the project will use:

1. One organism: *M. tuberculosis* H37Rv
2. One or a small number of genes
3. One Tn-seq essentiality dataset
4. One domain annotation source
5. One automated visualisation output

## Notes on raw data

Large raw datasets should not be committed directly to GitHub unless they are small example files or supervisor-approved. Download instructions and source links should be documented instead.
