This code for single cell analysis tranning for Huang Lab.

Project Name: Single-cell transcriptome analysis in mouse skin tissue reveals that the highly expressed genes are related to inhibitor and regulator which mostly lie in keratinocyte stem and epidermal cells.

Why this project is important: For a long time, moue has been used in research for it’s around 80% similarity to humans which has been yielded to various successful inventions to treat human disease.This research aims to investigate mouse skin tissue using transcriptomics data from individual cells to know the differences between cells in depth using single cell data.Single cell data which has gained popularity since 2014 helps to identify cell specific changes and yield more accurate information than bulk-cell RNA seq data[1].

Project Description: Single cell data for mice has been taken from Tabula Muris, a popular project , which combined around 100,00 cells information for around 20 organs and tissue.In this research, the skin tissue has been considered which has been sequenced using SMART-Seq2 method, a FACS based method. Two files regarding the data have been taken from the Tabula Muris website and they are counts of individual cells per gene and associated metadata(such as plate barcode, mouse sex and id).After manually downloading the data, the counts of individual cells per gene dataset has been transposed to make an expression matrix where each column and row refers to the gene and single cell respectively.For the convenience and simplicity of research only 553 cells have been considered[2].

The workflow here has been created through follwing the tutorial from single analysis worksop offered by the Chan Zuckerberg Initiative by using scanpy python libarary[3].

Workflow: The steps for the single cell data analysis are as follows: 1.Creation of AnnData object 2.Quality Control of cell and gene 3.Principal Component Analysis before and after Normalization 4.Embedding using tSNE(t-Distributed Stochastic Neighbour Embedding) and UMAP (Uniform Approximation and Projection) 5.Clustering using K-means and graph based 6.Differential gene expression.

References:

Tang, F., Barbacioru, C., Wang, Y. et al. mRNA-Seq whole-transcriptome analysis of a single cell. Nat Methods 6, 377–382 (2009). https://doi.org/10.1038/nmeth.1315
The Tabula Muris Consortium., Overall coordination., Logistical coordination. et al. Single-cell transcriptomics of 20 mouse organs creates a Tabula Muris. Nature 562, 367–372 (2018). https://doi.org/10.1038/s41586-018-0590-4
Wolf, F., Angerer, P. & Theis, F. SCANPY: large-scale single-cell gene expression data analysis. Genome Biol 19, 15 (2018). https://doi.org/10.1186/s13059-017-1382-0
