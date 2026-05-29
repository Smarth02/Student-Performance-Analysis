# Student-Performance-Analysis
<br>
<p>It's an exploratory data analysis (EDA) of student habits and academic outcomes — not to judge students, but to understand the ecosystem around them.</p>
<h2>What This Project is About</h2>
<p>Academic performance is rarely a matter of just intelligence. It’s a web of lifestyle choices, socio-economic factors and daily habits that quietly shape exam scores. This analysis takes a dataset of student behaviors and peels back the layers — looking at everything from study hours and sleep to mental health ratings, diet quality and social media consumption — to find what actually correlates with performance.
The aim here is not to build a predictive model (although this work sets the stage for doing so). The goal is to be able to see the data clearly and let it tell a coherent story.</p>
<h2>Datset</h2>
<p>The dataset used is student_habits_performance.csv directly loaded from this repository.<br>
It covers a broad spectrum of student characteristics.<br>
Taken from kaggle.com https://www.kaggle.com/code/jayaantanaath/student-habits-vs-academic-performance-ml-90/input
</p>
<h2>Analysis Overview</h2>
<ul>
  <li><b>Data loading and First look- </b>We start the notebook by loading the dataset and taking a quick look at its structure – shape, data types, a statistical summary – to get a feel for what we're dealing with before we touch anything.</li>
  <li><b>Cleaning Up- </b>Missing values are detected and deleted. Categorical columns such as diet_quality ("Fair", "Good", "Poor") and internet_quality ("Average", "Poor", "Good") are encoded as ordinal integers for meaningful correlation analysis.</li>
  <li><b>Correlation Heatmap- </b>Correlation matrix of all numerical features, visualized as heatmap. This is the bird’s eye view. It tells you which variables are closely related to exam scores, and which are noise.</li>
  <li><b>Distribution Plots- </b>Count plots across important categorical features give an idea of who the students in this dataset really are:
    <ul>
<li>Breakdown by gender
<li>How many are working part-time jobs
<li>Distribution of diet quality
<li>How often students exercise
<li>Parental level of education
<li>Quality of Internet access
<li>Participation in extra-curricular activities
    </ul></li>
<li><b>Scatter Plots - The Heart of the Story- </b>
Most telling: scatter plots of exam score vs.
<ul>
<li>Hours of study per day
<li>Social Media hours
<li>Netflix  hours
<li>Percentage of attendance
<li>Hours of sleep
<li>How often students exercise
<li>Rating: Mental Health.</ul>
These plots don't just indicate direction, they indicate shape. Is there a linear relationship? Noisy? 
<li><b>Group comparisons</b>
Bar charts of average exam scores by gender, quality of internet and involvement in extracurricular activities. Basic but good for noticing differences in systems.
<li><b>Box Plots-Outliers and Spread- </b>
Box plots of exam scores by categorical groups (gender, diet quality, parental education, internet quality, part-time job status) These show not just averages but distribution – where the outliers are, how wide the spread is, whether certain groups are more variable than others.
</ul>
<h2>Project Structure</h2>
Student-Performance-Analysis/<br>
│<br>
├── Student_performance_analysis.ipynb   # Main analysis notebook<br>
├── student_habits_performance.csv       # Dataset<br>
└── README.md                            # This file
