---
title: Welcome to Dev Chakraborty's AI/FROC Research
---

# Overview

This website is intended as a documentation and blogging platform for my AI/FROC research interests. 

# Glossary

* AI = Artificial Intelligence, formerly known as CAD (in the medical imaging context); 
* CAD = Computer Aided Detection;
* FROC = Free-response Receiver Operating Characteristic, data collected in a visual search task;
* ROC = Receiver Operating Characteristic, data collected in a binary classification task.


# Four repositories

* This website describes four [repositories](https://github.com/dpc10ster) addressing **observer performance and artificial intelligence systems modeling, analysis and validation**. Three of the repositories contain the source codes for online books.
* The repositories are:
    + [`RJafroc`](https://dpc10ster.github.io/RJafroc/) is the `R` software package that provides the common thread on which the online books depend; 
    + [`RJafrocQuickStart`](https://dpc10ster.github.io/RJafrocQuickStart) is an online book for those already somewhat familiar running Windows JAFROC. The obsolete Windows program has been replaced by `RJafroc`. This book dives into how to use `RJafroc` to analyze ROC or FROC datasets;
    + [`RJafrocRocBook`](https://dpc10ster.github.io/RJafrocRocBook) is an online book providing background on the ROC paradigm, modeling and analysis; 
    + [`RJafrocFrocBook`](https://dpc10ster.github.io/RJafrocFrocBook/) is an online book providing a detailed exposition of the FROC paradigm, modeling and analysis.

# History

The first CRAN-posted version of `RJafroc` was used to support the R-code examples in the book: Chakraborty DP: Observer Performance Methods for Diagnostic Imaging - Foundations, Modeling, and Applications with R-Based Examples, Taylor-Francis LLC, 2017. 

Since its publication in 2017 `RJafroc`, on which the `R` code examples in the print book depend, has evolved considerably, causing many of the examples to "break" if one uses the most current version of `RJafroc`. The code will still run if one uses [`RJafroc` 0.0.1](https://cran.r-project.org/src/contrib/Archive/RJafroc/) but this is sub-optimal as it misses out on many of the software improvements made since the print book appeared.

Unlike the print book the online books described in the links contain embedded R code (using the `bookdown` R package). Accordingly the books and the software are automatically synchronized and any software inconsistencies will throw errors in GitHub Actions, see [here](https://github.com/dpc10ster/RJafrocFrocBook/actions) for an example. 

The first CRAN-posted version of `RJafroc` was used to support the R-code examples in the book: Chakraborty DP: Observer Performance Methods for Diagnostic Imaging - Foundations, Modeling, and Applications with R-Based Examples, Taylor-Francis LLC, 2017. 

Since its publication in 2017 `RJafroc`, on which the `R` code examples in the print book depend, has evolved considerably, causing many of the examples to "break" if one uses the most current version of `RJafroc`. The code will still run if one uses [`RJafroc` 0.0.1](https://cran.r-project.org/src/contrib/Archive/RJafroc/) but this is sub-optimal as it misses out on many of the software improvements made since the print book appeared.

Unlike the print book the online books described in the links contain embedded R code (using the `bookdown` R package). Accordingly the books and the software are automatically synchronized and any software inconsistencies will throw errors in GitHub Actions, see [here](https://github.com/dpc10ster/RJafrocFrocBook/actions) for an example. 

This, and other considerations, led me to conclude that an update to the book is needed. 

This website links to the latest software and three online books that use the software and extend the 2017-book. 

The online books are under development and parts marked TBA (to be added) should be ignored. Each chapter has a **How Much Finished (HMF)** section giving a rough idea of the extent to which that chapter has been completed.


# Documentation

* HTML documentation for `RJafroc` (functions and update history) is available [here](https://dpc10ster.github.io/RJafroc/). The software is fairly stable and undergoing occasional updates. 

* The HTML online book `RJafrocQuickStart` is available [here](https://dpc10ster.github.io/RJafrocQuickStart/). 
* Go [here](https://github.com/dpc10ster/RJafrocQuickStart/blob/gh-pages/RJafrocQuickStart.pdf) and then click on `Download` to get the `RJafrocQuickStart.pdf` file. 
* Both are being continually updated (as of December 2022).  

* The HTML online book `RJafrocRocBook` is available [here](https://dpc10ster.github.io/RJafrocRocBook/). Go [here](https://github.com/dpc10ster/RJafrocRocBook/blob/gh-pages/RJafrocRocBook.pdf) and click on `Download` to get the `RJafrocRocBook.pdf` file. Both are being continually updated (as of December 2022).  


* The HTML online book `RJafrocFrocBook` is available [here](https://dpc10ster.github.io/RJafrocFrocBook/). Go [here](https://github.com/dpc10ster/RJafrocFrocBook/blob/gh-pages/RJafrocFrocBook.pdf) and then click on `Download` to get the `RJafrocFrocBook.pdf` file. Both are being continually updated (as of December 2022).  



# Applications

While most of the applications in this package are geared toward analyzing radiologist performance in search tasks such as finding lesions in medical images, the software applies to any task involving detection and localization of targets in images. For example, the functions in `RJafroc` can be used to analyze the performance of artificial intelligence (AI) algorithms. Two applications to AI are [here](https://dpc10ster.github.io/RJafrocFrocBook/), specifically:

* Measuring AI performance.
* Optimizing the reporting threshold of an AI algorithm.

The radiological search model (RSM), described [here](https://dpc10ster.github.io/RJafrocFrocBook/) is implemented in `RJafroc`. A fitting function `RJafroc::FitRsmRoc` estimates RSM parameters from ROC data These parameters are related to search and classification performances: 

* Search performance refers to finding lesions while simultaneously minimizing finding non-lesion locations 
* Classification performance measures ability to distinguish between lesion and non-lesion locations. 

Knowing the individual performances allows principled optimization of reader or AI algorithm performance.

# Relation to Windows software

* `RJafroc` extends Windows `JAFROC` software and runs on multiple platforms.
* Originally uploaded in 2004, the Windows software is many generations behind the software available on this website. However, many users find it to be easy to use and useful. Vignettes in `RJafroc` and the online book available [here](https://dpc10ster.github.io/RJafrocQuickStart/) should allow one to quickly transition to `RJafroc`.
* If you still need Windows `JAFROC` software it is still available [here](https://github.com/dpc10ster/WindowsJafroc).



This, and other considerations, led me to conclude that an update to the book is needed. 

This website links to the latest software and three online books that use the software and extend the 2017-book. 

The online books are under development and parts marked TBA (to be added) should be ignored. Each chapter has a **How much finished** section giving a rough idea of the extent to which that chapter has been completed.


# Documentation

* HTML documentation for `RJafroc` (functions and update history) is available [here](https://dpc10ster.github.io/RJafroc/). The software is fairly stable and undergoing occasional updates. 

* The HTML online book `RJafrocQuickStart` is available [here](https://dpc10ster.github.io/RJafrocQuickStart/). A link is provided there to download the pdf book. Both are being continually updated (as of December 2021).  

* The HTML online book `RJafrocRocBook` is available [here](https://dpc10ster.github.io/RJafrocRocBook/). A link is provided there to download the pdf book. Both of them are being continually updated.  

* The HTML online book `RJafrocFrocBook` is available [here](https://dpc10ster.github.io/RJafrocFrocBook/). A link is provided there to download the pdf book. Both are being continually updated.  


# Applications

While most of the applications in this package are geared toward analyzing radiologist performance in search tasks such as finding lesions in medical images, the software applies to any task involving detection and localization of targets in images. For example, the functions in `RJafroc` can be used to analyze the performance of artificial intelligence (AI) algorithms. Two applications to AI are [here](https://dpc10ster.github.io/RJafrocFrocBook/), specifically:

* Measuring AI performance.
* Optimizing the reporting threshold of an AI algorithm.

The radiological search model (RSM), described [here](https://dpc10ster.github.io/RJafrocFrocBook/) is implemented in `RJafroc`. A fitting function `RJafroc::FitRsmRoc` estimates RSM parameters from ROC data These parameters are related to search and classification performances: 

* Search performance refers to finding lesions while simultaneously minimizing finding non-lesion locations 
* Classification performance measures ability to distinguish between lesion and non-lesion locations. 

Knowing the individual performances allows principled optimization of reader or AI algorithm performance.


