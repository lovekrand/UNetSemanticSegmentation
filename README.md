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
* Numerical Learning Result: Train loss 0.575, Val loss: 0.72

## Experiment results
We provide some results over validation set
![output](https://github.com/user-attachments/assets/1a106317-bf97-46fa-b9d6-e8475e3997ec)
![output2](https://github.com/user-attachments/assets/01c39b17-f822-4b54-96eb-c681415f4f93)
![output3](https://github.com/user-attachments/assets/c3be9477-360b-4a10-8547-5e4362365f34)
![output4](https://github.com/user-attachments/assets/8481378b-0226-49cf-bc70-3bac8e674b43)
![output5](https://github.com/user-attachments/assets/95ace185-1b56-4013-be7a-a246518a90d6)
![output6](https://github.com/user-attachments/assets/009a5e7b-5b10-4b22-89f7-4029aa41048a)

## Overall comment
* Using cross-entropy loss showed a high tendency of over-fitting: used lovasz loss instead
* But validation loss still did not decrease much either. We may have to try out more training times.
* On optimizer, Adam based optimizer was much faster than SGD.
* Anyway, the results are a bit poor, some may be well captured but some are misclassified or not even correctly detected.
