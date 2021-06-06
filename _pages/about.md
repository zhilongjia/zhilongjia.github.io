---
permalink: /
title: "Mainpage of Zhilong Jia"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am an Assistant Professor in Chinese PLA General Hospital after obtaining a doctor of philosophy degree in biomedical engineering. My research interest is drug repositioning and bioinformatics. I developed drug repositioning methods, such as cogena, and applied them into cardiovascular disease, periodontal disease, mountain sickness and COVID-19.

Selected papers with Reproducible codes:
======
* _2020_ [Transcriptome-based drug repositioning for coronavirus disease 2019 (COVID-19)](https://academic.oup.com/femspd/article/78/4/ftaa036/5871823)
   + **Reproducible research**: [code](https://github.com/zhilongjia/COVID-19)
   
* _2020_ [Heightened Innate Immune Responses in the Respiratory Tract of COVID-19 Patients](https://www.sciencedirect.com/science/article/pii/S1931312820302444?via%3Dihub)
   + **Reproducible research (only related to my contributions)**: [code](https://github.com/zhilongjia/nCoV2019)

* _2019_ [Time-Course Transcriptome Analysis for Drug Repositioning in *Fusobacterium nucleatum*-Infected Human Gingival Fibroblasts](https://www.frontiersin.org/articles/10.3389/fcell.2019.00204/full) or [PubMed](http://www.ncbi.nlm.nih.gov/pmc/articles/pmc6771468/)
    + **Reproducible research**: [code](https://github.com/zhilongjia/Fn_HGFcell)


* _2019_ [Transcriptional profiling in the livers of rats after hypobaric hypoxia exposure.](https://peerj.com/articles/6499/)
    + **Reproducible research**: [code](https://github.com/zhilongjia/AMS_gut_liver_rat)

* _2016_ [Cogena, a novel tool for co-expressed gene-set enrichment analysis, applied to drug repositioning and drug mode of action discovery](http://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-016-2737-8)
    + **cogena**: [code](https://github.com/zhilongjia/cogena) or [Bioconductor](http://www.bioconductor.org/packages/devel/bioc/html/cogena.html)
    + **Reproducible research**: [code](https://github.com/zhilongjia/psoriasis)

*  _2015_ [Gene Ranking of RNA-Seq Data via Discriminant Non-Negative Matrix Factorization (DNMF)](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0137782)
    + **DNMF package**: [CRAN](https://cran.r-project.org/web/packages/DNMF/index.html)
    + **Reproducible research**: [code](https://github.com/zhilongjia/geneRanking)


Meeting with slides:
======
* [Drug repositioning based on coexpressed gene-set enrichment analysis (cogena)](https://github.com/zhilongjia/slides/blob/master/eurobioc2015_FlashlightII_cogena_ZhilongJia.pdf) at [European Bioconductor Developers' Conference 2015](https://sites.google.com/site/eurobioc2015/)

* [Co-expressed gene-set enrichment analysis for drug repositioning with examples of psoriasis and periodontal diseases](https://github.com/zhilongjia/slides/blob/master/ZhilongJia-BDF20191013-v7.pdf) at [The 4th Big Data Forum for Life and Health Sciences 2019](https://bigd.big.ac.cn/conference/bdf2019)

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

