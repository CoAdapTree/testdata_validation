# Testdata validation

Code used to validate allele frequency estimates from our poolSeq data by comparing estimates from the same individual sequence data, as well as to validate megaSNPs as likely regions where paralogs are likely misaligning and causing false positive SNPs in our data.

---
Below are the descriptions of notebooks in this repo. These notebooks are best viewed at https://nbviewer.jupyter.org using the github web address to each notebook. Notebooks 002 and 003 contain figures found in the main and supplemental texts.

__001_testdata_explore.ipynb__

Explore the data, isolate the set of SNPs intersecting both baseline-filtered datasets across both Doug-fir and Jack pine.

__002_testdata_compare_AFs.ipynb__

This notebook takes SNPs intesecting indSeq and poolSeq methods for Doug-fir and Jack pine from (001_testdata_explore.ipynb) and investigates filtering methods that will improve agreement between indSeq and poolSeq estimates.

__003_testdata_validate_megaSNPs.ipynb__

Validate sites that are called as heterozygote from haploid tissue as those potentially within a region subject to paralog misalignment.

---

### Usage    

If you use or are inspired by code from this repo, please site related manuscripts (update to follow).
