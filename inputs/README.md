Input data
==========

To subsample input data:

1. Get the number of rows of the fastqc file

```
wc -l SRR11517680.fastq
```

The reads number is given by the number of rows obtained by the previous command divided by 4.

2. Divide the number of rows in fastq by whatever multiple of 4 yuo need:

```
head -n 200000 SRR11517680.fastq > SRR11517680_test.fastq 
```
