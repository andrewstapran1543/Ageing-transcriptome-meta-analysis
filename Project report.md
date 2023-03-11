# Project report

Here will be text, references and pictures demonstrating the logic of our research. (All code will be placed in a separate notebook.)

style blocks from [jupyter_book](https://jupyterbook.org/en/stable/intro.html) API for making the report more beautiful.


## Introduction

In this project, we reproduce the results of a meta-analysis of gene expression in mice reported by Palmer, Daniel et al. in 2021 [Full text link](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7906136/#SD2).
Our task was to correctly preprocess the gene expression data from their article and apply the meta-analysis technique to the datasets in order to understand which genes are differentially expressed with age. Our hypothesis was ...

Create a separate bibtex file (`.bib` extension) to store the references. Any bibtex reference can be obtained from google scholar by clicking on `cite` button and choosing `bibtex` option. Use the following directive to cite something inside the text of your report {cite}`bibtex_citekey`. A useful bibtex guide is here [guide](https://www.bibtex.com/g/bibtex-format/).

## Results

This section is for presenting and describing out results. Put pictures, text, references, formulae and all that you need here. You are free to put code here also but it is quite redundant because you are also preparing the notebook with code and comments. 

Put mathematical formulae in the report if needed. Use, for example, the following directive for that

$$ y = wx + b$$

Put figures in your report. If some of the pictures were produced with python code, save them in a separate folder within the folder of your project. Use the following directive to put a figure inside the text:

```{figure} figs/hallmarks_taxonomy.png
:name: hallmarks_taxonomy
Hallmarks taxonomy.
```

Use the following directive to refer to a particular picture in the text {numref}`hallmarks_taxonomy`.

## Discussion

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
