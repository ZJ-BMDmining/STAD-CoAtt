# STAD-CoAtt

In order to exploit structure information about evolving gene graphs, spatiotemporal graph learning approaches are able to analyze structure disorder and disorganization of regulatory systems that govern disease states.  Using brain transcriptomics data, this study proposes a multi-view GCN model, which integrates changes of transcript level and gene graphs to evaluate neuropathological stages.  Under the framework of spatiotemporal graph learning, the proposed STAD-CoAtt method constructs joint spatiotemporal(ST) representations of brain snRNA-seq data, to predict neuropathological scores and cognitive decline.

## Architecture

![image-20241006010039202](./Architecture)

## Requirements

Python --- 3.8

Pytorch --- 2.0.0

cuda --- 11.8

tensorflow-gpu --- 2.5.0

pandas --- 1.4.2

numpy --- 1.19.5

## Data availability

The ROSMAP dataset is collected from the AMP-AD Knowledge Portal, which ID syn18485175.  For the second benchmark from the GEO platform, brain expression data with ID GSE129308 and GSE147528 are selected to validate the performance of STAD-CoAtt.

## Usage

1、Run the "Dynamic graph calculation.ipynb" file to obtain the final_spatial_fusion_GEO.csv or final_spatial_fusion_ROSMAP.csv file.

2、Take the result of "Dynamic graph calculation.ipynb" as input, run "STAD-CoAtt.ipynb" to get the final result.