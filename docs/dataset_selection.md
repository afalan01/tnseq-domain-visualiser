# Dataset Selection

## Project aim

This project aims to automate the visualisation of Tn-seq gene essentiality data at the protein-domain level.

The first dataset must therefore provide:
- a well-annotated bacterial reference genome
- gene coordinates
- Tn-seq insertion or essentiality data
- compatibility with protein-domain annotation sources
- enough insertion density to support sub-gene or domain-level interpretation

## Candidate datasets considered

| Dataset | Strengths | Limitations | Decision |
|---|---|---|---|
| DeJesus et al. 2017 Mycobacterium tuberculosis H37Rv | High-saturation Tn-seq dataset; previously used to identify essential-domain-containing genes; suitable benchmark dataset | Already used in previous MSc work, so should not be the only contribution | Use as benchmark/validation dataset |
| MtbTnDB Mycobacterium tuberculosis | Public standardised Tn-seq database; multiple conditions; useful for scalability | Need to confirm downloadable file formats | Use as primary/public data source if suitable |
| Mycobacterium bovis AF2122/97 | Useful comparison with M. tuberculosis; used in previous related work | May require supervisor-provided data; less straightforward access | Optional only if data access is confirmed |
| Brucella abortus | Published saturated Tn-seq dataset with examples of domain-level essentiality | New organism increases setup time | Possible second dataset if time allows |
| Burkholderia cenocepacia | Directly relevant paper on essential protein domains | Method does not fully map true annotated domains initially | Useful literature support, not first dataset |

## Selected initial organism

The initial organism selected for pipeline development is *Mycobacterium tuberculosis* H37Rv.

## Justification

*M. tuberculosis* H37Rv was selected because it has a well-characterised reference genome, extensive published Tn-seq essentiality data, and previous evidence of sub-gene-level essentiality. It is also biologically relevant as a major bacterial pathogen. The availability of high-saturation Tn-seq data makes it suitable for testing whether essential regions overlap with annotated protein domains.

The DeJesus et al. dataset provides a useful benchmark because it was previously used to identify essential-domain-containing genes. However, this project will avoid simply repeating previous work by using it as a validation case while developing a more automated and reusable workflow.

## Initial dataset decision

Primary organism: *Mycobacterium tuberculosis* H37Rv  
Reference genome accession: NC_000962.3  
Assembly accession: GCF_000195955.2  

Initial data to download:
1. Reference genome FASTA
2. Gene annotation GFF3
3. Tn-seq insertion or essentiality data
4. Protein-domain annotations
