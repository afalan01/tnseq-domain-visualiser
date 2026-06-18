# Download Notes

This document records where project data files were downloaded from and why they were selected.

## Organism 1: Mycobacterium tuberculosis H37Rv

Reason for selection:
M. tuberculosis H37Rv is being used as the first test organism because it has published Tn-seq essentiality datasets and was also used in previous domain-level essentiality visualisation work.

Required files:

| File | Purpose | Source | Status |
|---|---|---|---|
| Reference genome FASTA | Provides DNA sequence | NCBI RefSeq/GenBank | Not downloaded |
| Gene annotation GFF3 | Provides gene coordinates | NCBI RefSeq/GenBank | Not downloaded |
| Tn-seq insertion/essentiality data | Provides insertion counts or essentiality states | DeJesus et al. / MtbTnDB | Not downloaded |
| Protein domain annotations | Provides protein-domain coordinates | UniProt / InterPro / CDD | Not downloaded |

## Reference genome download: Mycobacterium tuberculosis H37Rv

Date downloaded: 18 June 2026

Organism: *Mycobacterium tuberculosis* H37Rv  
Assembly accession: GCF_000195955.2  
Reference sequence accession: NC_000962.3  

Source:
NCBI Datasets genome assembly page.

Files downloaded:
- Genomic FASTA: `data/raw/ncbi_dataset/ncbi_dataset/data/GCF_000195955.2/GCF_000195955.2_ASM19595v2_genomic.fna`
- Genomic GFF: `data/raw/ncbi_dataset/ncbi_dataset/data/GCF_000195955.2/genomic.gff`

Purpose:
These files provide the reference genome sequence and gene coordinates for the initial development of the domain-level Tn-seq visualisation pipeline.

