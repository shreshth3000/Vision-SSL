# Vision-SSL- SimCLR and MAE's

### Directions to run code: 
The files [simclr.ipynb](https://github.com/shreshth3000/Vision-SSL/blob/main/simclr.ipynb) and [mae.ipynb](https://github.com/shreshth3000/Vision-SSL/blob/main/mae.ipynb) are the source files for the SimCLR and MAE implementations, respectively. To run, import the ssl_dataset file into this directory after cloning.
The 2 options to run the code:
* Run all cells in each, thereby regenerating the simclr_encoder.pth and mae_encoder.pth files, which requires extensive compute.
* Run all but the pretraining cells (marked in the code), which will reduce runtime. This is possible due to the saved weight files.

## RESULTS AND INTERPRETATIONS
### SimCLR:
#### * **Linear Probe Accuracy:** 86.72%
#### * **Linear Probe F1 score:** 0.8642

  
![SimCLR LOSS Curve](SimCLR_loss.png)
![SimCLR Accuracy Curve](SimCLR_accuracy.png)

**The SimCLR loss and accuracy curve display tendencies of fitting the noise in the data (overfitting) due to their erratic/oscillatory nature near the end of the training cycle.
This may indicate inadequate pretraining or a flawed architecture for the linear probe.**


### MAE:
#### * **Linear Probe Accuracy:** 85.44%
#### * **Linear Probe F1 score:** 0.8567

![MAE LOSS Curve](mae_linear_probe_loss.png)
![MAE Accuracy Curve](mae_linear_probe_accuracy.png)

**The MAE loss and accuracy curves are comparatively much smoother, representing stable pretraining and convergence. Similar performance at lower compute costs are the benefits of using the MAE here, along with other specialised tasks like image restoration.**
