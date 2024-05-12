Datasets
================

The following datasets were used in our manuscript. We provided the details and sources of all datasets:
All data sets analyzed in this article are publicly available. We have shown the information in Data S1.
Specifically, the preprocessed version of Human immune data set can be retrieved from https://figshare.
com/ndownloader/files/25717328. Mouse brain data set can be downloaded from https://portal.
brain-map.org/atlases-and-data/rnaseq/mouse-whole-cortex-and-hippocampus-10x. Two atlases
of Multi-omics data set can be obtained from https://figshare.com/projects/Tabula_Muris_Transcriptomic
characterization_of_20_organs_and_tissues_from_Mus_musculus_at_single_cell_resolution/27733
and https://atlas.gs.washington.edu/mouse-atac/data/ respectively. The PBMC data set can be
obtained from https://www.10xgenomics.com/resources/datasets/8-k-pbm-cs-from-a-healthy-donor-2-s
and https://www.10xgenomics.com/resources/datasets/pbm-cs-of-a-healthy-donor-v-1-1-1-standard-
Multiple PBMC data set can be obtained from Single Cell Portal and the accession code is SCP424. Human
pancreas data set can be downloaded from https://hemberg-lab.github.io/scRNA.seq.datasets/
human/pancreas/.[43] COVID-19 PBMC dataset can be downloaded from https://figshare.com/articles/
dataset/seu_obj_h5ad/16922467. COVID-19 Lung can be obtained from GEO dataset and the accession
code is GSE171524.
.. list-table::
   :widths: 15 15 5 5 32 3 25
   :header-rows: 1

   * - Dataset
     - Protocol
     - Species
     - Tissues/Organs
     - Source
     - Features
   * - Chen-2019
     - SNARE-seq
     - Mouse
     - Cortex
     - `High-throughput sequencing of the transcriptome and chromatin accessibility in the same cell <https://doi.org/10.1038/s41587-019-0290-0>`__
     - `GEO <https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE126074>`__
     - | `Chen-2019-RNA.h5ad <http://download.gao-lab.org/GLUE/dataset/Chen-2019-RNA.h5ad>`__,
       | `Chen-2019-ATAC.h5ad <http://download.gao-lab.org/GLUE/dataset/Chen-2019-ATAC.h5ad>`__
   * - Ma-2020
     - SHARE-seq
     - Mouse
     - Skin
     - `Chromatin potential identified by shared single-cell profiling of RNA and chromatin <https://doi.org/10.1016/j.cell.2020.09.056>`__
     - `GEO <https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE140203>`__
     - | `Ma-2020-RNA.h5ad <http://download.gao-lab.org/GLUE/dataset/Ma-2020-RNA.h5ad>`__,
       | `Ma-2020-ATAC.h5ad <http://download.gao-lab.org/GLUE/dataset/Ma-2020-ATAC.h5ad>`__
   * - 10x-Multiome-Pbmc10k
     - 10x Multiome
     - Human
     - PBMC
     -
     - `10x Demo <https://support.10xgenomics.com/single-cell-multiome-atac-gex/datasets/1.0.0/pbmc_granulocyte_sorted_10k>`__
     - | `10x-Multiome-Pbmc10k-RNA.h5ad <http://download.gao-lab.org/GLUE/dataset/10x-Multiome-Pbmc10k-RNA.h5ad>`__,
       | `10x-Multiome-Pbmc10k-ATAC.h5ad <http://download.gao-lab.org/GLUE/dataset/10x-Multiome-Pbmc10k-ATAC.h5ad>`__
   * - Saunders-2018
     - Drop-seq
     - Mouse
     - Cortex
     - `Molecular diversity and specializations among the cells of the adult mouse brain <https://doi.org/10.1016/j.cell.2018.07.028>`__
     - `dropviz <http://dropviz.org/>`__
     - `Saunders-2018.h5ad <http://download.gao-lab.org/GLUE/dataset/Saunders-2018.h5ad>`__
   * - Luo-2017
     - snmC-seq
     - Mouse
     - Cortex
     - `Single-cell methylomes identify neuronal subtypes and regulatory elements in mammalian cortex <https://doi.org/10.1126/science.aan3351>`__
     - `annoj <https://brainome.ucsd.edu/annoj/brain_single_nuclei/>`__
     - `Luo-2017.h5ad <http://download.gao-lab.org/GLUE/dataset/Luo-2017.h5ad>`__
   * - 10x-ATAC-Brain5k
     - 10x ATAC
     - Mouse
     - Cortex
     -
     - `10x Demo <https://support.10xgenomics.com/single-cell-atac/datasets/1.1.0/atac_v1_adult_brain_fresh_5k>`__
     - `10x-ATAC-Brain5k.h5ad <http://download.gao-lab.org/GLUE/dataset/10x-ATAC-Brain5k.h5ad>`__
   * - Cao-2020
     - sci-RNA-seq3
     - Human
     - 15 organs
     - `A human cell atlas of fetal gene expression <https://doi.org/10.1126/science.aba7721>`__
     - `GEO <https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE156793>`__
     - `Cao-2020.h5ad <http://download.gao-lab.org/GLUE/dataset/Cao-2020.h5ad>`__
   * - Domcke-2020
     - sci-ATAC-seq3
     - Human
     - 15 organs
     - `A human cell atlas of fetal chromatin accessibility <https://doi.org/10.1126/science.aba7612>`__
     - `GEO <https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE149683>`__
     - `Domcke-2020.h5ad <http://download.gao-lab.org/GLUE/dataset/Domcke-2020.h5ad>`__
   * - Muto-2021
     - | snRNA-seq,
       | scATAC-seq
     - Human
     - Kidney
     - `Single cell transcriptional and chromatin accessibility profiling redefine cellular heterogeneity in the adult human kidney <https://doi.org/10.1038/s41467-021-22368-w>`__
     - `GEO <https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE151302>`__
     - | `Muto-2021-RNA.h5ad <http://download.gao-lab.org/GLUE/dataset/Muto-2021-RNA.h5ad>`__,
       | `Muto-2021-ATAC.h5ad <http://download.gao-lab.org/GLUE/dataset/Muto-2021-ATAC.h5ad>`__
   * - Yao-2021
     - | 10x RNA v3,
       | snATAC-seq
     - Mouse
     - MOp
     - `A transcriptomic and epigenomic cell atlas of the mouse primary motor cortex <https://doi.org/10.1038/s41586-021-03500-8>`__
     - `NeMO <https://assets.nemoarchive .org/dat-ch1nqb7>`__
     - | `Yao-2021-RNA.h5ad <http://download.gao-lab.org/GLUE/dataset/Yao-2021-RNA.h5ad>`__,
       | `Yao-2021-ATAC.h5ad <http://download.gao-lab.org/GLUE/dataset/Yao-2021-ATAC.h5ad>`__
