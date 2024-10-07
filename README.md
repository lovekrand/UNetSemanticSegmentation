# Semantic Segmentation task using U-Net model

## Experimental details
* Experiment date: Oct 7th 2024
* Dataset : Pascal VOC 2012
* Task: Semantic Segmentation
* Baseline model: U-Net
* Optimizer: AdamW
* Learning rate: Starting lr= 1e-4, ReduceLRonPlateau scheduler.
* Epoch: Total of 100(80mins)
* Loss: Lovasz softmax loss
* Result: Train loss 0.575, Val loss: 0.72

