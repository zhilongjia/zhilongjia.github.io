---
title: 'metabolite protein interaction network'
date: 2021-07-14
permalink: /posts/2021/07/MPI/
tags:
  - metabolite
  - protein
  - interaction
  - network
  - article
---

# A Metabolite-protein interactions (MPIs) dataset

By extracting and integrating MPIs from KEGG, Reactome, Human-GEM and BRENDA, the author build a directed MPI network.  
* 31236 unique MPIs covering 1870 metabolites and 4132 proteins (represented by the encoding genes)

"Most of the metabolite-interacting proteins (MIPros) belonged to metabolism pathways, some of them also participated in the other aspects like endocrine system, signal transduction, as well as immune system, highlighting that **metabolites can participate in various cellular processes via interactions with a variety of proteins.**"

The MPI data is [Table S1](https://onlinelibrary.wiley.com/action/downloadSupplement?doi=10.1002%2Fadvs.202100311&file=advs2770-sup-0002-TableS1.csv) .

Examples:

|a	      |b	      |two	   |From|	aids|	direction|
--- | --- | ---| --- | ---| ---
|Caffeine |	CYP1A2|	Caffeine CYP1A2|	Reactome|	C07481|	C07481 CYP1A2|
|Hydrogen Ion	|CYP1A2| 	Hydrogen Ion CYP1A2|	Reactome &GEM|	C00080|	C00080 CYP1A2;CYP1A2 C00080|

# PMI database

"A total of 49 785 entries were manually collected in the PMI-DB, corresponding to 23 small molecule metabolites, 9631 proteins and 4 species."

# References:

* [Chen D, Zhang Y, Wang W, Chen H, Ling T, Yang R, Wang Y, Duan C, Liu Y, Guo X, Fang L, Liu W, Liu X, Liu J, Otkur W, Qi H, Liu X, Xia T, Liu HX, Piao HL. Identification and Characterization of Robust Hepatocellular Carcinoma Prognostic Subtypes Based on an Integrative Metabolite-Protein Interaction Network. Adv Sci (Weinh). 2021 Jul 11:e2100311. doi: 10.1002/advs.202100311. Epub ahead of print. PMID: 34247449.](https://onlinelibrary.wiley.com/doi/10.1002/advs.202100311#)

* [Zhao T, Liu J, Zeng X, Wang W, Li S, Zang T, Peng J, Yang Y. Prediction and collection of protein-metabolite interactions. Brief Bioinform. 2021 Feb 8:bbab014. doi: 10.1093/bib/bbab014. Epub ahead of print. PMID: 33554247.](https://academic.oup.com/bib/advance-article-abstract/doi/10.1093/bib/bbab014/6130169?redirectedFrom=fulltext)
* [PMI database](http://easybioai.com/PMIDB/home)
