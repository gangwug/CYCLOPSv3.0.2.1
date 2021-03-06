## Introduction

CYCLOPS (Cyclic Ordering by Periodic Structure) is a tool designed to reconstruct the temporal ordering of high dimensional 
that is generated by a common periodic process. Detail descriptions of the CYCLOPS approach can be found online at 
[PNAS](http://www.pnas.org/content/early/2017/04/19/1619320114.full) (Anafi R.C. et al., CYCLOPS reveals human transcriptional
rhythms in health and disease. Proc Natl Acad Sci U S A. 2017. 114(20):5312-5317). The original and in-development version of
CYCLOPS could be found from the GitHub page of Dr. [Ron C. Anafi](https://github.com/ranafi). 

This repository contains the revised CYCLOPS pipleline that was developed to order ~300 human epidermis samples published on 
[PNAS](https://www.pnas.org/content/115/48/12313.long) (Wu G., et al., Population-level rhythms in human skin with implications for circadian medicine. Proc Natl Acad Sci U S A. 2018. 115(48):12313-12318). It was furter improved to order more human epidermis and dermis samples collected from different body sites. 

## Files

RonCYCLOPSv3: the source julia code file from CYCLOPS (julia version 0.3.12)

runCYCLOPS_Eigen.jl: the code file for getting the Eigen genes

runOscope.R: the code file for selecting Eigen clusters

runCYCLOPS_Order.jl: the code file for ordering

clockList.csv: the input seed gene list for ordering

CYCLOPSout: the output folder for CYCLOPS ordering

example.ToRunCYCLOPS.csv: an example of expression data

skinBenchmarkMatrixARNTLorder.csv: the benchmark correlation matrix used for down-sampling (minor different from the 17 clock and clock-associated genes, which may be helpful for avoiding the bias of using the same 17 seed gene list during ordering)

randomSampling.R: the code file for maximizing the oscillation signal by down-sampling

## License
This package is free and open source software, licensed under GPL(>= 2).

