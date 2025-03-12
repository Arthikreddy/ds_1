# ds_1

# Students Grading Dataset Analysis

## Overview
This project analyzes a dataset of students' grades to gain insights into their performance using data preprocessing, visualization, and statistical analysis techniques. The dataset undergoes various stages of cleaning, transformation, and exploratory data analysis (EDA) to uncover meaningful patterns.

## Dataset
The dataset consists of students' academic records, including numerical and categorical variables representing different attributes such as scores, demographics, and other relevant factors. The primary objectives are:
- Understanding grade distributions.
- Identifying correlations between variables.
- Detecting and handling missing values and outliers.
- Performing univariate, bivariate, and multivariate analysis.


##DATA
- Student_ID: Unique identifier for each student
-First_Name: First name of the student
-Last_Name: Last name of the student
-Email: Email address of the student
-Gender: Gender of the student
-Age: Age of the student
-Department: Department in which the student is enrolled
-Attendance (%): Attendance percentage of the student
-Midterm_Score: Midterm exam score
-Final_Score: Final exam score
-Assignments_Avg: Average score of assignments
-Quizzes_Avg: Average score of quizzes
-Participation_Score: Participation score
-Projects_Score: Projects score
-Total_Score: Total score
-Grade: Final grade
-Study_Hours_per_Week: Number of study hours per week
-Extracurricular_Activities: Participation in extracurricular activities (Yes/No)
-Internet_Access_at_Home: Internet access at home (Yes/No)
-Parent_Education_Level: Education level of the parents
-Family_Income_Level: Family income level
-Stress_Level (1-10): Stress level on a scale of 1 to 10
-Sleep_Hours_per_Night: Number of sleep hours per night

## Data Preprocessing
### 1. Handling Missing Values
- Identified missing values and filled them with mean, median, or mode as appropriate.
- Checked for duplicate rows and removed them to maintain data integrity.

### 2. Removing Unnecessary Columns
- Dropped columns that do not contribute significantly to the analysis.
- Removing the unwanted data.that is not affecting the outcome of the data

### 3. Handling Outliers
- Used box plots and statistical methods to identify outliers.
- Applied appropriate transformations or removals to handle extreme values.

## Data Analysis
### 1. Univariate Analysis
- Visualized individual variables using histograms, KDE plots, and box plots.
- Analyzed the distribution of numerical variables.
- Summarized categorical variables with bar plots and pie charts.

### 2. Bivariate Analysis
- Explored relationships between two variables using scatter plots, line plots, and bar charts.
- Used correlation coefficients to quantify relationships between numerical variables.
- Created crosstabs and heatmaps to analyze categorical dependencies.

### 3. Multivariate Analysis
- Constructed a correlation matrix to study relationships among multiple variables.
- Visualized correlations using a heatmap to identify highly correlated attributes.
- Applied clustering techniques or PCA (if required) for dimensionality reduction.

## Visualization
The project includes various plots to understand the dataset better:
- Histograms and KDE plots for distribution analysis.
- Box plots to detect outliers.
- Heatmaps for correlation visualization.
- Bar plots and pie charts for categorical insights.


 ##corelation
     Student_ID First_Name Last_Name                    Email  Gender  Age  \
0      S1000       Omar  Williams  student0@university.com  Female   22   
1      S1001      Maria     Brown  student1@university.com    Male   18   
2      S1002      Ahmed     Jones  student2@university.com    Male   24   
3      S1003       Omar  Williams  student3@university.com  Female   24   
4      S1004       John     Smith  student4@university.com  Female   23   

    Department  Attendance (%)  Midterm_Score  Final_Score  ...  \
0  Engineering           52.29          55.03        57.82  ...   
1  Engineering           97.27          97.23        45.80  ...   
2     Business           57.19          67.05        93.68  ...   
3  Mathematics           95.15          47.79        80.63  ...   
4           CS           54.18          46.59        78.89  ...   

   Projects_Score  Total_Score  Grade  Study_Hours_per_Week  \
0           85.90        56.09      F                   6.2   
1           55.65        50.64      A                  19.0   
2           73.79        70.30      D                  20.7   
3           92.12        61.63      A                  24.8   
4           68.42        66.13      F                  15.4   

   Extracurricular_Activities Internet_Access_at_Home  Parent_Education_Level  \
0                          No                     Yes             High School   
1                          No                     Yes                     NaN   
2                          No                     Yes                Master's   
...
Family_Income_Level              0
Stress_Level (1-10)              0
Sleep_Hours_per_Night            0
dtype: int64
Output is truncated. View as a scrollable element or open in a text editor. Adjust cell output settings...
Requirement already satisfied: seaborn in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (0.13.2)
Requirement already satisfied: numpy!=1.24.0,>=1.20 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from seaborn) (2.2.2)
Requirement already satisfied: pandas>=1.2 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from seaborn) (2.2.3)
Requirement already satisfied: matplotlib!=3.6.1,>=3.4 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from seaborn) (3.10.1)
Requirement already satisfied: contourpy>=1.0.1 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from matplotlib!=3.6.1,>=3.4->seaborn) (1.3.1)
Requirement already satisfied: cycler>=0.10 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from matplotlib!=3.6.1,>=3.4->seaborn) (0.12.1)
Requirement already satisfied: fonttools>=4.22.0 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from matplotlib!=3.6.1,>=3.4->seaborn) (4.56.0)
Requirement already satisfied: kiwisolver>=1.3.1 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from matplotlib!=3.6.1,>=3.4->seaborn) (1.4.8)
Requirement already satisfied: packaging>=20.0 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from matplotlib!=3.6.1,>=3.4->seaborn) (24.2)
Requirement already satisfied: pillow>=8 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from matplotlib!=3.6.1,>=3.4->seaborn) (11.1.0)
Requirement already satisfied: pyparsing>=2.3.1 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from matplotlib!=3.6.1,>=3.4->seaborn) (3.2.1)
Requirement already satisfied: python-dateutil>=2.7 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from matplotlib!=3.6.1,>=3.4->seaborn) (2.9.0.post0)
Requirement already satisfied: pytz>=2020.1 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from pandas>=1.2->seaborn) (2024.1)
Requirement already satisfied: tzdata>=2022.7 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from pandas>=1.2->seaborn) (2023.3)
Requirement already satisfied: six>=1.5 in c:\users\arthi\anaconda3\envs\ds_env\lib\site-packages (from python-dateutil>=2.7->matplotlib!=3.6.1,>=3.4->seaborn) (1.16.0)
Number of duplicate rows: 0
Empty DataFrame
Columns: [Student_ID, First_Name, Last_Name, Email, Gender, Age, Department, Attendance (%), Midterm_Score, Final_Score, Assignments_Avg, Quizzes_Avg, Participation_Score, Projects_Score, Total_Score, Grade, Study_Hours_per_Week, Extracurricular_Activities, Internet_Access_at_Home, Parent_Education_Level, Family_Income_Level, Stress_Level (1-10), Sleep_Hours_per_Night]
Index: []

[0 rows x 23 columns]
Student_ID                       0
First_Name                       0
Last_Name                        0
Email                            0
Gender                           0
Age                              0
Department                       0
Attendance (%)                   0
Midterm_Score                    0
Final_Score                      0
Assignments_Avg                  0
Quizzes_Avg                      0
Participation_Score              0
Projects_Score                   0
Total_Score                      0
Grade                            0
Study_Hours_per_Week             0
Extracurricular_Activities       0
Internet_Access_at_Home          0
...
Family_Income_Level              0
Stress_Level (1-10)              0
Sleep_Hours_per_Night            0
dtype: int64
Output is truncated. View as a scrollable element or open in a text editor. Adjust cell output settings...
C:\Users\arthi\AppData\Local\Temp\ipykernel_14952\1838877102.py:3: FutureWarning: A value is trying to be set on a copy of a DataFrame or Series through chained assignment using an inplace method.
The behavior will change in pandas 3.0. This inplace method will never work because the intermediate object on which we are setting values always behaves as a copy.

For example, when doing 'df[col].method(value, inplace=True)', try using 'df.method({col: value}, inplace=True)' or df[col] = df[col].method(value) instead, to perform the operation inplace on the original object.


  df['Attendance (%)'].fillna(attendance_mean, inplace=True)
C:\Users\arthi\AppData\Local\Temp\ipykernel_14952\1838877102.py:7: FutureWarning: A value is trying to be set on a copy of a DataFrame or Series through chained assignment using an inplace method.
The behavior will change in pandas 3.0. This inplace method will never work because the intermediate object on which we are setting values always behaves as a copy.

For example, when doing 'df[col].method(value, inplace=True)', try using 'df.method({col: value}, inplace=True)' or df[col] = df[col].method(value) instead, to perform the operation inplace on the original object.


  df['Assignments_Avg'].fillna(df['Total_Score'] - other_scores_sum, inplace=True)
<Axes: ylabel='Frequency'>

<Axes: ylabel='Density'>

np.float64(-0.02238469633213024)
<Axes: >

count    5000.000000
mean       75.121804
std        14.399941
min        50.020000
25%        62.835000
50%        75.395000
75%        87.652500
max        99.990000
Name: Total_Score, dtype: float64
count    5000.000000
mean       17.658860
std         7.275864
min         5.000000
25%        11.400000
50%        17.500000
75%        24.100000
max        30.000000
Name: Study_Hours_per_Week, dtype: float64
Attendance (%)	Midterm_Score	Final_Score	Assignments_Avg	Quizzes_Avg	Participation_Score	Projects_Score	Total_Score	Study_Hours_per_Week	Stress_Level (1-10)	Sleep_Hours_per_Night
count	5000.000000	5000.000000	5000.000000	5000.000000	5000.000000	5000.000000	5000.000000	5000.000000	5000.000000	5000.00000	5000.000000
mean	75.431409	70.326844	69.640788	44.365430	74.910728	4.980024	74.924860	75.121804	17.658860	5.48080	6.488140
std	13.610481	17.213209	17.238744	91.377065	14.504281	2.890136	14.423415	14.399941	7.275864	2.86155	1.452283
min	50.010000	40.000000	40.000000	-323.540000	50.030000	0.000000	50.010000	50.020000	5.000000	1.00000	4.000000
25%	64.737500	55.457500	54.667500	58.087500	62.490000	2.440000	62.320000	62.835000	11.400000	3.00000	5.200000
50%	75.431409	70.510000	69.735000	71.875000	74.695000	4.955000	74.980000	75.395000	17.500000	5.00000	6.500000
75%	86.182500	84.970000	84.500000	85.570000	87.630000	7.500000	87.367500	87.652500	24.100000	8.00000	7.700000
max	100.000000	99.980000	99.980000	99.980000	99.960000	10.000000	100.000000	99.990000	30.000000	10.00000	9.000000
<Axes: ylabel='Frequency'>

<Axes: ylabel='Density'>

np.float64(0.0007433558913855831)
<Axes: >

<Axes: >

<Axes: xlabel='Grade'>

<Axes: ylabel='count'>

<Axes: xlabel='Stress_Level (1-10)', ylabel='Grade'>

Gender	Female	Male
Grade		
A	30.788077	29.047432
B	19.232340	19.874559
C	15.639036	16.111329
D	17.884851	17.679341
F	16.455696	17.287338
Stress_Level (1-10)	1	2	3	4	5	6	7	8	9	10
Grade										
A	30.674847	30.753968	25.933202	31.332083	27.272727	31.185031	26.993865	28.053435	32.172131	34.836066
B	18.404908	17.460317	20.432220	18.198874	21.818182	19.334719	19.427403	21.564885	19.877049	19.057377
C	17.177914	14.285714	17.092338	15.009381	16.969697	16.839917	16.359918	14.312977	16.598361	14.344262
D	16.768916	19.246032	17.878193	20.450281	17.979798	16.008316	17.586912	20.038168	15.163934	16.188525
F	16.973415	18.253968	18.664047	15.009381	15.959596	16.632017	19.631902	16.030534	16.188525	15.573770
Stress_Level (1-10)	1	2	3	4	5	6	7	8	9	10
Gender										
Female	47.239264	50.0	47.740668	48.592871	49.89899	47.609148	47.034765	52.290076	50.409836	48.770492
Male	52.760736	50.0	52.259332	51.407129	50.10101	52.390852	52.965235	47.709924	49.590164	51.229508

np.float64(74.43559197324416)
Grade
A    1495
B     978
D     889
F     844
C     794
Name: count, dtype: int64



                      Department  Stress_Level (1-10)  Study_Hours_per_Week  
Department              1.000000            -0.005378             -0.028696   -0.017590
Stress_Level (1-10)    -0.005378             1.000000              0.004551   -0.247950
Study_Hours_per_Week   -0.028696             0.004551              1.000000   -0.0025960
Grade                  -0.010759            -0.024795             -0.002596    1.000000




## Conclusion
This project provides insights into students' grading patterns using statistical and visualization techniques. It helps in understanding key factors affecting performance and suggests areas for further investigation.

## Author
B.Arthik Reddy



