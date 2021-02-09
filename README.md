## Quartile-Based Prediction of Event Types and Event Time in Business Processes using Deep Learning 

This repository contains the source code and the associated files for the thesis/paper titled 'Quartile-Based Prediction of Event Types and Event Time in Business Processes using Deep Learning', submitted by Ishwar Venugopal.

The data is organised into five folders. The contents of each of the folders is described below:

### Datasets

This folder contains the three different datasets used in this work

### Data_Analysis

Contains codes for the initial data analysis using **PM4Py** ( *PM4Py_analysis_(Helpdesk Data).ipynb* )

### LSTM_Baseline

Contains the codes to implement the LSTM model presented in [Predictive Business Process Monitoring with LSTM Neural Networks](https://arxiv.org/abs/1612.02130)

### Model_Variants

In all of the codes present in this folder, change the dataset parameters accordingly in the cell titled 'Setting the Parameters'. Keep the seed value as 42 to obtain reproducible results from the Thesis.

The code to implement the GCN variants introduced in the thesis:

*   *GCNSeq_NextActivity_(FinalVersion).ipynb*
*   *GCNSeq_NextTimestamp_(FinalVersion).ipynb*

The code to implement the MLP model introduced in the thesis:

*   *MLP_NextActivity_(FinalVersion).ipynb*
*   *MLP_NextTimestamp_(FinalVersion).ipynb*

These codes can be used to train different model_variants.

The folders *Quartiles_basedOnEvents* and *Quartiles_basedOnTime* contain codes to evaluate trained models at different quartiles.

The folder *Evaluate_and_plot* contains codes to evaluate the overall performance of the trained models. It also includes the code to obtain plots from the saved results (*GCNSeq_Plots.ipynb*).


### Saved_Data_Files

Contains the files saved during training and evaluation for each of the datasets. 

Each dataset folder contains :

*   parameter files saved during the training of all model variants at different learning rates (*lr_all_variants*)
*   The parameter files for the models with the best performance for each variant (*best_models*)
*   The folder titled *quartiles* containing the evaluation results for the best model in each variant evaluated at quartiles based on number of events and case duration
*   *final_plots* containing all the plots correspoding the associated dataset






