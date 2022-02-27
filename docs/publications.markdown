---
layout: page
title: Publications 
permalink: /publications/
---
<!--
dropDownAbstract is a class name
-->
<head>
    <meta charset="utf-8">
    <link href="{{site.baseurl}}/css/publications.css" rel="stylesheet">
    <script type="text/javascript">
        /* When the user clicks on the button,
        toggle between hiding and showing the dropdown content */
        function openAbstract() {
          document.getElementById("abstract-dropdown").classList.toggle("show");
        }
        function openBibtex() {
          document.getElementById("bibtex-dropdown").classList.toggle("show");
        }

        // Close the dropdown menu if the user clicks outside of it
        window.onclick = function(event) {
          if (!event.target.matches('.dropbtn')) {
            var dropdowns = document.getElementsByClassName("dropdown-content");
            var i;
            for (i = 0; i < dropdowns.length; i++) {
              var openDropdown = dropdowns[i];
              if (openDropdown.classList.contains('show')) {
                openDropdown.classList.remove('show');
              }
            }
            
          }
        }
    </script>
</head>
<p>
Below are the published work I have so far
</p>

<h3 class="papertitle" id="cdmt"> Content Defined Merkle Tree (2021) </h3> 

<p>
As I was to implement Merkle tree in [Sciunit](https://sciunit.run/), I realized that Merkle tree cannot be used for blocks that are created with Content-Defined Chunking method. Therefore we came up with the idea of CDMT, which does the Content-Defined Chunking in the internal nodes. This data structure is now robust against the chunk-shift, which occurs using the Merkle trees on top of content-defined chunks. 
</p>
<p>
<a href="https://arxiv.org/abs/2104.02158#:~:text=Containerization%20simplifies%20the%20sharing%20and,push%20and%20pull%20container%20images.">Link to CDMT</a>
</p>

<h3 class="papertitle" id="provenanceAlignment">Efficient Provenance Alignment in Reproduced Executions (2020)</h3> 

<p>
<a href="https://github.com/ashish-gehani/SPADE">SPADE</a> and Sciunit use system calls to trace the provenance of the executions. Therefore this is our first attempt to look at the system call trace to make sure the two executions are aligned. 
</p>
<p>
<a href="https://www.usenix.org/conference/tapp2020/presentation/nakamura)
">Link to Provenance Alignment</a>
</p>

<!--
<ol class="bibliography">
<li><b>Nakamura, Y.</b>, Raza, A, Malik, T, Sampath, D., &amp; Coombes, K. R. (2019). <i>Identification and comparison of genes differentially regulate by transcription factors and miRNAs</i>. 
<button onclick="openAbstract()" class="dropbtn">Abstract</button>
<button onclick="openBibtex()" class="dropbtn">BibTeX</button>

    <div class="dropdown-content" id = "abstract-dropdown">
    Transcription factors and microRNAs (miRNA) both play a critical role in gene regulation and in the development of many diseases such as cancer. Understanding how transcription factors and miRNAs influence gene expression is thus important to understand, but complicated due to the large and interconnected nature of the human genome. To help better understand what genes are being regulated by transcription factors and/or miRNAs we looked at it over 8000 patient samples from 32 different cancer types collected from The Cancer Genome Atlas (TCGA). We started by clustering the transcription factors and miRNAs using Thresher to reduce the number of features. Using both the mRNA and miRNA sequencing data we constructed linear models to calculate the coefficient of determination (R2) for each mRNA based on the Thresher cluster expression. We generated three types of linear models: transcription factor, miRNA and transcription factor plus miRNA. We then determined genes that were highly explained or poorly explained by each of the three models based on the genes R2 value. We performed downstream gene enrichment analysis using ToppGene on the sets of well and poorly explained genes. This identified differences in gene regulation between transcription factors and miRNAs and showed what groups of gene are differentially regulated.
    </div>

    <div class="dropdown-content" id="bibtex-dropdown">
        <pre>@article{aans19a,
      title = {Identification and comparison of genes differentially regulated
                    by transcription factors and {miRNAs}},
      author = {Asiaee*, Amir and Abrams*, Zachary B and Nakayiza, Samantha and Sampath, Deepa and Coombes, Kevin R},
      archiveprefix = {bioRxiv},
      eprint = {803643},
      note = {https://doi.org/10.1101/803643},
      year = {2019}
    }
        </pre>
    </div>

-->
