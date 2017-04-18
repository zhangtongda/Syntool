Syntool README file

Syntool is a novel region-based intolerance score to single nucleotide substitution variation for synonymous mutations predictions.


##usage

##download 

##generate the index file by tabix

tabix -p bed Syntool.bed.gz

##predict the mutation: tabix Syntool.bed.gz chrom:start-end 

tabix Syntool.bed.gz chr1:103444941-103444941



