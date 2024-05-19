# OvCa-scRNAseq-Julia
ovarian cancer treatment resistance single-cell RNAseq analysis pipeline in Julia

### Overview
This repository contains code used in the analysis of single-cell RNA sequencing. These codes are written in Julia (tested on versions 1.9.3) and are presented in Jupyter Notebook. Code blocks within the Jupyter Notebook are intended to be run independently. 

### Requirements
- Julia (version 1.9.3)
- Jupyter Notebook

### Package requirements 
- DataFrames.jl
- CSV.jl
- StatsPlots.jl
- Statistics.jl
- StatsBase.jl
- Plots.jl
- Makie.jl
- IJulia.jl
- LinearAlgebra.jl
- MultivariateStats.jl
- MultipleTesting.jl
- NearestNeighbors.jl
- RCall.jl
- PyCall.jl
- SparseArrays.jl
- SCTransform.jl
- UMAP.jl
- TSne.jl
- PlotlyJS.jl
- MatrixMarket.jl
- Distances.jl
- CairoMakie.jl
- HypothesisTests.jl
- [Leiden.jl](https://github.com/bicycle1885/Leiden.jl)
- [CellScopes.jl](https://github.com/HaojiaWu/CellScopes.jl#julia_v1_9)
- [AutomaticSingleCellToolbox.jl](https://github.com/kaji331/ASCT.git)
- [SingleCellProjections.jl](https://github.com/BioJulia/SingleCellProjections.jl.git)

### Project contents
- `README.md` : this file with information about the repository.
- `A2780_ASCT.ipynb` : using AutomaticSingleCellToolbox.jl to run scRNA-seq analysis.
- `A2780_CellScopes.ipynb` : using CellScopes.jl to run scRNAseq but it doesn't execute at `scale_object` function.
- `A2780_SingleCellProjections.ipynb` : using SingleCellProjections.jl to run scRNA-seq analysis but it doesn't have clustering function.
- `A2780_emily.ipynb` : no systematic package used for analysis. Function are based on CellScopes algorithm.
- `A2780` : a folder of A2780 raw data.
- `A2780_QC` : a folder of A2780 data after QC by Seurat.
- `A2780_QC_filtered_mean` : a folder of A2780 data after QC and filtered the average expression value for each gene across all the cells during [0.125,3]
- `Data` : raw data with genes and cells names and metadata stored in csv and raw data stored in h5.
- `project.toml` & `manifest.toml` : Julia environment.

### Acknowledgments
We would like to thank Meghan C. Ferrall-Fairbanks and Adriana Del Pino Herrera for support and guidance.
