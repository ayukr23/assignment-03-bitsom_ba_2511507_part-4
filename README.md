# assignment-03-bitsom_ba_2511507_part-4
## Student Performance Analysis & Prediction
# Student Performance Analysis & Prediction

A beginner-friendly data science project that looks at student scores, attendance, and study habits to figure out what separates students who pass from those who fail — and then builds a simple model to predict it.

---

## What this project does

The dataset has 15 students with marks in 5 subjects (math, science, english, history, PE), their attendance percentage, how many hours they study per day, and whether they passed or failed.

The project is split into 4 tasks:

**Task 1 — Exploring the data with Pandas**
Just getting familiar with the dataset. Checking the shape, data types, basic stats, how many passed vs failed, and which student had the highest overall average (spoiler: it's Diana).

**Task 2 — Plotting with Matplotlib**
5 plots to visualise the data:
- Average score per subject (bar chart)
- How math scores are spread out (histogram)
- Study hours vs average score — coloured by pass/fail (scatter plot)
- Attendance comparison between passed and failed students (box plot)
- Math and science scores for every student side by side (line chart)

**Task 3 — Plotting with Seaborn**
2 more plots using Seaborn:
- Average math and science scores grouped by pass/fail
- Attendance vs average score with trend lines for each group

Seaborn honestly made these much easier to write compared to Matplotlib — grouping and trend lines came for free.

**Task 4 — Building a prediction model with scikit-learn**
Trained a Logistic Regression model to predict if a student will pass or fail based on their scores, attendance, and study hours. Also checked which features the model found most useful (english score turned out to be the strongest signal), and tested it on a brand new student.

---

## How to run it

1. Clone the repo
```bash
git clone https://github.com/your-username/student-performance-analysis.git
cd student-performance-analysis
```

2. Install the required libraries
```bash
pip install pandas matplotlib seaborn scikit-learn
```

3. Open `student_analysis.ipynb` in VS Code, add `%matplotlib inline` at the top of the first cell, and click **Run All**

Make sure `students.csv` is in the same folder as the notebook.

---

## Files in this repo

| File | What it is |
|------|------------|
| `student_analysis.ipynb` | Main notebook with all 4 tasks |
| `students.csv` | The dataset (15 students) |
| `plot1_bar.png` | Average score per subject |
| `plot2_histogram.png` | Math score distribution |
| `plot3_scatter.png` | Study hours vs average score |
| `plot4_boxplot.png` | Attendance: pass vs fail |
| `plot5_line.png` | Math & science per student |
| `plot6_seaborn_bar.png` | Seaborn grouped bar chart |
| `plot7_seaborn_scatter.png` | Seaborn regression scatter |
| `plot8_feature_importance.png` | Model feature coefficients |

---

## Libraries used

- `pandas` — loading and exploring the data
- `matplotlib` — making the charts
- `seaborn` — easier statistical plots
- `scikit-learn` — building and evaluating the ML model