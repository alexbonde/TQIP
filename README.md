# TQIP
Code accompanying the paper "Assessing the Utility of Deep Neural Networks in Dynamic Risk Prediction After Trauma"

We have published five Jupyter notebooks: 
* [Data preprocessing](https://github.com/alexbonde/TQIP/blob/main/1)%20Data_preprocessing.ipynb)
* [Pre-Hospital Model](https://github.com/alexbonde/TQIP/blob/main/2)%20Pre-Hospital_Model.ipynb)
* [ED Model](https://github.com/alexbonde/TQIP/blob/main/2)%20ED_Model.ipynb)
* [I-Hospital Model](https://github.com/alexbonde/TQIP/blob/main/2)%20In-Hospital_Model.ipynb)
* [Model Inference - Use the models on an external dataset] (https://github.com/alexbonde/TQIP/blob/main/5)%20Model%20Inferecence.ipynb)

Models and explainers are too big to be downloaded with git clone. 
Models can be downloaded manually [here](https://github.com/alexbonde/TQIP/tree/main/models)
Explainers can be downloaded manually [here](https://github.com/alexbonde/TQIP/tree/main/explainers)

### Objective
To assess the value of deep neural networks in trauma risk prediction. 

### Summary Background Data
Risks of post trauma complications (PTCs, including thrombosis, infectious and organ failure events) are modulated by the injury as well as the clinical trajectories, yet prediction models often used single time-point data.  We hypothesize that deep learning prediction models can be used for dynamic risk prediction after trauma.

### Methods:  
Data was obtained from the 2017 American College of Surgeons Trauma Quality Improvement Program (ACS TQIP) database, which included 997,970 trauma cases. The only patients that were excluded were patients with a missing length of stay (n = 18,962). We created an independent data set for final model testing (n = 81,040). The remaining dataset (n = 897,968) was randomly split into a training dataset (n = 718,375) and a validation dataset (n = 179,593). We developed three deep neural network models: one designed for the pre-hospital setting (Pre-Hospital Model), one for the emergency department (ED Model) and one for the second day of hospitalization (In-Hospital Model). Dependent variables included early- and late mortality and any of 17 PTC’s. Model performance was evaluated using the area under the receiver operating characteristic curves (ROC AUC). 

### Results 
As patients moved through the treatment trajectories, model performance increased. Models predicted early mortality and late mortality with ROC AUCs ranging from 0.980 to 0.994 and 0.910 to 0.972, respectively. For the remaining 17 PTCs mean performance ranged from 0.829 to 0.913. 

### Conclusions
Deep neural networks achieve excellent performance in risk stratification of trauma patients as they advance through clinical treatment trajectories
