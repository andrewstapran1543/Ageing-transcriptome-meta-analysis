# Project report

Here will be text, references and pictures demonstrating the logic of our research. (All code will be placed in a separate notebook.)

style blocks from [jupyter_book](https://jupyterbook.org/en/stable/intro.html) API for making the report more beautiful.

**!!!!!!!!!!!Our Project tasks/questions:**
1) Reproduce the results of the paper. Try to use a maximum of python for conducting meta-analysis. PyMare package can help you.
2) Describe some weak points of the paper (if any).
3) Could you suggest improvements to the approach?
4) Obtain a list of differentially expressed genes across aging. Intersect them with GenAge database. Describe some of these genes.
5) Conduct enrichment analysis.
6) Explain the ML approach used in the paper.

$ perl apply_references.pl References.bib Project report.md



## Introduction

Use the following directive to cite something inside the text of your report \cite{bibtex_citekey}. A useful bibtex guide is here [guide](https://www.bibtex.com/g/bibtex-format/). - ????

In this project, we reproduce the results of a meta-analysis of gene expression in mice reported by Palmer, Daniel et al. in 2021  [palmer2021ageing](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7906136/#SD2). In this study transcriptome signatures of ageing in brain, heart and muscle were derived from 127 public microarray and RNA-Seq datasets from mice, rats, and humans. 
The methodology of ... ...  [de2009meta](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2732303/). 

ML: list of GO terms that are enriched   build decision tree plot to understand wheather - enrichment term on each node of the tree (does the gene belong 
des tree for each gene based on the functional categories - decides if the gene are dif expressed
selected funct categories that predict best if the gene is diff expressed.



## Results

#### Preprocessing of the gene expression data

20 datasets from microarrays brain musce and heard 

in each dataset we have expression of 20000 genes

To estimate differencially expressied genes we build linear regression analysis for all the datasets, the slope of the regression indentifies the coefficien of diff expression. Significance of the dif expr was identified with F test with 0.05 cutoff. 

Cumulative binomial test - to identify genes signif dif expressed across the datasets. 

mets-regression???

#### Meta-analysis of the datasets

Global analysis 
Separately for each tissue 

Regression analysis for each gene - (?) PyMare package - conducts metaanalysis on the results of regression analysis 

$$ Y_{ij} = \beta_{0j} + \beta_{1j}Age_i + \epsilon_{ij}$$


The output: list of genes dif expressed across all datasets

This section is for presenting and describing out results. Put pictures, text, references, formulae and all that you need here. You are free to put code here also but it is quite redundant because you are also preparing the notebook with code and comments. 

Put figures in your report. If some of the pictures were produced with python code, save them in a separate folder within the folder of your project. Use the following directive to put a figure inside the text:

```{figure} figs/hallmarks_taxonomy.png
:name: hallmarks_taxonomy
Hallmarks taxonomy.
```

#### GO enrichment analysis


Use the following directive to refer to a particular picture in the text {numref}`hallmarks_taxonomy`.

## Discussion

#### The genes differentially expressed with age

Discuss your results here and answer additional questions from questions/tasks section of **project proposal**. 

## Credits
This text prepared by [Daria Kozhevnikova](https://linktoyourprofile/scholar/or/linkedin.com) 
The Jupiter Notebook for the data analysis prepared by Andrey Stapran

## References

```{bibliography}
Palmer, Daniel et al. “Ageing transcriptome meta-analysis reveals similarities and differences between key mammalian tissues.” Aging vol. 13,3 (2021): 3313-3341. doi:10.18632/aging.202648

de Magalhães, João Pedro et al. “Meta-analysis of age-related gene expression profiles identifies common signatures of aging.” Bioinformatics (Oxford, England) vol. 25,7 (2009): 875-81. doi:10.1093/bioinformatics/btp073
```

Footer
© 2023 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
