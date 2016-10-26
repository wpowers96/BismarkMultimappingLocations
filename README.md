# BismarkMultimappingLocations
This is a side-project of Bismark whose aim is to output multiply mapping read positions without any of the methylation specific features. I have included a new option call `--limit_multimapping` which sets the maxiumum number of alignments per thread, so the `--limit 20` would print up to 40 alignments in total, 20 for OT and 20 for OB for a default run. The option `--ambig_bam` is set by default. 

This script is highly experimental and works only for Bowtie2, single-end alignments for which we have set the parameter `-a`. Good luck!



An example USAGE is:

./bismarkMultimappingPositions --genome /bi/scratch/Genomes/Arabidopsis/TAIR10/ test.fq.gz --limit 20