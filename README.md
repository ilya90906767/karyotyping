# karyotyping
## Introduction
Hello. This repository is presented like a review on the instruments of **Karyotyping (bold)** especially of **aneuploidy detection (bold)**. 

My primary goal - to list all bioinformatics packages/tools/methods for this task and verify them by test data. Also I want to share a benchmark for each tool and specificate situation where you should use each tool. 

____
## Usefull libs and links
`karyoploteR` is good tool for R when you can display many features on chromosomes (Bernat Gel, Eduard Serra, karyoploteR: an R/Bioconductor package to plot customizable genomes displaying arbitrary data, Bioinformatics, Volume 33, Issue 19, October 2017, Pages 3088–3090,https://doi.org/10.1093/bioinformatics/btx346) 

https://doi.org/10.1095/biolreprod.113.116459 

https://www.sciencedirect.com/science/article/abs/pii/S0093775411002995?via%3Dihub 

https://academic.oup.com/bioinformatics/article/38/20/4677/6678978?searchresult=1

https://doi.org/10.1002/pd.4033 
____ 
## Chromosome Representation (CR) method 
This method described in `Li Wang, Xiaohong Wang, Jianguang Zhang, Zhuo Song, Shufang Wang, Yang Gao, Jun Wang, Yaning Luo, Ziru Niu, Xiaojing Yue, Genming Xu, David S. Cram, Yuanqing Yao, Detection of Chromosomal Aneuploidy in Human Preimplantation Embryos by Next-Generation Sequencing, Biology of Reproduction, Volume 90, Issue 5, 1 May 2014, 95, 1–6,` https://doi.org/10.1095/biolreprod.113.116459

For each chromosome GC% and CR were calculated. 

`CR = (count of the reads uniquely mapped to the chromosome of interest)/(total count of the reads uniquely mapped to all the autosomal chromosomes)`

and 

`GC% = (count of G and C in the reads uniquely mapped to the chromosome of interest)/(total count of A, C, G, and T bases in the reads uniquely mapped to the given chromosome of interest)`

`CR = 0,5` represent 1 chromosome copy number (CN) . With each 0,5 CN will increase by 1 chromosome. 
