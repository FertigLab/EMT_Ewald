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

### 2_cleanData.ipynb
#### Description - Preprocesses the combined data
##### Input 
* mergedAdata.h5ad
##### Output
* labelledAdata.h5ad
* data/dataMatrix.mtx'
* data/obs.csv
* data/var.csv
* rawCleanadata.h5ad
* data/dataMatrixClean.mtx
* data/obsClean.csv
* data/varClean.csv

### 3_ClusteringAfterBatchCorrection.Rmd
#### Description - Create CDS with the “clean” data. CDS is preprocessed.
##### Input 
* data/dataMatrixClean.mtx
* data/obsClean.csv
* data/varClean.csv
##### Output
* intermediateData/cdsBasic.RDS
* intermediateData/cdsBasic.RDS
* data/normalizedMatrix.mtx
* intermediateData/cdsNormalizedDimReduced.rds
* intermediateData/cdsDayCorrected.RDS

### 4_EJFPreprocessingAnalysis.Rmd
#### Description - Run pseudotime for matrigel and collagen
##### Input 
* intermediateData/cdsBasic.RDS
* geneList.csv
##### No Output

### 5_EJFPreprocessingAnalysis.R
#### Description - Run pseudotime for matrigel and collagen
##### Input 
* cdsBasic.RDS  
* geneList.csv
##### Output
* EJFPsuedotimeResults2Mar2020.Rda


