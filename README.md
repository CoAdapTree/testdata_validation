# Testdata validation

Code used to validate allele frequency estimates from our poolSeq data by comparing estimates from the same individual sequence data, as well as to validate megaSNPs as likely regions where paralogs are likely misaligning and causing false positive SNPs in our data.

---

### Usage    

If you use or are inspired by code from this repo, please site related manuscripts and data (update for code deposition to follow):

Data
- NCBI Bioproject PRJNA744263 - https://www.ncbi.nlm.nih.gov/bioproject/PRJNA744263/
- Dryad - contains all filtered SNP calls, pipeline config files, and metadata for SRA and Biosamples - https://doi.org/10.5061/dryad.k0p2ngf7w
- Zenodo - contains an archived release of this repository

Lind et al. (in press) Haploid, diploid, and pooled exome capture recapitulate features of biology and paralogy in two non-model tree species. Accepted to Molecular Ecology Resources. Available on bioRxiv https://doi.org/10.1101/2020.10.07.329961

---

### Repository structure

Below are the descriptions of notebooks in this repo. Notebooks can be viewed in the repository but are best viewed at https://nbviewer.jupyter.org (hyperlinks below). Notebooks 002 and 003 contain figures found in the main and supplemental texts.

[__Full repository__](https://nbviewer.jupyter.org/github/CoAdapTree/testdata_validation/tree/master/)

[__001_testdata_explore.ipynb__](https://nbviewer.jupyter.org/github/CoAdapTree/testdata_validation/blob/master/001_testdata_explore.ipynb)

Explore the data, isolate the set of SNPs intersecting both (indSeq and pooLSeq) baseline-filtered datasets across both Doug-fir and Jack pine.

[__002_testdata_compare_AFs.ipynb__](https://nbviewer.jupyter.org/github/CoAdapTree/testdata_validation/blob/master/002_testdata_compare_AFs.ipynb)

This notebook takes SNPs intesecting indSeq and poolSeq methods for Doug-fir and Jack pine from (001_testdata_explore.ipynb) and investigates filtering methods that will improve agreement between indSeq and poolSeq estimates.

[__003_testdata_validate_megaSNPs.ipynb__](https://nbviewer.jupyter.org/github/CoAdapTree/testdata_validation/blob/master/003_testdata_validate_megaSNPs.ipynb)

Validate sites that are called as heterozygote from haploid tissue as those potentially within a region subject to paralog misalignment.

[__004_misc_suppmat.ipynb__](https://nbviewer.jupyter.org/github/CoAdapTree/testdata_validation/blob/master/004_misc_suppmat.ipynb)

Calculate some numbers for some tables and the Supplemental Material

[__005_transfer_to_SRA.ipynb__](https://nbviewer.jupyter.org/github/CoAdapTree/testdata_validation/blob/master/005_transfer_to_SRA.ipynb)

Code to create SRA metadata, Biosample metadata, and to upload fastq files to NCBI Short Read Archive ftp with python


---

`pythonimports` in notebooks can be found here: https://github.com/brandonlind/pythonimports
