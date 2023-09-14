# Resume-Screening
## Description
Resume screening is the process of reviewing and evaluating job applicants' resumes or CVs to determine whether they meet the qualifications and requirements for a specific job or position. It is typically one of the initial steps in the hiring process and is used by employers to narrow down the pool of applicants before conducting interviews or further assessments.
## Installation
Use the package manager [pip](https://pip.pypa.io/en/stable/) to install numpy, pandas, matplotlib, sklearn
```blash
pip install (necessary packages)
```
* Numpy - "Numerical Python," is a fundamental Python library used for scientific computing.
* Pandas is for accessing datastructure and it deals with dataset.
* Matplotlib is used for creating static, animated, and interactive visualizations in Python.
* Sklearn is designed for machine learning and data mining tasks.
### After installing the required packages we need to import those stuffs in a jupyterhub.
## Data Preprocessing
#### 1.Acquire dataset
- I had collected the resume dataset in kaggle https://www.kaggle.com/code/gauravduttakiit/resume-screening-using-machine-learning/input .
#### 2.Import dataset
```
resumeDataSet = pd.read_csv('UpdatedResumeDataSet.csv')
resumeDataset
```
#### 3.Data description
It inclues the entire description of the dataset by using some terms as follows
* info() is for getting entire information about the dataset
* describe() is for the describtion of dataset such as check, count, top etc...
* Shape is for describing entire rows and columns that are existed in the dataset
* unique() is for viewing the unrepeated terms
* count() it shows the counting of that particular term
## Data Visualization
- Data visualization is a critical part of data exploration.
- It involves creating plots and graphs to visually explore and understand the data.
- Visualization helps identify patterns, relationships, and anomalies in the data.
- Common types of visualizations include histograms, scatter plots, box plots, and heatmaps.
  



