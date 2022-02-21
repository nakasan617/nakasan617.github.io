---
layout: page
title: Publications 
permalink: /publications/
---

Below are the published work I have so far

### Content Defined Merkle Tree (2021) ###
As I was to implement Merkle tree in [Sciunit](https://sciunit.run/), I realized that Merkle tree cannot be used for blocks that are created with Content-Defined Chunking method. Therefore we came up with the idea of CDMT, which does the Content-Defined Chunking in the internal nodes. This data structure is now robust against the chunk-shift, which occurs using the Merkle trees on top of content-defined chunks. 

[Link to CDMT](https://arxiv.org/abs/2104.02158#:~:text=Containerization%20simplifies%20the%20sharing%20and,push%20and%20pull%20container%20images.)

### Efficient Provenance Alignment in Reproduced Executions (2020) ###
[SPADE](https://github.com/ashish-gehani/SPADE) and Sciunit use system calls to trace the provenance of the executions. Therefore this is our first attempt to look at the system call trace to make sure the two executions are aligned. 

[Link to Provenance Alignment](https://www.usenix.org/conference/tapp2020/presentation/nakamura)
