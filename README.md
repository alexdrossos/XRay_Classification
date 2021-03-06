# Diagnosis of Respiratory Infections from Chest X-ray Images
This repository is the completed code for an Xray image classification model completed as part of the MIDS Applied Machine Learning course.
Co-contributors to this project include Hassan Saad, Anne Marshall, and Julia Hossu

## Research Question

How accurately can a machine learning model diagnose the following respiratory infections based on a chest x-ray?
* Pneumonia
* COVID-19 
* Tuberculosis

Link to Kaggle Dataset Used: https://www.kaggle.com/jtiptj/chest-xray-pneumoniacovid19tuberculosis

## File Overview
.  
├── NIHCC  
│   ├── NIHCC_MLP_Model.ipynb  
│   ├── NIHCC_SVM_Model.ipynb  
│   └── NIHCC_xray_data.py  
├── README.md  
├── models
│   ├── model_ensemble.ipynb 
│   ├── model_knn.ipynb
│   ├── model_naive_bayes.ipynb
│   ├── model_neural_nets.ipynb
│   ├── model_svm.ipynb
└── xray_data.py  

### Image Loading & Processing
The entirety of the x-ray image loading and processing applied to the data before any of the models were run is contained in the `xray_data.py` file. Each of the model notebooks imports and uses the functions defined here. Using this collection of methods assumes the Kaggle data linked above is downloaded to a `data` directory locally organized in the following way:  

.  
└── data  
   ├── test  
   │   ├── COVID19  
   │   ├── NORMAL  
   │   ├── PNEUMONIA  
   │   └── TURBERCULOSIS  
   ├── train  
   │   ├── COVID19  
   │   ├── NORMAL  
   │   ├── PNEUMONIA  
   │   └── TURBERCULOSIS  
   └── val  
       ├── COVID19  
       ├── NORMAL  
       ├── PNEUMONIA  
       └── TURBERCULOSIS  

### Models 
Work for each individual model that results are reported for (KNN, Naive Bayes, SVN and Multi-Layer Perceptron), as well as the ensemble model presented, is contained within a separate Jupyter notebook.  

| Model | File Name |  
| ----- | --------- |  
| KNN | model_knn.ipynb |  
| Naive Bayes | model_naive_bayes.ipynb |  
| SVN | model_svn.ipynb |  
| Multi-Layer Perceptron | model_neural_nets.ipynb |  
| Ensemble | model_ensemble.ipynb |  

### Experiment with NIHCC Data
The data loading and model files relevant to the experiment conducted with the NIHCC dataset (in which the best performing models using the Kaggle data set linked above are ran on the more extensive NIHCC dataset) are contained within the NIHCC directory.

### Archive
The files contiained within the `archive` directory contains various preliminary experiments with different image libraries and data processing, example files for standardizing model approaches between team-members and initial data analysis. 
