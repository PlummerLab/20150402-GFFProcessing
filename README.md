# 20150402-GFFProcessing
## Processing GFF output from CodingQuarry

**Author**: Darcy Jones <br />
**Contact**: darcy.ab.jones@gmail.com <br />
**Date**: 02/04/2015 

[CodingQuarry](https://sourceforge.net/projects/codingquarry/) is a gene prediction program optimised for annotating fungal genomes. 
We were having a problem extracting ORF sequences from the GFF output of CodingQuarry because it appears to code some exons as 'CDS' types. 
This notebook converts the type of multiple 'CDS' features with the same parent to 'exon' and recodes the ID appropriately. 
Then coding sequences of genes for each genome is extracted and saved as fasta files as nucleotide and amino acid sequences.

### Required software

This was run with Python 3.4.1 with the following packages:
- bcbio-gff (0.6.2)
- biopython (1.65)
- certifi (14.5.14)
- ipython (3.0.0)
- Jinja2 (2.7.3)
- jsonschema (2.4.0)
- MarkupSafe (0.23)
- pyzmq (14.5.0)
- six (1.9.0)
- tornado (4.1)
- mistune (0.5.1)
- Pygments (2.0.2)

### Relevant literature

Testa, A. C., Hane, J. K., Ellwood, S. R., and Oliver, R. P. 2015. [CodingQuarry: highly accurate hidden Markov model gene prediction in fungal genomes using RNA-seq transcripts.](http://www.biomedcentral.com/1471-2164/16/170) BMC Genomics. 16:1–12
