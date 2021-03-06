## BTN707 2021 Fall - Computational Genomics

### Term project guideline

* Windows10 users - if you like to use `linux` (unix) environment, install [WSL Windows Subsystem for Linux](https://docs.microsoft.com/ko-kr/windows/wsl/install)
* For python coding: use following tools (optional) 
  * [`conda`](https://www.anaconda.com/products/individual) - virtual environment control
    * [conda tutorial](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html) 
  * [`Pycharm`](https://www.jetbrains.com/ko-kr/pycharm/download/) - Integrated Development Environment (IDE), 통합개발환경
    * [pycharm tutorial](https://www.jetbrains.com/help/pycharm/quick-start-guide.html) 
* All individual projects will be maintained in the [Github `BTN707` repository](https://github.com/choilab/2021-compgen-class/)
  * What is `Git` and `Github`?
    * [생활코딩 Git](https://opentutorials.org/module/3733/22434)
    * [What is `Github`?](https://www.youtube.com/watch?v=w3jLJU7DT5E)
    * __it is not an obligation__
* Use `markdown` for documentation
  * [Markdown tutorial](https://guides.github.com/features/mastering-markdown/)
  * [Markdown tutorial - Korean](https://github.com/biospin/BigBio/blob/master/reference/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4.md)
* You can use [`jupyter notebook`](https://jupyter.org/) too
* Check [library](https://library.korea.ac.kr/) - there are plenty of reference books for python codings
* __Evaluation is on your *activity* rather than your *performance* (e.g. how frequently commit/update your codes/documents/discussions)__ 

---
### Term projects 
- You can choose following topics or suggest your own term project
- In following weeks, everyone will present and discuss about his/her intro/progress/issues/results, including 
  - i) what is the problem to solve? (_topic description/introduction_), 
  - ii) why is it important? (_biological meaning_), 
  - iii) how it can be solved (_algorithms/procedures_) - _how do you solve the problem?_ 
- Some projects are mostly related to `indexing` and `pattern matching` of sequences, which was handled in the previous class hours.

---
1. CRISPR Genome Editing - Prediction of On/Off Target & gRNA designer
   - Input: genome sequence/target gene/oligo (.fna/.fasta nucleotide)
   - Output: target/off-target site (.coordinate)
   - Options: # of mismatches/positional mismatches/insertion/deletion/base ambiguity
   - Thinkabouts: i) what is the problem to solve?, ii) why is it important? (biological meaning), iii) how can you design/build/test?... 
   - Example program & literature[^offfinder] - [CAS-off-finder http://www.rgenome.net/cas-offinder/](http://www.rgenome.net/cas-offinder/)
   [^offfinder]:[Cas-OFFinder: a fast and versatile algorithm that searches for potential off-target sites of Cas9 RNA-guided endonucleases](https://academic.oup.com/bioinformatics/article/30/10/1473/267560)

---
2. Anti-sense oligonucleotide (ASO) off-target finder - Almost similar to CAS9-off-finder
   - Input: target genome sequence/oligo sequence (.fna/.fasta nucleotide)
   - Output: target/off-target site (.coordinate)
   - Options: # of mismatches/positional mismatches/insertion/deletion/base ambiguity
   - Thinkabouts: i) what is the problem to solve?, ii) why is it important? (biological meaning), iii) how can you design/build/test?... 
   - Example program & literature[^gggenome] - [GGGenome https://gggenome.dbcls.jp/](https://gggenome.dbcls.jp/)
   [^gggenome]:[Evaluation of off‐target effects of gapmer antisense oligonucleotides using human cells](https://onlinelibrary.wiley.com/doi/full/10.1111/gtc.12730)

---
3. Open Reading Frame (ORF) finder
   - Input: microbial genome sequence (.fna/.fasta nucleotide)
   - Output: All possible open reading frames (.faa amino acids/.coordinate)
   - Options: strandedness/ATG/no-ATG
   - Thinkabouts: i) what is the problem to solve?, ii) why is it important? (biological meaning), iii) how can you design/build/test?... 
   - Example program & literature[^orffinder] - [ORFfinder https://www.ncbi.nlm.nih.gov/orffinder/](https://www.ncbi.nlm.nih.gov/orffinder/)
   [^orffinder]:[Borf: Improved ORF prediction in de-novo assembled transcriptome annotation](https://www.biorxiv.org/content/10.1101/2021.04.12.439551v1.full)

---
4. Gene Assembly Designer
   - Input: gene/gene cluster/chromosome
   - Output: a pool of variable lengths of oligos/fragments (overlapped) for synthetic full gene
   - Options: ssDNA/dsDNA/overlap length/# of fragments/restriction site removal
   - Thinkabouts: i) what is the problem to solve?, ii) why is it important? (biological meaning), iii) how can you design/build/test?... 
   - Example program & literature[^geneassembler] - [Assmebly PCR oligo Maker](https://academic.oup.com/nar/article/33/suppl_2/W521/2505480)
   [^geneassembler]:[Assembly of Designed Oligonucleotides: a useful tool in synthetic biology for creating high-quality combinatorial DNA libraries](https://pubmed.ncbi.nlm.nih.gov/25055779/)


