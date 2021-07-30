## ADDI Alzheimer's Detection Challenge

### 🕵️ Introduction

The Clock Drawing Test (CDT) is a simple test to detect signs of dementia. In this test the patient is asked to draw an analog clock with hands on the clock indicating ‘ten minutes past 11 o’clock.’ The test can be done on a blank paper or on a paper with a pre-drawn circle. This single test may be sensitive to dementia because it involves many cognitive areas that can be affected by dementia, including executive function, visuospatial abilities, motor programming, attention, and concentration. A qualified doctor then examines the drawing for the signs of dementia.

The results from cognitive assessments by CDT are used to diagnose underlying cognitive disabilities, including Alzheimer’s disease.


### 🖊  The Task
The challenge is to use the features extracted from the Clock Drawing Test to build an automated algorithm to predict whether each participant is in one of three phases:
1)    Pre-Alzheimer’s (Early Warning)
2)    Post-Alzheimer’s (Detection)
3)    Normal (Not an Alzheimer’s patient)

### 💾 Dataset
Each row in the data set represents the results from one clock drawing test of a single participant. The data set contains ~121 features(exact feature descriptions can be found here). The description of each feature is share in [Feature Documentation](https://github.com/cicycong/AIcrowd_ADDI_Alzheimers_Detection/blob/main/Feature-Documentation-%20ADDI%20Alzheimers%20Detection%20Challengev2.pdf).

Training data
Training data consists of 32,778 observations, which is a stratified random sample based on class labels of the original dataset. The labels are present as (Pre-Alzheimer’s, Post-Alzheimer’s, and Normal).

Testing data
The test data set consists of roughly 1,473  observations without label information. For each row predict a label (Pre-Alzheimer’s, Post-Alzheimer’s, and Normal). 

### 🔍 General Approach
✔ Data Cleaning  <br />
✔ Feature Engineering  <br />
✔ Variable Selection (XGBoost Feature Importance) <br /> 
✔ Modeling (LightGBM) <br /> 
✔ Hyper-parameter Tuning <br /> 
✔ Evaluation (Log loss) <br /> 
✔ Prediction & Submission

For detailed code, please refer [ADDI_Alzheimers_Detection.ipynb](https://github.com/cicycong/AIcrowd_ADDI_Alzheimers_Detection/blob/main/ADDI_Alzheimers_Detection.ipynb).
