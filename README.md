# Vision-SSL- SimCLR and MAE's

### Directions to run code: 
The files labelled simclr.ipynb and mae.ipynb are the source files for the SimCLR and MAE implementations, respectively. To run, import the ssl_dataset file into this directory after cloning.
The 2 options to run the code:
* Run all cells in each, thereby regenerating the simclr_encoder.pth and mae_encoder.pth files, which requires extensive compute.
* Run all but the pretraining cells (marked in the code), which will reduce runtime. This is possible due to the saved weight files.
  


### RESULTS AND INTERPRETATIONS
#### SimCLR:
Linear Probe Accuracy: 86.72%
Linear Probe F1 score- 0.8642
![SimCLR LOSS Curve] (SimCLR_loss.png)
![SimCLR Accuracy Curve] (SimCLR_accuracy.png)

#### MAE:
Linear Probe Accuracy: 86.72%
Linear Probe F1 score- 0.8642
!alt [SimCLR LOSS Curve] (SimCLR_loss.png)
