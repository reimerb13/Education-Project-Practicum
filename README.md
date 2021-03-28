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

# Western Data

The Western data subset consisted of 17 different counties: Mesa, Garfield, Eagle, Montrose, Delta, Summit, Routt, Chaffee, Gunnison, Pitkin, Moffat, Grand, Park, Rio Blanco, Lake, Ouray, and Jackson. The summary statistics for the Western data were calculated and then the top five counties where the total number of females completed high school.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112403565-8272b900-8cc3-11eb-89c1-dbe36f64dba7.png">

The top five counties where females completed high school were Mesa, Garfield, Eagle, Montrose, and Delta.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112403680-b4841b00-8cc3-11eb-9eba-00d16d72cfe7.png">

The top five counties where females completed high school were Mesa, Garfield, Eagle, Montrose, and Delta.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112403774-e5fce680-8cc3-11eb-9cf0-44b4758f4efa.png">

The top five Western counties for total number of years entering high school were Mesa, Garfield, Routt,
Montrose, and Grand.

# Eastern Data

The Eastern data subset consisted of 18 different counties: Weld, Pueblo, Bent, Morgan, Elbert, Otero, Logan, Prowers, Yuma, Kit Carson, Sedgwick, Phillips, Washington, Lincoln, Baca, Crowley, Cheyenne, and Kiowa. The summary statistics for the Eastern data were calculated and then the top five counties where the total number of females completed high school.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112404138-a4b90680-8cc4-11eb-8a0d-c6d7f1274e15.png">

The top 5 Eastern counties where females completed high school were Weld, Pueblo, Bent, Morgan, and Elbert.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112404239-d8942c00-8cc4-11eb-9f5a-65b3033c707f.png">

The top 5 Eastern counties where females completed high school were Weld, Pueblo, Bent, Morgan, and Elbert.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112404347-0d07e800-8cc5-11eb-9e94-73f4e6d1a163.png">

The top 5 eastern counties for students graduating high school after a number of years were Weld, Otero, Baca,
Washingtion, and Elbert.

# Southwestern Data

The Southwestern data subset consisted of 18 different counties: La Plata, Fremont, Montezuma, Teller, Alamosa, Rio Grande, Las Animas, Conejos, San Miguel, Archuleta, Saguache, Huerfano, Custer, Costilla, Dolores, Hinsdale, Mineral, and San Juan. The summary statistics for the Southwestern data were calculated and then the top five counties where the total number of females completed high school.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112404844-f9a94c80-8cc5-11eb-9c32-5d97df56639f.png">

The top 5 Southwestern counties where females completed high school were La Plata, Fremont, Montezuma, Teller, and Las Animas.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112404677-9f0ff080-8cc5-11eb-85ae-79944f123713.png">

The top 5 Southwestern counties where males completed high school were La Plata, Fremont, Montezuma, Teller, and Las Animas.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/79723505/112404915-180f4800-8cc6-11eb-8345-5b69d56f4da2.png">

The top 5 Southwestern counties for number of years students completing high school were Las Animas, Fremont, Conejos
Saguache, and Rio Grande.

# References

Colorado Department of Education. (2021).  Graduates and Completers by Districts, Gender, 
  and Race/Ethnicity.  Colorado Department of Education. Retrieved March 13, 2021 from 
  https://www.cde.state.co.us/cdereval/gradratecurrent.

DataScience Made Simple. (2021). BOX PLOT IN PYTHON WITH MATPLOTLIB. DataScience
	Made Simple. Retrieved March 28, 2021 from 
  https://www.datasciencemadesimple.com/box-plot-in-
  python/#:~:text=boxplot%28%29%20function%20takes%20the%20data%20array%20to
  %20be,plotted.%20Create%20box%20plot%20in%20python%20with%20notch.

Matplotlib development team. (2021). List of named colors. Matplotlib. Retrieved March 28, 
  2021 from https://matplotlib.org/stable/gallery/color/named_colors.html.

Nanduri, A. (2020). Different ways to create, subset, and combine data frames using	pandas. 
  Retrieved March 20, 2021 from https://towardsdatascience.com/different-ways-
  to-create-subset-and-combine-dataframes-using-pandas-e7227330a7f1.

OneStop_Data. (2020). Easy Outlier Detection in Python. OneStop Data Analysis. Retrieved
	March 28, 2021 from https://onestopdataanalysis.com/python-outlier-detection/. 










