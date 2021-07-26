# EMT_Ewald
Curated set of analysis scripts for single cell data from the Ewald Lab.

### 1_CombineData.ipynb
#### Description - Joins the counts data together
##### Input 
* D1-D3-D5-byHaiping/D1/filtered_feature_bc_matrix/matrix.mtx
* D1-D3-D5-byHaiping/D1/filtered_feature_bc_matrix/barcodes.tsv
* D1-D3-D5-byHaiping/D1/filtered_feature_bc_matrix/features.tsv
* D1-D3-D5-byHaiping/D3/filtered_feature_bc_matrix/matrix.mtx
* D1-D3-D5-byHaiping/D3/filtered_feature_bc_matrix/barcodes.tsv
* D1-D3-D5-byHaiping/D3/filtered_feature_bc_matrix/features.tsv
* D1-D3-D5-byHaiping/D5/filtered_feature_bc_matrix/matrix.mtx
* D1-D3-D5-byHaiping/D5/filtered_feature_bc_matrix/barcodes.tsv
* D1-D3-D5-byHaiping/D5/filtered_feature_bc_matrix/features.tsv
##### Output
* mergedAdata.h5ad

