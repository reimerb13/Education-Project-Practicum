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

The Metro data subset consisted of 10 different counties: El Paso, Arapahoe, Jefferson, Adams, Denver, Douglas, Boulder, Larimer, Clear Creek, and Gilpin. The summary statistics for the Metro data were calculated and then the top 5 counties where the total number of females completed high school.

<img width="469" alt="image" src="https://user-images.githubusercontent.com/79723505/112390306-eccb2f80-8caa-11eb-899b-528aefc5f8bf.png">

The top five counties where females completed high school were El Paso, Arapahoe, Jefferson, Adams, and Denver.
