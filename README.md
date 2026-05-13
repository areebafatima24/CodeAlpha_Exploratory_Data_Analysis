# Student Performance — Exploratory Data Analysis

---

> *Data does not speak. It whispers.*
> *EDA is the art of learning how to listen.*

---

## The Question That Started Everything

Before a single line of code was written, before any chart was drawn,
I sat down and asked one simple question:

**What does it actually take for a student to pass?**

Is it raw intelligence? Hours spent studying?
Just showing up every day?
Or is it something the numbers reveal that common sense misses?

This project is the answer.

---

## What This Is

A full Exploratory Data Analysis performed on a student performance
dataset — 100 students, 10 variables, and every question I could
think to ask before touching the data.

No machine learning. No predictions. Just honest, curious
investigation of what the data is actually saying.

---

## The Dataset At A Glance

| Column | Type | Description |
|--------|------|-------------|
| StudentID | Number | Unique student identifier |
| Age | Number | Age between 16 and 19 |
| Gender | Text | Male or Female |
| StudyHours | Number | Daily study hours (0.5 – 6) |
| Attendance | Number | Attendance percentage |
| MathScore | Number | Math exam result |
| EnglishScore | Number | English exam result |
| ScienceScore | Number | Science exam result |
| AverageScore | Number | Mean of all three subjects |
| PassFail | Text | Final outcome — Pass or Fail |

100 rows. 3 intentional missing values hidden inside.
Because real data is never clean.

---

## The Five Questions I Asked First

Before writing code, I wrote these down:

1. Do students who study more hours actually score higher?
2. Is showing up to class enough — or does effort matter more?
3. Are there score differences between male and female students?
4. Where are the data problems hiding?
5. What single variable best predicts whether a student passes?

Every chart and every line of code in this notebook
exists to answer one of these questions.

---

## What I Found

**The study hours effect is real**
Students averaging 4+ study hours daily passed at nearly
double the rate of those studying under 2 hours.
The correlation does not lie.

**Attendance helps — but it is not enough**
High attendance with low study hours still produced failures.
Presence without effort has limits.

**The data had secrets**
Three missing values were hiding in the StudyHours column —
invisible until you looked for them. Exactly the kind of problem
that breaks a model if you skip EDA and go straight to analysis.

**Gender showed minimal difference**
Average scores between male and female students were within
3 points of each other. Not a significant finding — which is
itself a finding worth noting.

---

## The Visualizations

### Image 1 — Distribution of average score
> Shows how scores are spread across all 100 students

![Score Distribution](distribution_avg_score.png)

---

### Image 2 — Study hours vs average score
> Each dot is one student — the upward trend is clear

![Study Hours vs Score](study_hours_vs_score.png)

---

### Image 3 — Attendance vs average score
> Attendance helps, but the pattern is weaker than study hours

![Attendance vs Score](attendance_vs_score.png)

---

### Image 4 — Average score by gender
> Comparing male and female student performance side by side

![Score by Gender](score_by_gender.png)

---

### Image 5 — Study hours: pass vs fail students
> Pass students clearly study more on average

![Pass Fail](study_hours_vs_passfail.png)

---

### Image 6 — Correlation heatmap
> Shows how strongly every variable relates to every other variable

![Correlation Heatmap](correlation_heatmap.png)

---

### Image 7 — Missing values heatmap
> Reveals exactly where data is missing before we do anything else

![Missing Values](missing_values_heatmap.png)

---

## How To Run This Yourself

No installation. No setup. Just:

1. Click the notebook file above
2. Hit **Open in Colab** at the top of the page
3. Go to **Runtime → Run All**
4. Watch everything run automatically

Total time: under 2 minutes.

---

## Tools Used

| Tool | Why |
|------|-----|
| Python | The language everything is written in |
| Pandas | Loading, shaping, and inspecting the data |
| Matplotlib | Building the core charts |
| Seaborn | Statistical visualizations and heatmaps |
| Google Colab | Cloud environment — runs in the browser |

---

## Video Walkthrough

I recorded a full explanation of every step, every chart,
and every finding in plain simple language.

🎥 [Watch the full walkthrough here](https://drive.google.com/file/d/1NUCh5EeJP4L-T1A95WJix1m54SzlIxaP/view?usp=sharing)

---

## Files In This Repository

| File | What it is |
|------|-----------|
| `task2_eda_student_performance.ipynb` | Full notebook with all code and outputs |
| `task2_eda_walkthrough.mp4` | Video explanation of every step |
| `distribution_avg_score.png` | Image 1 — score distribution |
| `study_hours_vs_score.png` | Image 2 — study hours vs score |
| `attendance_vs_score.png` | Image 3 — attendance vs score |
| `score_by_gender.png` | Image 4 — score by gender |
| `study_hours_vs_passfail.png` | Image 5 — pass vs fail study hours |
| `correlation_heatmap.png` | Image 6 — correlation heatmap |
| `missing_values_heatmap.png` | Image 7 — missing values |

---

*This is Task 2 of my data analysis journey.*
*The data had answers. I just had to ask the right questions.*
