
Tutorial
==================

************
Main package
************

The ``scglue`` package can be installed via conda using one of the following commands:

.. code-block:: bash
    :linenos:


************
Input format and preprocessing
************

For multiple scRNA-seq data sets, please process them into `AnnData` format. The`.obs` correspond to cells and `vars` correspond to genes. 

Preprocessing function has been implemented in the file `utils.py`. And `single_cell_data_process()` function can be used to preprocess the raw single cell data.

************
Running scintGAN
************

Before running scintGAN in terminal, please edit the file `hyper_parameters.py` to customize the input and output arguments according to the data (See Parameters section for more details), or you can use the default arguments.

Then, for multiple scRNA-seq data set files in the same file folder, run the following command in terminal to integrate multiple data sets, and the preprocessing step can be performed by setting the argument `pp` to 1:

```shell
python scintGAN.py --file_name adata1.h5ad adata2.h5ad adata3.h5ad --pp 1
```

The embeddings of stage one and stage two will be saved in `.obsm['X_scVGAN']` and `.obsm['X_scintGAN']` of `adata` which is input.

************
A quick tutorial of integration of PBMC data 
************

The PBMC data includes two batches of PBMC. We'll show how to use scintGAN integrate the PBMC data. The two batches of PBMC data can be obtained in https://cf.10xgenomics.com/samples/cell-vdj/3.1.0/vdj_v1_hs_pbmc3/vdj_v1_hs_pbmc3_filtered_feature_bc_matrix.tar.gz and https://cf.10xgenomics.com/samples/cell-exp/2.1.0/pbmc8k/pbmc8k_filtered_gene_bc_matrices.tar.gz respectively. We suppose the needed environment and scintGAN have been installed well.

************
Reading and save as `h5ad` format
************

After unzip these two file, `read_10x_mtx()` function in `Scanpy` package is recommended to read them.

```python
import scanpy as sc
adata_3 = sc.read_10x_mtx('./pbmc3/GRCh38/')
print(adata_3)
adata_5 = sc.read_10x_mtx('./pbmc5/')
print(adata_5)
adata_3.write('./pbmc3.h5ad',compression = 'gzip')
adata_5.write('./pbmc5.h5ad',compression = 'gzip')
'''
output:
AnnData object with n_obs × n_vars = 8381 × 33694
    var: 'gene_ids'
AnnData object with n_obs × n_vars = 7231 × 33538
    var: 'gene_ids', 'feature_types'
'''
```
************
Integration by using scintGAN
************

As shown in Running scintGAN section, we use the following command to integrate the two scRNA-seq PBMC data sets.

```
python scintGAN.py --file_name pbmc3.h5ad pbmc5.h5ad --pp 1
```

************
Output
************

The integration results of two PBMC data sets in two stages will be saved in  `.obsm['X_scVGAN']` and `.obsm['X_scintGAN']` of `adata` respectively. By default, the dimension of result embedding of each cell is 30 in two stages.

************
Visualization
************

For the integration results, we can use the following codes to visualize them.

```
adata = sc.read('./results.h5ad')
batch_key='dataset'
cell_type_key='cell_type'

sc.pp.neighbors(adata,use_rep='X_scintGAN')
sc.tl.umap(adata)

sc.pl.umap(adata, color=[batch_key],title='scintGAN'+' (Batch)')
sc.pl.umap(adata, color=[cell_type_key],title='scintGAN'+' (Cell Type)')
```


************
Parameters
************

The arguments settings of input and output can be customized in file `hyper_parameters` according to the settings you need. More arguments related to training details of scintGAN and the descriptions can be seen in file `hyper_parameters`. Though these arguments can be set according to what you need, the more recommended way is to use default values.

+ `batch_key`: The batch key in `adata.obs` .
+ `data_path`: The path of single cell data.
+ `file_name`: The file name of single cell data.
+ `save_data_path`: The path for results saving.
+ `save_file_name`: The file name of data after integration.
+ `pp`: The choice of whether to perform the preprocessing step. The argument type is integer. 0 represent that no preprocessing step will be performed, and any integer greater than or equal to 1 represent that the data set will be preprocessed.

************
Output
************

The integration results of stage one and stage two will be saved in  `.obsm['X_scVGAN']` and `.obsm['X_scintGAN']` of `adata` respectively.  

************
Visualization
************

Visualization of UMAP plots has been implemented in the file `visualization.py` . For a result integrated by scintGAN,  the following command can be used to visualize the UMAP plots.

```shell
python visualization.py --data_path ./results/results.h5ad
```
