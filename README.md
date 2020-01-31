# ICD Code and Mortality
A data analytics project focusing on ICD code and mortality data analysis. Washington University in St. Louis course "Foundation of Analytics" final project. <br/>

## Executive Summary:
Together with an Insurance company, we are adjusting strategies for series of product for them. In order to scientifically set the prices for our current and future insurance products, analysing the cause of death in the US is important. The research data provided are: CDC mortality data (2005 - 2015) & ICD code. Our main goals are: Find out the major causes of death in the US, find out potential trends by analysing CDC mortality data, performing prediction for the data for 2016, and find out if any of the 5000 patients have conditions associated with major causes of death. <br/>
The following are some of our major findings. The major causes of death in the US are Cause 2 - Neoplasms, Cause 9 - Diseases of the circulatory system, Cause 10 - Diseases of the respiratory system, and Cause 20 External causes of morbidity and mortality. For these 4 causes of death, neoplasms, circulatory system, respiratory system all have a pattern against age that most deaths happen after the age of 65. However, for the external cause of mortality, there is no pattern and it looks a bit random. Detail of death patterns against age will be shown in the report in later sections.


## Technical Description:
* Part 1: 
	* Feature encoding and engineering
	* Built and fit a regression model, utilizing statsmodels.api.GLM in Python, to analyze conditions’ implications on the causes of death
* Part 2:  
	* Vectorized 5021 instances of text with TF-IDF weighted measure, utilizing sklearn.feature_extraction.text.TfidfTransformer and calculated similarity matrix based on the vectors
	* Matched a disease with the highest similarity beyond the threshold for each of the transcription instance

## Code Implementation Instructions: 
* The file "statistics and model" implements preliminary analysis on the dataset for further modeling
* For part 1, please run the code in the order of data_preprocessing, GLM, and Beta
* For part 2, please follow the instructions at the beginning of the code