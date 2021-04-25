# Colorado High School Graduation Rates by Location

# Project Summary

The objective of this project is to use a specific data set to predict whether or not geographic location, such as metropolitan vs. rural areas, has an effect on high school graduation rates in Colorado. Each area is composed of different student populations based on gender and race.  The following is a dilemma which confronts many people in education: What data can be used to determine graduation rates amongst different counties in Colorado based on length of time.  Gaining insight into this dilemma will help the state of Colorado focus on which areas, metropolitan or rural, should be targeted to assist in improving graduation rates.

# Data Collection

The data was collected from the Colorado Department of Education website. The dataset chosen was an Excel file titled 'Graduates and Completers by Districts, Gender, and Race/Ethnicity’.

# The Graduate Dataset

The Graduate dataset contains 750 observations and 125 variables. Some of the variables that the dataset has includes the following:

County Name: Name of county where schools are located

Organization Name: Name of school/organization

"Class Of..." Anticipated Year of Graduation Cohort: Specific graduation year (2016-2017, 2017-2018, 2018-2019, 2019-2020)

Number of Years After Entering High School: Number of years after a student entered high school (4,5,6 or 7)

All Students Graduates Total: Number of students who graduated at a school/organization during a specific school year

All Students Graduation Rate: Graduation rate of students (in percentage) in 4, 5, 6, or 7 years from high school

All Students Completion Rate: Completion rate of students (in percentage) in 4, 5, 6, or 7 years from high school

# Libraries Used in Python

Here is the list of libraries used to complete the education project in Python:

* numpy
* pandas
* matplotlib.pyplot
* seaborn
* sklearn


# Data Preparation

The dataset, df, was uploaded into a Jupyter notebook using Anaconda. To begin preparing the data, the first five rows were dropped above because they were the totals from all of the data columns. These rows were excluded so that the main focus was the data without the data totals. The summary statistics of df was then determined and also the number of missing or NA values were calculated. The mean value for each column was imputed for the NA values and a new dataset was created (df2).

After the df2 dataset was created, the first five rows of the df2 dataset were removed since they were the totals for each data column. The summary statistics of df2 was then calculated. After seeing the summary statistics of df2, multiple boxplots were created to see if any outliers exist in the df2 data.

The df2 data was then split into 4 different geographic regions: Metro, Western Slope/Mountain, Eastern Plains, and Southwestern. 

# Metro Data

The Metro data subset consisted of 10 different counties: El Paso, Arapahoe, Jefferson, Adams, Denver, Douglas, Boulder, Larimer, Clear Creek, and Gilpin. The summary statistics for the Metro data were calculated and then the top five counties where the total number of females completed high school.

<img width="469" alt="image" src="https://user-images.githubusercontent.com/79723505/112390306-eccb2f80-8caa-11eb-899b-528aefc5f8bf.png">

The top five counties where females completed high school were El Paso, Arapahoe, Jefferson, Adams, and Denver.

The top five counties where the total number of males who completed high school were also calculated.

<img width="469" alt="image" src="https://user-images.githubusercontent.com/79723505/112390563-5c411f00-8cab-11eb-9ff7-1c2edf914e63.png">

The top five counties where males completed high school were El Paso, Arapahoe, Jefferson, Adams, and Denver.

The top five counties where total number of years entered high school was also determined.

<img width="469" alt="image" src="https://user-images.githubusercontent.com/79723505/112390720-94e0f880-8cab-11eb-8302-6a7fa3b18c62.png">

The top five Metro counties for total number of years entering high school was El Paso, Adams, Arapahoe, Larimer, and Boulder.

The top five Metro counties focusing on female graduation rates were also determined.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112772204-038bc200-8fdc-11eb-85b1-3340f504cd50.png">

The top five Metro counties with the best female graduation rate was El Paso, Adams, Arapahoe, Larimer, and Boulder.

The top five Metro counties focusing on male graduation rates were also determined.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112772230-2027fa00-8fdc-11eb-9a9f-4ff39c9e68be.png">

The top five Metro counties with the best male graduation rate was El Paso, Adams, Arapahoe, Larimer, and Boulder.

# Western Data

The Western data subset consisted of 17 different counties: Mesa, Garfield, Eagle, Montrose, Delta, Summit, Routt, Chaffee, Gunnison, Pitkin, Moffat, Grand, Park, Rio Blanco, Lake, Ouray, and Jackson. The summary statistics for the Western data were calculated and then the top five counties where the total number of females completed high school.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112403565-8272b900-8cc3-11eb-89c1-dbe36f64dba7.png">

The top five counties where females completed high school were Mesa, Garfield, Eagle, Montrose, and Delta.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112403680-b4841b00-8cc3-11eb-9eba-00d16d72cfe7.png">

The top five counties where females completed high school were Mesa, Garfield, Eagle, Montrose, and Delta.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112403774-e5fce680-8cc3-11eb-9cf0-44b4758f4efa.png">

The top five Western counties for total number of years entering high school were Mesa, Garfield, Routt,
Montrose, and Grand.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112772291-65e4c280-8fdc-11eb-94df-08896fe7cbc8.png">

The top five Western counties with the best female graduation rates were Routt, Garfield, Mesa, Ouray, and Rio Blanco.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112772311-83199100-8fdc-11eb-872a-ae5d7d80bbf8.png">

The top five Western counties with the best male graduation rate was Routt, Garfield, Mesa, Rio Blanco, and Ouray.

# Eastern Data

The Eastern data subset consisted of 18 different counties: Weld, Pueblo, Bent, Morgan, Elbert, Otero, Logan, Prowers, Yuma, Kit Carson, Sedgwick, Phillips, Washington, Lincoln, Baca, Crowley, Cheyenne, and Kiowa. The summary statistics for the Eastern data were calculated and then the top five counties where the total number of females completed high school.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112404138-a4b90680-8cc4-11eb-8a0d-c6d7f1274e15.png">

The top 5 Eastern counties where females completed high school were Weld, Pueblo, Bent, Morgan, and Elbert.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112404239-d8942c00-8cc4-11eb-9f5a-65b3033c707f.png">

The top 5 Eastern counties where females completed high school were Weld, Pueblo, Bent, Morgan, and Elbert.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112404347-0d07e800-8cc5-11eb-9e94-73f4e6d1a163.png">

The top 5 eastern counties for students graduating high school after a number of years were Weld, Otero, Baca,
Washingtion, and Elbert.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112772331-a2182300-8fdc-11eb-98b9-6d1ad9a11372.png">

The top five Eastern counties with the best female graduation rate was Weld, Otero, Elbert, Washington, and Baca.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112772343-b5c38980-8fdc-11eb-8fa6-e1146b76906f.png">

The top five Eastern counties with the best male graduation rate was Weld, Otero, Elbert, Washington, and Baca.

# Southwestern Data

The Southwestern data subset consisted of 18 different counties: La Plata, Fremont, Montezuma, Teller, Alamosa, Rio Grande, Las Animas, Conejos, San Miguel, Archuleta, Saguache, Huerfano, Custer, Costilla, Dolores, Hinsdale, Mineral, and San Juan. The summary statistics for the Southwestern data were calculated and then the top five counties where the total number of females completed high school.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112404844-f9a94c80-8cc5-11eb-9c32-5d97df56639f.png">

The top 5 Southwestern counties where females completed high school were La Plata, Fremont, Montezuma, Teller, and Las Animas.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112404677-9f0ff080-8cc5-11eb-85ae-79944f123713.png">

The top 5 Southwestern counties where males completed high school were La Plata, Fremont, Montezuma, Teller, and Las Animas.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112404915-180f4800-8cc6-11eb-8345-5b69d56f4da2.png">

The top 5 Southwestern counties for number of years students completing high school were Las Animas, Fremont, Conejos
Saguache, and Rio Grande.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112772367-d12e9480-8fdc-11eb-9499-8616e6a9a155.png">

The top five Eastern counties with the best female graduation rate was Las Animas, Conejos, Rio Grande, Fremont, and Montezuma.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112772375-e73c5500-8fdc-11eb-865d-193c15e8905e.png">

The top five Eastern counties with the best male graduation rate was Las Animas, Conejos, Rio Grande, Fremont, and Montezuma.

# Exploratory Data Analysis

During the exploratory data analysis, the male and female graduation rates were the primary focus based on ethnicities in each region. The ethnicity groups used were Asian, Black, Hispanic, White, and Other (Native Hawaiian or Other Pacific Islander). The summary statistics were found for each ethnicity in each region. The number of outliers were also calculated as well by ethnicity.

Female and Male Graduation Rates in Metro Counties by Ethnicity

|Ethnicity|Mean Graduation Rate|Number of Outliers|
|---------|--------------------|------------------|
|Asian|14.2%|2|
|Black|12.6%|2|
|Hispanic|12.7%|2|
|White|13.1%|2|
|Other|12.3%|4|

It was clear that the Asian ethnicity has the best graduation rate in Metro Counties. The most outliers occurred in the Other ethnicity.

Female and Male Graduation Rates in Western Counties by Ethnicity

|Ethnicity|Mean Graduation Rate|Number of Outliers|
|---------|--------------------|------------------|
|Asian|6.2%|0|
|Black|5.5%|0|
|Hispanic|5.7%|0|
|White|6.2%|0|
|Other|5.4%|0|

The Asian and White ethnicities had the best graduation rates in Western Counties. There were no outliers in the Western data.

Female and Male Graduation Rates in Eastern Counties by Ethnicity

|Ethnicity|Mean Graduation Rate|Number of Outliers|
|---------|--------------------|------------------|
|Asian|14.3%|2|
|Black|12.6%|2|
|Hispanic|13.8%|2|
|White|14.3%|2|
|Other|12.5%|4|

The Asian and White ethnicities had the best graduation rates in Eastern counties. The most outliers occurred in the Other ethnicity.

Female and Male Graduation Rates in Southwestern Counties by Ethnicity

|Ethnicity|Mean Graduation Rate|Number of Outliers|
|---------|--------------------|------------------|
|Asian|8.1%|2|
|Black|7.0%|2|
|Hispanic|7.9%|2|
|White|8.0%|1|
|Other|7.1%|3|

The Asian ethnicity had the best graduation rate in Southwestern Counties. The most outliers occurred in the Other ethinicity.

Due to the small number of outliers, they were left into the dataset since they wouldn't have an enormous effect on the results.

# Artificial Neural Networks (ANNs) 

The first machine learning task completed was creating artificial neural networks (ANN). Eight different ANN models were created to correctly predict the graduation rates based on region (Metro, Western, Eastern, or Southwestern), gender (Male or Female), and ethnicity (Asian, Black or African American, Hispanic, and White). The counties for each region were reclassified into numeric values in order to complete the ANN models. The data was split into 70:30 ratio for training and testing datasets.


|Gender|Precision|f1-Score|County with Best Results|
|------|----------|---------|-------------------------|
|Female|48%|48%|Denver County|
|Male|50%|45%|Boulder County|

The table above shows the results for the ANN models for the Metro_Female and Metro_Male data. The ANN models consisted of three hidden layers of 25 and a max iteration of 3,000. The results showed that the Metro_Female model had a 48% prediction rate when correctly predicting whether a female will graduate in the Metro dataset based on ethnicity. The county that showed the most accurate results was El Paso County for the Metro_Female model. The Metro_Male model had a 50% prediction rate when correctly predicting whether a male will graduate in the Metro dataset based on ethnicity. The county that showed the most accurate results was Boulder County for the Metro_Male model. It's clear that males had a slightly better prediction for graduation than females in the Metro region.


|Gender|Precision|f1-Score|County with Best Results|
|------|----------|---------|-------------------------|
|Female|23%|15%|Summit County|
|Male|25%|12%|Montrose County|

The table above shows the results for the ANN models for the Western_Female and Western_Male data. The ANN models consisted of three hidden layers of 20 and a max iteration of 3,000. The results showed that the Western_Female model had a 23% prediction rate when correctly predicting whether a female will graduate in the Western dataset based on ethnicity. The county that showed the most accurate results was Summit County for the Western_Female model. The Western_Male model had a 25% prediction rate when correctly predicting whether a male will graduate in the Western dataset based on ethnicity. The county that showed the most accurate results was Montrose County for the Metro_Male model. It's clear that males had a better prediction for graduation than females in the Western region.


|Gender|Precision|f1-Score|County with Best Results|
|------|----------|---------|-------------------------|
|Female|12%|8%|Pueblo County|
|Male|9%|8%|Weld County|

The table above shows the results for the ANN models for the Eastern_Female and Eastern_Male data. The ANN models consisted of three hidden layers of 50 and a max iteration of 3,000. The results showed that the Eastern_Female model had a 12% prediction rate when correctly predicting whether a female will graduate in the Eastern dataset based on ethnicity. The county that showed the most accurate results was Pueblo County for the Eastern_Female model. The Eastern_Male model had a 9% prediction rate when correctly predicting whether a male will graduate in the Eastern dataset based on ethnicity. The county that showed the most accurate results was Weld County for the Eastern_Male model. It's clear that females had a better prediction for graduation than males in the Eastern region.

The ANN model for the female and male Southwestern data consisted of three hidden layers of 100 and a max iteration of 3,000. Below is a table of the results.

|Gender|Precision|f1-Score|County with Best Results|
|------|----------|---------|-------------------------|
|Female|22%|14%|Fremont County|
|Male|9%|10%|Fremont County and La Plata County|

The table above shows the results for the ANN models for the Southwestern_Female and Southwestern_Male data. The Southwestern_Female ANN model consisted of three hidden layers of 100 and a max iteration of 3,000. The Southwestern_Male ANN model consisted of three hidden layers of 50 and a max iteration of 3,000. The results showed that the Southwestern_Female model had a 22% prediction rate when correctly predicting whether a female will graduate in the Southwestern dataset based on ethnicity. The county that showed the most accurate results was Fremont County for the Southwestern_Female model. The Southwestern_Male model had a 9% prediction rate when correctly predicting whether a male will graduate in the Southwestern dataset based on ethnicity. The county that showed the most accurate results was Fremont County and La Plata County for the Southwestern_Male model. It's clear that females had a better prediction for graduation than males in the Southwestern region.

# Decision Trees

After completing the ANN models, decision trees were created for each region (Metro, Western, Eastern, and Southwestern), gender (Male or Female), and ethnicity (Asian, Black or African American, Hispanic, and White). The accuracy rates for each decision tree were calculated as well.

|Region|Gender|Accuracy Rate|
|------|------|-------------|
|Metro|Female|45%|
|Metro|Male|34%|

The table above shows the accuracy rates of the decision trees for Metro_Female and Metro_Male. The accuracy rate for Metro_Female was 45%, which is a little bit lower than the accuracy rate for the Metro_Female ANN model. The accuracy rate for Metro_Male was 34%, which is significantly lower than the accuracy rate for the Metro_Male ANN model.

|Region|Gender|Accuracy Rate|
|------|------|-------------|
|Western|Female|14%|
|Western|Male|11%|

The table above shows the accuracy rates of the decision trees for Western_Female and Western_Male. The accuracy rate for Western_Female was 14%, which is significanly lower than the accuracy rate for the Western_Female ANN model. The accuracy rate for Western_Male was 11%, which is significantly lower than the accuracy rate for the Western_Male ANN model.

|Region|Gender|Accuracy Rate|
|------|------|-------------|
|Eastern|Female|13%|
|Eastern|Male|11%|

The table above shows the accuracy rates of the decision trees for Eastern_Female and Eastern_Male. The accuracy rate for Eastern_Female was 13%, which is significanly higher than the accuracy rate for the Eastern_Female ANN model. The accuracy rate for Eastern_Male was 11%, which is slightly lower than the accuracy rate for the Eastern_Male ANN model.

|Region|Gender|Accuracy Rate|
|------|------|-------------|
|Southwestern|Female|15%|
|Southwestern|Male|13%|

The table above shows the accuracy rates of the decision trees for Southwestern_Female and Southwestern_Male. The accuracy rate for Southwestern_Female was 15%, which is significanly lower than the accuracy rate for the Southwestern_Female ANN model. The accuracy rate for Southwestern_Male was 13%, which is significatly higher than the accuracy rate for the Southwestern_Male ANN model.

# Dendograms and Agglomerative Clustering of Female Metro Data

After completing the ANN models, the next machine learning model topic was to look at dendrograms and different clustering techniques. Dendrograms were created to determine the optimal number of clusters. One clustering technique that was conducted was agglomerative clustering. Agglomerative clustering was used to make predictions based on the numbers of clusters from the dendrograms. 

Below is a dendrogram created for the female Metro data.

<img width="395" alt="image" src="https://user-images.githubusercontent.com/79723505/115126258-27f31280-9f7a-11eb-8320-ed9763035b6a.png">

From the dendrogram, it appeared that the optimal number of clusters was 3. After viewing the dendrogram, agglomerative clustering was used to make predictions and then a graphical display was created of three clusters for the female Metro data.

<img width="395" alt="image" src="https://user-images.githubusercontent.com/79723505/115126314-920bb780-9f7a-11eb-8089-5a32b994d141.png">

There are three different clusters for the female Metro data. The three different colors used in this graphical display was red, blue, and green.

This process was used for all the different regions and genders. Below is a table of the potential number of clusters based on the respective dendrograms. A document of all visualizations for the dendrograms for each region and gender is attached to this instance page.

|Region|Gender|Optimal Number of Clusters from Dendrograms|
|------|------|-------------------------------------------|
|Metro|Female|3|
|Metro|Male|2|
|Western|Female|2|
|Western|Male|3|
|Eastern|Female|2|
|Eastern|Male|2|
|Southwestern|Female|2|
|Southwestern|Male|3|

# Elbow Method and Silhouette Method for K-Means of Metro Female Data

The final clustering techniques was the K-Means clustering techniques using the Elbow and Silhouette Methods. This was used for the regions, gender, and ethnicities. The data chosen to look at was the Metro Female data. 

<img width="395" alt="image" src="https://user-images.githubusercontent.com/79723505/115126614-c7190980-9f7c-11eb-8f35-0a023846ce59.png">

Using the Elbow method, it appeared that the optimal number of clusters was 3. The next method was using the Silhouette Method for K-Means clustering. 

<img width="419" alt="image" src="https://user-images.githubusercontent.com/79723505/115126647-05aec400-9f7d-11eb-807a-d03be00a1cac.png">

Looking at the Silhouette Method for the Metro Female data,the optimal number of clusters was 2 with a silhouette score of 0.607.

Below is a table created for the number of clusters for each region of data based on gender using the Elbow and Silhouette K-Means clustering techniques. A document of all visualizations for the elbow method and silhouette method for each region and gender is attached to this instance page.

|Region|Gender|Number of Clusters by Elbow Method|Number of Clusters by Silhouette Method|Silhouette Score|
|------|------|----------------------------------|---------------------------------------|----------------|
|Metro|Female|3|2|0.607|
|Metro|Male|2|2|0.474|
|Western|Female|2|2|0.771|
|Western|Male|3|4|0.649|
|Eastern|Female|3|2|0.679|
|Eastern|Male|2|14|0.556|
|Southwestern|Female|3|2|0.700|
|Southwestern|Male|3|13|0.540|

From the table above, the number of clusters from the Elbow Method and Silhouette Method were very similar with the exception of Eastern_Male and Southwestern_Male. The Eastern_Male optimal number of clusters by using the Elbow Method was projected to be 2 and the Silhouette Method project the optimal number of clusters to be 14. The Elbow Method projected the optimal number of clusters for Southwestern_Male data was 3 and the Silhouette Method projected the optimal number of clusters to be 13.

# Conclusions

The data shows that geographic location plays a role in high school graduation rates in Colorado. It was evident that ethnicity and gender played a role in Colorado high school graduation rates as well. The best accuracy rate for correctly predicting high school graduation rates in Colorado, based on the ANN models and decision trees, were in the Metro region. The least effective accuracy rate for correctly predicting high school graduation rates in Colorado, based on the ANN models and decision trees, were in the Eastern region. The ANN and decision trees showed that females generally had a better prediction for graduating high school in Colorado than males.

After viewing the results, I would encourage the Colorado Department of Education (CDE) to see why the correct prediction in graduation rate by ethnicity in the 
Eastern dataset was much lower than the other three regions (Metro, Western, and Southwestern). I would also recommend that CDE look into why the female graduation
rate in most of the regions had better predictions for the different regions than males. The CDE should invest resources in aiding graduation rates for the Eastern
region and for males in Colorado.

The results from the machine learning models included all of the different range of years a Colorado high school student can graduate (4, 5, 6, or 7 years). The results may have been different if only a specific year range would have been evaluated.

# Future Project Ideas

A future project idea would to be to look at other external factors that affect graduation rates for Colorado high school students outside of gender and ethnicity. By looking at other external factors, CDE could invest their time and resources into providing programs to aide Colorado high school students.

Another future project idea could be to project high school graduation rates and number of total completers by region, gender, and ethnicity over a span of time. By projecting future graduation rates, CDE could invest resources into accomplishing a specific high school graduation rate amongst Colorado high school students. An example of a goal could be to have Colorado high school graduation rates all be at 95% in all counties and regions in Colorado by the year 2040.

# References

A Detailed Introduction to K-Means Clustering in Python! (2020, December 3). Analytics 
	Vidhya. Retrieved April 11, 2021 from https://www.analyticsvidhya.com/blog/2020/12/a-detailed-introduction-to-k-means-clustering-in-python/.


Colorado Department of Education. (2021).  Graduates and Completers by Districts, Gender, 
  	and Race/Ethnicity.  Colorado Department of Education. Retrieved March 13, 2021 from 
 	 https://www.cde.state.co.us/cdereval/gradratecurrent.

DataScience Made Simple. (2021). BOX PLOT IN PYTHON WITH MATPLOTLIB. DataScience
	Made Simple. Retrieved March 28, 2021 from 
 	https://www.datasciencemadesimple.com/box-plot-in-
	python/#:~:text=boxplot%28%29%20function%20takes%20the%20data%20array%20to
	%20be,plotted.%20Create%20box%20plot%20in%20python%20with%20notch.


FTE. (2021). Week 5 – Artificial Neural Network (ANN). Retrieved April 2, 2021 from 
	http://localhost:8888/notebooks/Downloads/FTE_Week5(2).ipynb.
	
Hierarchical Clustering in Python, Step by Step Complete Guide. (2020, June 4). MLTut.com 
	Retrieved April 11, 2021 from https://www.mltut.com/hierarchical-clustering-in-python-
	step-by-step-complete guide/#:~:text=The%20final%20cluster%20in%20the%20Hierarchical%20cluster%20co
	mbines,gained%20brief%20knowledge%20about%20Clustering%20and%20its%20types.


Matplotlib development team. (2021). List of named colors. Matplotlib. Retrieved March 28, 
  	2021 from https://matplotlib.org/stable/gallery/color/named_colors.html.
  
Motwani, S. (2020). Decision Tree Implementation in Python with Example. Retrieved April 4,
	 2021 from https://in.springboard.com/blog/decision-tree-implementation-in-python/.
	 
Nanduri, A. (2020). Different ways to create, subset, and combine data frames using	pandas. 
  Retrieved March 20, 2021 from https://towardsdatascience.com/different-ways-
  to-create-subset-and-combine-dataframes-using-pandas-e7227330a7f1.

OneStop_Data. (2020). Easy Outlier Detection in Python. OneStop Data Analysis. Retrieved
	March 28, 2021 from https://onestopdataanalysis.com/python-outlier-detection/. 










