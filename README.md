# DMHMDA

DMHMDA is a biologically interpretable approach that utilizes a dual-channel strategy combining a set of "similarity-association-similarity" multi-hop metapaths and a heterogeneous-hyper network (HeteroHyperNet) for miRNA-disease association prediction. In DMHMDA, the "similarity-association-similarity" multi-hop metapaths learning method based on hierarchical attention perception is proposed as a channel to explore multiple specific long-distance associated pathways that connect potentially associated miRNAs and diseases. In parallel, a HeteroHyperNet learning approach integrating heterogeneous network and hyper network is designed as another channel to progressively learn direct and potential global association information between miRNA and disease. The ``similarity-association-similarity" metapaths with hierarchical attention significantly enhances the learning of long-distance biological associations, while the HeteroHyperNet comprehensively learns the known and potential global associations of miRNA-disease. This dual-channel learning method greatly improves the richness and accuracy of information.






# Requirements
  * Python 3.7 or higher
  * PyTorch 1.8.0 or higher
  * torch-geometric 2.0.4
  * GPU (default)

# Data
  * Download associated data and similarity data.
  * Multiple similarity calculations are detailed in the supplementary material.

# Running  the Code
  * Execute ```python main.py``` to run the code.
  * Parameter state='valid'. Start the 5-fold cross validation training model.
  * Parameter state='test'. Start the independent testing.

# Note
```
 1.Torch-geometric has a strong dependency, so it is recommended to install a matching version.
 2.The trained model are stored in folder named cross valid . You can import directly to implement valid and test.
```
