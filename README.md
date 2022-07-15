# Assessment-of-computational-methods-for-scATAC-seq


A. Background
    Recent innnovations in single-cell Assay for Transposase Accessible Chromatin using sequencing (scATAC-seq) enable profiling of the epigenetic landscape of thousands of individual cells. scATAC-seq data analysis presents unique methodological challenges. scATAC-seq data analysis presents unique methodological challenges. scATAC-seq experiments sample DNA; which, due to low copy numbers (diploid in humans), lead to inherent data sparsity (1-10% of peaks detected per cell) compared to transcriptomic (scRNA-seq) data (10-45% of expressed genes detected per cell). Such challenges in data generation emphasize the need for informative features to assess cell heterogeneity at the chromatin level. 
    
   *****

B. About the Repository
    This is a collection of methodologies utilized when analyzing scATAC-seq data. They are based on a range of differing R algorithms, including Signac, Seurat, Cicero, and Monocle3. 
    
    0. Pre-Analysis: quality checks (QC), filters, dimensional reduction and gene activity quantification
    1. Data Integration: add scRNA-seq information and compute co-embedding. 
    2. Coaccessibility: scores co-accessibility between peaks to predict cis-regulatory interactions, such as those between promoters and enhancers.
        2.1 *Recall motifs are found when proteins and RNA molecules bind to these motifs in a sequence-specific way to control transcription and subsequent                      sequestration or degradation of messenger RNA (mRNA). 
        
    3. Differentially-Accessible Peaks: Differences between chromatin accessibility in groups or clusters of cells. 
    4. Motif Analysis: Overrepresented motifs in a cluster of cells in comparison to another cluster of cells. Computes motif activities using ChromVAR. chromVAR is an R package for the analysis of sparse chromatin accessibiility. chromVAR takes as inputs aligned fragments (filtered for duplicates or low quality) from ATAC-seq or DNAse-seq experiments as well as genomic annotations such as motif positions. chromVAR computes for each annotation and each cell or sample a bias corrected "deviation" in accessibility from the expected accessibility based on the average of all the cells or samples.
    5. Transcription Factor Footprints (TFFs): Locates TF footprints. Similarly to nucleosomes, bound TFs hinder cleavage of DNA, thus resulting in defined regions of decreased signal strength within larger regions of higher signal, known as 'footprints'. 
    
    
    
    References:
    [1]
    [2]
    [3]
    [4]
    [5]
    [6]
    [7]
    [8]
    [9]
    [10]
    
    
