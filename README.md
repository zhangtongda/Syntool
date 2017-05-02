Syntool README file

Syntool is a novel region-based intolerance score  to single nucleotide substitution variation for synonymous mutations predictions. By compared with previous intolerance score (ExAC gene constraint Z score for synonymous), Syntool score can better discriminate synonymous variation in Human Gene Mutation Database (HGMD Professional) and clinvar database that do and do not cause disease.


##usage

##download 

##generate the index file by tabix

tabix -p bed Syntool.bed.gz

##using the GRCh37/hg19 coordinate for a synonymous variant to retrieve its Syntool score. like this: tabix Syntool.bed.gz chrom:start-end 

tabix Syntool.bed.gz chr1:103444941-103444941

##for the result, Syntool scores range from -28.62567126 to 59.26623025. The smaller the score the more likely the SNP has damaging effect. If a Syntool score is <=0 (or score percentile <=0.5) the corresponding mutation is predicted as cause disease-causing.



