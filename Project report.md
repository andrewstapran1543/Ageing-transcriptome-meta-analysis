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





## Introduction

In this project, we reproduce the results of a meta-analysis of gene expression in mice reported by Palmer, Daniel et al. in 2021  {cite}`palmer2021ageing` [Full text link](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7906136/#SD2). In this study transcriptome signatures of ageing were derived from 127 public microarray and RNA-Seq datasets from mice, rats, and humans. 

Create a separate bibtex file (`.bib` extension) to store the references. Any bibtex reference can be obtained from google scholar by clicking on `cite` button and choosing `bibtex` option. Use the following directive to cite something inside the text of your report {cite}`bibtex_citekey`. A useful bibtex guide is here [guide](https://www.bibtex.com/g/bibtex-format/).


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


The output: list of genes dif expressed across all datasets

This section is for presenting and describing out results. Put pictures, text, references, formulae and all that you need here. You are free to put code here also but it is quite redundant because you are also preparing the notebook with code and comments. 

Put mathematical formulae in the report if needed. Use, for example, the following directive for that

$$ y = wx + b$$

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
This text prepared by [Team member 1](https://linktoyourprofile/scholar/or/linkedin.com) ...

## References

```{bibliography}
Palmer, Daniel et al. “Ageing transcriptome meta-analysis reveals similarities and differences between key mammalian tissues.” Aging vol. 13,3 (2021): 3313-3341. doi:10.18632/aging.202648
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



## Introduction

In this project, we reproduce the results of a meta-analysis of gene expression in mice reported by Palmer, Daniel et al. in 2021 {cite}`palmer2021ageing` [Full text link](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7906136/#SD2). In this study transcriptome signatures of ageing were derived from 127 public microarray and RNA-Seq datasets from mice, rats, and humans. 

Create a separate bibtex file (`.bib` extension) to store the references. Any bibtex reference can be obtained from google scholar by clicking on `cite` button and choosing `bibtex` option. Use the following directive to cite something inside the text of your report {cite}`bibtex_citekey`. A useful bibtex guide is here [guide](https://www.bibtex.com/g/bibtex-format/).

ML: list of GO terms that are enriched   build decision tree plot to understand wheather - enrichment term on each node of the tree (does the gene belong 
des tree for each gene based on the functional categories - decides if the gene are dif expressed
selected funct categories that predict best if the gene is diff expressed.


