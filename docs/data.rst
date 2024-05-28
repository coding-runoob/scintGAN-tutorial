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
Example datasets
================

By courtesy of the original authors, we provide here the following preprocessed
data files used in our paper:

.. list-table::
   :widths: 15 15 5 5 32 3 25
   :header-rows: 1

   * - Dataset
     - Protocol
     - Species
     - Organs/Tissues
     - Source
     - Features
   * - Human immune
     - | 10X Chromium
       | Samrt-seq2
     - Human
     - | Peripheral blood
       | Bone marrow
     - `Preprocessed data <https://figshare.com/ndownloader/files/25717328>`__
     - | Continuous trajectories
       | Multiple technologies
       | Multiple tissues
   * - Mouse brain
     - 10X Chromium
     - Mouse
     - Brain
     - `Raw counts data <https://portal.brain-map.org/atlases-and-data/rnaseq/mouse-whole-cortex-and-hippocampus-10x>`__
     - | Large scale
       | Hierarchical organization
   * - Multiomics
     - | scATAC-seq
       | 10X Chromium
       | FACS-seq
     - Mouse
     - Atlas
     - | `RNA data <https://figshare.com/projects/Tabula_Muris_Transcriptomic_characterization_of_20_organs_and_tissues_from_Mus_musculus_at_single_cell_resolution/27733>`__
       | `ATAC data <https://atlas.gs.washington.edu/mouse-atac/data/>`__
     - | Atlas integration
       | Multi-omics
       | Multiple organs
       | Multiple technologies
   * - PBMC
     - 10X Chromium
     - Human
     - PBMC
     - | `Batch one <https://www.10xgenomics.com/resources/datasets/8-k-pbm-cs-from-a-healthy-donor-2-standard-2-1-0>`__
       | `Batch two <https://www.10xgenomics.com/resources/datasets/pbm-cs-of-a-healthy-donor-v-1-1-1-standard-3-1-0>`__
     - Widely used test data, identical cell type
   * - Multiple PBMC
     - | 10X Chromium
       | CEL-seq2
       | Drop-seq
       | Seq-Well
       | Smart-seq2
       | inDrops
     - Human
     - PBMC
     - Single cell portal, code:SCP424
     - | Multiple different protocols
       | Non-identical cell types
   * - Human pancreas
     - | inDrops
       | CEL-Seq2
       | Smart-Seq2
       | SMARTer
     - Human
     - Pancreas
     - `Preprocessed data <https://hemberg-lab.github.io/scRNA.seq.datasets/human/pancreas/>`__
     - | Different protocol
       | Non-identical cell type
   * - COVID-19 PBMC
     - single-cell V(D)J sequencing
     - Human
     - PBMC
     - `Preprocessed data <https://figshare.com/articles/dataset/seu_obj_h5ad/16922467>`__
     - | 22 donors (batches)
       | Multiple disease statuses
   * - COVID-19 Lung
     - 10X Chromium
     - Human
     - Lung
     - `GEO <https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE171524>`__
     - | 22 donors (batches)
       | Multiple disease statuses
