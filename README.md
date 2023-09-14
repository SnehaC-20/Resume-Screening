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
#### 4.Data Cleaning
To clean resume text by removing URLs, RT and cc mentions, hashtags, special characters, non-ASCII characters, and extra whitespace. It then applies this cleaning function to a DataFrame containing resume data and stores the cleaned text in a new column. This is a common preprocessing step when working with text data, as it helps standardize and prepare the text for further analysis or natural language processing tasks.
## Data Visualization
- Data visualization is a critical part of data exploration.
- It involves creating plots and graphs to visually explore and understand the data.
- Visualization helps identify patterns, relationships, and anomalies in the data.
- Common types of visualizations include histograms, scatter plots, box plots, and heatmaps.

<img width="650" alt="Screenshot 2023-09-14 114740" src="https://github.com/SnehaC-20/Resume-Screening/assets/138655723/e4ef7732-97cc-426e-8264-2e3f850d59ae">

The above image displays the plot in bar chart where the x-axis represents the unique categories in the "Category" column of your resumeDataSet, and the y-axis represents the count of occurrences for each category. Above each bar, will display the exact count for that category. The rotated x-axis labels make it easier to read the category names, especially if they are long or numerous. The gridlines help you visually align the bars and interpret the plot more effectively.

 <img width="455" alt="Screenshot 2023-09-14 120416" src="https://github.com/SnehaC-20/Resume-Screening/assets/138655723/3784c8c7-0dc6-4bb4-a313-a04fbfb36597">
 
A pie chart is a circular graphical representation used to visualize the distribution or composition of a categorical data set. It divides the data into slices or wedges, each of which represents a category, and the size of each slice corresponds to the proportion of that category in the resume dataset.

### Splitting dataset into Train and Test set
Splitting the dataset into train and test sets is one of the important parts of data pre-processing, as by doing so, we can improve the performance of our model and hence give better predictability.
### Training model
- Now the resume text data is converted into TF-IDF feature vectors and then splits the data into training and testing sets, making it ready for machine learning model training and evaluation. The TF-IDF vectors represent the text data in a numerical format that can be used as input to machine learning algorithms.
- The type of training data that we provide to the model is highly responsible for the model's accuracy and prediction ability. It means that the better the quality of the training data, the better will be the performance of the model. Training data is approximately more than or equal to 60% of the total data for an ML project.
### Testing model
- Once we train the model with the training dataset, it's time to test the model with the test dataset. This dataset evaluates the performance of the model and ensures that the model can generalize well with the new or unseen dataset. The test dataset is another subset of original data, which is independent of the training dataset.
- The testing data should represent the part of original dataset and also it should be large enough to give meaningful predictions.
  



  



