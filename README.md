# Fault Detection and Classification for Robotic Test-bench: A Data Challenge

Maintenance of industrial systems often cost as much as their initial investment. Implementing predictive maintenance via
system health analysis is one of the strategies to reduce maintenance costs. Health status and life estimation of the machinery
are the most researched topics in this context. In this paper, we present our analysis for [Sixth European Conference of
the Prognostics and Health Management Society 2021 Data Challenge](https://phm-europe.org/2021/data-challenge), which introduces a fuse test bench for qualitycontrol
system, and asks fault detection and classification for the test bench. We proposed classification workflows, which
deploy gradient boosting, linear discriminant analysis, and Gaussian process classifiers, and report their performance for
different window sizes. Our gradient boosting based solution has been ranked 4th in the data challenge.

In this repository we provide Jupyter Notebooks for gradient boosting pipeline for the Data Challange. 
Your results may be different than our results in the paper because of the randomness used in algorithm initializations.

Before you start, you shall download [challenge dataset]((https://phm-europe.org/2021/data-challenge)) and extract that in [input](input) folder. We provide the following notebooks:

* [01_Train_Models](01_Train_Models.ipynb) is used to train XGB based classifier and K-means based cluster models for the challenge tasks.
* [02_TestPerformance](02_TestPerformance.ipynb) is used to test first three tasks of the challenge. As part of the challenge the notebook is modified so as to load models in the previous step.
* [03_ClusterPerformance](03_ClusterPerformance.ipynb) is used to test bonus task of the challenge. As part of the challenge the notebook is modified so as to load models in the previous step.

You can cite our work as follows:

````
@InProceedings{PHME21-GTU,
    author = {Kürşat İnce and Uğur Ceylan and Nazife Nur Erdoğmuş and Engin Sirkeci and Yakup Genç},
    title = {Fault Detection and Classification for Robotic Test-bench: A Data Challenge},
    booktitle = {Proceedings of the European Conference of the PHM Society 2021 },
    month = July,
    year = 2021,
    publisher = {PHM Society},
    editor = {Phuc Do and Steve King and Olga Fink},
    note = {Available at https://papers.phmsociety.org/index.php/phme/article/view/3040}
}
````
