# MammaryGenomics

Genomic profiling of mouse mammary epithelial cells

Milevskiy, Coughlan and Visvader et al, Cell Genomics 2023 <br>
<strong>Three-dimensional genome architecture coordinates key regulators of lineage specification in mammary epithelial cells</strong> <br>

<a href="https://doi.org/10.1016/j.xgen.2023.100424"> Please cite out paper</a> <br>
<a href="https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE227750"> Raw data: GSE227750</a>
<br>

<img src="https://github.com/mmilevskiy/MammaryGenomics/blob/e51bd044029a9459e63541fecafe6f37c81725cf/EpiAtlas%20Methods%20Overview.png" alt="Graphical abstract">

We profiled genomics and transcriptomic attributes of mammary epithelial cells (MECs) sorted from mouse mammary glands. We provide bulk level data for five cellular populations: <br>
<ol>
  <li>Basal: lin–CD29hiCD24+ (ba)</li>
  <li>Luminal progenitor: lin–CD29loCD24+CD61hi (LP)</li>
  <li>Mature luminal: lin–CD29loCD24+CD61lo (ML)</li>
  <li>Activated basal: lin–CD29hiCD24+Tspan8- (P6)</li>
  <li>Quiescent basal: lin–CD29hiCD24+Tspan8+ (P7)</li>
</ol>

For each population we profiled:
<ol>
  <li>transcriptome: RNA-seq</li>
  <li>chromatin interaction profiles of transcription start sites (TSS): Omni-C </li>
  <li>histone modifications: CUT&Tag
    <ol>
      <li>H3K4me1</li>
      <li>H3K4me3</li>
      <li>H3K9ac</li>
      <li>H3K9me2</li>
      <li>H3K9me3</li>
      <li>H3K27ac</li>
      <li>H3K27me3</li>
      <li>H3K36me3</li>
      <li>H2AK119ub</li>
      <li>IgG control</li>
    </ol>  
  </li>
  <li>RNA Polymerase II: CUT&Tag</li>
  <li>chromatin accessiblity: ATAC-seq</li>
</ol>

All data was mapped to the mouse genome, mm10.

<strong>ChromHMM</strong><br>
We generated chromatin hidden markov modelling (ChromHMM) files for the CUT&Tag data, combined with the ATAC-seq. There are 24-chromatin states in this model, please see our paper above for details on this states, Figure 5A. These files are bed file format.

<strong>RNA-seq, CUT&Tag and ATAC-seq:</strong><br>
Data is provided as bigwig (.bw) files, normalised as reads per kilobase per million (RPKM). The ATAC-seq files were downsampled to reduce the file size for upload. For any analysis of these data, please see the fastq files in the GEO database. <br>

<strong>Omni-C:</strong><br>
Omni-C interaction data was extracted for transcription start sites (TSSs) and is provided as a bed paired-end (.bedpe) file. <br>
