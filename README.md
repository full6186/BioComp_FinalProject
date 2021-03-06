# BioComp_FinalProject
Scripts&amp;Products for Intro2BioComp Winter 2017 Quarter

Structure is a Bayesian clustering algorithm commonly used in population genetic studies (Pritchard et al., 2000). In fact, this program has been cited more than 10k times in the scientific literature (Puechmaille, 2016). Inferring the genetic structure of subpopulations is an important facet of many laboratories spanning multiple fields of evolutionary and ecological studies. The interest of subpopulations, or K-clusters, in genetic data has given rise to multiple methods of K-estimation(Puechmaille, 2016). During my Master's studies, I used microsatellite markers to capture genetic diversity in populations of a wild mountain flower of the North American west known as Gunnison's Sego Lily (Calochortus gunnisonii). Using the population clustering algorithm of the Structure program (Pritchard et al., 2000), combined with that of the highly popular Evanno Method (4,000+ citations; Puechmaille, 2016) as a K estimator, my data suggests a value of K=2 and further evidence of K=5 (Fuller and McGlaughlin, unpublished). However, some disparate sampling exists between populations, and Puechmaille, 2016 presents and tests four new methods for K-estimation in simulated and empirical datasets. His results suggest that these new methods may perform more accurately as estimators of K-clusters than the Evanno method when sampling is uneven. Using the supplementary materials of Puechmaille as a guide, I have embarked upon my first coding project to automate this K-estimation using Python. An R-code does exist and is written by Sebastian Puechmaille (find it here: http://batlab.ucd.ie/~spuechmaille/).

The following is code written to import Structure Results text files, cut out the block of data desired, and iterate/analyze all files in a user's 'Results' directory. This code is able to detect the number user-defined populations, K-clusters, and iterations -- providing an output for the MaxMean method created by Sebastian Puechmaille, 2016. It is suggested that researchers exhaustively examine their genetic data and clustering landscape by utilizing multiple K-means methods and ensure their conclusions are biologically realistic given their organism's natural history (Puechmaille, 2016).

Please find four compilations of code in this GitHub directory that estimate K. Useful guidance comments have been included in the coding block to assist the user. For my data involving C. gunnisonii, the 'MaxMean' method produced a best value of K=8. This will require further testing and vetting against other K-cluster algorithms.

Resources

Pritchard JK, Stephens M, Donnelly P (2000) Inference of population structure using multilocus genotype data. 
Genetics, 155, 945–959.

Puechmaille SJ (2016) The program STRUCTURE does not reliably recover the correct population structure when sampling is uneven: subsampling and new estimators alleviate the problem. Molecular Ecology Resources, 16, 608-627. (doi: 10.1111/1755-0998.12512)

**Since GitHub only allows me to upload 100 files from my Results Folder, I have included 15 iterations of K values 1-7 in my original dataset (90 files).
