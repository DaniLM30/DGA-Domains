# DGA-Domains
Repository containing DGA generated domains and Alexa Top 1 Million Domains from 2017.

To build this file, samples from the following datasets available online have been merged and analyzed:
1. UMUGDA Dataset: https://data.mendeley.com/datasets/y8ph45msv8/1
2. Johannes Bader GitHub Repository: https://github.com/baderj/domain_generation_algorithms
3. NetLab 260 Dataset: https://data.netlab.360.com/dga/

## DGA_Malware_Domains Folder
This folder contains 69 text files corresponding to each of the malware families that use DGA algorithms.

## Datasets_Comparison File
In this .xlsx file you will find 8 different sheets containing the following:

* Malware Families: This sheet shows all the malware families collected by each of the three datasets, highlighting with a different color those families that exist exclusively in a single dataset.
* Samples (Duplicated): This sheet contains the compilation by families of all the domain name samples, indicating in the first column to which dataset they belong. In this sheet there may be duplications of domain names between different datasets.
* Samples (Uniques): This sheet is exactly the same as the previous one, but with the particularity that the duplicates of the samples between datasets have been eliminated. Therefore, this sheet is the most complete and the one that could be most useful for the implementation of defense mechanisms.
* Common Samples (Duplicated): This sheet has the information of the Samples (Duplicates) sheet filtered to show only those families that belong to the 3 datasets simultaneously. The first column indicates the dataset to which each sample belongs, so there may be duplicate domain names.
* Common Samples (Uniques): This sheet is the result of the duplicate filter on the previous sheet, leaving only unique samples of the families common to all datasets.
* Common Samples (TLDs): This is another of the sheets that provide more information to the analysis, since in it we can see the TLDs used by each malware family of those that are common to the 3 datasets. Through this tab we can see the most common TLDs and thus plan the defense strategy with greater knowledge.
* Benigns: This tab only compiles the Alexa Top 1 Million Sites listing mentioned above.
* Statistics: Finally, the statistics tab shows the result of the analysis of the main characteristics of the different malware families. Thus, it shows in a summarized form much of the relevant information to be taken into account when dealing with the different DGAs.
