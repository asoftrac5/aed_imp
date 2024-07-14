This readme file was generated on 2024-06-16 by Dhan Raj Rai


GENERAL INFORMATION


Title: Training and Evaluation of K-Nearest Neighbors and Decision Tree Classifiers on the Avila Dataset for Copyist Prediction Based on Attribute Analysis


Author/Principal Investigator Information
Name: Dhan Raj Rai
Student ID: s4063739
Institution: RMIT University
Email: s4063739@student.rmit.edu.au


Name of Data set: 100-ml/u.data 


Source of Data set collection: Imported directly from the uploaded zip file in the Practical Data Science with Python course from the RMIT University canvas. 


DATA SET DESCRIPTION 
* ml-100k/u.data
* u.data: The full u data set, 100000 ratings by 943 users on 1682 items. Each user         has rated at least 20 movies.  
* Users and items are numbered consecutively         from 1.  
* The data is randomly ordered. This is a tab separated list of user id | item id | rating | timestamp. The time stamps are unix seconds since 1/1/1970 UTC.  


File List:
1. Assignment3_framework.ipynb:
* It is the implementation of the Adjusted Euclidean Distance (AED). It implements the AED approach as the solution for the memory-based collaborative filtering as presented by the researchers in “Sun, H., Peng, Y., Chen, J., Liu, C., & Sun, Y. (2011). A New Similarity Measure Based on Adjusted Euclidean Distance for Memory-based Collaborative Filtering. Journal of Software, 6(6). https://doi.org/10.4304/jsw.6.6.993-1000”
* Basic python libraries are imported.
* The ml-100k/u.data is loaded and structured as dataframe. The headers for the corresponding columns are assigned.
* Then the data set is split into train and test with 80:20 ratio by assigning test_size to 0.2. A random train test split followed wherein the value for random_state is assigned to 10. The train and test data sets are further refined.
* There is utils section in the code wherein a method named evaluate is defined. The method evaluate helps to calculate the MAE and RMSE of the implemented AED for the memory-based collaborative filtering in line with the given data set.
* The AED strategy to compute the similarity between the users’ rating vectors is implemented as reflected and explained in the research paper, “Sun, H., Peng, Y., Chen, J., Liu, C., & Sun, Y. (2011). A New Similarity Measure Based on Adjusted Euclidean Distance for Memory-based Collaborative Filtering. Journal of Software, 6(6). https://doi.org/10.4304/jsw.6.6.993-1000.” 
* The prediction using AED approach is implemented by appling over the test data set. The prediction logic as reflected in the research paper mentioned above is applied to make predictions for the users.
* Finally, using the method named evaluate, the MAE and RMSE scores are computed for the AED prediction approach.


2. Slides.pdf:
* The slide explains the following things in detailed manner after completion of the implementation.
* Explain why the Adjusted Euclidean Distance works by using your own language clearly and completely.
* Explain how the Adjusted Euclidean Distance works by using your own language clearly and completely.
* Compare and show that: your implementation of Adjusted Euclidean Distance leads to better recommendations when comparing with the User-user KNN based Collaborative Filtering with Centred Cosine similarity (without significance weighting). Note: for this question, no need to submit the corresponding code, and just put them in your presentation.
* The slides serve as the material for the presentation of the assignment taking all the three points into account.
3. Assignment3_recording_s4063739.mp4
* The recording contains the actual video presentation of the Slides.pdf that backs the assignment 3. The video recording explains all the aforementioned points that are presented in the Slides.pdf with my own understanding and perception. In the recording, I have presented the points in sequence as reflected in the Slides.pdf. The length of the video recording is exactly 10 minutes. 


Split technique: Randon Train Test Split
Split Ratio: 
Train        :  Test 
80           :  20
Random state = 10


METHODOLOGICAL INFORMATION


Evaluation: 
Method: Train test split (80:20).
Strategy: Evaluating using the test data.


AED similarity computation:
Category: Memory-based collaborative filtering
Technique of collaborative filtering: User-User Based Collaborative filtering


Significant weighting: Not applied
Gamma = 30 (For significant weighting case only)
EPSILON = 1e-9 (In case of zero division)


Item Prediction
Technique of prediction: User-Item Based Prediction
EPSILON = 1e-9 (In case of zero division)


K = 50 
The value of K is tuned as per the nature of data sets and other requisites such as the MAE and RMSE requirements and optimizations.


Evaluation Strategy:
Metrics Used: 
* Mean Absolute Error (MAE)
* Root Mean square Error (RMSE)


Instrument- or software-specific information needed to interpret the data: 
1. Software: Anaconda3-2021
2. IDE: Jupyter Notebook
3. Version: 6.4.12
4. Programming language: Python
5. Python version: 3.8.8
6. Scikit-learn libraries (only for train test split)


FURTHER INFORMATION ABOUT THE GROUPLENS RESEARCH PROJECT
==============================================


The GroupLens Research Project is a research group in the Department of Computer Science and Engineering at the University of Minnesota. Members of the GroupLens Research Project are involved in many research projects related to the fields of information filtering, collaborative filtering, and recommender systems. The project is lead by professors John Riedl and Joseph Konstan. The project began to explore automated collaborative filtering in 1992, but is most well known for its world wide trial of an automated collaborative filtering system for Usenet news in 1996.  The technology developed in the Usenet trial formed the base for the formation of Net Perceptions, Inc., which was founded by members of GroupLens Research. Since then the project has expanded its scope to research overall information filtering solutions, integrating in content-based methods as well as improving current collaborative filtering technology.


Further information on the GroupLens Research project, including research publications, can be found at the following web site:
* http://www.grouplens.org/


GroupLens Research currently operates a movie recommender based on collaborative filtering:
* http://www.movielens.org/




CITATION
==============================================


To acknowledge use of the dataset in publications, please cite the 
following paper:


* F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History and Context. ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4, Article 19 (December 2015), 19 pages. DOI=http://dx.doi.org/10.1145/2827872
* Sun, H., Peng, Y., Chen, J., Liu, C., & Sun, Y. (2011). A New Similarity Measure Based on Adjusted Euclidean Distance for Memory-based Collaborative Filtering. Journal of Software, 6(6). https://doi.org/10.4304/jsw.6.6.993-1000 
                        
***All other required libraries are already imported or loaded within the implementation part of the code. 
***Note that it is a complete and error-free code provided all the aforementioned requirements are met. 
***There is no part in the code that is left untouched or redundant. All the codes included in the “Assignment3.ipynb” file are important to fully execute the task.